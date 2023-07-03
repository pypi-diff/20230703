# Comparing `tmp/mypy-boto3-rbin-1.26.16.tar.gz` & `tmp/mypy-boto3-rbin-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rbin-1.26.16.tar", last modified: Wed Nov 23 20:46:58 2022, max compression
+gzip compressed data, was "mypy-boto3-rbin-1.27.0.tar", last modified: Mon Jul  3 19:51:17 2023, max compression
```

## Comparing `mypy-boto3-rbin-1.26.16.tar` & `mypy-boto3-rbin-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 20:46:58.365242 mypy-boto3-rbin-1.26.16/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13268 2022-11-23 20:46:58.365242 mypy-boto3-rbin-1.26.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11837 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 20:46:58.365242 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9110 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     9092 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7944 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7942 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     9423 2022-11-23 20:46:51.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9412 2022-11-23 20:46:51.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 20:46:58.365242 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13268 2022-11-23 20:46:58.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-11-23 20:46:58.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-23 20:46:58.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-23 20:46:58.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-23 20:46:58.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-23 20:46:58.000000 mypy-boto3-rbin-1.26.16/mypy_boto3_rbin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-23 20:46:58.365242 mypy-boto3-rbin-1.26.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-11-23 20:46:50.000000 mypy-boto3-rbin-1.26.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.779845 mypy-boto3-rbin-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-07-03 19:51:17.771845 mypy-boto3-rbin-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11811 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.771845 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.771845 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-07-03 19:51:17.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-03 19:51:17.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:17.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:17.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:17.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 19:51:17.000000 mypy-boto3-rbin-1.27.0/mypy_boto3_rbin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:17.779845 mypy-boto3-rbin-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-03 19:45:43.000000 mypy-boto3-rbin-1.27.0/setup.py
```

### Comparing `mypy-boto3-rbin-1.26.16/LICENSE` & `mypy-boto3-rbin-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-rbin-1.26.16/PKG-INFO` & `mypy-boto3-rbin-1.27.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rbin
-Version: 1.26.16
-Summary: Type annotations for boto3.RecycleBin 1.26.16 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.RecycleBin 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/
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
 
 <a id="mypy-boto3-rbin"></a>
 
 # mypy-boto3-rbin
 
 [![PyPI - mypy-boto3-rbin](https://img.shields.io/pypi/v/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rbin?color=blue)](https://pypistats.org/packages/mypy-boto3-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RecycleBin 1.26.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[boto3.RecycleBin 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [mypy-boto3-rbin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,29 +326,29 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rbin.type_defs import (
     ResourceTagTypeDef,
     RetentionPeriodTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     DeleteRuleRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     UnlockDelayTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UnlockRuleRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdateRuleResponseTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     LockConfigurationTypeDef,
     ListRulesResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     LockRuleRequestRequestTypeDef,
     LockRuleResponseTypeDef,
@@ -362,42 +363,42 @@
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

### Comparing `mypy-boto3-rbin-1.26.16/README.md` & `mypy-boto3-rbin-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-rbin"></a>
 
 # mypy-boto3-rbin
 
 [![PyPI - mypy-boto3-rbin](https://img.shields.io/pypi/v/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rbin?color=blue)](https://pypistats.org/packages/mypy-boto3-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RecycleBin 1.26.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[boto3.RecycleBin 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [mypy-boto3-rbin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -294,29 +294,29 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rbin.type_defs import (
     ResourceTagTypeDef,
     RetentionPeriodTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     DeleteRuleRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     UnlockDelayTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UnlockRuleRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdateRuleResponseTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     LockConfigurationTypeDef,
     ListRulesResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     LockRuleRequestRequestTypeDef,
     LockRuleResponseTypeDef,
@@ -331,42 +331,42 @@
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

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/__init__.py` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/__init__.pyi` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/__main__.py` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RecycleBin 1.26.16\nVersion:         1.26.16\nBuilder version:"
-        " 7.11.11\nDocs:           "
+        "Type annotations for boto3.RecycleBin 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.16")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/client.py` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/client.pyi` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/literals.py` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,30 +14,28 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListRulesPaginatorName",
     "LockStateType",
     "ResourceTypeType",
     "RetentionPeriodUnitType",
     "RuleStatusType",
     "UnlockDelayUnitType",
     "RecycleBinServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListRulesPaginatorName = Literal["list_rules"]
 LockStateType = Literal["locked", "pending_unlock", "unlocked"]
 ResourceTypeType = Literal["EBS_SNAPSHOT", "EC2_IMAGE"]
 RetentionPeriodUnitType = Literal["DAYS"]
 RuleStatusType = Literal["available", "pending"]
 UnlockDelayUnitType = Literal["DAYS"]
 RecycleBinServiceName = Literal["rbin"]
@@ -52,23 +50,25 @@
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
@@ -79,30 +79,34 @@
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
@@ -128,14 +132,15 @@
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
@@ -180,14 +185,15 @@
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
@@ -198,34 +204,38 @@
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
@@ -238,14 +248,15 @@
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
@@ -257,28 +268,35 @@
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
@@ -306,30 +324,34 @@
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
@@ -345,18 +367,21 @@
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
@@ -382,17 +407,19 @@
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
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/literals.pyi` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListRulesPaginatorName",
     "LockStateType",
     "ResourceTypeType",
     "RetentionPeriodUnitType",
     "RuleStatusType",
     "UnlockDelayUnitType",
     "RecycleBinServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ListRulesPaginatorName = Literal["list_rules"]
 LockStateType = Literal["locked", "pending_unlock", "unlocked"]
 ResourceTypeType = Literal["EBS_SNAPSHOT", "EC2_IMAGE"]
 RetentionPeriodUnitType = Literal["DAYS"]
 RuleStatusType = Literal["available", "pending"]
 UnlockDelayUnitType = Literal["DAYS"]
 RecycleBinServiceName = Literal["rbin"]
@@ -50,23 +52,25 @@
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
@@ -77,30 +81,34 @@
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
@@ -126,14 +134,15 @@
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
@@ -178,14 +187,15 @@
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
@@ -196,34 +206,38 @@
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
@@ -236,14 +250,15 @@
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
@@ -255,28 +270,35 @@
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
@@ -304,30 +326,34 @@
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
@@ -343,18 +369,21 @@
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
@@ -380,17 +409,19 @@
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
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/paginator.py` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 
     def paginate(
         self,
         *,
         ResourceType: ResourceTypeType,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...,
         LockState: LockStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/paginators/#listrulespaginator)
         """
```

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/paginator.pyi` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -44,13 +44,13 @@
 
     def paginate(
         self,
         *,
         ResourceType: ResourceTypeType,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...,
         LockState: LockStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/paginators/#listrulespaginator)
         """
```

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/type_defs.py` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,29 +27,29 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ResourceTagTypeDef",
     "RetentionPeriodTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "UnlockDelayTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UnlockRuleRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "UpdateRuleResponseTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "LockConfigurationTypeDef",
     "ListRulesResponseTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "LockRuleRequestRequestTypeDef",
     "LockRuleResponseTypeDef",
@@ -87,49 +87,28 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -137,14 +116,35 @@
     "UnlockDelayTypeDef",
     {
         "UnlockDelayValue": int,
         "UnlockDelayUnit": Literal["DAYS"],
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
 UnlockRuleRequestRequestTypeDef = TypedDict(
     "UnlockRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -152,14 +152,38 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_RequiredListRulesRequestListRulesPaginateTypeDef",
+    {
+        "ResourceType": ResourceTypeType,
+    },
+)
+_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_OptionalListRulesRequestListRulesPaginateTypeDef",
+    {
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "LockState": LockStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRulesRequestListRulesPaginateTypeDef(
+    _RequiredListRulesRequestListRulesPaginateTypeDef,
+    _OptionalListRulesRequestListRulesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListRulesRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeType,
     },
 )
 _OptionalListRulesRequestRequestTypeDef = TypedDict(
@@ -211,82 +235,58 @@
 
 class UpdateRuleRequestRequestTypeDef(
     _RequiredUpdateRuleRequestRequestTypeDef, _OptionalUpdateRuleRequestRequestTypeDef
 ):
     pass
 
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateRuleResponseTypeDef = TypedDict(
     "UpdateRuleResponseTypeDef",
     {
         "Identifier": str,
         "RetentionPeriod": RetentionPeriodTypeDef,
         "Description": str,
         "ResourceType": ResourceTypeType,
         "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
         "LockState": LockStateType,
         "LockEndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_RequiredListRulesRequestListRulesPaginateTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResourceType": ResourceTypeType,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_OptionalListRulesRequestListRulesPaginateTypeDef",
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-        "LockState": LockStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
-
-class ListRulesRequestListRulesPaginateTypeDef(
-    _RequiredListRulesRequestListRulesPaginateTypeDef,
-    _OptionalListRulesRequestListRulesPaginateTypeDef,
-):
-    pass
-
-
 LockConfigurationTypeDef = TypedDict(
     "LockConfigurationTypeDef",
     {
         "UnlockDelay": UnlockDelayTypeDef,
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "Rules": List[RuleSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleRequestRequestTypeDef",
     {
         "RetentionPeriod": RetentionPeriodTypeDef,
@@ -319,15 +319,15 @@
         "Description": str,
         "Tags": List[TagTypeDef],
         "ResourceType": ResourceTypeType,
         "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
         "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "Identifier": str,
@@ -335,15 +335,15 @@
         "ResourceType": ResourceTypeType,
         "RetentionPeriod": RetentionPeriodTypeDef,
         "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
         "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
         "LockEndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LockRuleRequestRequestTypeDef = TypedDict(
     "LockRuleRequestRequestTypeDef",
     {
         "Identifier": str,
@@ -358,15 +358,15 @@
         "Description": str,
         "ResourceType": ResourceTypeType,
         "RetentionPeriod": RetentionPeriodTypeDef,
         "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
         "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UnlockRuleResponseTypeDef = TypedDict(
     "UnlockRuleResponseTypeDef",
     {
         "Identifier": str,
@@ -374,10 +374,10 @@
         "ResourceType": ResourceTypeType,
         "RetentionPeriod": RetentionPeriodTypeDef,
         "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
         "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
         "LockEndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin/type_defs.pyi` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -26,29 +26,29 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ResourceTagTypeDef",
     "RetentionPeriodTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "UnlockDelayTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UnlockRuleRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "UpdateRuleResponseTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "LockConfigurationTypeDef",
     "ListRulesResponseTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "LockRuleRequestRequestTypeDef",
     "LockRuleResponseTypeDef",
@@ -84,49 +84,28 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -134,14 +113,35 @@
     "UnlockDelayTypeDef",
     {
         "UnlockDelayValue": int,
         "UnlockDelayUnit": Literal["DAYS"],
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
 UnlockRuleRequestRequestTypeDef = TypedDict(
     "UnlockRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -149,14 +149,36 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_RequiredListRulesRequestListRulesPaginateTypeDef",
+    {
+        "ResourceType": ResourceTypeType,
+    },
+)
+_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_OptionalListRulesRequestListRulesPaginateTypeDef",
+    {
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "LockState": LockStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRulesRequestListRulesPaginateTypeDef(
+    _RequiredListRulesRequestListRulesPaginateTypeDef,
+    _OptionalListRulesRequestListRulesPaginateTypeDef,
+):
+    pass
+
 _RequiredListRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListRulesRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeType,
     },
 )
 _OptionalListRulesRequestRequestTypeDef = TypedDict(
@@ -204,80 +226,58 @@
 )
 
 class UpdateRuleRequestRequestTypeDef(
     _RequiredUpdateRuleRequestRequestTypeDef, _OptionalUpdateRuleRequestRequestTypeDef
 ):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateRuleResponseTypeDef = TypedDict(
     "UpdateRuleResponseTypeDef",
     {
         "Identifier": str,
         "RetentionPeriod": RetentionPeriodTypeDef,
         "Description": str,
         "ResourceType": ResourceTypeType,
         "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
         "LockState": LockStateType,
         "LockEndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_RequiredListRulesRequestListRulesPaginateTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResourceType": ResourceTypeType,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_OptionalListRulesRequestListRulesPaginateTypeDef",
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-        "LockState": LockStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
-class ListRulesRequestListRulesPaginateTypeDef(
-    _RequiredListRulesRequestListRulesPaginateTypeDef,
-    _OptionalListRulesRequestListRulesPaginateTypeDef,
-):
-    pass
-
 LockConfigurationTypeDef = TypedDict(
     "LockConfigurationTypeDef",
     {
         "UnlockDelay": UnlockDelayTypeDef,
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "Rules": List[RuleSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleRequestRequestTypeDef",
     {
         "RetentionPeriod": RetentionPeriodTypeDef,
@@ -308,15 +308,15 @@
         "Description": str,
         "Tags": List[TagTypeDef],
         "ResourceType": ResourceTypeType,
         "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
         "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "Identifier": str,
@@ -324,15 +324,15 @@
         "ResourceType": ResourceTypeType,
         "RetentionPeriod": RetentionPeriodTypeDef,
         "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
         "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
         "LockEndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LockRuleRequestRequestTypeDef = TypedDict(
     "LockRuleRequestRequestTypeDef",
     {
         "Identifier": str,
@@ -347,15 +347,15 @@
         "Description": str,
         "ResourceType": ResourceTypeType,
         "RetentionPeriod": RetentionPeriodTypeDef,
         "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
         "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UnlockRuleResponseTypeDef = TypedDict(
     "UnlockRuleResponseTypeDef",
     {
         "Identifier": str,
@@ -363,10 +363,10 @@
         "ResourceType": ResourceTypeType,
         "RetentionPeriod": RetentionPeriodTypeDef,
         "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
         "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
         "LockEndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin.egg-info/PKG-INFO` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rbin
-Version: 1.26.16
-Summary: Type annotations for boto3.RecycleBin 1.26.16 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.RecycleBin 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/
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
 
 <a id="mypy-boto3-rbin"></a>
 
 # mypy-boto3-rbin
 
 [![PyPI - mypy-boto3-rbin](https://img.shields.io/pypi/v/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rbin?color=blue)](https://pypistats.org/packages/mypy-boto3-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RecycleBin 1.26.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[boto3.RecycleBin 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [mypy-boto3-rbin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,29 +326,29 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rbin.type_defs import (
     ResourceTagTypeDef,
     RetentionPeriodTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     DeleteRuleRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     UnlockDelayTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UnlockRuleRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdateRuleResponseTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     LockConfigurationTypeDef,
     ListRulesResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     LockRuleRequestRequestTypeDef,
     LockRuleResponseTypeDef,
@@ -362,42 +363,42 @@
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

### Comparing `mypy-boto3-rbin-1.26.16/mypy_boto3_rbin.egg-info/SOURCES.txt` & `mypy-boto3-rbin-1.27.0/mypy_boto3_rbin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.26.16/setup.py` & `mypy-boto3-rbin-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-rbin.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rbin",
-    version="1.26.16",
+    version="1.27.0",
     packages=["mypy_boto3_rbin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RecycleBin 1.26.16 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.RecycleBin 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 rbin type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_rbin": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_rbin": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/",
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


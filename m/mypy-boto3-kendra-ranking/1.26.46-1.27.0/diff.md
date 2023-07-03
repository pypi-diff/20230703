# Comparing `tmp/mypy-boto3-kendra-ranking-1.26.46.tar.gz` & `tmp/mypy-boto3-kendra-ranking-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kendra-ranking-1.26.46.tar", last modified: Mon Jan  9 20:27:39 2023, max compression
+gzip compressed data, was "mypy-boto3-kendra-ranking-1.27.0.tar", last modified: Mon Jul  3 19:50:58 2023, max compression
```

## Comparing `mypy-boto3-kendra-ranking-1.26.46.tar` & `mypy-boto3-kendra-ranking-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.388431 mypy-boto3-kendra-ranking-1.26.46/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-01-09 20:27:39.388431 mypy-boto3-kendra-ranking-1.26.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.384431 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.388431 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-01-09 20:27:39.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-01-09 20:27:39.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-09 20:27:39.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-09 20:27:39.000000 mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 20:27:39.388431 mypy-boto3-kendra-ranking-1.26.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-01-09 20:27:25.000000 mypy-boto3-kendra-ranking-1.26.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:58.543504 mypy-boto3-kendra-ranking-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:15.000000 mypy-boto3-kendra-ranking-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-07-03 19:50:58.543504 mypy-boto3-kendra-ranking-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-07-03 19:40:15.000000 mypy-boto3-kendra-ranking-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:58.543504 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-03 19:40:15.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-03 19:40:15.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:40:15.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-07-03 19:40:15.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-03 19:40:15.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-07-03 19:40:16.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-07-03 19:40:15.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:15.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-03 19:40:16.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-03 19:40:16.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:15.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:58.543504 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-07-03 19:50:58.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 19:50:58.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:58.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:58.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:58.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:50:58.000000 mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:58.543504 mypy-boto3-kendra-ranking-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-03 19:40:15.000000 mypy-boto3-kendra-ranking-1.27.0/setup.py
```

### Comparing `mypy-boto3-kendra-ranking-1.26.46/LICENSE` & `mypy-boto3-kendra-ranking-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-kendra-ranking-1.26.46/PKG-INFO` & `mypy-boto3-kendra-ranking-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra-ranking
-Version: 1.26.46
-Summary: Type annotations for boto3.KendraRanking 1.26.46 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.KendraRanking 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-kendra-ranking"></a>
 
 # mypy-boto3-kendra-ranking
 
 [![PyPI - mypy-boto3-kendra-ranking](https://img.shields.io/pypi/v/mypy-boto3-kendra-ranking.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra-ranking)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra-ranking.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra-ranking)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra-ranking?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra-ranking)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KendraRanking 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
+[boto3.KendraRanking 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kendra-ranking docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,14 +281,15 @@
 
 ```python
 from mypy_boto3_kendra_ranking.literals import (
     RescoreExecutionPlanStatusType,
     KendraRankingServiceName,
     ServiceName,
     ResourceServiceName,
+    RegionName,
 )
 
 
 def check_value(value: RescoreExecutionPlanStatusType) -> bool:
     ...
 ```
 
@@ -299,30 +300,30 @@
 `mypy_boto3_kendra_ranking.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kendra_ranking.type_defs import (
     CapacityUnitsConfigurationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateRescoreExecutionPlanResponseTypeDef,
     DeleteRescoreExecutionPlanRequestRequestTypeDef,
     DescribeRescoreExecutionPlanRequestRequestTypeDef,
     DocumentTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListRescoreExecutionPlansRequestRequestTypeDef,
     RescoreExecutionPlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RescoreResultItemTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    DescribeRescoreExecutionPlanResponseTypeDef,
     UpdateRescoreExecutionPlanRequestRequestTypeDef,
     CreateRescoreExecutionPlanRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateRescoreExecutionPlanResponseTypeDef,
-    DescribeRescoreExecutionPlanResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     RescoreRequestRequestTypeDef,
     ListRescoreExecutionPlansResponseTypeDef,
     RescoreResultTypeDef,
 )
 
 
 def get_structure() -> CapacityUnitsConfigurationTypeDef:
@@ -332,42 +333,42 @@
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

### Comparing `mypy-boto3-kendra-ranking-1.26.46/README.md` & `mypy-boto3-kendra-ranking-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-kendra-ranking"></a>
 
 # mypy-boto3-kendra-ranking
 
 [![PyPI - mypy-boto3-kendra-ranking](https://img.shields.io/pypi/v/mypy-boto3-kendra-ranking.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra-ranking)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra-ranking.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra-ranking)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra-ranking?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra-ranking)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KendraRanking 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
+[boto3.KendraRanking 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kendra-ranking docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/).
 
 See how it helps to find and fix potential bugs:
 
@@ -249,14 +249,15 @@
 
 ```python
 from mypy_boto3_kendra_ranking.literals import (
     RescoreExecutionPlanStatusType,
     KendraRankingServiceName,
     ServiceName,
     ResourceServiceName,
+    RegionName,
 )
 
 
 def check_value(value: RescoreExecutionPlanStatusType) -> bool:
     ...
 ```
 
@@ -267,30 +268,30 @@
 `mypy_boto3_kendra_ranking.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kendra_ranking.type_defs import (
     CapacityUnitsConfigurationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateRescoreExecutionPlanResponseTypeDef,
     DeleteRescoreExecutionPlanRequestRequestTypeDef,
     DescribeRescoreExecutionPlanRequestRequestTypeDef,
     DocumentTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListRescoreExecutionPlansRequestRequestTypeDef,
     RescoreExecutionPlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RescoreResultItemTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    DescribeRescoreExecutionPlanResponseTypeDef,
     UpdateRescoreExecutionPlanRequestRequestTypeDef,
     CreateRescoreExecutionPlanRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateRescoreExecutionPlanResponseTypeDef,
-    DescribeRescoreExecutionPlanResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     RescoreRequestRequestTypeDef,
     ListRescoreExecutionPlansResponseTypeDef,
     RescoreResultTypeDef,
 )
 
 
 def get_structure() -> CapacityUnitsConfigurationTypeDef:
@@ -300,42 +301,42 @@
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

### Comparing `mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/__main__.py` & `mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KendraRanking 1.26.46\nVersion:         1.26.46\nBuilder"
-        " version: 7.12.2\nDocs:           "
+        "Type annotations for boto3.KendraRanking 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.46")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/client.py` & `mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/client.pyi` & `mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/literals.py` & `mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/literals.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 __all__ = (
     "RescoreExecutionPlanStatusType",
     "KendraRankingServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "RegionName",
 )
 
 
 RescoreExecutionPlanStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 KendraRankingServiceName = Literal["kendra-ranking"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -40,14 +41,15 @@
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
@@ -68,31 +70,34 @@
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
@@ -171,14 +176,15 @@
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
@@ -189,14 +195,15 @@
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
@@ -232,14 +239,15 @@
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
@@ -258,16 +266,19 @@
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
@@ -347,18 +358,21 @@
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
@@ -376,7 +390,34 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+RegionName = Literal[
+    "af-south-1",
+    "ap-east-1",
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-northeast-3",
+    "ap-south-1",
+    "ap-south-2",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
+    "ca-central-1",
+    "eu-central-2",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
+    "eu-west-1",
+    "eu-west-3",
+    "me-central-1",
+    "me-south-1",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/literals.pyi` & `mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/literals.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     from typing_extensions import Literal
 
 __all__ = (
     "RescoreExecutionPlanStatusType",
     "KendraRankingServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "RegionName",
 )
 
 RescoreExecutionPlanStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 KendraRankingServiceName = Literal["kendra-ranking"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -38,14 +39,15 @@
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
@@ -66,31 +68,34 @@
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
@@ -169,14 +174,15 @@
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
@@ -187,14 +193,15 @@
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
@@ -230,14 +237,15 @@
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
@@ -256,16 +264,19 @@
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
@@ -345,18 +356,21 @@
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
@@ -374,7 +388,34 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+RegionName = Literal[
+    "af-south-1",
+    "ap-east-1",
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-northeast-3",
+    "ap-south-1",
+    "ap-south-2",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
+    "ca-central-1",
+    "eu-central-2",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
+    "eu-west-1",
+    "eu-west-3",
+    "me-central-1",
+    "me-south-1",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/type_defs.py` & `mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -18,34 +18,33 @@
 from .literals import RescoreExecutionPlanStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CapacityUnitsConfigurationTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateRescoreExecutionPlanResponseTypeDef",
     "DeleteRescoreExecutionPlanRequestRequestTypeDef",
     "DescribeRescoreExecutionPlanRequestRequestTypeDef",
     "DocumentTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListRescoreExecutionPlansRequestRequestTypeDef",
     "RescoreExecutionPlanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RescoreResultItemTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "DescribeRescoreExecutionPlanResponseTypeDef",
     "UpdateRescoreExecutionPlanRequestRequestTypeDef",
     "CreateRescoreExecutionPlanRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateRescoreExecutionPlanResponseTypeDef",
-    "DescribeRescoreExecutionPlanResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "RescoreRequestRequestTypeDef",
     "ListRescoreExecutionPlansResponseTypeDef",
     "RescoreResultTypeDef",
 )
 
 CapacityUnitsConfigurationTypeDef = TypedDict(
     "CapacityUnitsConfigurationTypeDef",
@@ -58,22 +57,20 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateRescoreExecutionPlanResponseTypeDef = TypedDict(
+    "CreateRescoreExecutionPlanResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Id": str,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRescoreExecutionPlanRequestRequestTypeDef = TypedDict(
     "DeleteRescoreExecutionPlanRequestRequestTypeDef",
     {
         "Id": str,
@@ -102,18 +99,23 @@
         "Body": str,
         "TokenizedTitle": Sequence[str],
         "TokenizedBody": Sequence[str],
     },
     total=False,
 )
 
-
 class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ListRescoreExecutionPlansRequestRequestTypeDef = TypedDict(
     "ListRescoreExecutionPlansRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
@@ -144,22 +146,49 @@
     {
         "DocumentId": str,
         "Score": float,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+DescribeRescoreExecutionPlanResponseTypeDef = TypedDict(
+    "DescribeRescoreExecutionPlanResponseTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "Status": RescoreExecutionPlanStatusType,
+        "ErrorMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateRescoreExecutionPlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRescoreExecutionPlanRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateRescoreExecutionPlanRequestRequestTypeDef = TypedDict(
@@ -168,22 +197,20 @@
         "Name": str,
         "Description": str,
         "CapacityUnits": CapacityUnitsConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateRescoreExecutionPlanRequestRequestTypeDef(
     _RequiredUpdateRescoreExecutionPlanRequestRequestTypeDef,
     _OptionalUpdateRescoreExecutionPlanRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateRescoreExecutionPlanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRescoreExecutionPlanRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateRescoreExecutionPlanRequestRequestTypeDef = TypedDict(
@@ -193,89 +220,55 @@
         "CapacityUnits": CapacityUnitsConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateRescoreExecutionPlanRequestRequestTypeDef(
     _RequiredCreateRescoreExecutionPlanRequestRequestTypeDef,
     _OptionalCreateRescoreExecutionPlanRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateRescoreExecutionPlanResponseTypeDef = TypedDict(
-    "CreateRescoreExecutionPlanResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRescoreExecutionPlanResponseTypeDef = TypedDict(
-    "DescribeRescoreExecutionPlanResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "Status": RescoreExecutionPlanStatusType,
-        "ErrorMessage": str,
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
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RescoreRequestRequestTypeDef = TypedDict(
     "RescoreRequestRequestTypeDef",
     {
         "RescoreExecutionPlanId": str,
         "SearchQuery": str,
         "Documents": Sequence[DocumentTypeDef],
     },
 )
 
 ListRescoreExecutionPlansResponseTypeDef = TypedDict(
     "ListRescoreExecutionPlansResponseTypeDef",
     {
         "SummaryItems": List[RescoreExecutionPlanSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RescoreResultTypeDef = TypedDict(
     "RescoreResultTypeDef",
     {
         "RescoreId": str,
         "ResultItems": List[RescoreResultItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking/type_defs.pyi` & `mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,33 +18,34 @@
 from .literals import RescoreExecutionPlanStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CapacityUnitsConfigurationTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateRescoreExecutionPlanResponseTypeDef",
     "DeleteRescoreExecutionPlanRequestRequestTypeDef",
     "DescribeRescoreExecutionPlanRequestRequestTypeDef",
     "DocumentTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListRescoreExecutionPlansRequestRequestTypeDef",
     "RescoreExecutionPlanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RescoreResultItemTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "DescribeRescoreExecutionPlanResponseTypeDef",
     "UpdateRescoreExecutionPlanRequestRequestTypeDef",
     "CreateRescoreExecutionPlanRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateRescoreExecutionPlanResponseTypeDef",
-    "DescribeRescoreExecutionPlanResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "RescoreRequestRequestTypeDef",
     "ListRescoreExecutionPlansResponseTypeDef",
     "RescoreResultTypeDef",
 )
 
 CapacityUnitsConfigurationTypeDef = TypedDict(
     "CapacityUnitsConfigurationTypeDef",
@@ -57,22 +58,20 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateRescoreExecutionPlanResponseTypeDef = TypedDict(
+    "CreateRescoreExecutionPlanResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Id": str,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRescoreExecutionPlanRequestRequestTypeDef = TypedDict(
     "DeleteRescoreExecutionPlanRequestRequestTypeDef",
     {
         "Id": str,
@@ -101,17 +100,26 @@
         "Body": str,
         "TokenizedTitle": Sequence[str],
         "TokenizedBody": Sequence[str],
     },
     total=False,
 )
 
+
 class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
     pass
 
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListRescoreExecutionPlansRequestRequestTypeDef = TypedDict(
     "ListRescoreExecutionPlansRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -141,22 +149,49 @@
     {
         "DocumentId": str,
         "Score": float,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+DescribeRescoreExecutionPlanResponseTypeDef = TypedDict(
+    "DescribeRescoreExecutionPlanResponseTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "Status": RescoreExecutionPlanStatusType,
+        "ErrorMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateRescoreExecutionPlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRescoreExecutionPlanRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateRescoreExecutionPlanRequestRequestTypeDef = TypedDict(
@@ -165,20 +200,22 @@
         "Name": str,
         "Description": str,
         "CapacityUnits": CapacityUnitsConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateRescoreExecutionPlanRequestRequestTypeDef(
     _RequiredUpdateRescoreExecutionPlanRequestRequestTypeDef,
     _OptionalUpdateRescoreExecutionPlanRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateRescoreExecutionPlanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRescoreExecutionPlanRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateRescoreExecutionPlanRequestRequestTypeDef = TypedDict(
@@ -188,65 +225,35 @@
         "CapacityUnits": CapacityUnitsConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateRescoreExecutionPlanRequestRequestTypeDef(
     _RequiredCreateRescoreExecutionPlanRequestRequestTypeDef,
     _OptionalCreateRescoreExecutionPlanRequestRequestTypeDef,
 ):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateRescoreExecutionPlanResponseTypeDef = TypedDict(
-    "CreateRescoreExecutionPlanResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRescoreExecutionPlanResponseTypeDef = TypedDict(
-    "DescribeRescoreExecutionPlanResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "Status": RescoreExecutionPlanStatusType,
-        "ErrorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 RescoreRequestRequestTypeDef = TypedDict(
     "RescoreRequestRequestTypeDef",
     {
         "RescoreExecutionPlanId": str,
@@ -256,19 +263,19 @@
 )
 
 ListRescoreExecutionPlansResponseTypeDef = TypedDict(
     "ListRescoreExecutionPlansResponseTypeDef",
     {
         "SummaryItems": List[RescoreExecutionPlanSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RescoreResultTypeDef = TypedDict(
     "RescoreResultTypeDef",
     {
         "RescoreId": str,
         "ResultItems": List[RescoreResultItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking.egg-info/PKG-INFO` & `mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra-ranking
-Version: 1.26.46
-Summary: Type annotations for boto3.KendraRanking 1.26.46 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.KendraRanking 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-kendra-ranking"></a>
 
 # mypy-boto3-kendra-ranking
 
 [![PyPI - mypy-boto3-kendra-ranking](https://img.shields.io/pypi/v/mypy-boto3-kendra-ranking.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra-ranking)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra-ranking.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra-ranking)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra-ranking?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra-ranking)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KendraRanking 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
+[boto3.KendraRanking 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kendra-ranking docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,14 +281,15 @@
 
 ```python
 from mypy_boto3_kendra_ranking.literals import (
     RescoreExecutionPlanStatusType,
     KendraRankingServiceName,
     ServiceName,
     ResourceServiceName,
+    RegionName,
 )
 
 
 def check_value(value: RescoreExecutionPlanStatusType) -> bool:
     ...
 ```
 
@@ -299,30 +300,30 @@
 `mypy_boto3_kendra_ranking.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kendra_ranking.type_defs import (
     CapacityUnitsConfigurationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateRescoreExecutionPlanResponseTypeDef,
     DeleteRescoreExecutionPlanRequestRequestTypeDef,
     DescribeRescoreExecutionPlanRequestRequestTypeDef,
     DocumentTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListRescoreExecutionPlansRequestRequestTypeDef,
     RescoreExecutionPlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RescoreResultItemTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    DescribeRescoreExecutionPlanResponseTypeDef,
     UpdateRescoreExecutionPlanRequestRequestTypeDef,
     CreateRescoreExecutionPlanRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateRescoreExecutionPlanResponseTypeDef,
-    DescribeRescoreExecutionPlanResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     RescoreRequestRequestTypeDef,
     ListRescoreExecutionPlansResponseTypeDef,
     RescoreResultTypeDef,
 )
 
 
 def get_structure() -> CapacityUnitsConfigurationTypeDef:
@@ -332,42 +333,42 @@
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

### Comparing `mypy-boto3-kendra-ranking-1.26.46/mypy_boto3_kendra_ranking.egg-info/SOURCES.txt` & `mypy-boto3-kendra-ranking-1.27.0/mypy_boto3_kendra_ranking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-ranking-1.26.46/setup.py` & `mypy-boto3-kendra-ranking-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-kendra-ranking.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kendra-ranking",
-    version="1.26.46",
+    version="1.27.0",
     packages=["mypy_boto3_kendra_ranking"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KendraRanking 1.26.46 service generated with mypy-boto3-builder"
-        " 7.12.2"
+        "Type annotations for boto3.KendraRanking 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/",
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


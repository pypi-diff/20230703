# Comparing `tmp/mypy-boto3-route53-recovery-readiness-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-route53-recovery-readiness-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-recovery-readiness-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:55 2022, max compression
+gzip compressed data, was "mypy-boto3-route53-recovery-readiness-1.27.0.tar", last modified: Mon Jul  3 19:51:21 2023, max compression
```

## Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1.tar` & `mypy-boto3-route53-recovery-readiness-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:55.712845 mypy-boto3-route53-recovery-readiness-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18993 2022-11-01 21:43:55.712845 mypy-boto3-route53-recovery-readiness-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17478 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:55.712845 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/
--rw-r--r--   0 runner    (1001) docker     (121)     2904 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28532 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    28483 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8579 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8577 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13220 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    13208 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    29755 2022-11-01 21:40:15.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    29718 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:55.712845 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18993 2022-11-01 21:43:55.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-11-01 21:43:55.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:55.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:55.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:55.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:55.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:55.712845 mypy-boto3-route53-recovery-readiness-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2139 2022-11-01 21:40:14.000000 mypy-boto3-route53-recovery-readiness-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.887905 mypy-boto3-route53-recovery-readiness-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:33.000000 mypy-boto3-route53-recovery-readiness-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19034 2023-07-03 19:51:21.883905 mypy-boto3-route53-recovery-readiness-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17475 2023-07-03 19:46:33.000000 mypy-boto3-route53-recovery-readiness-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.883905 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-03 19:46:33.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-03 19:46:33.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-03 19:46:33.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-07-03 19:46:34.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28483 2023-07-03 19:46:34.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-07-03 19:46:34.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-07-03 19:46:34.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-07-03 19:46:34.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-07-03 19:46:34.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:33.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29827 2023-07-03 19:46:34.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29790 2023-07-03 19:46:34.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:33.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.883905 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19034 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:21.887905 mypy-boto3-route53-recovery-readiness-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-03 19:46:33.000000 mypy-boto3-route53-recovery-readiness-1.27.0/setup.py
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/LICENSE` & `mypy-boto3-route53-recovery-readiness-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/PKG-INFO` & `mypy-boto3-route53-recovery-readiness-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-readiness
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Route53RecoveryReadiness 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Route53RecoveryReadiness 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/
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
 
 <a id="mypy-boto3-route53-recovery-readiness"></a>
 
 # mypy-boto3-route53-recovery-readiness
 
 [![PyPI - mypy-boto3-route53-recovery-readiness](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-readiness?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryReadiness 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[boto3.Route53RecoveryReadiness 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,79 +365,79 @@
 `mypy_boto3_route53_recovery_readiness.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53_recovery_readiness.type_defs import (
     CellOutputTypeDef,
     CreateCellRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateCellResponseTypeDef,
     CreateCrossAccountAuthorizationRequestRequestTypeDef,
+    CreateCrossAccountAuthorizationResponseTypeDef,
     CreateReadinessCheckRequestRequestTypeDef,
+    CreateReadinessCheckResponseTypeDef,
     CreateRecoveryGroupRequestRequestTypeDef,
+    CreateRecoveryGroupResponseTypeDef,
     DeleteCellRequestRequestTypeDef,
     DeleteCrossAccountAuthorizationRequestRequestTypeDef,
     DeleteReadinessCheckRequestRequestTypeDef,
     DeleteRecoveryGroupRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetArchitectureRecommendationsRequestRequestTypeDef,
     RecommendationTypeDef,
-    PaginatorConfigTypeDef,
+    GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
     GetCellReadinessSummaryRequestRequestTypeDef,
     ReadinessCheckSummaryTypeDef,
     GetCellRequestRequestTypeDef,
+    GetCellResponseTypeDef,
     GetReadinessCheckRequestRequestTypeDef,
+    GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
     GetReadinessCheckResourceStatusRequestRequestTypeDef,
+    GetReadinessCheckResponseTypeDef,
+    GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
     GetReadinessCheckStatusRequestRequestTypeDef,
     MessageTypeDef,
     ResourceResultTypeDef,
+    GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
     GetRecoveryGroupReadinessSummaryRequestRequestTypeDef,
     GetRecoveryGroupRequestRequestTypeDef,
+    GetRecoveryGroupResponseTypeDef,
     GetResourceSetRequestRequestTypeDef,
+    ListCellsRequestListCellsPaginateTypeDef,
     ListCellsRequestRequestTypeDef,
+    ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef,
     ListCrossAccountAuthorizationsRequestRequestTypeDef,
+    ListCrossAccountAuthorizationsResponseTypeDef,
+    ListReadinessChecksRequestListReadinessChecksPaginateTypeDef,
     ListReadinessChecksRequestRequestTypeDef,
     ReadinessCheckOutputTypeDef,
+    ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef,
     ListRecoveryGroupsRequestRequestTypeDef,
     RecoveryGroupOutputTypeDef,
+    ListResourceSetsRequestListResourceSetsPaginateTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ListRulesOutputTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
+    ListTagsForResourcesResponseTypeDef,
     NLBResourceTypeDef,
+    PaginatorConfigTypeDef,
     R53ResourceRecordTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCellRequestRequestTypeDef,
-    UpdateReadinessCheckRequestRequestTypeDef,
-    UpdateRecoveryGroupRequestRequestTypeDef,
-    CreateCellResponseTypeDef,
-    CreateCrossAccountAuthorizationResponseTypeDef,
-    CreateReadinessCheckResponseTypeDef,
-    CreateRecoveryGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCellResponseTypeDef,
-    GetReadinessCheckResponseTypeDef,
-    GetRecoveryGroupResponseTypeDef,
-    ListCellsResponseTypeDef,
-    ListCrossAccountAuthorizationsResponseTypeDef,
-    ListTagsForResourcesResponseTypeDef,
     UpdateCellResponseTypeDef,
+    UpdateReadinessCheckRequestRequestTypeDef,
     UpdateReadinessCheckResponseTypeDef,
+    UpdateRecoveryGroupRequestRequestTypeDef,
     UpdateRecoveryGroupResponseTypeDef,
+    ListCellsResponseTypeDef,
     GetArchitectureRecommendationsResponseTypeDef,
-    GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
-    GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
-    GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
-    GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
-    ListCellsRequestListCellsPaginateTypeDef,
-    ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef,
-    ListReadinessChecksRequestListReadinessChecksPaginateTypeDef,
-    ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef,
-    ListResourceSetsRequestListResourceSetsPaginateTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     GetCellReadinessSummaryResponseTypeDef,
     GetRecoveryGroupReadinessSummaryResponseTypeDef,
     RuleResultTypeDef,
     GetReadinessCheckStatusResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListRulesResponseTypeDef,
@@ -461,42 +462,42 @@
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

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/README.md` & `mypy-boto3-route53-recovery-readiness-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-route53-recovery-readiness"></a>
 
 # mypy-boto3-route53-recovery-readiness
 
 [![PyPI - mypy-boto3-route53-recovery-readiness](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-readiness?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryReadiness 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[boto3.Route53RecoveryReadiness 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,79 +333,79 @@
 `mypy_boto3_route53_recovery_readiness.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53_recovery_readiness.type_defs import (
     CellOutputTypeDef,
     CreateCellRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateCellResponseTypeDef,
     CreateCrossAccountAuthorizationRequestRequestTypeDef,
+    CreateCrossAccountAuthorizationResponseTypeDef,
     CreateReadinessCheckRequestRequestTypeDef,
+    CreateReadinessCheckResponseTypeDef,
     CreateRecoveryGroupRequestRequestTypeDef,
+    CreateRecoveryGroupResponseTypeDef,
     DeleteCellRequestRequestTypeDef,
     DeleteCrossAccountAuthorizationRequestRequestTypeDef,
     DeleteReadinessCheckRequestRequestTypeDef,
     DeleteRecoveryGroupRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetArchitectureRecommendationsRequestRequestTypeDef,
     RecommendationTypeDef,
-    PaginatorConfigTypeDef,
+    GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
     GetCellReadinessSummaryRequestRequestTypeDef,
     ReadinessCheckSummaryTypeDef,
     GetCellRequestRequestTypeDef,
+    GetCellResponseTypeDef,
     GetReadinessCheckRequestRequestTypeDef,
+    GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
     GetReadinessCheckResourceStatusRequestRequestTypeDef,
+    GetReadinessCheckResponseTypeDef,
+    GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
     GetReadinessCheckStatusRequestRequestTypeDef,
     MessageTypeDef,
     ResourceResultTypeDef,
+    GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
     GetRecoveryGroupReadinessSummaryRequestRequestTypeDef,
     GetRecoveryGroupRequestRequestTypeDef,
+    GetRecoveryGroupResponseTypeDef,
     GetResourceSetRequestRequestTypeDef,
+    ListCellsRequestListCellsPaginateTypeDef,
     ListCellsRequestRequestTypeDef,
+    ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef,
     ListCrossAccountAuthorizationsRequestRequestTypeDef,
+    ListCrossAccountAuthorizationsResponseTypeDef,
+    ListReadinessChecksRequestListReadinessChecksPaginateTypeDef,
     ListReadinessChecksRequestRequestTypeDef,
     ReadinessCheckOutputTypeDef,
+    ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef,
     ListRecoveryGroupsRequestRequestTypeDef,
     RecoveryGroupOutputTypeDef,
+    ListResourceSetsRequestListResourceSetsPaginateTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ListRulesOutputTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
+    ListTagsForResourcesResponseTypeDef,
     NLBResourceTypeDef,
+    PaginatorConfigTypeDef,
     R53ResourceRecordTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCellRequestRequestTypeDef,
-    UpdateReadinessCheckRequestRequestTypeDef,
-    UpdateRecoveryGroupRequestRequestTypeDef,
-    CreateCellResponseTypeDef,
-    CreateCrossAccountAuthorizationResponseTypeDef,
-    CreateReadinessCheckResponseTypeDef,
-    CreateRecoveryGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCellResponseTypeDef,
-    GetReadinessCheckResponseTypeDef,
-    GetRecoveryGroupResponseTypeDef,
-    ListCellsResponseTypeDef,
-    ListCrossAccountAuthorizationsResponseTypeDef,
-    ListTagsForResourcesResponseTypeDef,
     UpdateCellResponseTypeDef,
+    UpdateReadinessCheckRequestRequestTypeDef,
     UpdateReadinessCheckResponseTypeDef,
+    UpdateRecoveryGroupRequestRequestTypeDef,
     UpdateRecoveryGroupResponseTypeDef,
+    ListCellsResponseTypeDef,
     GetArchitectureRecommendationsResponseTypeDef,
-    GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
-    GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
-    GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
-    GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
-    ListCellsRequestListCellsPaginateTypeDef,
-    ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef,
-    ListReadinessChecksRequestListReadinessChecksPaginateTypeDef,
-    ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef,
-    ListResourceSetsRequestListResourceSetsPaginateTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     GetCellReadinessSummaryResponseTypeDef,
     GetRecoveryGroupReadinessSummaryResponseTypeDef,
     RuleResultTypeDef,
     GetReadinessCheckStatusResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListRulesResponseTypeDef,
@@ -430,42 +430,42 @@
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

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/__init__.py` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/__init__.pyi` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/__main__.py` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53RecoveryReadiness 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.Route53RecoveryReadiness 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness\nOther"
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

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/client.py` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/client.pyi` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/literals.py` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,23 +61,25 @@
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
@@ -87,30 +89,35 @@
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
@@ -136,14 +143,15 @@
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
@@ -188,51 +196,57 @@
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
@@ -245,14 +259,15 @@
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
@@ -264,28 +279,35 @@
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
@@ -294,14 +316,15 @@
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
@@ -312,55 +335,64 @@
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

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/literals.pyi` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -59,23 +59,25 @@
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
@@ -85,30 +87,35 @@
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
@@ -134,14 +141,15 @@
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
@@ -186,51 +194,57 @@
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
@@ -243,14 +257,15 @@
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
@@ -262,28 +277,35 @@
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
@@ -292,14 +314,15 @@
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
@@ -310,55 +333,64 @@
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

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/paginator.py` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 class GetCellReadinessSummaryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetCellReadinessSummary)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getcellreadinesssummarypaginator)
     """
 
     def paginate(
-        self, *, CellName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CellName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCellReadinessSummaryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetCellReadinessSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getcellreadinesssummarypaginator)
         """
 
 
@@ -101,133 +101,133 @@
     """
 
     def paginate(
         self,
         *,
         ReadinessCheckName: str,
         ResourceIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetReadinessCheckResourceStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckResourceStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getreadinesscheckresourcestatuspaginator)
         """
 
 
 class GetReadinessCheckStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getreadinesscheckstatuspaginator)
     """
 
     def paginate(
-        self, *, ReadinessCheckName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReadinessCheckName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetReadinessCheckStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getreadinesscheckstatuspaginator)
         """
 
 
 class GetRecoveryGroupReadinessSummaryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetRecoveryGroupReadinessSummary)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getrecoverygroupreadinesssummarypaginator)
     """
 
     def paginate(
-        self, *, RecoveryGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, RecoveryGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRecoveryGroupReadinessSummaryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetRecoveryGroupReadinessSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getrecoverygroupreadinesssummarypaginator)
         """
 
 
 class ListCellsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCells)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcellspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCellsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCells.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcellspaginator)
         """
 
 
 class ListCrossAccountAuthorizationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCrossAccountAuthorizations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcrossaccountauthorizationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCrossAccountAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCrossAccountAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcrossaccountauthorizationspaginator)
         """
 
 
 class ListReadinessChecksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListReadinessChecks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listreadinesscheckspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReadinessChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListReadinessChecks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listreadinesscheckspaginator)
         """
 
 
 class ListRecoveryGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRecoveryGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrecoverygroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecoveryGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRecoveryGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrecoverygroupspaginator)
         """
 
 
 class ListResourceSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListResourceSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listresourcesetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListResourceSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listresourcesetspaginator)
         """
 
 
 class ListRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrulespaginator)
     """
 
     def paginate(
-        self, *, ResourceType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrulespaginator)
         """
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/paginator.pyi` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 class GetCellReadinessSummaryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetCellReadinessSummary)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getcellreadinesssummarypaginator)
     """
 
     def paginate(
-        self, *, CellName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CellName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCellReadinessSummaryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetCellReadinessSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getcellreadinesssummarypaginator)
         """
 
 class GetReadinessCheckResourceStatusPaginator(Paginator):
@@ -97,125 +97,125 @@
     """
 
     def paginate(
         self,
         *,
         ReadinessCheckName: str,
         ResourceIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetReadinessCheckResourceStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckResourceStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getreadinesscheckresourcestatuspaginator)
         """
 
 class GetReadinessCheckStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getreadinesscheckstatuspaginator)
     """
 
     def paginate(
-        self, *, ReadinessCheckName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReadinessCheckName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetReadinessCheckStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getreadinesscheckstatuspaginator)
         """
 
 class GetRecoveryGroupReadinessSummaryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetRecoveryGroupReadinessSummary)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getrecoverygroupreadinesssummarypaginator)
     """
 
     def paginate(
-        self, *, RecoveryGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, RecoveryGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRecoveryGroupReadinessSummaryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetRecoveryGroupReadinessSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getrecoverygroupreadinesssummarypaginator)
         """
 
 class ListCellsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCells)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcellspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCellsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCells.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcellspaginator)
         """
 
 class ListCrossAccountAuthorizationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCrossAccountAuthorizations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcrossaccountauthorizationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCrossAccountAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCrossAccountAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcrossaccountauthorizationspaginator)
         """
 
 class ListReadinessChecksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListReadinessChecks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listreadinesscheckspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReadinessChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListReadinessChecks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listreadinesscheckspaginator)
         """
 
 class ListRecoveryGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRecoveryGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrecoverygroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecoveryGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRecoveryGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrecoverygroupspaginator)
         """
 
 class ListResourceSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListResourceSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listresourcesetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListResourceSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listresourcesetspaginator)
         """
 
 class ListRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrulespaginator)
     """
 
     def paginate(
-        self, *, ResourceType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrulespaginator)
         """
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/type_defs.py` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,79 +22,79 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CellOutputTypeDef",
     "CreateCellRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateCellResponseTypeDef",
     "CreateCrossAccountAuthorizationRequestRequestTypeDef",
+    "CreateCrossAccountAuthorizationResponseTypeDef",
     "CreateReadinessCheckRequestRequestTypeDef",
+    "CreateReadinessCheckResponseTypeDef",
     "CreateRecoveryGroupRequestRequestTypeDef",
+    "CreateRecoveryGroupResponseTypeDef",
     "DeleteCellRequestRequestTypeDef",
     "DeleteCrossAccountAuthorizationRequestRequestTypeDef",
     "DeleteReadinessCheckRequestRequestTypeDef",
     "DeleteRecoveryGroupRequestRequestTypeDef",
     "DeleteResourceSetRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetArchitectureRecommendationsRequestRequestTypeDef",
     "RecommendationTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
     "GetCellReadinessSummaryRequestRequestTypeDef",
     "ReadinessCheckSummaryTypeDef",
     "GetCellRequestRequestTypeDef",
+    "GetCellResponseTypeDef",
     "GetReadinessCheckRequestRequestTypeDef",
+    "GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
     "GetReadinessCheckResourceStatusRequestRequestTypeDef",
+    "GetReadinessCheckResponseTypeDef",
+    "GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
     "GetReadinessCheckStatusRequestRequestTypeDef",
     "MessageTypeDef",
     "ResourceResultTypeDef",
+    "GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
     "GetRecoveryGroupReadinessSummaryRequestRequestTypeDef",
     "GetRecoveryGroupRequestRequestTypeDef",
+    "GetRecoveryGroupResponseTypeDef",
     "GetResourceSetRequestRequestTypeDef",
+    "ListCellsRequestListCellsPaginateTypeDef",
     "ListCellsRequestRequestTypeDef",
+    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
     "ListCrossAccountAuthorizationsRequestRequestTypeDef",
+    "ListCrossAccountAuthorizationsResponseTypeDef",
+    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
     "ListReadinessChecksRequestRequestTypeDef",
     "ReadinessCheckOutputTypeDef",
+    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
     "ListRecoveryGroupsRequestRequestTypeDef",
     "RecoveryGroupOutputTypeDef",
+    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ListRulesOutputTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "ListTagsForResourcesRequestRequestTypeDef",
+    "ListTagsForResourcesResponseTypeDef",
     "NLBResourceTypeDef",
+    "PaginatorConfigTypeDef",
     "R53ResourceRecordTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCellRequestRequestTypeDef",
-    "UpdateReadinessCheckRequestRequestTypeDef",
-    "UpdateRecoveryGroupRequestRequestTypeDef",
-    "CreateCellResponseTypeDef",
-    "CreateCrossAccountAuthorizationResponseTypeDef",
-    "CreateReadinessCheckResponseTypeDef",
-    "CreateRecoveryGroupResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetCellResponseTypeDef",
-    "GetReadinessCheckResponseTypeDef",
-    "GetRecoveryGroupResponseTypeDef",
-    "ListCellsResponseTypeDef",
-    "ListCrossAccountAuthorizationsResponseTypeDef",
-    "ListTagsForResourcesResponseTypeDef",
     "UpdateCellResponseTypeDef",
+    "UpdateReadinessCheckRequestRequestTypeDef",
     "UpdateReadinessCheckResponseTypeDef",
+    "UpdateRecoveryGroupRequestRequestTypeDef",
     "UpdateRecoveryGroupResponseTypeDef",
+    "ListCellsResponseTypeDef",
     "GetArchitectureRecommendationsResponseTypeDef",
-    "GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
-    "GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
-    "GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
-    "GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
-    "ListCellsRequestListCellsPaginateTypeDef",
-    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
-    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
-    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
-    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "GetCellReadinessSummaryResponseTypeDef",
     "GetRecoveryGroupReadinessSummaryResponseTypeDef",
     "RuleResultTypeDef",
     "GetReadinessCheckStatusResponseTypeDef",
     "ListReadinessChecksResponseTypeDef",
     "ListRecoveryGroupsResponseTypeDef",
     "ListRulesResponseTypeDef",
@@ -151,32 +151,41 @@
 
 class CreateCellRequestRequestTypeDef(
     _RequiredCreateCellRequestRequestTypeDef, _OptionalCreateCellRequestRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateCellResponseTypeDef = TypedDict(
+    "CreateCellResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "CellArn": str,
+        "CellName": str,
+        "Cells": List[str],
+        "ParentReadinessScopes": List[str],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCrossAccountAuthorizationRequestRequestTypeDef = TypedDict(
     "CreateCrossAccountAuthorizationRequestRequestTypeDef",
     {
         "CrossAccountAuthorization": str,
     },
 )
 
+CreateCrossAccountAuthorizationResponseTypeDef = TypedDict(
+    "CreateCrossAccountAuthorizationResponseTypeDef",
+    {
+        "CrossAccountAuthorization": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateReadinessCheckRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReadinessCheckRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
         "ResourceSetName": str,
     },
 )
@@ -192,14 +201,25 @@
 class CreateReadinessCheckRequestRequestTypeDef(
     _RequiredCreateReadinessCheckRequestRequestTypeDef,
     _OptionalCreateReadinessCheckRequestRequestTypeDef,
 ):
     pass
 
 
+CreateReadinessCheckResponseTypeDef = TypedDict(
+    "CreateReadinessCheckResponseTypeDef",
+    {
+        "ReadinessCheckArn": str,
+        "ReadinessCheckName": str,
+        "ResourceSet": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateRecoveryGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecoveryGroupRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 _OptionalCreateRecoveryGroupRequestRequestTypeDef = TypedDict(
@@ -215,14 +235,25 @@
 class CreateRecoveryGroupRequestRequestTypeDef(
     _RequiredCreateRecoveryGroupRequestRequestTypeDef,
     _OptionalCreateRecoveryGroupRequestRequestTypeDef,
 ):
     pass
 
 
+CreateRecoveryGroupResponseTypeDef = TypedDict(
+    "CreateRecoveryGroupResponseTypeDef",
+    {
+        "Cells": List[str],
+        "RecoveryGroupArn": str,
+        "RecoveryGroupName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteCellRequestRequestTypeDef = TypedDict(
     "DeleteCellRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 
@@ -250,14 +281,21 @@
 DeleteResourceSetRequestRequestTypeDef = TypedDict(
     "DeleteResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetArchitectureRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetArchitectureRecommendationsRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 _OptionalGetArchitectureRecommendationsRequestRequestTypeDef = TypedDict(
@@ -280,24 +318,36 @@
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "RecommendationText": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
+    "_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "CellName": str,
+    },
+)
+_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
+    "_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef(
+    _RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+    _OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetCellReadinessSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetCellReadinessSummaryRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 _OptionalGetCellReadinessSummaryRequestRequestTypeDef = TypedDict(
@@ -329,21 +379,56 @@
 GetCellRequestRequestTypeDef = TypedDict(
     "GetCellRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 
+GetCellResponseTypeDef = TypedDict(
+    "GetCellResponseTypeDef",
+    {
+        "CellArn": str,
+        "CellName": str,
+        "Cells": List[str],
+        "ParentReadinessScopes": List[str],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetReadinessCheckRequestRequestTypeDef = TypedDict(
     "GetReadinessCheckRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
     },
 )
 
+_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
+    "_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
+    {
+        "ReadinessCheckName": str,
+        "ResourceIdentifier": str,
+    },
+)
+_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
+    "_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef(
+    _RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
+    _OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetReadinessCheckResourceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetReadinessCheckResourceStatusRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
         "ResourceIdentifier": str,
     },
 )
@@ -360,14 +445,47 @@
 class GetReadinessCheckResourceStatusRequestRequestTypeDef(
     _RequiredGetReadinessCheckResourceStatusRequestRequestTypeDef,
     _OptionalGetReadinessCheckResourceStatusRequestRequestTypeDef,
 ):
     pass
 
 
+GetReadinessCheckResponseTypeDef = TypedDict(
+    "GetReadinessCheckResponseTypeDef",
+    {
+        "ReadinessCheckArn": str,
+        "ReadinessCheckName": str,
+        "ResourceSet": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
+    "_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
+    {
+        "ReadinessCheckName": str,
+    },
+)
+_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
+    "_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef(
+    _RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
+    _OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetReadinessCheckStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetReadinessCheckStatusRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
     },
 )
 _OptionalGetReadinessCheckStatusRequestRequestTypeDef = TypedDict(
@@ -412,14 +530,36 @@
 )
 
 
 class ResourceResultTypeDef(_RequiredResourceResultTypeDef, _OptionalResourceResultTypeDef):
     pass
 
 
+_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
+    "_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
+    {
+        "RecoveryGroupName": str,
+    },
+)
+_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
+    "_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef(
+    _RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
+    _OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetRecoveryGroupReadinessSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecoveryGroupReadinessSummaryRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 _OptionalGetRecoveryGroupReadinessSummaryRequestRequestTypeDef = TypedDict(
@@ -442,39 +582,83 @@
 GetRecoveryGroupRequestRequestTypeDef = TypedDict(
     "GetRecoveryGroupRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 
+GetRecoveryGroupResponseTypeDef = TypedDict(
+    "GetRecoveryGroupResponseTypeDef",
+    {
+        "Cells": List[str],
+        "RecoveryGroupArn": str,
+        "RecoveryGroupName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
     },
 )
 
+ListCellsRequestListCellsPaginateTypeDef = TypedDict(
+    "ListCellsRequestListCellsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCellsRequestRequestTypeDef = TypedDict(
     "ListCellsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef = TypedDict(
+    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCrossAccountAuthorizationsRequestRequestTypeDef = TypedDict(
     "ListCrossAccountAuthorizationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListCrossAccountAuthorizationsResponseTypeDef = TypedDict(
+    "ListCrossAccountAuthorizationsResponseTypeDef",
+    {
+        "CrossAccountAuthorizations": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListReadinessChecksRequestListReadinessChecksPaginateTypeDef = TypedDict(
+    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReadinessChecksRequestRequestTypeDef = TypedDict(
     "ListReadinessChecksRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -499,14 +683,22 @@
 
 class ReadinessCheckOutputTypeDef(
     _RequiredReadinessCheckOutputTypeDef, _OptionalReadinessCheckOutputTypeDef
 ):
     pass
 
 
+ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef = TypedDict(
+    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRecoveryGroupsRequestRequestTypeDef = TypedDict(
     "ListRecoveryGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -531,14 +723,22 @@
 
 class RecoveryGroupOutputTypeDef(
     _RequiredRecoveryGroupOutputTypeDef, _OptionalRecoveryGroupOutputTypeDef
 ):
     pass
 
 
+ListResourceSetsRequestListResourceSetsPaginateTypeDef = TypedDict(
+    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListResourceSetsRequestRequestTypeDef = TypedDict(
     "ListResourceSetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -549,14 +749,23 @@
     {
         "ResourceType": str,
         "RuleDescription": str,
         "RuleId": str,
     },
 )
 
+ListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "ListRulesRequestListRulesPaginateTypeDef",
+    {
+        "ResourceType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRulesRequestRequestTypeDef = TypedDict(
     "ListRulesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ResourceType": str,
     },
@@ -566,31 +775,60 @@
 ListTagsForResourcesRequestRequestTypeDef = TypedDict(
     "ListTagsForResourcesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourcesResponseTypeDef = TypedDict(
+    "ListTagsForResourcesResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NLBResourceTypeDef = TypedDict(
     "NLBResourceTypeDef",
     {
         "Arn": str,
     },
     total=False,
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
 R53ResourceRecordTypeDef = TypedDict(
     "R53ResourceRecordTypeDef",
     {
         "DomainName": str,
         "RecordSetId": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -607,338 +845,100 @@
     "UpdateCellRequestRequestTypeDef",
     {
         "CellName": str,
         "Cells": Sequence[str],
     },
 )
 
-UpdateReadinessCheckRequestRequestTypeDef = TypedDict(
-    "UpdateReadinessCheckRequestRequestTypeDef",
-    {
-        "ReadinessCheckName": str,
-        "ResourceSetName": str,
-    },
-)
-
-UpdateRecoveryGroupRequestRequestTypeDef = TypedDict(
-    "UpdateRecoveryGroupRequestRequestTypeDef",
-    {
-        "Cells": Sequence[str],
-        "RecoveryGroupName": str,
-    },
-)
-
-CreateCellResponseTypeDef = TypedDict(
-    "CreateCellResponseTypeDef",
+UpdateCellResponseTypeDef = TypedDict(
+    "UpdateCellResponseTypeDef",
     {
         "CellArn": str,
         "CellName": str,
         "Cells": List[str],
         "ParentReadinessScopes": List[str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCrossAccountAuthorizationResponseTypeDef = TypedDict(
-    "CreateCrossAccountAuthorizationResponseTypeDef",
+UpdateReadinessCheckRequestRequestTypeDef = TypedDict(
+    "UpdateReadinessCheckRequestRequestTypeDef",
     {
-        "CrossAccountAuthorization": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ReadinessCheckName": str,
+        "ResourceSetName": str,
     },
 )
 
-CreateReadinessCheckResponseTypeDef = TypedDict(
-    "CreateReadinessCheckResponseTypeDef",
+UpdateReadinessCheckResponseTypeDef = TypedDict(
+    "UpdateReadinessCheckResponseTypeDef",
     {
         "ReadinessCheckArn": str,
         "ReadinessCheckName": str,
         "ResourceSet": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateRecoveryGroupResponseTypeDef = TypedDict(
-    "CreateRecoveryGroupResponseTypeDef",
+UpdateRecoveryGroupRequestRequestTypeDef = TypedDict(
+    "UpdateRecoveryGroupRequestRequestTypeDef",
     {
-        "Cells": List[str],
-        "RecoveryGroupArn": str,
+        "Cells": Sequence[str],
         "RecoveryGroupName": str,
-        "Tags": Dict[str, str],
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
-GetCellResponseTypeDef = TypedDict(
-    "GetCellResponseTypeDef",
-    {
-        "CellArn": str,
-        "CellName": str,
-        "Cells": List[str],
-        "ParentReadinessScopes": List[str],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetReadinessCheckResponseTypeDef = TypedDict(
-    "GetReadinessCheckResponseTypeDef",
-    {
-        "ReadinessCheckArn": str,
-        "ReadinessCheckName": str,
-        "ResourceSet": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetRecoveryGroupResponseTypeDef = TypedDict(
-    "GetRecoveryGroupResponseTypeDef",
+UpdateRecoveryGroupResponseTypeDef = TypedDict(
+    "UpdateRecoveryGroupResponseTypeDef",
     {
         "Cells": List[str],
         "RecoveryGroupArn": str,
         "RecoveryGroupName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCellsResponseTypeDef = TypedDict(
     "ListCellsResponseTypeDef",
     {
         "Cells": List[CellOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCrossAccountAuthorizationsResponseTypeDef = TypedDict(
-    "ListCrossAccountAuthorizationsResponseTypeDef",
-    {
-        "CrossAccountAuthorizations": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourcesResponseTypeDef = TypedDict(
-    "ListTagsForResourcesResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateCellResponseTypeDef = TypedDict(
-    "UpdateCellResponseTypeDef",
-    {
-        "CellArn": str,
-        "CellName": str,
-        "Cells": List[str],
-        "ParentReadinessScopes": List[str],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateReadinessCheckResponseTypeDef = TypedDict(
-    "UpdateReadinessCheckResponseTypeDef",
-    {
-        "ReadinessCheckArn": str,
-        "ReadinessCheckName": str,
-        "ResourceSet": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRecoveryGroupResponseTypeDef = TypedDict(
-    "UpdateRecoveryGroupResponseTypeDef",
-    {
-        "Cells": List[str],
-        "RecoveryGroupArn": str,
-        "RecoveryGroupName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetArchitectureRecommendationsResponseTypeDef = TypedDict(
     "GetArchitectureRecommendationsResponseTypeDef",
     {
         "LastAuditTimestamp": datetime,
         "NextToken": str,
         "Recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
-    "_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
-    {
-        "CellName": str,
-    },
-)
-_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
-    "_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef(
-    _RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
-    _OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
-    "_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
-    {
-        "ReadinessCheckName": str,
-        "ResourceIdentifier": str,
-    },
-)
-_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
-    "_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef(
-    _RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
-    _OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
-    "_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
-    {
-        "ReadinessCheckName": str,
-    },
-)
-_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
-    "_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef(
-    _RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
-    _OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
-    "_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
-    {
-        "RecoveryGroupName": str,
-    },
-)
-_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
-    "_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef(
-    _RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
-    _OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
-):
-    pass
-
-
-ListCellsRequestListCellsPaginateTypeDef = TypedDict(
-    "ListCellsRequestListCellsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef = TypedDict(
-    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReadinessChecksRequestListReadinessChecksPaginateTypeDef = TypedDict(
-    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef = TypedDict(
-    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListResourceSetsRequestListResourceSetsPaginateTypeDef = TypedDict(
-    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "ListRulesRequestListRulesPaginateTypeDef",
-    {
-        "ResourceType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 GetCellReadinessSummaryResponseTypeDef = TypedDict(
     "GetCellReadinessSummaryResponseTypeDef",
     {
         "NextToken": str,
         "Readiness": ReadinessType,
         "ReadinessChecks": List[ReadinessCheckSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecoveryGroupReadinessSummaryResponseTypeDef = TypedDict(
     "GetRecoveryGroupReadinessSummaryResponseTypeDef",
     {
         "NextToken": str,
         "Readiness": ReadinessType,
         "ReadinessChecks": List[ReadinessCheckSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleResultTypeDef = TypedDict(
     "RuleResultTypeDef",
     {
         "LastCheckedTimestamp": datetime,
@@ -951,42 +951,42 @@
 GetReadinessCheckStatusResponseTypeDef = TypedDict(
     "GetReadinessCheckStatusResponseTypeDef",
     {
         "Messages": List[MessageTypeDef],
         "NextToken": str,
         "Readiness": ReadinessType,
         "Resources": List[ResourceResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReadinessChecksResponseTypeDef = TypedDict(
     "ListReadinessChecksResponseTypeDef",
     {
         "NextToken": str,
         "ReadinessChecks": List[ReadinessCheckOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecoveryGroupsResponseTypeDef = TypedDict(
     "ListRecoveryGroupsResponseTypeDef",
     {
         "NextToken": str,
         "RecoveryGroups": List[RecoveryGroupOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "NextToken": str,
         "Rules": List[ListRulesOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TargetResourceTypeDef = TypedDict(
     "TargetResourceTypeDef",
     {
         "NLBResource": NLBResourceTypeDef,
@@ -997,15 +997,15 @@
 
 GetReadinessCheckResourceStatusResponseTypeDef = TypedDict(
     "GetReadinessCheckResourceStatusResponseTypeDef",
     {
         "NextToken": str,
         "Readiness": ReadinessType,
         "Rules": List[RuleResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DNSTargetResourceTypeDef = TypedDict(
     "DNSTargetResourceTypeDef",
     {
         "DomainName": str,
@@ -1055,27 +1055,27 @@
     "CreateResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
         "Resources": List[ResourceTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
         "Resources": List[ResourceTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredResourceSetOutputTypeDef = TypedDict(
     "_RequiredResourceSetOutputTypeDef",
     {
         "ResourceSetArn": str,
@@ -1112,19 +1112,19 @@
     "UpdateResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
         "Resources": List[ResourceTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "NextToken": str,
         "ResourceSets": List[ResourceSetOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness/type_defs.pyi` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -21,79 +21,79 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CellOutputTypeDef",
     "CreateCellRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateCellResponseTypeDef",
     "CreateCrossAccountAuthorizationRequestRequestTypeDef",
+    "CreateCrossAccountAuthorizationResponseTypeDef",
     "CreateReadinessCheckRequestRequestTypeDef",
+    "CreateReadinessCheckResponseTypeDef",
     "CreateRecoveryGroupRequestRequestTypeDef",
+    "CreateRecoveryGroupResponseTypeDef",
     "DeleteCellRequestRequestTypeDef",
     "DeleteCrossAccountAuthorizationRequestRequestTypeDef",
     "DeleteReadinessCheckRequestRequestTypeDef",
     "DeleteRecoveryGroupRequestRequestTypeDef",
     "DeleteResourceSetRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetArchitectureRecommendationsRequestRequestTypeDef",
     "RecommendationTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
     "GetCellReadinessSummaryRequestRequestTypeDef",
     "ReadinessCheckSummaryTypeDef",
     "GetCellRequestRequestTypeDef",
+    "GetCellResponseTypeDef",
     "GetReadinessCheckRequestRequestTypeDef",
+    "GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
     "GetReadinessCheckResourceStatusRequestRequestTypeDef",
+    "GetReadinessCheckResponseTypeDef",
+    "GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
     "GetReadinessCheckStatusRequestRequestTypeDef",
     "MessageTypeDef",
     "ResourceResultTypeDef",
+    "GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
     "GetRecoveryGroupReadinessSummaryRequestRequestTypeDef",
     "GetRecoveryGroupRequestRequestTypeDef",
+    "GetRecoveryGroupResponseTypeDef",
     "GetResourceSetRequestRequestTypeDef",
+    "ListCellsRequestListCellsPaginateTypeDef",
     "ListCellsRequestRequestTypeDef",
+    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
     "ListCrossAccountAuthorizationsRequestRequestTypeDef",
+    "ListCrossAccountAuthorizationsResponseTypeDef",
+    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
     "ListReadinessChecksRequestRequestTypeDef",
     "ReadinessCheckOutputTypeDef",
+    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
     "ListRecoveryGroupsRequestRequestTypeDef",
     "RecoveryGroupOutputTypeDef",
+    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ListRulesOutputTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "ListTagsForResourcesRequestRequestTypeDef",
+    "ListTagsForResourcesResponseTypeDef",
     "NLBResourceTypeDef",
+    "PaginatorConfigTypeDef",
     "R53ResourceRecordTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCellRequestRequestTypeDef",
-    "UpdateReadinessCheckRequestRequestTypeDef",
-    "UpdateRecoveryGroupRequestRequestTypeDef",
-    "CreateCellResponseTypeDef",
-    "CreateCrossAccountAuthorizationResponseTypeDef",
-    "CreateReadinessCheckResponseTypeDef",
-    "CreateRecoveryGroupResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetCellResponseTypeDef",
-    "GetReadinessCheckResponseTypeDef",
-    "GetRecoveryGroupResponseTypeDef",
-    "ListCellsResponseTypeDef",
-    "ListCrossAccountAuthorizationsResponseTypeDef",
-    "ListTagsForResourcesResponseTypeDef",
     "UpdateCellResponseTypeDef",
+    "UpdateReadinessCheckRequestRequestTypeDef",
     "UpdateReadinessCheckResponseTypeDef",
+    "UpdateRecoveryGroupRequestRequestTypeDef",
     "UpdateRecoveryGroupResponseTypeDef",
+    "ListCellsResponseTypeDef",
     "GetArchitectureRecommendationsResponseTypeDef",
-    "GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
-    "GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
-    "GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
-    "GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
-    "ListCellsRequestListCellsPaginateTypeDef",
-    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
-    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
-    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
-    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "GetCellReadinessSummaryResponseTypeDef",
     "GetRecoveryGroupReadinessSummaryResponseTypeDef",
     "RuleResultTypeDef",
     "GetReadinessCheckStatusResponseTypeDef",
     "ListReadinessChecksResponseTypeDef",
     "ListRecoveryGroupsResponseTypeDef",
     "ListRulesResponseTypeDef",
@@ -146,32 +146,41 @@
 )
 
 class CreateCellRequestRequestTypeDef(
     _RequiredCreateCellRequestRequestTypeDef, _OptionalCreateCellRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateCellResponseTypeDef = TypedDict(
+    "CreateCellResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "CellArn": str,
+        "CellName": str,
+        "Cells": List[str],
+        "ParentReadinessScopes": List[str],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCrossAccountAuthorizationRequestRequestTypeDef = TypedDict(
     "CreateCrossAccountAuthorizationRequestRequestTypeDef",
     {
         "CrossAccountAuthorization": str,
     },
 )
 
+CreateCrossAccountAuthorizationResponseTypeDef = TypedDict(
+    "CreateCrossAccountAuthorizationResponseTypeDef",
+    {
+        "CrossAccountAuthorization": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateReadinessCheckRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReadinessCheckRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
         "ResourceSetName": str,
     },
 )
@@ -185,14 +194,25 @@
 
 class CreateReadinessCheckRequestRequestTypeDef(
     _RequiredCreateReadinessCheckRequestRequestTypeDef,
     _OptionalCreateReadinessCheckRequestRequestTypeDef,
 ):
     pass
 
+CreateReadinessCheckResponseTypeDef = TypedDict(
+    "CreateReadinessCheckResponseTypeDef",
+    {
+        "ReadinessCheckArn": str,
+        "ReadinessCheckName": str,
+        "ResourceSet": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateRecoveryGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecoveryGroupRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 _OptionalCreateRecoveryGroupRequestRequestTypeDef = TypedDict(
@@ -206,14 +226,25 @@
 
 class CreateRecoveryGroupRequestRequestTypeDef(
     _RequiredCreateRecoveryGroupRequestRequestTypeDef,
     _OptionalCreateRecoveryGroupRequestRequestTypeDef,
 ):
     pass
 
+CreateRecoveryGroupResponseTypeDef = TypedDict(
+    "CreateRecoveryGroupResponseTypeDef",
+    {
+        "Cells": List[str],
+        "RecoveryGroupArn": str,
+        "RecoveryGroupName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteCellRequestRequestTypeDef = TypedDict(
     "DeleteCellRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 
@@ -241,14 +272,21 @@
 DeleteResourceSetRequestRequestTypeDef = TypedDict(
     "DeleteResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetArchitectureRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetArchitectureRecommendationsRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 _OptionalGetArchitectureRecommendationsRequestRequestTypeDef = TypedDict(
@@ -269,24 +307,34 @@
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "RecommendationText": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
+    "_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "CellName": str,
+    },
+)
+_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
+    "_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef(
+    _RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+    _OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+):
+    pass
+
 _RequiredGetCellReadinessSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetCellReadinessSummaryRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 _OptionalGetCellReadinessSummaryRequestRequestTypeDef = TypedDict(
@@ -316,21 +364,54 @@
 GetCellRequestRequestTypeDef = TypedDict(
     "GetCellRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 
+GetCellResponseTypeDef = TypedDict(
+    "GetCellResponseTypeDef",
+    {
+        "CellArn": str,
+        "CellName": str,
+        "Cells": List[str],
+        "ParentReadinessScopes": List[str],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetReadinessCheckRequestRequestTypeDef = TypedDict(
     "GetReadinessCheckRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
     },
 )
 
+_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
+    "_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
+    {
+        "ReadinessCheckName": str,
+        "ResourceIdentifier": str,
+    },
+)
+_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
+    "_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef(
+    _RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
+    _OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
+):
+    pass
+
 _RequiredGetReadinessCheckResourceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetReadinessCheckResourceStatusRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
         "ResourceIdentifier": str,
     },
 )
@@ -345,14 +426,45 @@
 
 class GetReadinessCheckResourceStatusRequestRequestTypeDef(
     _RequiredGetReadinessCheckResourceStatusRequestRequestTypeDef,
     _OptionalGetReadinessCheckResourceStatusRequestRequestTypeDef,
 ):
     pass
 
+GetReadinessCheckResponseTypeDef = TypedDict(
+    "GetReadinessCheckResponseTypeDef",
+    {
+        "ReadinessCheckArn": str,
+        "ReadinessCheckName": str,
+        "ResourceSet": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
+    "_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
+    {
+        "ReadinessCheckName": str,
+    },
+)
+_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
+    "_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef(
+    _RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
+    _OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
+):
+    pass
+
 _RequiredGetReadinessCheckStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetReadinessCheckStatusRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
     },
 )
 _OptionalGetReadinessCheckStatusRequestRequestTypeDef = TypedDict(
@@ -393,14 +505,34 @@
     },
     total=False,
 )
 
 class ResourceResultTypeDef(_RequiredResourceResultTypeDef, _OptionalResourceResultTypeDef):
     pass
 
+_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
+    "_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
+    {
+        "RecoveryGroupName": str,
+    },
+)
+_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
+    "_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef(
+    _RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
+    _OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
+):
+    pass
+
 _RequiredGetRecoveryGroupReadinessSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecoveryGroupReadinessSummaryRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 _OptionalGetRecoveryGroupReadinessSummaryRequestRequestTypeDef = TypedDict(
@@ -421,39 +553,83 @@
 GetRecoveryGroupRequestRequestTypeDef = TypedDict(
     "GetRecoveryGroupRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 
+GetRecoveryGroupResponseTypeDef = TypedDict(
+    "GetRecoveryGroupResponseTypeDef",
+    {
+        "Cells": List[str],
+        "RecoveryGroupArn": str,
+        "RecoveryGroupName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
     },
 )
 
+ListCellsRequestListCellsPaginateTypeDef = TypedDict(
+    "ListCellsRequestListCellsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCellsRequestRequestTypeDef = TypedDict(
     "ListCellsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef = TypedDict(
+    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCrossAccountAuthorizationsRequestRequestTypeDef = TypedDict(
     "ListCrossAccountAuthorizationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListCrossAccountAuthorizationsResponseTypeDef = TypedDict(
+    "ListCrossAccountAuthorizationsResponseTypeDef",
+    {
+        "CrossAccountAuthorizations": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListReadinessChecksRequestListReadinessChecksPaginateTypeDef = TypedDict(
+    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReadinessChecksRequestRequestTypeDef = TypedDict(
     "ListReadinessChecksRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -476,14 +652,22 @@
 )
 
 class ReadinessCheckOutputTypeDef(
     _RequiredReadinessCheckOutputTypeDef, _OptionalReadinessCheckOutputTypeDef
 ):
     pass
 
+ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef = TypedDict(
+    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRecoveryGroupsRequestRequestTypeDef = TypedDict(
     "ListRecoveryGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -506,14 +690,22 @@
 )
 
 class RecoveryGroupOutputTypeDef(
     _RequiredRecoveryGroupOutputTypeDef, _OptionalRecoveryGroupOutputTypeDef
 ):
     pass
 
+ListResourceSetsRequestListResourceSetsPaginateTypeDef = TypedDict(
+    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListResourceSetsRequestRequestTypeDef = TypedDict(
     "ListResourceSetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -524,14 +716,23 @@
     {
         "ResourceType": str,
         "RuleDescription": str,
         "RuleId": str,
     },
 )
 
+ListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "ListRulesRequestListRulesPaginateTypeDef",
+    {
+        "ResourceType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRulesRequestRequestTypeDef = TypedDict(
     "ListRulesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ResourceType": str,
     },
@@ -541,31 +742,60 @@
 ListTagsForResourcesRequestRequestTypeDef = TypedDict(
     "ListTagsForResourcesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourcesResponseTypeDef = TypedDict(
+    "ListTagsForResourcesResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NLBResourceTypeDef = TypedDict(
     "NLBResourceTypeDef",
     {
         "Arn": str,
     },
     total=False,
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
 R53ResourceRecordTypeDef = TypedDict(
     "R53ResourceRecordTypeDef",
     {
         "DomainName": str,
         "RecordSetId": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -582,330 +812,100 @@
     "UpdateCellRequestRequestTypeDef",
     {
         "CellName": str,
         "Cells": Sequence[str],
     },
 )
 
-UpdateReadinessCheckRequestRequestTypeDef = TypedDict(
-    "UpdateReadinessCheckRequestRequestTypeDef",
-    {
-        "ReadinessCheckName": str,
-        "ResourceSetName": str,
-    },
-)
-
-UpdateRecoveryGroupRequestRequestTypeDef = TypedDict(
-    "UpdateRecoveryGroupRequestRequestTypeDef",
-    {
-        "Cells": Sequence[str],
-        "RecoveryGroupName": str,
-    },
-)
-
-CreateCellResponseTypeDef = TypedDict(
-    "CreateCellResponseTypeDef",
+UpdateCellResponseTypeDef = TypedDict(
+    "UpdateCellResponseTypeDef",
     {
         "CellArn": str,
         "CellName": str,
         "Cells": List[str],
         "ParentReadinessScopes": List[str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCrossAccountAuthorizationResponseTypeDef = TypedDict(
-    "CreateCrossAccountAuthorizationResponseTypeDef",
+UpdateReadinessCheckRequestRequestTypeDef = TypedDict(
+    "UpdateReadinessCheckRequestRequestTypeDef",
     {
-        "CrossAccountAuthorization": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ReadinessCheckName": str,
+        "ResourceSetName": str,
     },
 )
 
-CreateReadinessCheckResponseTypeDef = TypedDict(
-    "CreateReadinessCheckResponseTypeDef",
+UpdateReadinessCheckResponseTypeDef = TypedDict(
+    "UpdateReadinessCheckResponseTypeDef",
     {
         "ReadinessCheckArn": str,
         "ReadinessCheckName": str,
         "ResourceSet": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateRecoveryGroupResponseTypeDef = TypedDict(
-    "CreateRecoveryGroupResponseTypeDef",
+UpdateRecoveryGroupRequestRequestTypeDef = TypedDict(
+    "UpdateRecoveryGroupRequestRequestTypeDef",
     {
-        "Cells": List[str],
-        "RecoveryGroupArn": str,
+        "Cells": Sequence[str],
         "RecoveryGroupName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetCellResponseTypeDef = TypedDict(
-    "GetCellResponseTypeDef",
-    {
-        "CellArn": str,
-        "CellName": str,
-        "Cells": List[str],
-        "ParentReadinessScopes": List[str],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetReadinessCheckResponseTypeDef = TypedDict(
-    "GetReadinessCheckResponseTypeDef",
-    {
-        "ReadinessCheckArn": str,
-        "ReadinessCheckName": str,
-        "ResourceSet": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRecoveryGroupResponseTypeDef = TypedDict(
-    "GetRecoveryGroupResponseTypeDef",
+UpdateRecoveryGroupResponseTypeDef = TypedDict(
+    "UpdateRecoveryGroupResponseTypeDef",
     {
         "Cells": List[str],
         "RecoveryGroupArn": str,
         "RecoveryGroupName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCellsResponseTypeDef = TypedDict(
     "ListCellsResponseTypeDef",
     {
         "Cells": List[CellOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCrossAccountAuthorizationsResponseTypeDef = TypedDict(
-    "ListCrossAccountAuthorizationsResponseTypeDef",
-    {
-        "CrossAccountAuthorizations": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourcesResponseTypeDef = TypedDict(
-    "ListTagsForResourcesResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateCellResponseTypeDef = TypedDict(
-    "UpdateCellResponseTypeDef",
-    {
-        "CellArn": str,
-        "CellName": str,
-        "Cells": List[str],
-        "ParentReadinessScopes": List[str],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateReadinessCheckResponseTypeDef = TypedDict(
-    "UpdateReadinessCheckResponseTypeDef",
-    {
-        "ReadinessCheckArn": str,
-        "ReadinessCheckName": str,
-        "ResourceSet": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRecoveryGroupResponseTypeDef = TypedDict(
-    "UpdateRecoveryGroupResponseTypeDef",
-    {
-        "Cells": List[str],
-        "RecoveryGroupArn": str,
-        "RecoveryGroupName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetArchitectureRecommendationsResponseTypeDef = TypedDict(
     "GetArchitectureRecommendationsResponseTypeDef",
     {
         "LastAuditTimestamp": datetime,
         "NextToken": str,
         "Recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
-    "_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
-    {
-        "CellName": str,
-    },
-)
-_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
-    "_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef(
-    _RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
-    _OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
-):
-    pass
-
-_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
-    "_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
-    {
-        "ReadinessCheckName": str,
-        "ResourceIdentifier": str,
-    },
-)
-_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
-    "_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef(
-    _RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
-    _OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
-):
-    pass
-
-_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
-    "_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
-    {
-        "ReadinessCheckName": str,
-    },
-)
-_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
-    "_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef(
-    _RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
-    _OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
-):
-    pass
-
-_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
-    "_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
-    {
-        "RecoveryGroupName": str,
-    },
-)
-_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
-    "_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-class GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef(
-    _RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
-    _OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
-):
-    pass
-
-ListCellsRequestListCellsPaginateTypeDef = TypedDict(
-    "ListCellsRequestListCellsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef = TypedDict(
-    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReadinessChecksRequestListReadinessChecksPaginateTypeDef = TypedDict(
-    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef = TypedDict(
-    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListResourceSetsRequestListResourceSetsPaginateTypeDef = TypedDict(
-    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "ListRulesRequestListRulesPaginateTypeDef",
-    {
-        "ResourceType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 GetCellReadinessSummaryResponseTypeDef = TypedDict(
     "GetCellReadinessSummaryResponseTypeDef",
     {
         "NextToken": str,
         "Readiness": ReadinessType,
         "ReadinessChecks": List[ReadinessCheckSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecoveryGroupReadinessSummaryResponseTypeDef = TypedDict(
     "GetRecoveryGroupReadinessSummaryResponseTypeDef",
     {
         "NextToken": str,
         "Readiness": ReadinessType,
         "ReadinessChecks": List[ReadinessCheckSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleResultTypeDef = TypedDict(
     "RuleResultTypeDef",
     {
         "LastCheckedTimestamp": datetime,
@@ -918,42 +918,42 @@
 GetReadinessCheckStatusResponseTypeDef = TypedDict(
     "GetReadinessCheckStatusResponseTypeDef",
     {
         "Messages": List[MessageTypeDef],
         "NextToken": str,
         "Readiness": ReadinessType,
         "Resources": List[ResourceResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReadinessChecksResponseTypeDef = TypedDict(
     "ListReadinessChecksResponseTypeDef",
     {
         "NextToken": str,
         "ReadinessChecks": List[ReadinessCheckOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecoveryGroupsResponseTypeDef = TypedDict(
     "ListRecoveryGroupsResponseTypeDef",
     {
         "NextToken": str,
         "RecoveryGroups": List[RecoveryGroupOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "NextToken": str,
         "Rules": List[ListRulesOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TargetResourceTypeDef = TypedDict(
     "TargetResourceTypeDef",
     {
         "NLBResource": NLBResourceTypeDef,
@@ -964,15 +964,15 @@
 
 GetReadinessCheckResourceStatusResponseTypeDef = TypedDict(
     "GetReadinessCheckResourceStatusResponseTypeDef",
     {
         "NextToken": str,
         "Readiness": ReadinessType,
         "Rules": List[RuleResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DNSTargetResourceTypeDef = TypedDict(
     "DNSTargetResourceTypeDef",
     {
         "DomainName": str,
@@ -1020,27 +1020,27 @@
     "CreateResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
         "Resources": List[ResourceTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
         "Resources": List[ResourceTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredResourceSetOutputTypeDef = TypedDict(
     "_RequiredResourceSetOutputTypeDef",
     {
         "ResourceSetArn": str,
@@ -1075,19 +1075,19 @@
     "UpdateResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
         "Resources": List[ResourceTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "NextToken": str,
         "ResourceSets": List[ResourceSetOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-readiness
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Route53RecoveryReadiness 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Route53RecoveryReadiness 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/
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
 
 <a id="mypy-boto3-route53-recovery-readiness"></a>
 
 # mypy-boto3-route53-recovery-readiness
 
 [![PyPI - mypy-boto3-route53-recovery-readiness](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-readiness?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryReadiness 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[boto3.Route53RecoveryReadiness 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,79 +365,79 @@
 `mypy_boto3_route53_recovery_readiness.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53_recovery_readiness.type_defs import (
     CellOutputTypeDef,
     CreateCellRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateCellResponseTypeDef,
     CreateCrossAccountAuthorizationRequestRequestTypeDef,
+    CreateCrossAccountAuthorizationResponseTypeDef,
     CreateReadinessCheckRequestRequestTypeDef,
+    CreateReadinessCheckResponseTypeDef,
     CreateRecoveryGroupRequestRequestTypeDef,
+    CreateRecoveryGroupResponseTypeDef,
     DeleteCellRequestRequestTypeDef,
     DeleteCrossAccountAuthorizationRequestRequestTypeDef,
     DeleteReadinessCheckRequestRequestTypeDef,
     DeleteRecoveryGroupRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetArchitectureRecommendationsRequestRequestTypeDef,
     RecommendationTypeDef,
-    PaginatorConfigTypeDef,
+    GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
     GetCellReadinessSummaryRequestRequestTypeDef,
     ReadinessCheckSummaryTypeDef,
     GetCellRequestRequestTypeDef,
+    GetCellResponseTypeDef,
     GetReadinessCheckRequestRequestTypeDef,
+    GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
     GetReadinessCheckResourceStatusRequestRequestTypeDef,
+    GetReadinessCheckResponseTypeDef,
+    GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
     GetReadinessCheckStatusRequestRequestTypeDef,
     MessageTypeDef,
     ResourceResultTypeDef,
+    GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
     GetRecoveryGroupReadinessSummaryRequestRequestTypeDef,
     GetRecoveryGroupRequestRequestTypeDef,
+    GetRecoveryGroupResponseTypeDef,
     GetResourceSetRequestRequestTypeDef,
+    ListCellsRequestListCellsPaginateTypeDef,
     ListCellsRequestRequestTypeDef,
+    ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef,
     ListCrossAccountAuthorizationsRequestRequestTypeDef,
+    ListCrossAccountAuthorizationsResponseTypeDef,
+    ListReadinessChecksRequestListReadinessChecksPaginateTypeDef,
     ListReadinessChecksRequestRequestTypeDef,
     ReadinessCheckOutputTypeDef,
+    ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef,
     ListRecoveryGroupsRequestRequestTypeDef,
     RecoveryGroupOutputTypeDef,
+    ListResourceSetsRequestListResourceSetsPaginateTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ListRulesOutputTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
+    ListTagsForResourcesResponseTypeDef,
     NLBResourceTypeDef,
+    PaginatorConfigTypeDef,
     R53ResourceRecordTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCellRequestRequestTypeDef,
-    UpdateReadinessCheckRequestRequestTypeDef,
-    UpdateRecoveryGroupRequestRequestTypeDef,
-    CreateCellResponseTypeDef,
-    CreateCrossAccountAuthorizationResponseTypeDef,
-    CreateReadinessCheckResponseTypeDef,
-    CreateRecoveryGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCellResponseTypeDef,
-    GetReadinessCheckResponseTypeDef,
-    GetRecoveryGroupResponseTypeDef,
-    ListCellsResponseTypeDef,
-    ListCrossAccountAuthorizationsResponseTypeDef,
-    ListTagsForResourcesResponseTypeDef,
     UpdateCellResponseTypeDef,
+    UpdateReadinessCheckRequestRequestTypeDef,
     UpdateReadinessCheckResponseTypeDef,
+    UpdateRecoveryGroupRequestRequestTypeDef,
     UpdateRecoveryGroupResponseTypeDef,
+    ListCellsResponseTypeDef,
     GetArchitectureRecommendationsResponseTypeDef,
-    GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
-    GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
-    GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
-    GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
-    ListCellsRequestListCellsPaginateTypeDef,
-    ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef,
-    ListReadinessChecksRequestListReadinessChecksPaginateTypeDef,
-    ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef,
-    ListResourceSetsRequestListResourceSetsPaginateTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     GetCellReadinessSummaryResponseTypeDef,
     GetRecoveryGroupReadinessSummaryResponseTypeDef,
     RuleResultTypeDef,
     GetReadinessCheckStatusResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListRulesResponseTypeDef,
@@ -461,42 +462,42 @@
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

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt` & `mypy-boto3-route53-recovery-readiness-1.27.0/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.26.0.post1/setup.py` & `mypy-boto3-route53-recovery-readiness-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 """
 Setup script for mypy-boto3-route53-recovery-readiness.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53-recovery-readiness",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_route53_recovery_readiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53RecoveryReadiness 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.Route53RecoveryReadiness 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
     keywords=(
         "boto3 route53-recovery-readiness type-annotations boto3-stubs mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_route53_recovery_readiness": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_route53_recovery_readiness": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/"
         ),
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


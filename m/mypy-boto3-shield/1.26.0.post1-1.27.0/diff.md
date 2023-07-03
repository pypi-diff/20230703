# Comparing `tmp/mypy-boto3-shield-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-shield-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-shield-1.26.0.post1.tar", last modified: Tue Nov  1 21:44:00 2022, max compression
+gzip compressed data, was "mypy-boto3-shield-1.27.0.tar", last modified: Mon Jul  3 19:51:28 2023, max compression
```

## Comparing `mypy-boto3-shield-1.26.0.post1.tar` & `mypy-boto3-shield-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:00.880850 mypy-boto3-shield-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:41:27.000000 mypy-boto3-shield-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15740 2022-11-01 21:44:00.876850 mypy-boto3-shield-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14303 2022-11-01 21:41:27.000000 mypy-boto3-shield-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:00.868850 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-01 21:41:27.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-11-01 21:41:27.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-11-01 21:41:27.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25578 2022-11-01 21:41:28.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    25533 2022-11-01 21:41:27.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8460 2022-11-01 21:41:28.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8458 2022-11-01 21:41:28.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-11-01 21:41:28.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3085 2022-11-01 21:41:28.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:41:27.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    22131 2022-11-01 21:41:28.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    22112 2022-11-01 21:41:28.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:41:27.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:00.876850 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15740 2022-11-01 21:44:00.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-11-01 21:44:00.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:00.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:00.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:44:00.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-01 21:44:00.000000 mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:44:00.880850 mypy-boto3-shield-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-11-01 21:41:27.000000 mypy-boto3-shield-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:28.296013 mypy-boto3-shield-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-03 19:51:28.288013 mypy-boto3-shield-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:28.288013 mypy-boto3-shield-1.27.0/mypy_boto3_shield/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25575 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22168 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:28.288013 mypy-boto3-shield-1.27.0/mypy_boto3_shield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-03 19:51:28.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 19:51:28.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:28.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:28.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:28.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:51:28.000000 mypy-boto3-shield-1.27.0/mypy_boto3_shield.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:28.296013 mypy-boto3-shield-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:48:12.000000 mypy-boto3-shield-1.27.0/setup.py
```

### Comparing `mypy-boto3-shield-1.26.0.post1/LICENSE` & `mypy-boto3-shield-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-shield-1.26.0.post1/PKG-INFO` & `mypy-boto3-shield-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-shield
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Shield 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Shield 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/
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
 
 <a id="mypy-boto3-shield"></a>
 
 # mypy-boto3-shield
 
 [![PyPI - mypy-boto3-shield](https://img.shields.io/pypi/v/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-shield?color=blue)](https://pypistats.org/packages/mypy-boto3-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Shield 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[boto3.Shield 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,61 +341,61 @@
     EmergencyContactTypeDef,
     MitigationTypeDef,
     SummarizedCounterTypeDef,
     ContributorTypeDef,
     AttackVectorDescriptionTypeDef,
     AttackVolumeStatisticsTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateProtectionResponseTypeDef,
     DeleteProtectionGroupRequestRequestTypeDef,
     DeleteProtectionRequestRequestTypeDef,
     DescribeAttackRequestRequestTypeDef,
     TimeRangeTypeDef,
+    DescribeDRTAccessResponseTypeDef,
     DescribeProtectionGroupRequestRequestTypeDef,
     ProtectionGroupTypeDef,
     DescribeProtectionRequestRequestTypeDef,
     DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
+    GetSubscriptionStateResponseTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
-    PaginatorConfigTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
+    ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
     EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
+    DescribeEmergencyContactSettingsResponseTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
     SummarizedAttackVectorTypeDef,
     AttackPropertyTypeDef,
     AttackSummaryTypeDef,
     AttackVolumeTypeDef,
     CreateProtectionGroupRequestRequestTypeDef,
     CreateProtectionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateProtectionResponseTypeDef,
-    DescribeDRTAccessResponseTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
-    GetSubscriptionStateResponseTypeDef,
-    ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
+    ListAttacksRequestListAttacksPaginateTypeDef,
     ListAttacksRequestRequestTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
+    ListProtectionsRequestListProtectionsPaginateTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListProtectionsRequestListProtectionsPaginateTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
     DescribeProtectionResponseTypeDef,
@@ -415,42 +416,42 @@
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

### Comparing `mypy-boto3-shield-1.26.0.post1/README.md` & `mypy-boto3-shield-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-shield"></a>
 
 # mypy-boto3-shield
 
 [![PyPI - mypy-boto3-shield](https://img.shields.io/pypi/v/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-shield?color=blue)](https://pypistats.org/packages/mypy-boto3-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Shield 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[boto3.Shield 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,61 +309,61 @@
     EmergencyContactTypeDef,
     MitigationTypeDef,
     SummarizedCounterTypeDef,
     ContributorTypeDef,
     AttackVectorDescriptionTypeDef,
     AttackVolumeStatisticsTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateProtectionResponseTypeDef,
     DeleteProtectionGroupRequestRequestTypeDef,
     DeleteProtectionRequestRequestTypeDef,
     DescribeAttackRequestRequestTypeDef,
     TimeRangeTypeDef,
+    DescribeDRTAccessResponseTypeDef,
     DescribeProtectionGroupRequestRequestTypeDef,
     ProtectionGroupTypeDef,
     DescribeProtectionRequestRequestTypeDef,
     DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
+    GetSubscriptionStateResponseTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
-    PaginatorConfigTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
+    ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
     EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
+    DescribeEmergencyContactSettingsResponseTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
     SummarizedAttackVectorTypeDef,
     AttackPropertyTypeDef,
     AttackSummaryTypeDef,
     AttackVolumeTypeDef,
     CreateProtectionGroupRequestRequestTypeDef,
     CreateProtectionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateProtectionResponseTypeDef,
-    DescribeDRTAccessResponseTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
-    GetSubscriptionStateResponseTypeDef,
-    ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
+    ListAttacksRequestListAttacksPaginateTypeDef,
     ListAttacksRequestRequestTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
+    ListProtectionsRequestListProtectionsPaginateTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListProtectionsRequestListProtectionsPaginateTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
     DescribeProtectionResponseTypeDef,
@@ -384,42 +384,42 @@
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

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/__init__.py` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/__init__.pyi` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/__main__.py` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Shield 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Shield 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield\nOther"
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

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/client.py` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.create_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#create_subscription)
         """
 
     def delete_protection(self, *, ProtectionId: str) -> Dict[str, Any]:
         """
-        Deletes an Shield Advanced  Protection .
+        Deletes an Shield Advanced  Protection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.delete_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#delete_protection)
         """
 
     def delete_protection_group(self, *, ProtectionGroupId: str) -> Dict[str, Any]:
         """
@@ -362,15 +362,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#generate_presigned_url)
         """
 
     def get_subscription_state(self) -> GetSubscriptionStateResponseTypeDef:
         """
-        Returns the `SubscriptionState` , either `Active` or `Inactive` .
+        Returns the `SubscriptionState`, either `Active` or `Inactive`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.get_subscription_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#get_subscription_state)
         """
 
     def list_attacks(
         self,
```

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/client.pyi` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         Activates Shield Advanced for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.create_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#create_subscription)
         """
     def delete_protection(self, *, ProtectionId: str) -> Dict[str, Any]:
         """
-        Deletes an Shield Advanced  Protection .
+        Deletes an Shield Advanced  Protection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.delete_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#delete_protection)
         """
     def delete_protection_group(self, *, ProtectionGroupId: str) -> Dict[str, Any]:
         """
         Removes the specified protection group.
@@ -330,15 +330,15 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#generate_presigned_url)
         """
     def get_subscription_state(self) -> GetSubscriptionStateResponseTypeDef:
         """
-        Returns the `SubscriptionState` , either `Active` or `Inactive` .
+        Returns the `SubscriptionState`, either `Active` or `Inactive`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.get_subscription_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#get_subscription_state)
         """
     def list_attacks(
         self,
         *,
```

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/literals.py` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationLayerAutomaticResponseStatusType",
     "AttackLayerType",
     "AttackPropertyIdentifierType",
     "AutoRenewType",
     "ListAttacksPaginatorName",
     "ListProtectionsPaginatorName",
@@ -35,15 +34,14 @@
     "UnitType",
     "ShieldServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ApplicationLayerAutomaticResponseStatusType = Literal["DISABLED", "ENABLED"]
 AttackLayerType = Literal["APPLICATION", "NETWORK"]
 AttackPropertyIdentifierType = Literal[
     "DESTINATION_URL",
     "REFERRER",
     "SOURCE_ASN",
     "SOURCE_COUNTRY",
@@ -81,23 +79,25 @@
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
@@ -107,30 +107,35 @@
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
@@ -156,14 +161,15 @@
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
@@ -208,51 +214,57 @@
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
@@ -265,14 +277,15 @@
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
@@ -284,28 +297,35 @@
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
@@ -314,14 +334,15 @@
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
@@ -332,55 +353,64 @@
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

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/literals.pyi` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ApplicationLayerAutomaticResponseStatusType",
     "AttackLayerType",
     "AttackPropertyIdentifierType",
     "AutoRenewType",
     "ListAttacksPaginatorName",
     "ListProtectionsPaginatorName",
@@ -34,14 +35,15 @@
     "UnitType",
     "ShieldServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 ApplicationLayerAutomaticResponseStatusType = Literal["DISABLED", "ENABLED"]
 AttackLayerType = Literal["APPLICATION", "NETWORK"]
 AttackPropertyIdentifierType = Literal[
     "DESTINATION_URL",
     "REFERRER",
     "SOURCE_ASN",
     "SOURCE_COUNTRY",
@@ -79,23 +81,25 @@
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
@@ -105,30 +109,35 @@
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
@@ -154,14 +163,15 @@
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
@@ -206,51 +216,57 @@
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
@@ -263,14 +279,15 @@
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
@@ -282,28 +299,35 @@
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
@@ -312,14 +336,15 @@
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
@@ -330,55 +355,64 @@
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

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/paginator.py` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
         StartTime: TimeRangeTypeDef = ...,
         EndTime: TimeRangeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listattackspaginator)
         """
 
 
@@ -72,13 +72,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listprotectionspaginator)
     """
 
     def paginate(
         self,
         *,
         InclusionFilters: InclusionProtectionFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProtectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listprotectionspaginator)
         """
```

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/paginator.pyi` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
         StartTime: TimeRangeTypeDef = ...,
         EndTime: TimeRangeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listattackspaginator)
         """
 
 class ListProtectionsPaginator(Paginator):
@@ -68,13 +68,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listprotectionspaginator)
     """
 
     def paginate(
         self,
         *,
         InclusionFilters: InclusionProtectionFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProtectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listprotectionspaginator)
         """
```

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/type_defs.py` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,61 +43,61 @@
     "EmergencyContactTypeDef",
     "MitigationTypeDef",
     "SummarizedCounterTypeDef",
     "ContributorTypeDef",
     "AttackVectorDescriptionTypeDef",
     "AttackVolumeStatisticsTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateProtectionResponseTypeDef",
     "DeleteProtectionGroupRequestRequestTypeDef",
     "DeleteProtectionRequestRequestTypeDef",
     "DescribeAttackRequestRequestTypeDef",
     "TimeRangeTypeDef",
+    "DescribeDRTAccessResponseTypeDef",
     "DescribeProtectionGroupRequestRequestTypeDef",
     "ProtectionGroupTypeDef",
     "DescribeProtectionRequestRequestTypeDef",
     "DisableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "DisassociateDRTLogBucketRequestRequestTypeDef",
     "DisassociateHealthCheckRequestRequestTypeDef",
+    "GetSubscriptionStateResponseTypeDef",
     "InclusionProtectionFiltersTypeDef",
     "InclusionProtectionGroupFiltersTypeDef",
     "LimitTypeDef",
-    "PaginatorConfigTypeDef",
     "ListResourcesInProtectionGroupRequestRequestTypeDef",
+    "ListResourcesInProtectionGroupResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProtectionGroupRequestRequestTypeDef",
     "UpdateSubscriptionRequestRequestTypeDef",
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
     "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
+    "DescribeEmergencyContactSettingsResponseTypeDef",
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     "SummarizedAttackVectorTypeDef",
     "AttackPropertyTypeDef",
     "AttackSummaryTypeDef",
     "AttackVolumeTypeDef",
     "CreateProtectionGroupRequestRequestTypeDef",
     "CreateProtectionRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateProtectionResponseTypeDef",
-    "DescribeDRTAccessResponseTypeDef",
-    "DescribeEmergencyContactSettingsResponseTypeDef",
-    "GetSubscriptionStateResponseTypeDef",
-    "ListResourcesInProtectionGroupResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "ListAttacksRequestListAttacksPaginateTypeDef",
     "ListAttacksRequestRequestTypeDef",
     "DescribeProtectionGroupResponseTypeDef",
     "ListProtectionGroupsResponseTypeDef",
+    "ListProtectionsRequestListProtectionsPaginateTypeDef",
     "ListProtectionsRequestRequestTypeDef",
     "ListProtectionGroupsRequestRequestTypeDef",
     "ProtectionLimitsTypeDef",
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    "ListProtectionsRequestListProtectionsPaginateTypeDef",
     "ProtectionGroupPatternTypeLimitsTypeDef",
     "ProtectionTypeDef",
     "SubResourceSummaryTypeDef",
     "ListAttacksResponseTypeDef",
     "AttackStatisticsDataItemTypeDef",
     "ProtectionGroupLimitsTypeDef",
     "DescribeProtectionResponseTypeDef",
@@ -210,22 +210,19 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateProtectionResponseTypeDef = TypedDict(
+    "CreateProtectionResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ProtectionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteProtectionGroupRequestRequestTypeDef = TypedDict(
     "DeleteProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
@@ -251,14 +248,23 @@
     {
         "FromInclusive": datetime,
         "ToExclusive": datetime,
     },
     total=False,
 )
 
+DescribeDRTAccessResponseTypeDef = TypedDict(
+    "DescribeDRTAccessResponseTypeDef",
+    {
+        "RoleArn": str,
+        "LogBucketList": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeProtectionGroupRequestRequestTypeDef = TypedDict(
     "DescribeProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 
@@ -312,14 +318,22 @@
     "DisassociateHealthCheckRequestRequestTypeDef",
     {
         "ProtectionId": str,
         "HealthCheckArn": str,
     },
 )
 
+GetSubscriptionStateResponseTypeDef = TypedDict(
+    "GetSubscriptionStateResponseTypeDef",
+    {
+        "SubscriptionState": SubscriptionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InclusionProtectionFiltersTypeDef = TypedDict(
     "InclusionProtectionFiltersTypeDef",
     {
         "ResourceArns": Sequence[str],
         "ProtectionNames": Sequence[str],
         "ResourceTypes": Sequence[ProtectedResourceTypeType],
     },
@@ -342,24 +356,14 @@
     {
         "Type": str,
         "Max": int,
     },
     total=False,
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
 _RequiredListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesInProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 _OptionalListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
@@ -375,28 +379,58 @@
 class ListResourcesInProtectionGroupRequestRequestTypeDef(
     _RequiredListResourcesInProtectionGroupRequestRequestTypeDef,
     _OptionalListResourcesInProtectionGroupRequestRequestTypeDef,
 ):
     pass
 
 
+ListResourcesInProtectionGroupResponseTypeDef = TypedDict(
+    "ListResourcesInProtectionGroupResponseTypeDef",
+    {
+        "ResourceArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 ProtectionGroupArbitraryPatternLimitsTypeDef = TypedDict(
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     {
         "MaxMembers": int,
     },
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
@@ -461,14 +495,22 @@
 AssociateProactiveEngagementDetailsRequestRequestTypeDef = TypedDict(
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
     },
 )
 
+DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
+    "DescribeEmergencyContactSettingsResponseTypeDef",
+    {
+        "EmergencyContactList": List[EmergencyContactTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateEmergencyContactSettingsRequestRequestTypeDef = TypedDict(
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
     },
     total=False,
 )
@@ -572,70 +614,39 @@
 
 class CreateProtectionRequestRequestTypeDef(
     _RequiredCreateProtectionRequestRequestTypeDef, _OptionalCreateProtectionRequestRequestTypeDef
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
-CreateProtectionResponseTypeDef = TypedDict(
-    "CreateProtectionResponseTypeDef",
-    {
-        "ProtectionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDRTAccessResponseTypeDef = TypedDict(
-    "DescribeDRTAccessResponseTypeDef",
-    {
-        "RoleArn": str,
-        "LogBucketList": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
-    "DescribeEmergencyContactSettingsResponseTypeDef",
-    {
-        "EmergencyContactList": List[EmergencyContactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSubscriptionStateResponseTypeDef = TypedDict(
-    "GetSubscriptionStateResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "SubscriptionState": SubscriptionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListResourcesInProtectionGroupResponseTypeDef = TypedDict(
-    "ListResourcesInProtectionGroupResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ResourceArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
+    "ListAttacksRequestListAttacksPaginateTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
 ListAttacksRequestRequestTypeDef = TypedDict(
     "ListAttacksRequestRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "StartTime": TimeRangeTypeDef,
@@ -646,25 +657,34 @@
     total=False,
 )
 
 DescribeProtectionGroupResponseTypeDef = TypedDict(
     "DescribeProtectionGroupResponseTypeDef",
     {
         "ProtectionGroup": ProtectionGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProtectionGroupsResponseTypeDef = TypedDict(
     "ListProtectionGroupsResponseTypeDef",
     {
         "ProtectionGroups": List[ProtectionGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
+    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+    {
+        "InclusionFilters": InclusionProtectionFiltersTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
 ListProtectionsRequestRequestTypeDef = TypedDict(
     "ListProtectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -686,34 +706,14 @@
 ProtectionLimitsTypeDef = TypedDict(
     "ProtectionLimitsTypeDef",
     {
         "ProtectedResourceTypeLimits": List[LimitTypeDef],
     },
 )
 
-ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
-    "ListProtectionsRequestListProtectionsPaginateTypeDef",
-    {
-        "InclusionFilters": InclusionProtectionFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
     "ProtectionGroupPatternTypeLimitsTypeDef",
     {
         "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
     },
 )
 
@@ -721,15 +721,17 @@
     "ProtectionTypeDef",
     {
         "Id": str,
         "Name": str,
         "ResourceArn": str,
         "HealthCheckIds": List[str],
         "ProtectionArn": str,
-        "ApplicationLayerAutomaticResponseConfiguration": ApplicationLayerAutomaticResponseConfigurationTypeDef,
+        "ApplicationLayerAutomaticResponseConfiguration": (
+            ApplicationLayerAutomaticResponseConfigurationTypeDef
+        ),
     },
     total=False,
 )
 
 SubResourceSummaryTypeDef = TypedDict(
     "SubResourceSummaryTypeDef",
     {
@@ -742,15 +744,15 @@
 )
 
 ListAttacksResponseTypeDef = TypedDict(
     "ListAttacksResponseTypeDef",
     {
         "AttackSummaries": List[AttackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAttackStatisticsDataItemTypeDef = TypedDict(
     "_RequiredAttackStatisticsDataItemTypeDef",
     {
         "AttackCount": int,
@@ -779,24 +781,24 @@
     },
 )
 
 DescribeProtectionResponseTypeDef = TypedDict(
     "DescribeProtectionResponseTypeDef",
     {
         "Protection": ProtectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProtectionsResponseTypeDef = TypedDict(
     "ListProtectionsResponseTypeDef",
     {
         "Protections": List[ProtectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttackDetailTypeDef = TypedDict(
     "AttackDetailTypeDef",
     {
         "AttackId": str,
@@ -812,15 +814,15 @@
 )
 
 DescribeAttackStatisticsResponseTypeDef = TypedDict(
     "DescribeAttackStatisticsResponseTypeDef",
     {
         "TimeRange": TimeRangeTypeDef,
         "DataItems": List[AttackStatisticsDataItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubscriptionLimitsTypeDef = TypedDict(
     "SubscriptionLimitsTypeDef",
     {
         "ProtectionLimits": ProtectionLimitsTypeDef,
@@ -828,15 +830,15 @@
     },
 )
 
 DescribeAttackResponseTypeDef = TypedDict(
     "DescribeAttackResponseTypeDef",
     {
         "Attack": AttackDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSubscriptionTypeDef = TypedDict(
     "_RequiredSubscriptionTypeDef",
     {
         "SubscriptionLimits": SubscriptionLimitsTypeDef,
@@ -861,10 +863,10 @@
     pass
 
 
 DescribeSubscriptionResponseTypeDef = TypedDict(
     "DescribeSubscriptionResponseTypeDef",
     {
         "Subscription": SubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield/type_defs.pyi` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,61 +42,61 @@
     "EmergencyContactTypeDef",
     "MitigationTypeDef",
     "SummarizedCounterTypeDef",
     "ContributorTypeDef",
     "AttackVectorDescriptionTypeDef",
     "AttackVolumeStatisticsTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateProtectionResponseTypeDef",
     "DeleteProtectionGroupRequestRequestTypeDef",
     "DeleteProtectionRequestRequestTypeDef",
     "DescribeAttackRequestRequestTypeDef",
     "TimeRangeTypeDef",
+    "DescribeDRTAccessResponseTypeDef",
     "DescribeProtectionGroupRequestRequestTypeDef",
     "ProtectionGroupTypeDef",
     "DescribeProtectionRequestRequestTypeDef",
     "DisableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "DisassociateDRTLogBucketRequestRequestTypeDef",
     "DisassociateHealthCheckRequestRequestTypeDef",
+    "GetSubscriptionStateResponseTypeDef",
     "InclusionProtectionFiltersTypeDef",
     "InclusionProtectionGroupFiltersTypeDef",
     "LimitTypeDef",
-    "PaginatorConfigTypeDef",
     "ListResourcesInProtectionGroupRequestRequestTypeDef",
+    "ListResourcesInProtectionGroupResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProtectionGroupRequestRequestTypeDef",
     "UpdateSubscriptionRequestRequestTypeDef",
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
     "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
+    "DescribeEmergencyContactSettingsResponseTypeDef",
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     "SummarizedAttackVectorTypeDef",
     "AttackPropertyTypeDef",
     "AttackSummaryTypeDef",
     "AttackVolumeTypeDef",
     "CreateProtectionGroupRequestRequestTypeDef",
     "CreateProtectionRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateProtectionResponseTypeDef",
-    "DescribeDRTAccessResponseTypeDef",
-    "DescribeEmergencyContactSettingsResponseTypeDef",
-    "GetSubscriptionStateResponseTypeDef",
-    "ListResourcesInProtectionGroupResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "ListAttacksRequestListAttacksPaginateTypeDef",
     "ListAttacksRequestRequestTypeDef",
     "DescribeProtectionGroupResponseTypeDef",
     "ListProtectionGroupsResponseTypeDef",
+    "ListProtectionsRequestListProtectionsPaginateTypeDef",
     "ListProtectionsRequestRequestTypeDef",
     "ListProtectionGroupsRequestRequestTypeDef",
     "ProtectionLimitsTypeDef",
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    "ListProtectionsRequestListProtectionsPaginateTypeDef",
     "ProtectionGroupPatternTypeLimitsTypeDef",
     "ProtectionTypeDef",
     "SubResourceSummaryTypeDef",
     "ListAttacksResponseTypeDef",
     "AttackStatisticsDataItemTypeDef",
     "ProtectionGroupLimitsTypeDef",
     "DescribeProtectionResponseTypeDef",
@@ -207,22 +207,19 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateProtectionResponseTypeDef = TypedDict(
+    "CreateProtectionResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ProtectionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteProtectionGroupRequestRequestTypeDef = TypedDict(
     "DeleteProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
@@ -248,14 +245,23 @@
     {
         "FromInclusive": datetime,
         "ToExclusive": datetime,
     },
     total=False,
 )
 
+DescribeDRTAccessResponseTypeDef = TypedDict(
+    "DescribeDRTAccessResponseTypeDef",
+    {
+        "RoleArn": str,
+        "LogBucketList": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeProtectionGroupRequestRequestTypeDef = TypedDict(
     "DescribeProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 
@@ -307,14 +313,22 @@
     "DisassociateHealthCheckRequestRequestTypeDef",
     {
         "ProtectionId": str,
         "HealthCheckArn": str,
     },
 )
 
+GetSubscriptionStateResponseTypeDef = TypedDict(
+    "GetSubscriptionStateResponseTypeDef",
+    {
+        "SubscriptionState": SubscriptionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InclusionProtectionFiltersTypeDef = TypedDict(
     "InclusionProtectionFiltersTypeDef",
     {
         "ResourceArns": Sequence[str],
         "ProtectionNames": Sequence[str],
         "ResourceTypes": Sequence[ProtectedResourceTypeType],
     },
@@ -337,24 +351,14 @@
     {
         "Type": str,
         "Max": int,
     },
     total=False,
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
 _RequiredListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesInProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 _OptionalListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
@@ -368,28 +372,58 @@
 
 class ListResourcesInProtectionGroupRequestRequestTypeDef(
     _RequiredListResourcesInProtectionGroupRequestRequestTypeDef,
     _OptionalListResourcesInProtectionGroupRequestRequestTypeDef,
 ):
     pass
 
+ListResourcesInProtectionGroupResponseTypeDef = TypedDict(
+    "ListResourcesInProtectionGroupResponseTypeDef",
+    {
+        "ResourceArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 ProtectionGroupArbitraryPatternLimitsTypeDef = TypedDict(
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     {
         "MaxMembers": int,
     },
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
@@ -452,14 +486,22 @@
 AssociateProactiveEngagementDetailsRequestRequestTypeDef = TypedDict(
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
     },
 )
 
+DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
+    "DescribeEmergencyContactSettingsResponseTypeDef",
+    {
+        "EmergencyContactList": List[EmergencyContactTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateEmergencyContactSettingsRequestRequestTypeDef = TypedDict(
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
     },
     total=False,
 )
@@ -557,70 +599,39 @@
 )
 
 class CreateProtectionRequestRequestTypeDef(
     _RequiredCreateProtectionRequestRequestTypeDef, _OptionalCreateProtectionRequestRequestTypeDef
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
-CreateProtectionResponseTypeDef = TypedDict(
-    "CreateProtectionResponseTypeDef",
-    {
-        "ProtectionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDRTAccessResponseTypeDef = TypedDict(
-    "DescribeDRTAccessResponseTypeDef",
-    {
-        "RoleArn": str,
-        "LogBucketList": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
-    "DescribeEmergencyContactSettingsResponseTypeDef",
-    {
-        "EmergencyContactList": List[EmergencyContactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSubscriptionStateResponseTypeDef = TypedDict(
-    "GetSubscriptionStateResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "SubscriptionState": SubscriptionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListResourcesInProtectionGroupResponseTypeDef = TypedDict(
-    "ListResourcesInProtectionGroupResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ResourceArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
+    "ListAttacksRequestListAttacksPaginateTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
 ListAttacksRequestRequestTypeDef = TypedDict(
     "ListAttacksRequestRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "StartTime": TimeRangeTypeDef,
@@ -631,25 +642,34 @@
     total=False,
 )
 
 DescribeProtectionGroupResponseTypeDef = TypedDict(
     "DescribeProtectionGroupResponseTypeDef",
     {
         "ProtectionGroup": ProtectionGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProtectionGroupsResponseTypeDef = TypedDict(
     "ListProtectionGroupsResponseTypeDef",
     {
         "ProtectionGroups": List[ProtectionGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
+    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+    {
+        "InclusionFilters": InclusionProtectionFiltersTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
 ListProtectionsRequestRequestTypeDef = TypedDict(
     "ListProtectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -671,34 +691,14 @@
 ProtectionLimitsTypeDef = TypedDict(
     "ProtectionLimitsTypeDef",
     {
         "ProtectedResourceTypeLimits": List[LimitTypeDef],
     },
 )
 
-ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
-    "ListProtectionsRequestListProtectionsPaginateTypeDef",
-    {
-        "InclusionFilters": InclusionProtectionFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
     "ProtectionGroupPatternTypeLimitsTypeDef",
     {
         "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
     },
 )
 
@@ -706,15 +706,17 @@
     "ProtectionTypeDef",
     {
         "Id": str,
         "Name": str,
         "ResourceArn": str,
         "HealthCheckIds": List[str],
         "ProtectionArn": str,
-        "ApplicationLayerAutomaticResponseConfiguration": ApplicationLayerAutomaticResponseConfigurationTypeDef,
+        "ApplicationLayerAutomaticResponseConfiguration": (
+            ApplicationLayerAutomaticResponseConfigurationTypeDef
+        ),
     },
     total=False,
 )
 
 SubResourceSummaryTypeDef = TypedDict(
     "SubResourceSummaryTypeDef",
     {
@@ -727,15 +729,15 @@
 )
 
 ListAttacksResponseTypeDef = TypedDict(
     "ListAttacksResponseTypeDef",
     {
         "AttackSummaries": List[AttackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAttackStatisticsDataItemTypeDef = TypedDict(
     "_RequiredAttackStatisticsDataItemTypeDef",
     {
         "AttackCount": int,
@@ -762,24 +764,24 @@
     },
 )
 
 DescribeProtectionResponseTypeDef = TypedDict(
     "DescribeProtectionResponseTypeDef",
     {
         "Protection": ProtectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProtectionsResponseTypeDef = TypedDict(
     "ListProtectionsResponseTypeDef",
     {
         "Protections": List[ProtectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttackDetailTypeDef = TypedDict(
     "AttackDetailTypeDef",
     {
         "AttackId": str,
@@ -795,15 +797,15 @@
 )
 
 DescribeAttackStatisticsResponseTypeDef = TypedDict(
     "DescribeAttackStatisticsResponseTypeDef",
     {
         "TimeRange": TimeRangeTypeDef,
         "DataItems": List[AttackStatisticsDataItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubscriptionLimitsTypeDef = TypedDict(
     "SubscriptionLimitsTypeDef",
     {
         "ProtectionLimits": ProtectionLimitsTypeDef,
@@ -811,15 +813,15 @@
     },
 )
 
 DescribeAttackResponseTypeDef = TypedDict(
     "DescribeAttackResponseTypeDef",
     {
         "Attack": AttackDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSubscriptionTypeDef = TypedDict(
     "_RequiredSubscriptionTypeDef",
     {
         "SubscriptionLimits": SubscriptionLimitsTypeDef,
@@ -842,10 +844,10 @@
 class SubscriptionTypeDef(_RequiredSubscriptionTypeDef, _OptionalSubscriptionTypeDef):
     pass
 
 DescribeSubscriptionResponseTypeDef = TypedDict(
     "DescribeSubscriptionResponseTypeDef",
     {
         "Subscription": SubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield.egg-info/PKG-INFO` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-shield
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Shield 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Shield 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/
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
 
 <a id="mypy-boto3-shield"></a>
 
 # mypy-boto3-shield
 
 [![PyPI - mypy-boto3-shield](https://img.shields.io/pypi/v/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-shield?color=blue)](https://pypistats.org/packages/mypy-boto3-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Shield 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[boto3.Shield 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,61 +341,61 @@
     EmergencyContactTypeDef,
     MitigationTypeDef,
     SummarizedCounterTypeDef,
     ContributorTypeDef,
     AttackVectorDescriptionTypeDef,
     AttackVolumeStatisticsTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateProtectionResponseTypeDef,
     DeleteProtectionGroupRequestRequestTypeDef,
     DeleteProtectionRequestRequestTypeDef,
     DescribeAttackRequestRequestTypeDef,
     TimeRangeTypeDef,
+    DescribeDRTAccessResponseTypeDef,
     DescribeProtectionGroupRequestRequestTypeDef,
     ProtectionGroupTypeDef,
     DescribeProtectionRequestRequestTypeDef,
     DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
+    GetSubscriptionStateResponseTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
-    PaginatorConfigTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
+    ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
     EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
+    DescribeEmergencyContactSettingsResponseTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
     SummarizedAttackVectorTypeDef,
     AttackPropertyTypeDef,
     AttackSummaryTypeDef,
     AttackVolumeTypeDef,
     CreateProtectionGroupRequestRequestTypeDef,
     CreateProtectionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateProtectionResponseTypeDef,
-    DescribeDRTAccessResponseTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
-    GetSubscriptionStateResponseTypeDef,
-    ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
+    ListAttacksRequestListAttacksPaginateTypeDef,
     ListAttacksRequestRequestTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
+    ListProtectionsRequestListProtectionsPaginateTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListProtectionsRequestListProtectionsPaginateTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
     DescribeProtectionResponseTypeDef,
@@ -415,42 +416,42 @@
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

### Comparing `mypy-boto3-shield-1.26.0.post1/mypy_boto3_shield.egg-info/SOURCES.txt` & `mypy-boto3-shield-1.27.0/mypy_boto3_shield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.26.0.post1/setup.py` & `mypy-boto3-shield-1.27.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-shield.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-shield",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_shield"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Shield 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.Shield 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 shield type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_shield": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_shield": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/",
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


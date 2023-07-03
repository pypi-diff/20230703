# Comparing `tmp/mypy-boto3-codestar-notifications-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-codestar-notifications-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codestar-notifications-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:15 2022, max compression
+gzip compressed data, was "mypy-boto3-codestar-notifications-1.27.0.tar", last modified: Mon Jul  3 19:50:34 2023, max compression
```

## Comparing `mypy-boto3-codestar-notifications-1.26.0.post1.tar` & `mypy-boto3-codestar-notifications-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:15.652818 mypy-boto3-codestar-notifications-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15146 2022-11-01 21:43:15.652818 mypy-boto3-codestar-notifications-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13646 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:15.652818 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13881 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13858 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8318 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8316 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4602 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4597 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    10907 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    10898 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:15.652818 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15146 2022-11-01 21:43:15.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-01 21:43:15.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:15.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:15.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:15.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-01 21:43:15.000000 mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:15.652818 mypy-boto3-codestar-notifications-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-11-01 21:32:01.000000 mypy-boto3-codestar-notifications-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.023025 mypy-boto3-codestar-notifications-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:30.000000 mypy-boto3-codestar-notifications-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-07-03 19:50:34.019025 mypy-boto3-codestar-notifications-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-07-03 19:34:30.000000 mypy-boto3-codestar-notifications-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.011025 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-03 19:34:30.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-03 19:34:30.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-03 19:34:30.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-07-03 19:34:30.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-07-03 19:34:30.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-03 19:34:31.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-07-03 19:34:31.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-03 19:34:30.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-03 19:34:30.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:30.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-07-03 19:34:31.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-07-03 19:34:31.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:30.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.019025 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-07-03 19:50:33.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-03 19:50:33.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:33.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:33.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:33.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-03 19:50:33.000000 mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:34.023025 mypy-boto3-codestar-notifications-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-03 19:34:30.000000 mypy-boto3-codestar-notifications-1.27.0/setup.py
```

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/LICENSE` & `mypy-boto3-codestar-notifications-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/PKG-INFO` & `mypy-boto3-codestar-notifications-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar-notifications
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeStarNotifications 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeStarNotifications 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/
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
 
 <a id="mypy-boto3-codestar-notifications"></a>
 
 # mypy-boto3-codestar-notifications
 
 [![PyPI - mypy-boto3-codestar-notifications](https://img.shields.io/pypi/v/mypy-boto3-codestar-notifications.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-notifications)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-notifications.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-notifications)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codestar-notifications?color=blue)](https://pypistats.org/packages/mypy-boto3-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarNotifications 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
+[boto3.CodeStarNotifications 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
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
 [mypy-boto3-codestar-notifications docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,43 +337,43 @@
 
 `mypy_boto3_codestar_notifications.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar_notifications.type_defs import (
     TargetTypeDef,
-    ResponseMetadataTypeDef,
+    CreateNotificationRuleResultTypeDef,
     DeleteNotificationRuleRequestRequestTypeDef,
+    DeleteNotificationRuleResultTypeDef,
     DeleteTargetRequestRequestTypeDef,
     DescribeNotificationRuleRequestRequestTypeDef,
     EventTypeSummaryTypeDef,
     TargetSummaryTypeDef,
     ListEventTypesFilterTypeDef,
-    PaginatorConfigTypeDef,
     ListNotificationRulesFilterTypeDef,
     NotificationRuleSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     ListTargetsFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    SubscribeResultTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagResourceResultTypeDef,
     UnsubscribeRequestRequestTypeDef,
+    UnsubscribeResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateNotificationRuleRequestRequestTypeDef,
     SubscribeRequestRequestTypeDef,
     UpdateNotificationRuleRequestRequestTypeDef,
-    CreateNotificationRuleResultTypeDef,
-    DeleteNotificationRuleResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    SubscribeResultTypeDef,
-    TagResourceResultTypeDef,
-    UnsubscribeResultTypeDef,
     ListEventTypesResultTypeDef,
     DescribeNotificationRuleResultTypeDef,
     ListTargetsResultTypeDef,
-    ListEventTypesRequestRequestTypeDef,
     ListEventTypesRequestListEventTypesPaginateTypeDef,
+    ListEventTypesRequestRequestTypeDef,
     ListNotificationRulesRequestListNotificationRulesPaginateTypeDef,
     ListNotificationRulesRequestRequestTypeDef,
     ListNotificationRulesResultTypeDef,
     ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
 )
 
@@ -384,42 +385,42 @@
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

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/README.md` & `mypy-boto3-codestar-notifications-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codestar-notifications"></a>
 
 # mypy-boto3-codestar-notifications
 
 [![PyPI - mypy-boto3-codestar-notifications](https://img.shields.io/pypi/v/mypy-boto3-codestar-notifications.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-notifications)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-notifications.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-notifications)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codestar-notifications?color=blue)](https://pypistats.org/packages/mypy-boto3-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarNotifications 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
+[boto3.CodeStarNotifications 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
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
 [mypy-boto3-codestar-notifications docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,43 +305,43 @@
 
 `mypy_boto3_codestar_notifications.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar_notifications.type_defs import (
     TargetTypeDef,
-    ResponseMetadataTypeDef,
+    CreateNotificationRuleResultTypeDef,
     DeleteNotificationRuleRequestRequestTypeDef,
+    DeleteNotificationRuleResultTypeDef,
     DeleteTargetRequestRequestTypeDef,
     DescribeNotificationRuleRequestRequestTypeDef,
     EventTypeSummaryTypeDef,
     TargetSummaryTypeDef,
     ListEventTypesFilterTypeDef,
-    PaginatorConfigTypeDef,
     ListNotificationRulesFilterTypeDef,
     NotificationRuleSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     ListTargetsFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    SubscribeResultTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagResourceResultTypeDef,
     UnsubscribeRequestRequestTypeDef,
+    UnsubscribeResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateNotificationRuleRequestRequestTypeDef,
     SubscribeRequestRequestTypeDef,
     UpdateNotificationRuleRequestRequestTypeDef,
-    CreateNotificationRuleResultTypeDef,
-    DeleteNotificationRuleResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    SubscribeResultTypeDef,
-    TagResourceResultTypeDef,
-    UnsubscribeResultTypeDef,
     ListEventTypesResultTypeDef,
     DescribeNotificationRuleResultTypeDef,
     ListTargetsResultTypeDef,
-    ListEventTypesRequestRequestTypeDef,
     ListEventTypesRequestListEventTypesPaginateTypeDef,
+    ListEventTypesRequestRequestTypeDef,
     ListNotificationRulesRequestListNotificationRulesPaginateTypeDef,
     ListNotificationRulesRequestRequestTypeDef,
     ListNotificationRulesResultTypeDef,
     ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
 )
 
@@ -353,42 +353,42 @@
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

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/__init__.py` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/__init__.pyi` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/__main__.py` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeStarNotifications 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CodeStarNotifications 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications\nOther"
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

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/client.py` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/client.pyi` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/literals.py` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,23 +60,25 @@
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
@@ -86,30 +88,35 @@
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
@@ -135,14 +142,15 @@
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
@@ -187,51 +195,57 @@
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
@@ -244,14 +258,15 @@
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
@@ -263,28 +278,35 @@
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
@@ -293,14 +315,15 @@
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
@@ -311,55 +334,64 @@
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

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/literals.pyi` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -58,23 +58,25 @@
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
@@ -84,30 +86,35 @@
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
@@ -133,14 +140,15 @@
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
@@ -185,51 +193,57 @@
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
@@ -242,14 +256,15 @@
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
@@ -261,28 +276,35 @@
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
@@ -291,14 +313,15 @@
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
@@ -309,55 +332,64 @@
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

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/paginator.py` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listeventtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListEventTypesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventTypesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListEventTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listeventtypespaginator)
         """
 
 
@@ -74,15 +74,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listnotificationrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListNotificationRulesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNotificationRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListNotificationRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listnotificationrulespaginator)
         """
 
 
@@ -92,13 +92,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listtargetspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListTargetsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listtargetspaginator)
         """
```

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/paginator.pyi` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listeventtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListEventTypesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventTypesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListEventTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listeventtypespaginator)
         """
 
 class ListNotificationRulesPaginator(Paginator):
@@ -70,15 +70,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listnotificationrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListNotificationRulesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNotificationRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListNotificationRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listnotificationrulespaginator)
         """
 
 class ListTargetsPaginator(Paginator):
@@ -87,13 +87,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listtargetspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListTargetsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listtargetspaginator)
         """
```

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/type_defs.py` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,43 +28,43 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TargetTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateNotificationRuleResultTypeDef",
     "DeleteNotificationRuleRequestRequestTypeDef",
+    "DeleteNotificationRuleResultTypeDef",
     "DeleteTargetRequestRequestTypeDef",
     "DescribeNotificationRuleRequestRequestTypeDef",
     "EventTypeSummaryTypeDef",
     "TargetSummaryTypeDef",
     "ListEventTypesFilterTypeDef",
-    "PaginatorConfigTypeDef",
     "ListNotificationRulesFilterTypeDef",
     "NotificationRuleSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "ListTargetsFilterTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "SubscribeResultTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TagResourceResultTypeDef",
     "UnsubscribeRequestRequestTypeDef",
+    "UnsubscribeResultTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CreateNotificationRuleRequestRequestTypeDef",
     "SubscribeRequestRequestTypeDef",
     "UpdateNotificationRuleRequestRequestTypeDef",
-    "CreateNotificationRuleResultTypeDef",
-    "DeleteNotificationRuleResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "SubscribeResultTypeDef",
-    "TagResourceResultTypeDef",
-    "UnsubscribeResultTypeDef",
     "ListEventTypesResultTypeDef",
     "DescribeNotificationRuleResultTypeDef",
     "ListTargetsResultTypeDef",
-    "ListEventTypesRequestRequestTypeDef",
     "ListEventTypesRequestListEventTypesPaginateTypeDef",
+    "ListEventTypesRequestRequestTypeDef",
     "ListNotificationRulesRequestListNotificationRulesPaginateTypeDef",
     "ListNotificationRulesRequestRequestTypeDef",
     "ListNotificationRulesResultTypeDef",
     "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListTargetsRequestRequestTypeDef",
 )
 
@@ -73,32 +73,37 @@
     {
         "TargetType": str,
         "TargetAddress": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateNotificationRuleResultTypeDef = TypedDict(
+    "CreateNotificationRuleResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteNotificationRuleRequestRequestTypeDef = TypedDict(
     "DeleteNotificationRuleRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeleteNotificationRuleResultTypeDef = TypedDict(
+    "DeleteNotificationRuleResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteTargetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTargetRequestRequestTypeDef",
     {
         "TargetAddress": str,
     },
 )
 _OptionalDeleteTargetRequestRequestTypeDef = TypedDict(
@@ -148,24 +153,14 @@
     "ListEventTypesFilterTypeDef",
     {
         "Name": ListEventTypesFilterNameType,
         "Value": str,
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
 ListNotificationRulesFilterTypeDef = TypedDict(
     "ListNotificationRulesFilterTypeDef",
     {
         "Name": ListNotificationRulesFilterNameType,
         "Value": str,
     },
 )
@@ -182,38 +177,91 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTargetsFilterTypeDef = TypedDict(
     "ListTargetsFilterTypeDef",
     {
         "Name": ListTargetsFilterNameType,
         "Value": str,
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
+SubscribeResultTypeDef = TypedDict(
+    "SubscribeResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+TagResourceResultTypeDef = TypedDict(
+    "TagResourceResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UnsubscribeRequestRequestTypeDef = TypedDict(
     "UnsubscribeRequestRequestTypeDef",
     {
         "Arn": str,
         "TargetAddress": str,
     },
 )
 
+UnsubscribeResultTypeDef = TypedDict(
+    "UnsubscribeResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -290,68 +338,20 @@
 class UpdateNotificationRuleRequestRequestTypeDef(
     _RequiredUpdateNotificationRuleRequestRequestTypeDef,
     _OptionalUpdateNotificationRuleRequestRequestTypeDef,
 ):
     pass
 
 
-CreateNotificationRuleResultTypeDef = TypedDict(
-    "CreateNotificationRuleResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteNotificationRuleResultTypeDef = TypedDict(
-    "DeleteNotificationRuleResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SubscribeResultTypeDef = TypedDict(
-    "SubscribeResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TagResourceResultTypeDef = TypedDict(
-    "TagResourceResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UnsubscribeResultTypeDef = TypedDict(
-    "UnsubscribeResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListEventTypesResultTypeDef = TypedDict(
     "ListEventTypesResultTypeDef",
     {
         "EventTypes": List[EventTypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeNotificationRuleResultTypeDef = TypedDict(
     "DescribeNotificationRuleResultTypeDef",
     {
         "Arn": str,
@@ -361,51 +361,51 @@
         "Targets": List[TargetSummaryTypeDef],
         "DetailType": DetailTypeType,
         "CreatedBy": str,
         "Status": NotificationRuleStatusType,
         "CreatedTimestamp": datetime,
         "LastModifiedTimestamp": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTargetsResultTypeDef = TypedDict(
     "ListTargetsResultTypeDef",
     {
         "Targets": List[TargetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEventTypesRequestRequestTypeDef = TypedDict(
-    "ListEventTypesRequestRequestTypeDef",
+ListEventTypesRequestListEventTypesPaginateTypeDef = TypedDict(
+    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     {
         "Filters": Sequence[ListEventTypesFilterTypeDef],
-        "NextToken": str,
-        "MaxResults": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListEventTypesRequestListEventTypesPaginateTypeDef = TypedDict(
-    "ListEventTypesRequestListEventTypesPaginateTypeDef",
+ListEventTypesRequestRequestTypeDef = TypedDict(
+    "ListEventTypesRequestRequestTypeDef",
     {
         "Filters": Sequence[ListEventTypesFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
 ListNotificationRulesRequestListNotificationRulesPaginateTypeDef = TypedDict(
     "ListNotificationRulesRequestListNotificationRulesPaginateTypeDef",
     {
         "Filters": Sequence[ListNotificationRulesFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListNotificationRulesRequestRequestTypeDef = TypedDict(
     "ListNotificationRulesRequestRequestTypeDef",
     {
@@ -417,23 +417,23 @@
 )
 
 ListNotificationRulesResultTypeDef = TypedDict(
     "ListNotificationRulesResultTypeDef",
     {
         "NextToken": str,
         "NotificationRules": List[NotificationRuleSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
     "ListTargetsRequestListTargetsPaginateTypeDef",
     {
         "Filters": Sequence[ListTargetsFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTargetsRequestRequestTypeDef = TypedDict(
     "ListTargetsRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications/type_defs.pyi` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -27,43 +27,43 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TargetTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateNotificationRuleResultTypeDef",
     "DeleteNotificationRuleRequestRequestTypeDef",
+    "DeleteNotificationRuleResultTypeDef",
     "DeleteTargetRequestRequestTypeDef",
     "DescribeNotificationRuleRequestRequestTypeDef",
     "EventTypeSummaryTypeDef",
     "TargetSummaryTypeDef",
     "ListEventTypesFilterTypeDef",
-    "PaginatorConfigTypeDef",
     "ListNotificationRulesFilterTypeDef",
     "NotificationRuleSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "ListTargetsFilterTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "SubscribeResultTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TagResourceResultTypeDef",
     "UnsubscribeRequestRequestTypeDef",
+    "UnsubscribeResultTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CreateNotificationRuleRequestRequestTypeDef",
     "SubscribeRequestRequestTypeDef",
     "UpdateNotificationRuleRequestRequestTypeDef",
-    "CreateNotificationRuleResultTypeDef",
-    "DeleteNotificationRuleResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "SubscribeResultTypeDef",
-    "TagResourceResultTypeDef",
-    "UnsubscribeResultTypeDef",
     "ListEventTypesResultTypeDef",
     "DescribeNotificationRuleResultTypeDef",
     "ListTargetsResultTypeDef",
-    "ListEventTypesRequestRequestTypeDef",
     "ListEventTypesRequestListEventTypesPaginateTypeDef",
+    "ListEventTypesRequestRequestTypeDef",
     "ListNotificationRulesRequestListNotificationRulesPaginateTypeDef",
     "ListNotificationRulesRequestRequestTypeDef",
     "ListNotificationRulesResultTypeDef",
     "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListTargetsRequestRequestTypeDef",
 )
 
@@ -72,32 +72,37 @@
     {
         "TargetType": str,
         "TargetAddress": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateNotificationRuleResultTypeDef = TypedDict(
+    "CreateNotificationRuleResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteNotificationRuleRequestRequestTypeDef = TypedDict(
     "DeleteNotificationRuleRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeleteNotificationRuleResultTypeDef = TypedDict(
+    "DeleteNotificationRuleResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteTargetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTargetRequestRequestTypeDef",
     {
         "TargetAddress": str,
     },
 )
 _OptionalDeleteTargetRequestRequestTypeDef = TypedDict(
@@ -145,24 +150,14 @@
     "ListEventTypesFilterTypeDef",
     {
         "Name": ListEventTypesFilterNameType,
         "Value": str,
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
 ListNotificationRulesFilterTypeDef = TypedDict(
     "ListNotificationRulesFilterTypeDef",
     {
         "Name": ListNotificationRulesFilterNameType,
         "Value": str,
     },
 )
@@ -179,38 +174,91 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTargetsFilterTypeDef = TypedDict(
     "ListTargetsFilterTypeDef",
     {
         "Name": ListTargetsFilterNameType,
         "Value": str,
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
+SubscribeResultTypeDef = TypedDict(
+    "SubscribeResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+TagResourceResultTypeDef = TypedDict(
+    "TagResourceResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UnsubscribeRequestRequestTypeDef = TypedDict(
     "UnsubscribeRequestRequestTypeDef",
     {
         "Arn": str,
         "TargetAddress": str,
     },
 )
 
+UnsubscribeResultTypeDef = TypedDict(
+    "UnsubscribeResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -281,68 +329,20 @@
 
 class UpdateNotificationRuleRequestRequestTypeDef(
     _RequiredUpdateNotificationRuleRequestRequestTypeDef,
     _OptionalUpdateNotificationRuleRequestRequestTypeDef,
 ):
     pass
 
-CreateNotificationRuleResultTypeDef = TypedDict(
-    "CreateNotificationRuleResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteNotificationRuleResultTypeDef = TypedDict(
-    "DeleteNotificationRuleResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SubscribeResultTypeDef = TypedDict(
-    "SubscribeResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TagResourceResultTypeDef = TypedDict(
-    "TagResourceResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UnsubscribeResultTypeDef = TypedDict(
-    "UnsubscribeResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListEventTypesResultTypeDef = TypedDict(
     "ListEventTypesResultTypeDef",
     {
         "EventTypes": List[EventTypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeNotificationRuleResultTypeDef = TypedDict(
     "DescribeNotificationRuleResultTypeDef",
     {
         "Arn": str,
@@ -352,51 +352,51 @@
         "Targets": List[TargetSummaryTypeDef],
         "DetailType": DetailTypeType,
         "CreatedBy": str,
         "Status": NotificationRuleStatusType,
         "CreatedTimestamp": datetime,
         "LastModifiedTimestamp": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTargetsResultTypeDef = TypedDict(
     "ListTargetsResultTypeDef",
     {
         "Targets": List[TargetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEventTypesRequestRequestTypeDef = TypedDict(
-    "ListEventTypesRequestRequestTypeDef",
+ListEventTypesRequestListEventTypesPaginateTypeDef = TypedDict(
+    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     {
         "Filters": Sequence[ListEventTypesFilterTypeDef],
-        "NextToken": str,
-        "MaxResults": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListEventTypesRequestListEventTypesPaginateTypeDef = TypedDict(
-    "ListEventTypesRequestListEventTypesPaginateTypeDef",
+ListEventTypesRequestRequestTypeDef = TypedDict(
+    "ListEventTypesRequestRequestTypeDef",
     {
         "Filters": Sequence[ListEventTypesFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
 ListNotificationRulesRequestListNotificationRulesPaginateTypeDef = TypedDict(
     "ListNotificationRulesRequestListNotificationRulesPaginateTypeDef",
     {
         "Filters": Sequence[ListNotificationRulesFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListNotificationRulesRequestRequestTypeDef = TypedDict(
     "ListNotificationRulesRequestRequestTypeDef",
     {
@@ -408,23 +408,23 @@
 )
 
 ListNotificationRulesResultTypeDef = TypedDict(
     "ListNotificationRulesResultTypeDef",
     {
         "NextToken": str,
         "NotificationRules": List[NotificationRuleSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
     "ListTargetsRequestListTargetsPaginateTypeDef",
     {
         "Filters": Sequence[ListTargetsFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTargetsRequestRequestTypeDef = TypedDict(
     "ListTargetsRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications.egg-info/PKG-INFO` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar-notifications
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeStarNotifications 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeStarNotifications 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/
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
 
 <a id="mypy-boto3-codestar-notifications"></a>
 
 # mypy-boto3-codestar-notifications
 
 [![PyPI - mypy-boto3-codestar-notifications](https://img.shields.io/pypi/v/mypy-boto3-codestar-notifications.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-notifications)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-notifications.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-notifications)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codestar-notifications?color=blue)](https://pypistats.org/packages/mypy-boto3-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarNotifications 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
+[boto3.CodeStarNotifications 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
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
 [mypy-boto3-codestar-notifications docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,43 +337,43 @@
 
 `mypy_boto3_codestar_notifications.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar_notifications.type_defs import (
     TargetTypeDef,
-    ResponseMetadataTypeDef,
+    CreateNotificationRuleResultTypeDef,
     DeleteNotificationRuleRequestRequestTypeDef,
+    DeleteNotificationRuleResultTypeDef,
     DeleteTargetRequestRequestTypeDef,
     DescribeNotificationRuleRequestRequestTypeDef,
     EventTypeSummaryTypeDef,
     TargetSummaryTypeDef,
     ListEventTypesFilterTypeDef,
-    PaginatorConfigTypeDef,
     ListNotificationRulesFilterTypeDef,
     NotificationRuleSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     ListTargetsFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    SubscribeResultTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagResourceResultTypeDef,
     UnsubscribeRequestRequestTypeDef,
+    UnsubscribeResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateNotificationRuleRequestRequestTypeDef,
     SubscribeRequestRequestTypeDef,
     UpdateNotificationRuleRequestRequestTypeDef,
-    CreateNotificationRuleResultTypeDef,
-    DeleteNotificationRuleResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    SubscribeResultTypeDef,
-    TagResourceResultTypeDef,
-    UnsubscribeResultTypeDef,
     ListEventTypesResultTypeDef,
     DescribeNotificationRuleResultTypeDef,
     ListTargetsResultTypeDef,
-    ListEventTypesRequestRequestTypeDef,
     ListEventTypesRequestListEventTypesPaginateTypeDef,
+    ListEventTypesRequestRequestTypeDef,
     ListNotificationRulesRequestListNotificationRulesPaginateTypeDef,
     ListNotificationRulesRequestRequestTypeDef,
     ListNotificationRulesResultTypeDef,
     ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
 )
 
@@ -384,42 +385,42 @@
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

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/mypy_boto3_codestar_notifications.egg-info/SOURCES.txt` & `mypy-boto3-codestar-notifications-1.27.0/mypy_boto3_codestar_notifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.26.0.post1/setup.py` & `mypy-boto3-codestar-notifications-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """
 Setup script for mypy-boto3-codestar-notifications.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codestar-notifications",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_codestar_notifications"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeStarNotifications 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.CodeStarNotifications 1.27.0 service generated with"
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
     keywords="boto3 codestar-notifications type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_codestar_notifications": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_codestar_notifications": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/"
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


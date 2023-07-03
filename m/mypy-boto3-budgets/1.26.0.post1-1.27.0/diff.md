# Comparing `tmp/mypy-boto3-budgets-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-budgets-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-budgets-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:09 2022, max compression
+gzip compressed data, was "mypy-boto3-budgets-1.27.0.tar", last modified: Mon Jul  3 19:50:27 2023, max compression
```

## Comparing `mypy-boto3-budgets-1.26.0.post1.tar` & `mypy-boto3-budgets-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:09.816836 mypy-boto3-budgets-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    17649 2022-11-01 21:43:09.808837 mypy-boto3-budgets-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16208 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:09.808837 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/
--rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2721 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21967 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    21929 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9947 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9945 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10983 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    10973 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    31328 2022-11-01 21:31:03.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    31279 2022-11-01 21:31:03.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:09.808837 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17649 2022-11-01 21:43:09.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-11-01 21:43:09.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:09.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:09.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:09.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-01 21:43:09.000000 mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:09.816836 mypy-boto3-budgets-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-11-01 21:31:02.000000 mypy-boto3-budgets-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.066902 mypy-boto3-budgets-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-07-03 19:50:27.066902 mypy-boto3-budgets-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.062902 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21965 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21927 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10654 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31372 2023-07-03 19:33:13.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31323 2023-07-03 19:33:13.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.066902 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-07-03 19:50:26.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 19:50:26.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:26.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:26.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:26.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:50:26.000000 mypy-boto3-budgets-1.27.0/mypy_boto3_budgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:27.066902 mypy-boto3-budgets-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:33:12.000000 mypy-boto3-budgets-1.27.0/setup.py
```

### Comparing `mypy-boto3-budgets-1.26.0.post1/LICENSE` & `mypy-boto3-budgets-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-budgets-1.26.0.post1/PKG-INFO` & `mypy-boto3-budgets-1.27.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-budgets
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Budgets 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Budgets 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
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
 
 <a id="mypy-boto3-budgets"></a>
 
 # mypy-boto3-budgets
 
 [![PyPI - mypy-boto3-budgets](https://img.shields.io/pypi/v/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-budgets?color=blue)](https://pypistats.org/packages/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,56 +375,56 @@
     ActionThresholdTypeDef,
     SubscriberTypeDef,
     HistoricalOptionsTypeDef,
     NotificationTypeDef,
     CostTypesTypeDef,
     SpendTypeDef,
     TimePeriodTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBudgetActionResponseTypeDef,
     IamActionDefinitionTypeDef,
     ScpActionDefinitionTypeDef,
     SsmActionDefinitionTypeDef,
     DeleteBudgetActionRequestRequestTypeDef,
     DeleteBudgetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     DescribeBudgetActionRequestRequestTypeDef,
+    DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
     DescribeBudgetActionsForAccountRequestRequestTypeDef,
+    DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
     DescribeBudgetActionsForBudgetRequestRequestTypeDef,
+    DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
     DescribeBudgetNotificationsForAccountRequestRequestTypeDef,
     DescribeBudgetRequestRequestTypeDef,
+    DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
     DescribeBudgetsRequestRequestTypeDef,
+    DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
     DescribeNotificationsForBudgetRequestRequestTypeDef,
     ExecuteBudgetActionRequestRequestTypeDef,
+    ExecuteBudgetActionResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    DescribeSubscribersForNotificationResponseTypeDef,
     AutoAdjustDataTypeDef,
     BudgetNotificationsForAccountTypeDef,
     CreateNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     DeleteNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
+    DescribeNotificationsForBudgetResponseTypeDef,
+    DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeSubscribersForNotificationRequestRequestTypeDef,
     NotificationWithSubscribersTypeDef,
     UpdateNotificationRequestRequestTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CalculatedSpendTypeDef,
     BudgetedAndActualAmountsTypeDef,
+    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     DescribeBudgetActionHistoriesRequestRequestTypeDef,
+    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-    CreateBudgetActionResponseTypeDef,
-    DescribeNotificationsForBudgetResponseTypeDef,
-    DescribeSubscribersForNotificationResponseTypeDef,
-    ExecuteBudgetActionResponseTypeDef,
     DefinitionTypeDef,
-    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
-    DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
-    DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
-    DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
-    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
-    DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
-    DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
-    DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     BudgetTypeDef,
     BudgetPerformanceHistoryTypeDef,
     ActionTypeDef,
     CreateBudgetActionRequestRequestTypeDef,
     UpdateBudgetActionRequestRequestTypeDef,
     CreateBudgetRequestRequestTypeDef,
@@ -449,42 +450,42 @@
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

### Comparing `mypy-boto3-budgets-1.26.0.post1/README.md` & `mypy-boto3-budgets-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-budgets"></a>
 
 # mypy-boto3-budgets
 
 [![PyPI - mypy-boto3-budgets](https://img.shields.io/pypi/v/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-budgets?color=blue)](https://pypistats.org/packages/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,56 +343,56 @@
     ActionThresholdTypeDef,
     SubscriberTypeDef,
     HistoricalOptionsTypeDef,
     NotificationTypeDef,
     CostTypesTypeDef,
     SpendTypeDef,
     TimePeriodTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBudgetActionResponseTypeDef,
     IamActionDefinitionTypeDef,
     ScpActionDefinitionTypeDef,
     SsmActionDefinitionTypeDef,
     DeleteBudgetActionRequestRequestTypeDef,
     DeleteBudgetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     DescribeBudgetActionRequestRequestTypeDef,
+    DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
     DescribeBudgetActionsForAccountRequestRequestTypeDef,
+    DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
     DescribeBudgetActionsForBudgetRequestRequestTypeDef,
+    DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
     DescribeBudgetNotificationsForAccountRequestRequestTypeDef,
     DescribeBudgetRequestRequestTypeDef,
+    DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
     DescribeBudgetsRequestRequestTypeDef,
+    DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
     DescribeNotificationsForBudgetRequestRequestTypeDef,
     ExecuteBudgetActionRequestRequestTypeDef,
+    ExecuteBudgetActionResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    DescribeSubscribersForNotificationResponseTypeDef,
     AutoAdjustDataTypeDef,
     BudgetNotificationsForAccountTypeDef,
     CreateNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     DeleteNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
+    DescribeNotificationsForBudgetResponseTypeDef,
+    DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeSubscribersForNotificationRequestRequestTypeDef,
     NotificationWithSubscribersTypeDef,
     UpdateNotificationRequestRequestTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CalculatedSpendTypeDef,
     BudgetedAndActualAmountsTypeDef,
+    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     DescribeBudgetActionHistoriesRequestRequestTypeDef,
+    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-    CreateBudgetActionResponseTypeDef,
-    DescribeNotificationsForBudgetResponseTypeDef,
-    DescribeSubscribersForNotificationResponseTypeDef,
-    ExecuteBudgetActionResponseTypeDef,
     DefinitionTypeDef,
-    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
-    DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
-    DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
-    DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
-    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
-    DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
-    DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
-    DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     BudgetTypeDef,
     BudgetPerformanceHistoryTypeDef,
     ActionTypeDef,
     CreateBudgetActionRequestRequestTypeDef,
     UpdateBudgetActionRequestRequestTypeDef,
     CreateBudgetRequestRequestTypeDef,
@@ -418,42 +418,42 @@
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

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/__init__.py` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/__init__.pyi` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/__main__.py` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Budgets 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Budgets 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets\nOther"
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

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/client.py` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         AccountId: str,
         BudgetName: str,
         TimePeriod: TimePeriodTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
-        Describes the history for `DAILY` , `MONTHLY` , and `QUARTERLY` budgets.
+        Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#describe_budget_performance_history)
         """
 
     def describe_budgets(
         self, *, AccountId: str, MaxResults: int = ..., NextToken: str = ...
```

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/client.pyi` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
         AccountId: str,
         BudgetName: str,
         TimePeriod: TimePeriodTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
-        Describes the history for `DAILY` , `MONTHLY` , and `QUARTERLY` budgets.
+        Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#describe_budget_performance_history)
         """
     def describe_budgets(
         self, *, AccountId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeBudgetsResponseTypeDef:
```

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/literals.py` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,23 +107,25 @@
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
@@ -133,30 +135,35 @@
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
@@ -182,14 +189,15 @@
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
@@ -234,51 +242,57 @@
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
@@ -291,14 +305,15 @@
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
@@ -310,28 +325,35 @@
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
@@ -340,14 +362,15 @@
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
@@ -358,55 +381,64 @@
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

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/literals.pyi` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -105,23 +105,25 @@
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
@@ -131,30 +133,35 @@
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
@@ -180,14 +187,15 @@
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
@@ -232,51 +240,57 @@
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
@@ -289,14 +303,15 @@
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
@@ -308,28 +323,35 @@
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
@@ -338,14 +360,15 @@
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
@@ -356,55 +379,64 @@
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

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/paginator.py` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,60 +82,60 @@
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBudgetActionHistoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
 
 class DescribeBudgetActionsForAccountPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforaccountpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBudgetActionsForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforaccountpaginator)
         """
 
 
 class DescribeBudgetActionsForBudgetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforbudgetpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, BudgetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AccountId: str, BudgetName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBudgetActionsForBudgetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforbudgetpaginator)
         """
 
 
 class DescribeBudgetNotificationsForAccountPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetnotificationsforaccountpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBudgetNotificationsForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetnotificationsforaccountpaginator)
         """
 
 
@@ -147,45 +147,45 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
 
 
 class DescribeBudgetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetspaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBudgetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetspaginator)
         """
 
 
 class DescribeNotificationsForBudgetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describenotificationsforbudgetpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, BudgetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AccountId: str, BudgetName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeNotificationsForBudgetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describenotificationsforbudgetpaginator)
         """
 
 
@@ -197,13 +197,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSubscribersForNotificationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeSubscribersForNotification.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describesubscribersfornotificationpaginator)
         """
```

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/paginator.pyi` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -79,57 +79,57 @@
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBudgetActionHistoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
 class DescribeBudgetActionsForAccountPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforaccountpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBudgetActionsForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforaccountpaginator)
         """
 
 class DescribeBudgetActionsForBudgetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforbudgetpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, BudgetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AccountId: str, BudgetName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBudgetActionsForBudgetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforbudgetpaginator)
         """
 
 class DescribeBudgetNotificationsForAccountPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetnotificationsforaccountpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBudgetNotificationsForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetnotificationsforaccountpaginator)
         """
 
 class DescribeBudgetPerformanceHistoryPaginator(Paginator):
@@ -140,43 +140,43 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
 
 class DescribeBudgetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetspaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBudgetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetspaginator)
         """
 
 class DescribeNotificationsForBudgetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describenotificationsforbudgetpaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, BudgetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AccountId: str, BudgetName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeNotificationsForBudgetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describenotificationsforbudgetpaginator)
         """
 
 class DescribeSubscribersForNotificationPaginator(Paginator):
@@ -187,13 +187,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSubscribersForNotificationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeSubscribersForNotification.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describesubscribersfornotificationpaginator)
         """
```

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/type_defs.py` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,56 +42,56 @@
     "ActionThresholdTypeDef",
     "SubscriberTypeDef",
     "HistoricalOptionsTypeDef",
     "NotificationTypeDef",
     "CostTypesTypeDef",
     "SpendTypeDef",
     "TimePeriodTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateBudgetActionResponseTypeDef",
     "IamActionDefinitionTypeDef",
     "ScpActionDefinitionTypeDef",
     "SsmActionDefinitionTypeDef",
     "DeleteBudgetActionRequestRequestTypeDef",
     "DeleteBudgetRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "DescribeBudgetActionRequestRequestTypeDef",
+    "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
     "DescribeBudgetActionsForAccountRequestRequestTypeDef",
+    "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
     "DescribeBudgetActionsForBudgetRequestRequestTypeDef",
+    "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
     "DescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     "DescribeBudgetRequestRequestTypeDef",
+    "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
     "DescribeBudgetsRequestRequestTypeDef",
+    "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
     "DescribeNotificationsForBudgetRequestRequestTypeDef",
     "ExecuteBudgetActionRequestRequestTypeDef",
+    "ExecuteBudgetActionResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "DescribeSubscribersForNotificationResponseTypeDef",
     "AutoAdjustDataTypeDef",
     "BudgetNotificationsForAccountTypeDef",
     "CreateNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "DeleteNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
+    "DescribeNotificationsForBudgetResponseTypeDef",
+    "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
     "DescribeSubscribersForNotificationRequestRequestTypeDef",
     "NotificationWithSubscribersTypeDef",
     "UpdateNotificationRequestRequestTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CalculatedSpendTypeDef",
     "BudgetedAndActualAmountsTypeDef",
+    "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
     "DescribeBudgetActionHistoriesRequestRequestTypeDef",
+    "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    "CreateBudgetActionResponseTypeDef",
-    "DescribeNotificationsForBudgetResponseTypeDef",
-    "DescribeSubscribersForNotificationResponseTypeDef",
-    "ExecuteBudgetActionResponseTypeDef",
     "DefinitionTypeDef",
-    "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
-    "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
-    "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
-    "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
-    "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
-    "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
-    "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
-    "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
     "BudgetTypeDef",
     "BudgetPerformanceHistoryTypeDef",
     "ActionTypeDef",
     "CreateBudgetActionRequestRequestTypeDef",
     "UpdateBudgetActionRequestRequestTypeDef",
     "CreateBudgetRequestRequestTypeDef",
@@ -199,22 +199,21 @@
     {
         "Start": Union[datetime, str],
         "End": Union[datetime, str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateBudgetActionResponseTypeDef = TypedDict(
+    "CreateBudgetActionResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AccountId": str,
+        "BudgetName": str,
+        "ActionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredIamActionDefinitionTypeDef = TypedDict(
     "_RequiredIamActionDefinitionTypeDef",
     {
         "PolicyArn": str,
@@ -267,33 +266,45 @@
     "DeleteBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
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
 DescribeBudgetActionRequestRequestTypeDef = TypedDict(
     "DescribeBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
     },
 )
 
+_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef(
+    _RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
+    _OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeBudgetActionsForAccountRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetActionsForAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetActionsForAccountRequestRequestTypeDef = TypedDict(
@@ -309,14 +320,37 @@
 class DescribeBudgetActionsForAccountRequestRequestTypeDef(
     _RequiredDescribeBudgetActionsForAccountRequestRequestTypeDef,
     _OptionalDescribeBudgetActionsForAccountRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+    },
+)
+_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef(
+    _RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
+    _OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeBudgetActionsForBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetActionsForBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
@@ -333,14 +367,36 @@
 class DescribeBudgetActionsForBudgetRequestRequestTypeDef(
     _RequiredDescribeBudgetActionsForBudgetRequestRequestTypeDef,
     _OptionalDescribeBudgetActionsForBudgetRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef(
+    _RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+    _OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeBudgetNotificationsForAccountRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetNotificationsForAccountRequestRequestTypeDef = TypedDict(
@@ -364,14 +420,36 @@
     "DescribeBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
 
+_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef(
+    _RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
+    _OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeBudgetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetsRequestRequestTypeDef = TypedDict(
@@ -386,14 +464,37 @@
 
 class DescribeBudgetsRequestRequestTypeDef(
     _RequiredDescribeBudgetsRequestRequestTypeDef, _OptionalDescribeBudgetsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+    },
+)
+_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef(
+    _RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+    _OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeNotificationsForBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNotificationsForBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
@@ -420,14 +521,55 @@
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ExecutionType": ExecutionTypeType,
     },
 )
 
+ExecuteBudgetActionResponseTypeDef = TypedDict(
+    "ExecuteBudgetActionResponseTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "ActionId": str,
+        "ExecutionType": ExecutionTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
+DescribeSubscribersForNotificationResponseTypeDef = TypedDict(
+    "DescribeSubscribersForNotificationResponseTypeDef",
+    {
+        "Subscribers": List[SubscriberTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAutoAdjustDataTypeDef = TypedDict(
     "_RequiredAutoAdjustDataTypeDef",
     {
         "AutoAdjustType": AutoAdjustTypeType,
     },
 )
 _OptionalAutoAdjustDataTypeDef = TypedDict(
@@ -488,14 +630,47 @@
         "AccountId": str,
         "BudgetName": str,
         "Notification": NotificationTypeDef,
         "Subscriber": SubscriberTypeDef,
     },
 )
 
+DescribeNotificationsForBudgetResponseTypeDef = TypedDict(
+    "DescribeNotificationsForBudgetResponseTypeDef",
+    {
+        "Notifications": List[NotificationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+    },
+)
+_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
+    _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+    _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeSubscribersForNotificationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSubscribersForNotificationRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "Notification": NotificationTypeDef,
     },
@@ -571,114 +746,14 @@
         "BudgetedAmount": SpendTypeDef,
         "ActualAmount": SpendTypeDef,
         "TimePeriod": TimePeriodTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
-    },
-)
-_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef",
-    {
-        "TimePeriod": TimePeriodTypeDef,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class DescribeBudgetActionHistoriesRequestRequestTypeDef(
-    _RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef,
-    _OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-    },
-)
-_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    {
-        "TimePeriod": TimePeriodTypeDef,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
-    _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-    _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-):
-    pass
-
-
-CreateBudgetActionResponseTypeDef = TypedDict(
-    "CreateBudgetActionResponseTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeNotificationsForBudgetResponseTypeDef = TypedDict(
-    "DescribeNotificationsForBudgetResponseTypeDef",
-    {
-        "Notifications": List[NotificationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSubscribersForNotificationResponseTypeDef = TypedDict(
-    "DescribeSubscribersForNotificationResponseTypeDef",
-    {
-        "Subscribers": List[SubscriberTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExecuteBudgetActionResponseTypeDef = TypedDict(
-    "ExecuteBudgetActionResponseTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
-        "ExecutionType": ExecutionTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DefinitionTypeDef = TypedDict(
-    "DefinitionTypeDef",
-    {
-        "IamActionDefinition": IamActionDefinitionTypeDef,
-        "ScpActionDefinition": ScpActionDefinitionTypeDef,
-        "SsmActionDefinition": SsmActionDefinitionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
     TypedDict(
         "_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
         {
             "AccountId": str,
             "BudgetName": str,
             "ActionId": str,
@@ -686,91 +761,50 @@
     )
 )
 _OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
     TypedDict(
         "_OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
         {
             "TimePeriod": TimePeriodTypeDef,
-            "PaginationConfig": PaginatorConfigTypeDef,
+            "PaginationConfig": "PaginatorConfigTypeDef",
         },
         total=False,
     )
 )
 
 
 class DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef(
     _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     _OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef(
-    _RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
-    _OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
+_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
+        "ActionId": str,
     },
 )
-_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef(
-    _RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
-    _OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
+_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "TimePeriod": TimePeriodTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
 
-class DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef(
-    _RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
-    _OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+class DescribeBudgetActionHistoriesRequestRequestTypeDef(
+    _RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef,
+    _OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef,
 ):
     pass
 
 
 _RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
     "_RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     {
@@ -778,102 +812,68 @@
         "BudgetName": str,
     },
 )
 _OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
     "_OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     {
         "TimePeriod": TimePeriodTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef(
     _RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     _OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
 ):
     pass
 
 
-_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef(
-    _RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
-    _OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
-_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "TimePeriod": TimePeriodTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
 
-class DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef(
-    _RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
-    _OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
+    _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
+    _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-    },
-)
-_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+DefinitionTypeDef = TypedDict(
+    "DefinitionTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "IamActionDefinition": IamActionDefinitionTypeDef,
+        "ScpActionDefinition": ScpActionDefinitionTypeDef,
+        "SsmActionDefinition": SsmActionDefinitionTypeDef,
     },
     total=False,
 )
 
-
-class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
-    _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
-    _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
-):
-    pass
-
-
 DescribeBudgetNotificationsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
     {
         "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBudgetTypeDef = TypedDict(
     "_RequiredBudgetTypeDef",
     {
         "BudgetName": str,
@@ -996,24 +996,24 @@
     pass
 
 
 DescribeBudgetResponseTypeDef = TypedDict(
     "DescribeBudgetResponseTypeDef",
     {
         "Budget": BudgetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBudgetsResponseTypeDef = TypedDict(
     "DescribeBudgetsResponseTypeDef",
     {
         "Budgets": List[BudgetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBudgetRequestRequestTypeDef = TypedDict(
     "UpdateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -1022,15 +1022,15 @@
 )
 
 DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
     "DescribeBudgetPerformanceHistoryResponseTypeDef",
     {
         "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActionHistoryDetailsTypeDef = TypedDict(
     "ActionHistoryDetailsTypeDef",
     {
         "Message": str,
@@ -1040,54 +1040,54 @@
 
 DeleteBudgetActionResponseTypeDef = TypedDict(
     "DeleteBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "Action": ActionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBudgetActionResponseTypeDef = TypedDict(
     "DescribeBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "Action": ActionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBudgetActionsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetActionsForAccountResponseTypeDef",
     {
         "Actions": List[ActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBudgetActionsForBudgetResponseTypeDef = TypedDict(
     "DescribeBudgetActionsForBudgetResponseTypeDef",
     {
         "Actions": List[ActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBudgetActionResponseTypeDef = TypedDict(
     "UpdateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "OldAction": ActionTypeDef,
         "NewAction": ActionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActionHistoryTypeDef = TypedDict(
     "ActionHistoryTypeDef",
     {
         "Timestamp": datetime,
@@ -1098,10 +1098,10 @@
 )
 
 DescribeBudgetActionHistoriesResponseTypeDef = TypedDict(
     "DescribeBudgetActionHistoriesResponseTypeDef",
     {
         "ActionHistories": List[ActionHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets/type_defs.pyi` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -41,56 +41,56 @@
     "ActionThresholdTypeDef",
     "SubscriberTypeDef",
     "HistoricalOptionsTypeDef",
     "NotificationTypeDef",
     "CostTypesTypeDef",
     "SpendTypeDef",
     "TimePeriodTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateBudgetActionResponseTypeDef",
     "IamActionDefinitionTypeDef",
     "ScpActionDefinitionTypeDef",
     "SsmActionDefinitionTypeDef",
     "DeleteBudgetActionRequestRequestTypeDef",
     "DeleteBudgetRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "DescribeBudgetActionRequestRequestTypeDef",
+    "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
     "DescribeBudgetActionsForAccountRequestRequestTypeDef",
+    "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
     "DescribeBudgetActionsForBudgetRequestRequestTypeDef",
+    "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
     "DescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     "DescribeBudgetRequestRequestTypeDef",
+    "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
     "DescribeBudgetsRequestRequestTypeDef",
+    "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
     "DescribeNotificationsForBudgetRequestRequestTypeDef",
     "ExecuteBudgetActionRequestRequestTypeDef",
+    "ExecuteBudgetActionResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "DescribeSubscribersForNotificationResponseTypeDef",
     "AutoAdjustDataTypeDef",
     "BudgetNotificationsForAccountTypeDef",
     "CreateNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "DeleteNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
+    "DescribeNotificationsForBudgetResponseTypeDef",
+    "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
     "DescribeSubscribersForNotificationRequestRequestTypeDef",
     "NotificationWithSubscribersTypeDef",
     "UpdateNotificationRequestRequestTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CalculatedSpendTypeDef",
     "BudgetedAndActualAmountsTypeDef",
+    "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
     "DescribeBudgetActionHistoriesRequestRequestTypeDef",
+    "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    "CreateBudgetActionResponseTypeDef",
-    "DescribeNotificationsForBudgetResponseTypeDef",
-    "DescribeSubscribersForNotificationResponseTypeDef",
-    "ExecuteBudgetActionResponseTypeDef",
     "DefinitionTypeDef",
-    "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
-    "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
-    "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
-    "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
-    "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
-    "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
-    "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
-    "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
     "BudgetTypeDef",
     "BudgetPerformanceHistoryTypeDef",
     "ActionTypeDef",
     "CreateBudgetActionRequestRequestTypeDef",
     "UpdateBudgetActionRequestRequestTypeDef",
     "CreateBudgetRequestRequestTypeDef",
@@ -194,22 +194,21 @@
     {
         "Start": Union[datetime, str],
         "End": Union[datetime, str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateBudgetActionResponseTypeDef = TypedDict(
+    "CreateBudgetActionResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AccountId": str,
+        "BudgetName": str,
+        "ActionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredIamActionDefinitionTypeDef = TypedDict(
     "_RequiredIamActionDefinitionTypeDef",
     {
         "PolicyArn": str,
@@ -260,33 +259,43 @@
     "DeleteBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
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
 DescribeBudgetActionRequestRequestTypeDef = TypedDict(
     "DescribeBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
     },
 )
 
+_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef(
+    _RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
+    _OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeBudgetActionsForAccountRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetActionsForAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetActionsForAccountRequestRequestTypeDef = TypedDict(
@@ -300,14 +309,35 @@
 
 class DescribeBudgetActionsForAccountRequestRequestTypeDef(
     _RequiredDescribeBudgetActionsForAccountRequestRequestTypeDef,
     _OptionalDescribeBudgetActionsForAccountRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+    },
+)
+_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef(
+    _RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
+    _OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeBudgetActionsForBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetActionsForBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
@@ -322,14 +352,34 @@
 
 class DescribeBudgetActionsForBudgetRequestRequestTypeDef(
     _RequiredDescribeBudgetActionsForBudgetRequestRequestTypeDef,
     _OptionalDescribeBudgetActionsForBudgetRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef(
+    _RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+    _OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeBudgetNotificationsForAccountRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetNotificationsForAccountRequestRequestTypeDef = TypedDict(
@@ -351,14 +401,34 @@
     "DescribeBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
 
+_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef(
+    _RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
+    _OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeBudgetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeBudgetsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetsRequestRequestTypeDef = TypedDict(
@@ -371,14 +441,35 @@
 )
 
 class DescribeBudgetsRequestRequestTypeDef(
     _RequiredDescribeBudgetsRequestRequestTypeDef, _OptionalDescribeBudgetsRequestRequestTypeDef
 ):
     pass
 
+_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+    },
+)
+_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef(
+    _RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+    _OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeNotificationsForBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNotificationsForBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
@@ -403,14 +494,55 @@
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ExecutionType": ExecutionTypeType,
     },
 )
 
+ExecuteBudgetActionResponseTypeDef = TypedDict(
+    "ExecuteBudgetActionResponseTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "ActionId": str,
+        "ExecutionType": ExecutionTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
+DescribeSubscribersForNotificationResponseTypeDef = TypedDict(
+    "DescribeSubscribersForNotificationResponseTypeDef",
+    {
+        "Subscribers": List[SubscriberTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAutoAdjustDataTypeDef = TypedDict(
     "_RequiredAutoAdjustDataTypeDef",
     {
         "AutoAdjustType": AutoAdjustTypeType,
     },
 )
 _OptionalAutoAdjustDataTypeDef = TypedDict(
@@ -469,14 +601,45 @@
         "AccountId": str,
         "BudgetName": str,
         "Notification": NotificationTypeDef,
         "Subscriber": SubscriberTypeDef,
     },
 )
 
+DescribeNotificationsForBudgetResponseTypeDef = TypedDict(
+    "DescribeNotificationsForBudgetResponseTypeDef",
+    {
+        "Notifications": List[NotificationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+    },
+)
+_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
+    _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+    _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeSubscribersForNotificationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSubscribersForNotificationRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "Notification": NotificationTypeDef,
     },
@@ -548,110 +711,14 @@
         "BudgetedAmount": SpendTypeDef,
         "ActualAmount": SpendTypeDef,
         "TimePeriod": TimePeriodTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
-    },
-)
-_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef",
-    {
-        "TimePeriod": TimePeriodTypeDef,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class DescribeBudgetActionHistoriesRequestRequestTypeDef(
-    _RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef,
-    _OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef,
-):
-    pass
-
-_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-    },
-)
-_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    {
-        "TimePeriod": TimePeriodTypeDef,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
-    _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-    _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-):
-    pass
-
-CreateBudgetActionResponseTypeDef = TypedDict(
-    "CreateBudgetActionResponseTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeNotificationsForBudgetResponseTypeDef = TypedDict(
-    "DescribeNotificationsForBudgetResponseTypeDef",
-    {
-        "Notifications": List[NotificationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSubscribersForNotificationResponseTypeDef = TypedDict(
-    "DescribeSubscribersForNotificationResponseTypeDef",
-    {
-        "Subscribers": List[SubscriberTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExecuteBudgetActionResponseTypeDef = TypedDict(
-    "ExecuteBudgetActionResponseTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
-        "ExecutionType": ExecutionTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DefinitionTypeDef = TypedDict(
-    "DefinitionTypeDef",
-    {
-        "IamActionDefinition": IamActionDefinitionTypeDef,
-        "ScpActionDefinition": ScpActionDefinitionTypeDef,
-        "SsmActionDefinition": SsmActionDefinitionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
     TypedDict(
         "_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
         {
             "AccountId": str,
             "BudgetName": str,
             "ActionId": str,
@@ -659,178 +726,111 @@
     )
 )
 _OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
     TypedDict(
         "_OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
         {
             "TimePeriod": TimePeriodTypeDef,
-            "PaginationConfig": PaginatorConfigTypeDef,
+            "PaginationConfig": "PaginatorConfigTypeDef",
         },
         total=False,
     )
 )
 
 class DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef(
     _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     _OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
 ):
     pass
 
-_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef(
-    _RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
-    _OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
+_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
+        "ActionId": str,
     },
 )
-_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef(
-    _RequiredDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
-    _OptionalDescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
+_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "TimePeriod": TimePeriodTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-class DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef(
-    _RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
-    _OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
+class DescribeBudgetActionHistoriesRequestRequestTypeDef(
+    _RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef,
+    _OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef,
 ):
     pass
 
 _RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
     "_RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
 _OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
     "_OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     {
         "TimePeriod": TimePeriodTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef(
     _RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     _OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
 ):
     pass
 
-_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef(
-    _RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
-    _OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
     },
 )
-_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
+_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "TimePeriod": TimePeriodTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-class DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef(
-    _RequiredDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
-    _OptionalDescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
+class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
+    _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
+    _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-    },
-)
-_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+DefinitionTypeDef = TypedDict(
+    "DefinitionTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "IamActionDefinition": IamActionDefinitionTypeDef,
+        "ScpActionDefinition": ScpActionDefinitionTypeDef,
+        "SsmActionDefinition": SsmActionDefinitionTypeDef,
     },
     total=False,
 )
 
-class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
-    _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
-    _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
-):
-    pass
-
 DescribeBudgetNotificationsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
     {
         "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBudgetTypeDef = TypedDict(
     "_RequiredBudgetTypeDef",
     {
         "BudgetName": str,
@@ -947,24 +947,24 @@
 ):
     pass
 
 DescribeBudgetResponseTypeDef = TypedDict(
     "DescribeBudgetResponseTypeDef",
     {
         "Budget": BudgetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBudgetsResponseTypeDef = TypedDict(
     "DescribeBudgetsResponseTypeDef",
     {
         "Budgets": List[BudgetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBudgetRequestRequestTypeDef = TypedDict(
     "UpdateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -973,15 +973,15 @@
 )
 
 DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
     "DescribeBudgetPerformanceHistoryResponseTypeDef",
     {
         "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActionHistoryDetailsTypeDef = TypedDict(
     "ActionHistoryDetailsTypeDef",
     {
         "Message": str,
@@ -991,54 +991,54 @@
 
 DeleteBudgetActionResponseTypeDef = TypedDict(
     "DeleteBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "Action": ActionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBudgetActionResponseTypeDef = TypedDict(
     "DescribeBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "Action": ActionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBudgetActionsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetActionsForAccountResponseTypeDef",
     {
         "Actions": List[ActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBudgetActionsForBudgetResponseTypeDef = TypedDict(
     "DescribeBudgetActionsForBudgetResponseTypeDef",
     {
         "Actions": List[ActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBudgetActionResponseTypeDef = TypedDict(
     "UpdateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "OldAction": ActionTypeDef,
         "NewAction": ActionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActionHistoryTypeDef = TypedDict(
     "ActionHistoryTypeDef",
     {
         "Timestamp": datetime,
@@ -1049,10 +1049,10 @@
 )
 
 DescribeBudgetActionHistoriesResponseTypeDef = TypedDict(
     "DescribeBudgetActionHistoriesResponseTypeDef",
     {
         "ActionHistories": List[ActionHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets.egg-info/PKG-INFO` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-budgets
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Budgets 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Budgets 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
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
 
 <a id="mypy-boto3-budgets"></a>
 
 # mypy-boto3-budgets
 
 [![PyPI - mypy-boto3-budgets](https://img.shields.io/pypi/v/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-budgets?color=blue)](https://pypistats.org/packages/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,56 +375,56 @@
     ActionThresholdTypeDef,
     SubscriberTypeDef,
     HistoricalOptionsTypeDef,
     NotificationTypeDef,
     CostTypesTypeDef,
     SpendTypeDef,
     TimePeriodTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBudgetActionResponseTypeDef,
     IamActionDefinitionTypeDef,
     ScpActionDefinitionTypeDef,
     SsmActionDefinitionTypeDef,
     DeleteBudgetActionRequestRequestTypeDef,
     DeleteBudgetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     DescribeBudgetActionRequestRequestTypeDef,
+    DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
     DescribeBudgetActionsForAccountRequestRequestTypeDef,
+    DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
     DescribeBudgetActionsForBudgetRequestRequestTypeDef,
+    DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
     DescribeBudgetNotificationsForAccountRequestRequestTypeDef,
     DescribeBudgetRequestRequestTypeDef,
+    DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
     DescribeBudgetsRequestRequestTypeDef,
+    DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
     DescribeNotificationsForBudgetRequestRequestTypeDef,
     ExecuteBudgetActionRequestRequestTypeDef,
+    ExecuteBudgetActionResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    DescribeSubscribersForNotificationResponseTypeDef,
     AutoAdjustDataTypeDef,
     BudgetNotificationsForAccountTypeDef,
     CreateNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     DeleteNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
+    DescribeNotificationsForBudgetResponseTypeDef,
+    DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeSubscribersForNotificationRequestRequestTypeDef,
     NotificationWithSubscribersTypeDef,
     UpdateNotificationRequestRequestTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CalculatedSpendTypeDef,
     BudgetedAndActualAmountsTypeDef,
+    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     DescribeBudgetActionHistoriesRequestRequestTypeDef,
+    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-    CreateBudgetActionResponseTypeDef,
-    DescribeNotificationsForBudgetResponseTypeDef,
-    DescribeSubscribersForNotificationResponseTypeDef,
-    ExecuteBudgetActionResponseTypeDef,
     DefinitionTypeDef,
-    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
-    DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
-    DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
-    DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
-    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
-    DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
-    DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
-    DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     BudgetTypeDef,
     BudgetPerformanceHistoryTypeDef,
     ActionTypeDef,
     CreateBudgetActionRequestRequestTypeDef,
     UpdateBudgetActionRequestRequestTypeDef,
     CreateBudgetRequestRequestTypeDef,
@@ -449,42 +450,42 @@
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

### Comparing `mypy-boto3-budgets-1.26.0.post1/mypy_boto3_budgets.egg-info/SOURCES.txt` & `mypy-boto3-budgets-1.27.0/mypy_boto3_budgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.26.0.post1/setup.py` & `mypy-boto3-budgets-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 """
 Setup script for mypy-boto3-budgets.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-budgets",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_budgets"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Budgets 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.Budgets 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 budgets type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_budgets": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_budgets": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/",
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


# Comparing `tmp/mypy-boto3-license-manager-user-subscriptions-1.26.18.tar.gz` & `tmp/mypy-boto3-license-manager-user-subscriptions-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-user-subscriptions-1.26.18.tar", last modified: Tue Nov 29 06:12:20 2022, max compression
+gzip compressed data, was "mypy-boto3-license-manager-user-subscriptions-1.27.0.tar", last modified: Mon Jul  3 19:51:01 2023, max compression
```

## Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18.tar` & `mypy-boto3-license-manager-user-subscriptions-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:20.457836 mypy-boto3-license-manager-user-subscriptions-1.26.18/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    16161 2022-11-29 06:12:20.457836 mypy-boto3-license-manager-user-subscriptions-1.26.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14619 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:20.457836 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1510 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1021 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14524 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    14502 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     8189 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)     8187 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     6348 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6342 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    15829 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    15800 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-29 06:10:27.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:20.457836 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    16161 2022-11-29 06:12:20.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2022-11-29 06:12:20.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 06:12:20.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 06:12:20.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-29 06:12:20.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2022-11-29 06:12:20.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 06:12:20.457836 mypy-boto3-license-manager-user-subscriptions-1.26.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2022-11-29 06:10:26.000000 mypy-boto3-license-manager-user-subscriptions-1.26.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.951566 mypy-boto3-license-manager-user-subscriptions-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-07-03 19:51:01.951566 mypy-boto3-license-manager-user-subscriptions-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14623 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.951566 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-03 19:41:03.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-03 19:41:03.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-03 19:41:03.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-07-03 19:41:03.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-03 19:41:03.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-03 19:41:03.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15859 2023-07-03 19:41:03.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-03 19:41:03.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.951566 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:01.951566 mypy-boto3-license-manager-user-subscriptions-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-user-subscriptions-1.27.0/setup.py
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/LICENSE` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/PKG-INFO` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-user-subscriptions
-Version: 1.26.18
-Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.26.18 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/
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
 
 <a id="mypy-boto3-license-manager-user-subscriptions"></a>
 
 # mypy-boto3-license-manager-user-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-user-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager-user-subscriptions?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerUserSubscriptions 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[boto3.LicenseManagerUserSubscriptions 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,26 +347,26 @@
 `mypy_boto3_license_manager_user_subscriptions.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_user_subscriptions.type_defs import (
     ActiveDirectoryIdentityProviderTypeDef,
-    ResponseMetadataTypeDef,
     FilterTypeDef,
     SettingsTypeDef,
     InstanceSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateSettingsTypeDef,
     IdentityProviderTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
     IdentityProviderSummaryTypeDef,
     InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
@@ -396,42 +397,42 @@
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

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/README.md` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-license-manager-user-subscriptions"></a>
 
 # mypy-boto3-license-manager-user-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-user-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager-user-subscriptions?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerUserSubscriptions 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[boto3.LicenseManagerUserSubscriptions 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -315,26 +315,26 @@
 `mypy_boto3_license_manager_user_subscriptions.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_user_subscriptions.type_defs import (
     ActiveDirectoryIdentityProviderTypeDef,
-    ResponseMetadataTypeDef,
     FilterTypeDef,
     SettingsTypeDef,
     InstanceSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateSettingsTypeDef,
     IdentityProviderTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
     IdentityProviderSummaryTypeDef,
     InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
@@ -365,42 +365,42 @@
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

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/__init__.py` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/__init__.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/client.py` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/client.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/literals.py` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,15 @@
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
@@ -76,30 +77,34 @@
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
@@ -125,14 +130,15 @@
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
@@ -177,14 +183,15 @@
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
@@ -195,34 +202,38 @@
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
@@ -235,14 +246,15 @@
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
@@ -255,28 +267,34 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -304,30 +322,34 @@
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
@@ -343,18 +365,21 @@
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

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/literals.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
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
@@ -74,30 +75,34 @@
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
@@ -123,14 +128,15 @@
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
@@ -175,14 +181,15 @@
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
@@ -193,34 +200,38 @@
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
@@ -233,14 +244,15 @@
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
@@ -253,28 +265,34 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -302,30 +320,34 @@
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
@@ -341,18 +363,21 @@
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

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/paginator.py` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 class ListIdentityProvidersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listidentityproviderspaginator)
         """
 
 
@@ -78,15 +78,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listinstancespaginator)
         """
 
 
@@ -98,15 +98,15 @@
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProductSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListProductSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listproductsubscriptionspaginator)
         """
 
 
@@ -118,13 +118,13 @@
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUserAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListUserAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listuserassociationspaginator)
         """
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/paginator.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 class ListIdentityProvidersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listidentityproviderspaginator)
         """
 
 class ListInstancesPaginator(Paginator):
@@ -74,15 +74,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listinstancespaginator)
         """
 
 class ListProductSubscriptionsPaginator(Paginator):
@@ -93,15 +93,15 @@
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProductSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListProductSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listproductsubscriptionspaginator)
         """
 
 class ListUserAssociationsPaginator(Paginator):
@@ -112,13 +112,13 @@
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUserAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListUserAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listuserassociationspaginator)
         """
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/type_defs.py` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,26 +18,26 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActiveDirectoryIdentityProviderTypeDef",
-    "ResponseMetadataTypeDef",
     "FilterTypeDef",
     "SettingsTypeDef",
     "InstanceSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateSettingsTypeDef",
     "IdentityProviderTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
     "AssociateUserRequestRequestTypeDef",
     "DeregisterIdentityProviderRequestRequestTypeDef",
     "DisassociateUserRequestRequestTypeDef",
     "IdentityProviderSummaryTypeDef",
     "InstanceUserSummaryTypeDef",
     "ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     "ListProductSubscriptionsRequestRequestTypeDef",
@@ -64,25 +64,14 @@
     "ActiveDirectoryIdentityProviderTypeDef",
     {
         "DirectoryId": str,
     },
     total=False,
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
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Attribute": str,
         "Operation": str,
         "Value": str,
     },
@@ -115,33 +104,52 @@
 )
 
 
 class InstanceSummaryTypeDef(_RequiredInstanceSummaryTypeDef, _OptionalInstanceSummaryTypeDef):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListIdentityProvidersRequestRequestTypeDef = TypedDict(
     "ListIdentityProvidersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
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
 _RequiredUpdateSettingsTypeDef = TypedDict(
     "_RequiredUpdateSettingsTypeDef",
     {
         "AddSubnets": Sequence[str],
         "RemoveSubnets": Sequence[str],
     },
 )
@@ -162,14 +170,23 @@
     "IdentityProviderTypeDef",
     {
         "ActiveDirectoryIdentityProvider": ActiveDirectoryIdentityProviderTypeDef,
     },
     total=False,
 )
 
+ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "ListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInstancesRequestRequestTypeDef = TypedDict(
     "ListInstancesRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -177,35 +194,18 @@
 )
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "InstanceSummaries": List[InstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "ListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredAssociateUserRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
         "Username": str,
     },
@@ -314,15 +314,15 @@
         "Product": str,
     },
 )
 _OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef = TypedDict(
     "_OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef(
     _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
@@ -363,15 +363,15 @@
         "InstanceId": str,
     },
 )
 _OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef = TypedDict(
     "_OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListUserAssociationsRequestListUserAssociationsPaginateTypeDef(
     _RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
@@ -512,85 +512,85 @@
     },
 )
 
 DeregisterIdentityProviderResponseTypeDef = TypedDict(
     "DeregisterIdentityProviderResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "IdentityProviderSummaries": List[IdentityProviderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterIdentityProviderResponseTypeDef = TypedDict(
     "RegisterIdentityProviderResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateIdentityProviderSettingsResponseTypeDef = TypedDict(
     "UpdateIdentityProviderSettingsResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateUserResponseTypeDef = TypedDict(
     "AssociateUserResponseTypeDef",
     {
         "InstanceUserSummary": InstanceUserSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateUserResponseTypeDef = TypedDict(
     "DisassociateUserResponseTypeDef",
     {
         "InstanceUserSummary": InstanceUserSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUserAssociationsResponseTypeDef = TypedDict(
     "ListUserAssociationsResponseTypeDef",
     {
         "InstanceUserSummaries": List[InstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProductSubscriptionsResponseTypeDef = TypedDict(
     "ListProductSubscriptionsResponseTypeDef",
     {
         "NextToken": str,
         "ProductUserSummaries": List[ProductUserSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartProductSubscriptionResponseTypeDef = TypedDict(
     "StartProductSubscriptionResponseTypeDef",
     {
         "ProductUserSummary": ProductUserSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopProductSubscriptionResponseTypeDef = TypedDict(
     "StopProductSubscriptionResponseTypeDef",
     {
         "ProductUserSummary": ProductUserSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActiveDirectoryIdentityProviderTypeDef",
-    "ResponseMetadataTypeDef",
     "FilterTypeDef",
     "SettingsTypeDef",
     "InstanceSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateSettingsTypeDef",
     "IdentityProviderTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
     "AssociateUserRequestRequestTypeDef",
     "DeregisterIdentityProviderRequestRequestTypeDef",
     "DisassociateUserRequestRequestTypeDef",
     "IdentityProviderSummaryTypeDef",
     "InstanceUserSummaryTypeDef",
     "ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     "ListProductSubscriptionsRequestRequestTypeDef",
@@ -63,25 +63,14 @@
     "ActiveDirectoryIdentityProviderTypeDef",
     {
         "DirectoryId": str,
     },
     total=False,
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
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Attribute": str,
         "Operation": str,
         "Value": str,
     },
@@ -112,33 +101,52 @@
     },
     total=False,
 )
 
 class InstanceSummaryTypeDef(_RequiredInstanceSummaryTypeDef, _OptionalInstanceSummaryTypeDef):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListIdentityProvidersRequestRequestTypeDef = TypedDict(
     "ListIdentityProvidersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
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
 _RequiredUpdateSettingsTypeDef = TypedDict(
     "_RequiredUpdateSettingsTypeDef",
     {
         "AddSubnets": Sequence[str],
         "RemoveSubnets": Sequence[str],
     },
 )
@@ -157,14 +165,23 @@
     "IdentityProviderTypeDef",
     {
         "ActiveDirectoryIdentityProvider": ActiveDirectoryIdentityProviderTypeDef,
     },
     total=False,
 )
 
+ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "ListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInstancesRequestRequestTypeDef = TypedDict(
     "ListInstancesRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -172,35 +189,18 @@
 )
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "InstanceSummaries": List[InstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "ListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredAssociateUserRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
         "Username": str,
     },
@@ -301,15 +301,15 @@
         "Product": str,
     },
 )
 _OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef = TypedDict(
     "_OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef(
     _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     _OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
@@ -346,15 +346,15 @@
         "InstanceId": str,
     },
 )
 _OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef = TypedDict(
     "_OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListUserAssociationsRequestListUserAssociationsPaginateTypeDef(
     _RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
     _OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
@@ -483,85 +483,85 @@
     },
 )
 
 DeregisterIdentityProviderResponseTypeDef = TypedDict(
     "DeregisterIdentityProviderResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "IdentityProviderSummaries": List[IdentityProviderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterIdentityProviderResponseTypeDef = TypedDict(
     "RegisterIdentityProviderResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateIdentityProviderSettingsResponseTypeDef = TypedDict(
     "UpdateIdentityProviderSettingsResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateUserResponseTypeDef = TypedDict(
     "AssociateUserResponseTypeDef",
     {
         "InstanceUserSummary": InstanceUserSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateUserResponseTypeDef = TypedDict(
     "DisassociateUserResponseTypeDef",
     {
         "InstanceUserSummary": InstanceUserSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUserAssociationsResponseTypeDef = TypedDict(
     "ListUserAssociationsResponseTypeDef",
     {
         "InstanceUserSummaries": List[InstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProductSubscriptionsResponseTypeDef = TypedDict(
     "ListProductSubscriptionsResponseTypeDef",
     {
         "NextToken": str,
         "ProductUserSummaries": List[ProductUserSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartProductSubscriptionResponseTypeDef = TypedDict(
     "StartProductSubscriptionResponseTypeDef",
     {
         "ProductUserSummary": ProductUserSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopProductSubscriptionResponseTypeDef = TypedDict(
     "StopProductSubscriptionResponseTypeDef",
     {
         "ProductUserSummary": ProductUserSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-user-subscriptions
-Version: 1.26.18
-Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.26.18 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/
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
 
 <a id="mypy-boto3-license-manager-user-subscriptions"></a>
 
 # mypy-boto3-license-manager-user-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-user-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager-user-subscriptions?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerUserSubscriptions 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[boto3.LicenseManagerUserSubscriptions 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,26 +347,26 @@
 `mypy_boto3_license_manager_user_subscriptions.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_user_subscriptions.type_defs import (
     ActiveDirectoryIdentityProviderTypeDef,
-    ResponseMetadataTypeDef,
     FilterTypeDef,
     SettingsTypeDef,
     InstanceSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateSettingsTypeDef,
     IdentityProviderTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
     IdentityProviderSummaryTypeDef,
     InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
@@ -396,42 +397,42 @@
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

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.26.18/setup.py` & `mypy-boto3-license-manager-user-subscriptions-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,58 @@
 """
 Setup script for mypy-boto3-license-manager-user-subscriptions.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager-user-subscriptions",
-    version="1.26.18",
+    version="1.27.0",
     packages=["mypy_boto3_license_manager_user_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.26.18 service generated with"
-        " mypy-boto3-builder 7.11.11"
+        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.27.0 service generated with"
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
         "boto3 license-manager-user-subscriptions type-annotations boto3-stubs mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={
-        "": ["LICENSE"],
-        "mypy_boto3_license_manager_user_subscriptions": ["py.typed", "*.pyi"],
-    },
+    package_data={"mypy_boto3_license_manager_user_subscriptions": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/",
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


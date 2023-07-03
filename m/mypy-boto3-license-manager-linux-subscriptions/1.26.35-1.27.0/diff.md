# Comparing `tmp/mypy-boto3-license-manager-linux-subscriptions-1.26.35.tar.gz` & `tmp/mypy-boto3-license-manager-linux-subscriptions-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-linux-subscriptions-1.26.35.tar", last modified: Wed Dec 21 21:23:13 2022, max compression
+gzip compressed data, was "mypy-boto3-license-manager-linux-subscriptions-1.27.0.tar", last modified: Mon Jul  3 19:51:01 2023, max compression
```

## Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35.tar` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 21:23:13.067076 mypy-boto3-license-manager-linux-subscriptions-1.26.35/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15093 2022-12-21 21:23:13.067076 mypy-boto3-license-manager-linux-subscriptions-1.26.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 21:23:13.059076 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-21 21:22:18.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 21:23:13.067076 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15093 2022-12-21 21:23:12.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2022-12-21 21:23:12.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 21:23:12.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 21:23:12.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-21 21:23:12.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-21 21:23:12.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 21:23:13.067076 mypy-boto3-license-manager-linux-subscriptions-1.26.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2022-12-21 21:22:17.000000 mypy-boto3-license-manager-linux-subscriptions-1.26.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.703561 mypy-boto3-license-manager-linux-subscriptions-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-03 19:51:01.699561 mypy-boto3-license-manager-linux-subscriptions-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13519 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.691561 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.699561 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:01.703561 mypy-boto3-license-manager-linux-subscriptions-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-03 19:41:02.000000 mypy-boto3-license-manager-linux-subscriptions-1.27.0/setup.py
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/LICENSE` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/PKG-INFO` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-linux-subscriptions
-Version: 1.26.35
-Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.26.35 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-license-manager-linux-subscriptions"></a>
 
 # mypy-boto3-license-manager-linux-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-linux-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager-linux-subscriptions?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager-linux-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerLinuxSubscriptions 1.26.35](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
+[boto3.LicenseManagerLinuxSubscriptions 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-license-manager-linux-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,14 +325,15 @@
     OperatorType,
     OrganizationIntegrationType,
     StatusType,
     LicenseManagerLinuxSubscriptionsServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    RegionName,
 )
 
 
 def check_value(value: LinuxSubscriptionsDiscoveryType) -> bool:
     ...
 ```
 
@@ -344,26 +345,26 @@
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_linux_subscriptions.type_defs import (
     FilterTypeDef,
     LinuxSubscriptionsDiscoverySettingsTypeDef,
-    ResponseMetadataTypeDef,
     InstanceTypeDef,
-    PaginatorConfigTypeDef,
     SubscriptionTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
     ListLinuxSubscriptionInstancesRequestRequestTypeDef,
+    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsRequestRequestTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
+    UpdateServiceSettingsRequestRequestTypeDef,
     UpdateServiceSettingsResponseTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
-    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
-    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
 )
 
 
 def get_structure() -> FilterTypeDef:
     return {...}
 ```
@@ -371,42 +372,42 @@
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

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/README.md` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-license-manager-linux-subscriptions"></a>
 
 # mypy-boto3-license-manager-linux-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-linux-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager-linux-subscriptions?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager-linux-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerLinuxSubscriptions 1.26.35](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
+[boto3.LicenseManagerLinuxSubscriptions 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-license-manager-linux-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,14 +293,15 @@
     OperatorType,
     OrganizationIntegrationType,
     StatusType,
     LicenseManagerLinuxSubscriptionsServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    RegionName,
 )
 
 
 def check_value(value: LinuxSubscriptionsDiscoveryType) -> bool:
     ...
 ```
 
@@ -312,26 +313,26 @@
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_linux_subscriptions.type_defs import (
     FilterTypeDef,
     LinuxSubscriptionsDiscoverySettingsTypeDef,
-    ResponseMetadataTypeDef,
     InstanceTypeDef,
-    PaginatorConfigTypeDef,
     SubscriptionTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
     ListLinuxSubscriptionInstancesRequestRequestTypeDef,
+    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsRequestRequestTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
+    UpdateServiceSettingsRequestRequestTypeDef,
     UpdateServiceSettingsResponseTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
-    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
-    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
 )
 
 
 def get_structure() -> FilterTypeDef:
     return {...}
 ```
@@ -339,42 +340,42 @@
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

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/__init__.py` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/__main__.py` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.26.35\nVersion:        "
-        " 1.26.35\nBuilder version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.35")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/client.py` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/client.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/literals.py` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "OperatorType",
     "OrganizationIntegrationType",
     "StatusType",
     "LicenseManagerLinuxSubscriptionsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
+    "RegionName",
 )
 
 
 LinuxSubscriptionsDiscoveryType = Literal["Disabled", "Enabled"]
 ListLinuxSubscriptionInstancesPaginatorName = Literal["list_linux_subscription_instances"]
 ListLinuxSubscriptionsPaginatorName = Literal["list_linux_subscriptions"]
 OperatorType = Literal["Contains", "Equal", "NotEqual"]
@@ -51,14 +52,15 @@
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
@@ -79,31 +81,34 @@
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
@@ -182,14 +187,15 @@
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
@@ -200,18 +206,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -242,14 +250,15 @@
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
@@ -268,16 +277,19 @@
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
@@ -357,18 +369,21 @@
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
@@ -387,7 +402,36 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_linux_subscription_instances", "list_linux_subscriptions"]
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
+    "eu-central-1",
+    "eu-central-2",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
+    "eu-west-1",
+    "eu-west-2",
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

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/literals.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/literals.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "OperatorType",
     "OrganizationIntegrationType",
     "StatusType",
     "LicenseManagerLinuxSubscriptionsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
+    "RegionName",
 )
 
 LinuxSubscriptionsDiscoveryType = Literal["Disabled", "Enabled"]
 ListLinuxSubscriptionInstancesPaginatorName = Literal["list_linux_subscription_instances"]
 ListLinuxSubscriptionsPaginatorName = Literal["list_linux_subscriptions"]
 OperatorType = Literal["Contains", "Equal", "NotEqual"]
 OrganizationIntegrationType = Literal["Disabled", "Enabled"]
@@ -49,14 +50,15 @@
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
@@ -77,31 +79,34 @@
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
@@ -198,18 +204,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -240,14 +248,15 @@
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
@@ -266,16 +275,19 @@
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
@@ -355,18 +367,21 @@
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
@@ -385,7 +400,36 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_linux_subscription_instances", "list_linux_subscriptions"]
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
+    "eu-central-1",
+    "eu-central-2",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
+    "eu-west-1",
+    "eu-west-2",
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

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/paginator.py` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptioninstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLinuxSubscriptionInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Paginator.ListLinuxSubscriptionInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptioninstancespaginator)
         """
 
 
@@ -69,13 +69,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLinuxSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Paginator.ListLinuxSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptionspaginator)
         """
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptioninstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLinuxSubscriptionInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Paginator.ListLinuxSubscriptionInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptioninstancespaginator)
         """
 
 class ListLinuxSubscriptionsPaginator(Paginator):
@@ -65,13 +65,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLinuxSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Paginator.ListLinuxSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptionspaginator)
         """
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/type_defs.py` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,26 +26,26 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FilterTypeDef",
     "LinuxSubscriptionsDiscoverySettingsTypeDef",
-    "ResponseMetadataTypeDef",
     "InstanceTypeDef",
-    "PaginatorConfigTypeDef",
     "SubscriptionTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
+    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsRequestRequestTypeDef",
-    "UpdateServiceSettingsRequestRequestTypeDef",
     "GetServiceSettingsResponseTypeDef",
+    "UpdateServiceSettingsRequestRequestTypeDef",
     "UpdateServiceSettingsResponseTypeDef",
     "ListLinuxSubscriptionInstancesResponseTypeDef",
-    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
-    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsResponseTypeDef",
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
@@ -59,25 +59,14 @@
     "LinuxSubscriptionsDiscoverySettingsTypeDef",
     {
         "OrganizationIntegration": OrganizationIntegrationType,
         "SourceRegions": List[str],
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
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "AccountID": str,
         "AmiId": str,
         "InstanceID": str,
         "InstanceType": str,
@@ -87,54 +76,95 @@
         "Status": str,
         "SubscriptionName": str,
         "UsageOperation": str,
     },
     total=False,
 )
 
+SubscriptionTypeDef = TypedDict(
+    "SubscriptionTypeDef",
+    {
+        "InstanceCount": int,
+        "Name": str,
+        "Type": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-SubscriptionTypeDef = TypedDict(
-    "SubscriptionTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "InstanceCount": int,
-        "Name": str,
-        "Type": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef = TypedDict(
+    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListLinuxSubscriptionInstancesRequestRequestTypeDef = TypedDict(
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef = TypedDict(
+    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLinuxSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListLinuxSubscriptionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+GetServiceSettingsResponseTypeDef = TypedDict(
+    "GetServiceSettingsResponseTypeDef",
+    {
+        "HomeRegions": List[str],
+        "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
+        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
+        "Status": StatusType,
+        "StatusMessage": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceSettingsRequestRequestTypeDef",
     {
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
         "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
     },
 )
@@ -150,66 +180,36 @@
 class UpdateServiceSettingsRequestRequestTypeDef(
     _RequiredUpdateServiceSettingsRequestRequestTypeDef,
     _OptionalUpdateServiceSettingsRequestRequestTypeDef,
 ):
     pass
 
 
-GetServiceSettingsResponseTypeDef = TypedDict(
-    "GetServiceSettingsResponseTypeDef",
-    {
-        "HomeRegions": List[str],
-        "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
-        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
-        "Status": StatusType,
-        "StatusMessage": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateServiceSettingsResponseTypeDef = TypedDict(
     "UpdateServiceSettingsResponseTypeDef",
     {
         "HomeRegions": List[str],
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
         "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
         "Status": StatusType,
         "StatusMessage": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLinuxSubscriptionInstancesResponseTypeDef = TypedDict(
     "ListLinuxSubscriptionInstancesResponseTypeDef",
     {
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef = TypedDict(
-    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef = TypedDict(
-    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListLinuxSubscriptionsResponseTypeDef = TypedDict(
     "ListLinuxSubscriptionsResponseTypeDef",
     {
         "NextToken": str,
         "Subscriptions": List[SubscriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -25,26 +25,26 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FilterTypeDef",
     "LinuxSubscriptionsDiscoverySettingsTypeDef",
-    "ResponseMetadataTypeDef",
     "InstanceTypeDef",
-    "PaginatorConfigTypeDef",
     "SubscriptionTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
+    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsRequestRequestTypeDef",
-    "UpdateServiceSettingsRequestRequestTypeDef",
     "GetServiceSettingsResponseTypeDef",
+    "UpdateServiceSettingsRequestRequestTypeDef",
     "UpdateServiceSettingsResponseTypeDef",
     "ListLinuxSubscriptionInstancesResponseTypeDef",
-    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
-    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsResponseTypeDef",
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
@@ -58,25 +58,14 @@
     "LinuxSubscriptionsDiscoverySettingsTypeDef",
     {
         "OrganizationIntegration": OrganizationIntegrationType,
         "SourceRegions": List[str],
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
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "AccountID": str,
         "AmiId": str,
         "InstanceID": str,
         "InstanceType": str,
@@ -86,54 +75,95 @@
         "Status": str,
         "SubscriptionName": str,
         "UsageOperation": str,
     },
     total=False,
 )
 
+SubscriptionTypeDef = TypedDict(
+    "SubscriptionTypeDef",
+    {
+        "InstanceCount": int,
+        "Name": str,
+        "Type": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-SubscriptionTypeDef = TypedDict(
-    "SubscriptionTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "InstanceCount": int,
-        "Name": str,
-        "Type": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef = TypedDict(
+    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListLinuxSubscriptionInstancesRequestRequestTypeDef = TypedDict(
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef = TypedDict(
+    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLinuxSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListLinuxSubscriptionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+GetServiceSettingsResponseTypeDef = TypedDict(
+    "GetServiceSettingsResponseTypeDef",
+    {
+        "HomeRegions": List[str],
+        "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
+        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
+        "Status": StatusType,
+        "StatusMessage": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceSettingsRequestRequestTypeDef",
     {
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
         "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
     },
 )
@@ -147,66 +177,36 @@
 
 class UpdateServiceSettingsRequestRequestTypeDef(
     _RequiredUpdateServiceSettingsRequestRequestTypeDef,
     _OptionalUpdateServiceSettingsRequestRequestTypeDef,
 ):
     pass
 
-GetServiceSettingsResponseTypeDef = TypedDict(
-    "GetServiceSettingsResponseTypeDef",
-    {
-        "HomeRegions": List[str],
-        "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
-        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
-        "Status": StatusType,
-        "StatusMessage": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateServiceSettingsResponseTypeDef = TypedDict(
     "UpdateServiceSettingsResponseTypeDef",
     {
         "HomeRegions": List[str],
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
         "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
         "Status": StatusType,
         "StatusMessage": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLinuxSubscriptionInstancesResponseTypeDef = TypedDict(
     "ListLinuxSubscriptionInstancesResponseTypeDef",
     {
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef = TypedDict(
-    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef = TypedDict(
-    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListLinuxSubscriptionsResponseTypeDef = TypedDict(
     "ListLinuxSubscriptionsResponseTypeDef",
     {
         "NextToken": str,
         "Subscriptions": List[SubscriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-linux-subscriptions
-Version: 1.26.35
-Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.26.35 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-license-manager-linux-subscriptions"></a>
 
 # mypy-boto3-license-manager-linux-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-linux-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager-linux-subscriptions?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager-linux-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerLinuxSubscriptions 1.26.35](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
+[boto3.LicenseManagerLinuxSubscriptions 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-license-manager-linux-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,14 +325,15 @@
     OperatorType,
     OrganizationIntegrationType,
     StatusType,
     LicenseManagerLinuxSubscriptionsServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    RegionName,
 )
 
 
 def check_value(value: LinuxSubscriptionsDiscoveryType) -> bool:
     ...
 ```
 
@@ -344,26 +345,26 @@
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_linux_subscriptions.type_defs import (
     FilterTypeDef,
     LinuxSubscriptionsDiscoverySettingsTypeDef,
-    ResponseMetadataTypeDef,
     InstanceTypeDef,
-    PaginatorConfigTypeDef,
     SubscriptionTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
     ListLinuxSubscriptionInstancesRequestRequestTypeDef,
+    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsRequestRequestTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
+    UpdateServiceSettingsRequestRequestTypeDef,
     UpdateServiceSettingsResponseTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
-    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
-    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
 )
 
 
 def get_structure() -> FilterTypeDef:
     return {...}
 ```
@@ -371,42 +372,42 @@
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

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.26.35/setup.py` & `mypy-boto3-license-manager-linux-subscriptions-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-license-manager-linux-subscriptions.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager-linux-subscriptions",
-    version="1.26.35",
+    version="1.27.0",
     packages=["mypy_boto3_license_manager_linux_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.26.35 service generated with"
-        " mypy-boto3-builder 7.12.0"
+        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -48,11 +48,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/",
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


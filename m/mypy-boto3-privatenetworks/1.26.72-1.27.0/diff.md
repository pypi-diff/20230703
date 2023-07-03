# Comparing `tmp/mypy-boto3-privatenetworks-1.26.72.tar.gz` & `tmp/mypy-boto3-privatenetworks-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-privatenetworks-1.26.72.tar", last modified: Wed Feb 15 22:27:56 2023, max compression
+gzip compressed data, was "mypy-boto3-privatenetworks-1.27.0.tar", last modified: Mon Jul  3 19:51:17 2023, max compression
```

## Comparing `mypy-boto3-privatenetworks-1.26.72.tar` & `mypy-boto3-privatenetworks-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.854127 mypy-boto3-privatenetworks-1.26.72/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-02-15 22:27:56.854127 mypy-boto3-privatenetworks-1.26.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.854127 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21049 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21011 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27299 2023-02-15 22:27:26.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27250 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.854127 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-02-15 22:27:56.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-15 22:27:56.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 22:27:56.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-15 22:27:56.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 22:27:56.854127 mypy-boto3-privatenetworks-1.26.72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.011833 mypy-boto3-privatenetworks-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-07-03 19:51:17.011833 mypy-boto3-privatenetworks-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.007832 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21342 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-07-03 19:43:49.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28957 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:47.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.011833 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-07-03 19:51:16.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-03 19:51:16.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:16.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:16.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:16.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 19:51:16.000000 mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:17.011833 mypy-boto3-privatenetworks-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-03 19:43:46.000000 mypy-boto3-privatenetworks-1.27.0/setup.py
```

### Comparing `mypy-boto3-privatenetworks-1.26.72/LICENSE` & `mypy-boto3-privatenetworks-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-privatenetworks-1.26.72/PKG-INFO` & `mypy-boto3-privatenetworks-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-privatenetworks
-Version: 1.26.72
-Summary: Type annotations for boto3.Private5G 1.26.72 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Private5G 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-privatenetworks"></a>
 
 # mypy-boto3-privatenetworks
 
 [![PyPI - mypy-boto3-privatenetworks](https://img.shields.io/pypi/v/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-privatenetworks?color=blue)](https://pypistats.org/packages/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,14 +312,15 @@
 
 `mypy_boto3_privatenetworks.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_privatenetworks.literals import (
     AcknowledgmentStatusType,
+    CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
     ElevationUnitType,
     HealthStatusType,
     ListDeviceIdentifiersPaginatorName,
     ListNetworkResourcesPaginatorName,
@@ -353,71 +354,74 @@
 
 `mypy_boto3_privatenetworks.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
     AddressTypeDef,
+    CommitmentConfigurationTypeDef,
     PositionTypeDef,
     CreateNetworkRequestRequestTypeDef,
     NetworkTypeDef,
     DeactivateDeviceIdentifierRequestRequestTypeDef,
     DeleteNetworkRequestRequestTypeDef,
     DeleteNetworkSiteRequestRequestTypeDef,
     GetDeviceIdentifierRequestRequestTypeDef,
     GetNetworkRequestRequestTypeDef,
     GetNetworkResourceRequestRequestTypeDef,
     GetNetworkSiteRequestRequestTypeDef,
     GetOrderRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
     ListDeviceIdentifiersRequestRequestTypeDef,
+    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
     ListNetworkResourcesRequestRequestTypeDef,
+    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
     ListNetworkSitesRequestRequestTypeDef,
+    ListNetworksRequestListNetworksPaginateTypeDef,
     ListNetworksRequestRequestTypeDef,
+    ListOrdersRequestListOrdersPaginateTypeDef,
     ListOrdersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NameValuePairTypeDef,
     TrackingInformationTypeDef,
+    PaginatorConfigTypeDef,
+    PingResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateNetworkSiteRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PingResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
     ListDeviceIdentifiersResponseTypeDef,
-    ActivateNetworkSiteRequestRequestTypeDef,
     ReturnInformationTypeDef,
+    ActivateNetworkSiteRequestRequestTypeDef,
+    CommitmentInformationTypeDef,
+    OrderedResourceDefinitionTypeDef,
     StartNetworkResourceUpdateRequestRequestTypeDef,
     ConfigureAccessPointRequestRequestTypeDef,
     CreateNetworkResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     GetNetworkResponseTypeDef,
     ListNetworksResponseTypeDef,
-    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-    ListNetworksRequestListNetworksPaginateTypeDef,
-    ListOrdersRequestListOrdersPaginateTypeDef,
     NetworkResourceDefinitionTypeDef,
-    OrderTypeDef,
     NetworkResourceTypeDef,
+    OrderTypeDef,
     SitePlanTypeDef,
-    AcknowledgeOrderReceiptResponseTypeDef,
-    GetOrderResponseTypeDef,
-    ListOrdersResponseTypeDef,
     ConfigureAccessPointResponseTypeDef,
     GetNetworkResourceResponseTypeDef,
     ListNetworkResourcesResponseTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
+    AcknowledgeOrderReceiptResponseTypeDef,
+    GetOrderResponseTypeDef,
+    ListOrdersResponseTypeDef,
     CreateNetworkSiteRequestRequestTypeDef,
     NetworkSiteTypeDef,
     UpdateNetworkSitePlanRequestRequestTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetNetworkSiteResponseTypeDef,
@@ -433,42 +437,42 @@
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

### Comparing `mypy-boto3-privatenetworks-1.26.72/README.md` & `mypy-boto3-privatenetworks-1.27.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-privatenetworks"></a>
 
 # mypy-boto3-privatenetworks
 
 [![PyPI - mypy-boto3-privatenetworks](https://img.shields.io/pypi/v/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-privatenetworks?color=blue)](https://pypistats.org/packages/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,14 +280,15 @@
 
 `mypy_boto3_privatenetworks.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_privatenetworks.literals import (
     AcknowledgmentStatusType,
+    CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
     ElevationUnitType,
     HealthStatusType,
     ListDeviceIdentifiersPaginatorName,
     ListNetworkResourcesPaginatorName,
@@ -321,71 +322,74 @@
 
 `mypy_boto3_privatenetworks.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
     AddressTypeDef,
+    CommitmentConfigurationTypeDef,
     PositionTypeDef,
     CreateNetworkRequestRequestTypeDef,
     NetworkTypeDef,
     DeactivateDeviceIdentifierRequestRequestTypeDef,
     DeleteNetworkRequestRequestTypeDef,
     DeleteNetworkSiteRequestRequestTypeDef,
     GetDeviceIdentifierRequestRequestTypeDef,
     GetNetworkRequestRequestTypeDef,
     GetNetworkResourceRequestRequestTypeDef,
     GetNetworkSiteRequestRequestTypeDef,
     GetOrderRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
     ListDeviceIdentifiersRequestRequestTypeDef,
+    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
     ListNetworkResourcesRequestRequestTypeDef,
+    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
     ListNetworkSitesRequestRequestTypeDef,
+    ListNetworksRequestListNetworksPaginateTypeDef,
     ListNetworksRequestRequestTypeDef,
+    ListOrdersRequestListOrdersPaginateTypeDef,
     ListOrdersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NameValuePairTypeDef,
     TrackingInformationTypeDef,
+    PaginatorConfigTypeDef,
+    PingResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateNetworkSiteRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PingResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
     ListDeviceIdentifiersResponseTypeDef,
-    ActivateNetworkSiteRequestRequestTypeDef,
     ReturnInformationTypeDef,
+    ActivateNetworkSiteRequestRequestTypeDef,
+    CommitmentInformationTypeDef,
+    OrderedResourceDefinitionTypeDef,
     StartNetworkResourceUpdateRequestRequestTypeDef,
     ConfigureAccessPointRequestRequestTypeDef,
     CreateNetworkResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     GetNetworkResponseTypeDef,
     ListNetworksResponseTypeDef,
-    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-    ListNetworksRequestListNetworksPaginateTypeDef,
-    ListOrdersRequestListOrdersPaginateTypeDef,
     NetworkResourceDefinitionTypeDef,
-    OrderTypeDef,
     NetworkResourceTypeDef,
+    OrderTypeDef,
     SitePlanTypeDef,
-    AcknowledgeOrderReceiptResponseTypeDef,
-    GetOrderResponseTypeDef,
-    ListOrdersResponseTypeDef,
     ConfigureAccessPointResponseTypeDef,
     GetNetworkResourceResponseTypeDef,
     ListNetworkResourcesResponseTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
+    AcknowledgeOrderReceiptResponseTypeDef,
+    GetOrderResponseTypeDef,
+    ListOrdersResponseTypeDef,
     CreateNetworkSiteRequestRequestTypeDef,
     NetworkSiteTypeDef,
     UpdateNetworkSitePlanRequestRequestTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetNetworkSiteResponseTypeDef,
@@ -401,42 +405,42 @@
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

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/__init__.py` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/__init__.pyi` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/__main__.py` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Private5G 1.26.72\nVersion:         1.26.72\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Private5G 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.72")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/client.py` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     ListOrdersPaginator,
 )
 from .type_defs import (
     AcknowledgeOrderReceiptResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     AddressTypeDef,
+    CommitmentConfigurationTypeDef,
     ConfigureAccessPointResponseTypeDef,
     CreateNetworkResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
@@ -119,15 +120,20 @@
         Activates the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_device_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#activate_device_identifier)
         """
 
     def activate_network_site(
-        self, *, networkSiteArn: str, shippingAddress: AddressTypeDef, clientToken: str = ...
+        self,
+        *,
+        networkSiteArn: str,
+        shippingAddress: AddressTypeDef,
+        clientToken: str = ...,
+        commitmentConfiguration: CommitmentConfigurationTypeDef = ...
     ) -> ActivateNetworkSiteResponseTypeDef:
         """
         Activates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#activate_network_site)
         """
@@ -376,19 +382,21 @@
         """
 
     def start_network_resource_update(
         self,
         *,
         networkResourceArn: str,
         updateType: UpdateTypeType,
+        commitmentConfiguration: CommitmentConfigurationTypeDef = ...,
         returnReason: str = ...,
         shippingAddress: AddressTypeDef = ...
     ) -> StartNetworkResourceUpdateResponseTypeDef:
         """
-        Starts an update of the specified network resource.
+        Use this action to do the following tasks: * Update the duration and renewal
+        status of the commitment period for a radio unit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.start_network_resource_update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#start_network_resource_update)
         """
 
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
```

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/client.pyi` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     ListOrdersPaginator,
 )
 from .type_defs import (
     AcknowledgeOrderReceiptResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     AddressTypeDef,
+    CommitmentConfigurationTypeDef,
     ConfigureAccessPointResponseTypeDef,
     CreateNetworkResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
@@ -112,15 +113,20 @@
         """
         Activates the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_device_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#activate_device_identifier)
         """
     def activate_network_site(
-        self, *, networkSiteArn: str, shippingAddress: AddressTypeDef, clientToken: str = ...
+        self,
+        *,
+        networkSiteArn: str,
+        shippingAddress: AddressTypeDef,
+        clientToken: str = ...,
+        commitmentConfiguration: CommitmentConfigurationTypeDef = ...
     ) -> ActivateNetworkSiteResponseTypeDef:
         """
         Activates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#activate_network_site)
         """
@@ -347,19 +353,21 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#ping)
         """
     def start_network_resource_update(
         self,
         *,
         networkResourceArn: str,
         updateType: UpdateTypeType,
+        commitmentConfiguration: CommitmentConfigurationTypeDef = ...,
         returnReason: str = ...,
         shippingAddress: AddressTypeDef = ...
     ) -> StartNetworkResourceUpdateResponseTypeDef:
         """
-        Starts an update of the specified network resource.
+        Use this action to do the following tasks: * Update the duration and renewal
+        status of the commitment period for a radio unit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.start_network_resource_update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#start_network_resource_update)
         """
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds tags to the specified resource.
```

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/literals.py` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AcknowledgmentStatusType",
+    "CommitmentLengthType",
     "DeviceIdentifierFilterKeysType",
     "DeviceIdentifierStatusType",
     "ElevationReferenceType",
     "ElevationUnitType",
     "HealthStatusType",
     "ListDeviceIdentifiersPaginatorName",
     "ListNetworkResourcesPaginatorName",
@@ -45,14 +46,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
 
 AcknowledgmentStatusType = Literal["ACKNOWLEDGED", "ACKNOWLEDGING", "UNACKNOWLEDGED"]
+CommitmentLengthType = Literal["ONE_YEAR", "SIXTY_DAYS", "THREE_YEARS"]
 DeviceIdentifierFilterKeysType = Literal["ORDER", "STATUS", "TRAFFIC_GROUP"]
 DeviceIdentifierStatusType = Literal["ACTIVE", "INACTIVE"]
 ElevationReferenceType = Literal["AGL", "AMSL"]
 ElevationUnitType = Literal["FEET"]
 HealthStatusType = Literal["HEALTHY", "INITIAL", "UNHEALTHY"]
 ListDeviceIdentifiersPaginatorName = Literal["list_device_identifiers"]
 ListNetworkResourcesPaginatorName = Literal["list_network_resources"]
@@ -74,15 +76,15 @@
     "SHIPPED",
 ]
 NetworkResourceTypeType = Literal["RADIO_UNIT"]
 NetworkSiteFilterKeysType = Literal["STATUS"]
 NetworkSiteStatusType = Literal["AVAILABLE", "CREATED", "DELETED", "DEPROVISIONING", "PROVISIONING"]
 NetworkStatusType = Literal["AVAILABLE", "CREATED", "DELETED", "DEPROVISIONING", "PROVISIONING"]
 OrderFilterKeysType = Literal["NETWORK_SITE", "STATUS"]
-UpdateTypeType = Literal["REPLACE", "RETURN"]
+UpdateTypeType = Literal["COMMITMENT", "REPLACE", "RETURN"]
 Private5GServiceName = Literal["privatenetworks"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -91,14 +93,15 @@
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
@@ -138,14 +141,15 @@
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
@@ -224,14 +228,15 @@
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
@@ -242,14 +247,15 @@
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
@@ -285,14 +291,15 @@
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
@@ -311,16 +318,19 @@
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
@@ -400,18 +410,21 @@
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

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/literals.pyi` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AcknowledgmentStatusType",
+    "CommitmentLengthType",
     "DeviceIdentifierFilterKeysType",
     "DeviceIdentifierStatusType",
     "ElevationReferenceType",
     "ElevationUnitType",
     "HealthStatusType",
     "ListDeviceIdentifiersPaginatorName",
     "ListNetworkResourcesPaginatorName",
@@ -43,14 +44,15 @@
     "Private5GServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
 AcknowledgmentStatusType = Literal["ACKNOWLEDGED", "ACKNOWLEDGING", "UNACKNOWLEDGED"]
+CommitmentLengthType = Literal["ONE_YEAR", "SIXTY_DAYS", "THREE_YEARS"]
 DeviceIdentifierFilterKeysType = Literal["ORDER", "STATUS", "TRAFFIC_GROUP"]
 DeviceIdentifierStatusType = Literal["ACTIVE", "INACTIVE"]
 ElevationReferenceType = Literal["AGL", "AMSL"]
 ElevationUnitType = Literal["FEET"]
 HealthStatusType = Literal["HEALTHY", "INITIAL", "UNHEALTHY"]
 ListDeviceIdentifiersPaginatorName = Literal["list_device_identifiers"]
 ListNetworkResourcesPaginatorName = Literal["list_network_resources"]
@@ -72,15 +74,15 @@
     "SHIPPED",
 ]
 NetworkResourceTypeType = Literal["RADIO_UNIT"]
 NetworkSiteFilterKeysType = Literal["STATUS"]
 NetworkSiteStatusType = Literal["AVAILABLE", "CREATED", "DELETED", "DEPROVISIONING", "PROVISIONING"]
 NetworkStatusType = Literal["AVAILABLE", "CREATED", "DELETED", "DEPROVISIONING", "PROVISIONING"]
 OrderFilterKeysType = Literal["NETWORK_SITE", "STATUS"]
-UpdateTypeType = Literal["REPLACE", "RETURN"]
+UpdateTypeType = Literal["COMMITMENT", "REPLACE", "RETURN"]
 Private5GServiceName = Literal["privatenetworks"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -89,14 +91,15 @@
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
@@ -136,14 +139,15 @@
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
@@ -222,14 +226,15 @@
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
@@ -240,14 +245,15 @@
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
@@ -283,14 +289,15 @@
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
@@ -309,16 +316,19 @@
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
@@ -398,18 +408,21 @@
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

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/paginator.py` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeviceIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListDeviceIdentifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listdeviceidentifierspaginator)
         """
 
 
@@ -97,15 +97,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNetworkResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworkResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworkresourcespaginator)
         """
 
 
@@ -116,15 +116,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNetworkSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworkSites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworksitespaginator)
         """
 
 
@@ -134,15 +134,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworkspaginator)
         """
 
 
@@ -153,13 +153,13 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOrdersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListOrders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listorderspaginator)
         """
```

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/paginator.pyi` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeviceIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListDeviceIdentifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listdeviceidentifierspaginator)
         """
 
 class ListNetworkResourcesPaginator(Paginator):
@@ -92,15 +92,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNetworkResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworkResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworkresourcespaginator)
         """
 
 class ListNetworkSitesPaginator(Paginator):
@@ -110,15 +110,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNetworkSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworkSites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworksitespaginator)
         """
 
 class ListNetworksPaginator(Paginator):
@@ -127,15 +127,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworkspaginator)
         """
 
 class ListOrdersPaginator(Paginator):
@@ -145,13 +145,13 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOrdersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListOrders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listorderspaginator)
         """
```

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/type_defs.py` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AcknowledgmentStatusType,
+    CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
     HealthStatusType,
     NetworkResourceDefinitionTypeType,
     NetworkResourceFilterKeysType,
     NetworkResourceStatusType,
@@ -35,74 +36,76 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ActivateDeviceIdentifierRequestRequestTypeDef",
     "DeviceIdentifierTypeDef",
     "AddressTypeDef",
+    "CommitmentConfigurationTypeDef",
     "PositionTypeDef",
     "CreateNetworkRequestRequestTypeDef",
     "NetworkTypeDef",
     "DeactivateDeviceIdentifierRequestRequestTypeDef",
     "DeleteNetworkRequestRequestTypeDef",
     "DeleteNetworkSiteRequestRequestTypeDef",
     "GetDeviceIdentifierRequestRequestTypeDef",
     "GetNetworkRequestRequestTypeDef",
     "GetNetworkResourceRequestRequestTypeDef",
     "GetNetworkSiteRequestRequestTypeDef",
     "GetOrderRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
     "ListDeviceIdentifiersRequestRequestTypeDef",
+    "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
     "ListNetworkResourcesRequestRequestTypeDef",
+    "ListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
     "ListNetworkSitesRequestRequestTypeDef",
+    "ListNetworksRequestListNetworksPaginateTypeDef",
     "ListNetworksRequestRequestTypeDef",
+    "ListOrdersRequestListOrdersPaginateTypeDef",
     "ListOrdersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "NameValuePairTypeDef",
     "TrackingInformationTypeDef",
+    "PaginatorConfigTypeDef",
+    "PingResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateNetworkSiteRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PingResponseTypeDef",
     "ActivateDeviceIdentifierResponseTypeDef",
     "DeactivateDeviceIdentifierResponseTypeDef",
     "GetDeviceIdentifierResponseTypeDef",
     "ListDeviceIdentifiersResponseTypeDef",
-    "ActivateNetworkSiteRequestRequestTypeDef",
     "ReturnInformationTypeDef",
+    "ActivateNetworkSiteRequestRequestTypeDef",
+    "CommitmentInformationTypeDef",
+    "OrderedResourceDefinitionTypeDef",
     "StartNetworkResourceUpdateRequestRequestTypeDef",
     "ConfigureAccessPointRequestRequestTypeDef",
     "CreateNetworkResponseTypeDef",
     "DeleteNetworkResponseTypeDef",
     "GetNetworkResponseTypeDef",
     "ListNetworksResponseTypeDef",
-    "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
-    "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
-    "ListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
-    "ListNetworksRequestListNetworksPaginateTypeDef",
-    "ListOrdersRequestListOrdersPaginateTypeDef",
     "NetworkResourceDefinitionTypeDef",
-    "OrderTypeDef",
     "NetworkResourceTypeDef",
+    "OrderTypeDef",
     "SitePlanTypeDef",
-    "AcknowledgeOrderReceiptResponseTypeDef",
-    "GetOrderResponseTypeDef",
-    "ListOrdersResponseTypeDef",
     "ConfigureAccessPointResponseTypeDef",
     "GetNetworkResourceResponseTypeDef",
     "ListNetworkResourcesResponseTypeDef",
     "StartNetworkResourceUpdateResponseTypeDef",
+    "AcknowledgeOrderReceiptResponseTypeDef",
+    "GetOrderResponseTypeDef",
+    "ListOrdersResponseTypeDef",
     "CreateNetworkSiteRequestRequestTypeDef",
     "NetworkSiteTypeDef",
     "UpdateNetworkSitePlanRequestRequestTypeDef",
     "ActivateNetworkSiteResponseTypeDef",
     "CreateNetworkSiteResponseTypeDef",
     "DeleteNetworkSiteResponseTypeDef",
     "GetNetworkSiteResponseTypeDef",
@@ -113,47 +116,34 @@
 AcknowledgeOrderReceiptRequestRequestTypeDef = TypedDict(
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
     {
         "orderArn": str,
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
 _RequiredActivateDeviceIdentifierRequestRequestTypeDef = TypedDict(
     "_RequiredActivateDeviceIdentifierRequestRequestTypeDef",
     {
         "deviceIdentifierArn": str,
     },
 )
 _OptionalActivateDeviceIdentifierRequestRequestTypeDef = TypedDict(
     "_OptionalActivateDeviceIdentifierRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class ActivateDeviceIdentifierRequestRequestTypeDef(
     _RequiredActivateDeviceIdentifierRequestRequestTypeDef,
     _OptionalActivateDeviceIdentifierRequestRequestTypeDef,
 ):
     pass
 
-
 DeviceIdentifierTypeDef = TypedDict(
     "DeviceIdentifierTypeDef",
     {
         "createdAt": datetime,
         "deviceIdentifierArn": str,
         "iccid": str,
         "imsi": str,
@@ -177,25 +167,32 @@
         "street1": str,
     },
 )
 _OptionalAddressTypeDef = TypedDict(
     "_OptionalAddressTypeDef",
     {
         "company": str,
+        "emailAddress": str,
         "phoneNumber": str,
         "street2": str,
         "street3": str,
     },
     total=False,
 )
 
-
 class AddressTypeDef(_RequiredAddressTypeDef, _OptionalAddressTypeDef):
     pass
 
+CommitmentConfigurationTypeDef = TypedDict(
+    "CommitmentConfigurationTypeDef",
+    {
+        "automaticRenewal": bool,
+        "commitmentLength": CommitmentLengthType,
+    },
+)
 
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "elevation": float,
         "elevationReference": ElevationReferenceType,
         "elevationUnit": Literal["FEET"],
@@ -217,21 +214,19 @@
         "clientToken": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateNetworkRequestRequestTypeDef(
     _RequiredCreateNetworkRequestRequestTypeDef, _OptionalCreateNetworkRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredNetworkTypeDef = TypedDict(
     "_RequiredNetworkTypeDef",
     {
         "networkArn": str,
         "networkName": str,
         "status": NetworkStatusType,
     },
@@ -242,83 +237,75 @@
         "createdAt": datetime,
         "description": str,
         "statusReason": str,
     },
     total=False,
 )
 
-
 class NetworkTypeDef(_RequiredNetworkTypeDef, _OptionalNetworkTypeDef):
     pass
 
-
 _RequiredDeactivateDeviceIdentifierRequestRequestTypeDef = TypedDict(
     "_RequiredDeactivateDeviceIdentifierRequestRequestTypeDef",
     {
         "deviceIdentifierArn": str,
     },
 )
 _OptionalDeactivateDeviceIdentifierRequestRequestTypeDef = TypedDict(
     "_OptionalDeactivateDeviceIdentifierRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeactivateDeviceIdentifierRequestRequestTypeDef(
     _RequiredDeactivateDeviceIdentifierRequestRequestTypeDef,
     _OptionalDeactivateDeviceIdentifierRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteNetworkRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalDeleteNetworkRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteNetworkRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteNetworkRequestRequestTypeDef(
     _RequiredDeleteNetworkRequestRequestTypeDef, _OptionalDeleteNetworkRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteNetworkSiteRequestRequestTypeDef",
     {
         "networkSiteArn": str,
     },
 )
 _OptionalDeleteNetworkSiteRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteNetworkSiteRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteNetworkSiteRequestRequestTypeDef(
     _RequiredDeleteNetworkSiteRequestRequestTypeDef, _OptionalDeleteNetworkSiteRequestRequestTypeDef
 ):
     pass
 
-
 GetDeviceIdentifierRequestRequestTypeDef = TypedDict(
     "GetDeviceIdentifierRequestRequestTypeDef",
     {
         "deviceIdentifierArn": str,
     },
 )
 
@@ -346,24 +333,35 @@
 GetOrderRequestRequestTypeDef = TypedDict(
     "GetOrderRequestRequestTypeDef",
     {
         "orderArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "networkArn": str,
+    },
+)
+_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
+    {
+        "filters": Mapping[DeviceIdentifierFilterKeysType, Sequence[str]],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef(
+    _RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+    _OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+):
+    pass
+
 _RequiredListDeviceIdentifiersRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceIdentifiersRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListDeviceIdentifiersRequestRequestTypeDef = TypedDict(
@@ -372,21 +370,40 @@
         "filters": Mapping[DeviceIdentifierFilterKeysType, Sequence[str]],
         "maxResults": int,
         "startToken": str,
     },
     total=False,
 )
 
-
 class ListDeviceIdentifiersRequestRequestTypeDef(
     _RequiredListDeviceIdentifiersRequestRequestTypeDef,
     _OptionalListDeviceIdentifiersRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
+    {
+        "filters": Mapping[NetworkResourceFilterKeysType, Sequence[str]],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef(
+    _RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
+    _OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
+):
+    pass
 
 _RequiredListNetworkResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListNetworkResourcesRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
@@ -396,21 +413,40 @@
         "filters": Mapping[NetworkResourceFilterKeysType, Sequence[str]],
         "maxResults": int,
         "startToken": str,
     },
     total=False,
 )
 
-
 class ListNetworkResourcesRequestRequestTypeDef(
     _RequiredListNetworkResourcesRequestRequestTypeDef,
     _OptionalListNetworkResourcesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
+    "_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
+    "_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
+    {
+        "filters": Mapping[Literal["STATUS"], Sequence[str]],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListNetworkSitesRequestListNetworkSitesPaginateTypeDef(
+    _RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
+    _OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
+):
+    pass
 
 _RequiredListNetworkSitesRequestRequestTypeDef = TypedDict(
     "_RequiredListNetworkSitesRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
@@ -420,31 +456,59 @@
         "filters": Mapping[Literal["STATUS"], Sequence[str]],
         "maxResults": int,
         "startToken": str,
     },
     total=False,
 )
 
-
 class ListNetworkSitesRequestRequestTypeDef(
     _RequiredListNetworkSitesRequestRequestTypeDef, _OptionalListNetworkSitesRequestRequestTypeDef
 ):
     pass
 
+ListNetworksRequestListNetworksPaginateTypeDef = TypedDict(
+    "ListNetworksRequestListNetworksPaginateTypeDef",
+    {
+        "filters": Mapping[Literal["STATUS"], Sequence[str]],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListNetworksRequestRequestTypeDef = TypedDict(
     "ListNetworksRequestRequestTypeDef",
     {
         "filters": Mapping[Literal["STATUS"], Sequence[str]],
         "maxResults": int,
         "startToken": str,
     },
     total=False,
 )
 
+_RequiredListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
+    "_RequiredListOrdersRequestListOrdersPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
+    "_OptionalListOrdersRequestListOrdersPaginateTypeDef",
+    {
+        "filters": Mapping[OrderFilterKeysType, Sequence[str]],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListOrdersRequestListOrdersPaginateTypeDef(
+    _RequiredListOrdersRequestListOrdersPaginateTypeDef,
+    _OptionalListOrdersRequestListOrdersPaginateTypeDef,
+):
+    pass
+
 _RequiredListOrdersRequestRequestTypeDef = TypedDict(
     "_RequiredListOrdersRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListOrdersRequestRequestTypeDef = TypedDict(
@@ -453,55 +517,88 @@
         "filters": Mapping[OrderFilterKeysType, Sequence[str]],
         "maxResults": int,
         "startToken": str,
     },
     total=False,
 )
 
-
 class ListOrdersRequestRequestTypeDef(
     _RequiredListOrdersRequestRequestTypeDef, _OptionalListOrdersRequestRequestTypeDef
 ):
     pass
 
-
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
 _RequiredNameValuePairTypeDef = TypedDict(
     "_RequiredNameValuePairTypeDef",
     {
         "name": str,
     },
 )
 _OptionalNameValuePairTypeDef = TypedDict(
     "_OptionalNameValuePairTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class NameValuePairTypeDef(_RequiredNameValuePairTypeDef, _OptionalNameValuePairTypeDef):
     pass
 
-
 TrackingInformationTypeDef = TypedDict(
     "TrackingInformationTypeDef",
     {
         "trackingNumber": str,
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
+PingResponseTypeDef = TypedDict(
+    "PingResponseTypeDef",
+    {
+        "status": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -525,130 +622,150 @@
     {
         "clientToken": str,
         "description": str,
     },
     total=False,
 )
 
-
 class UpdateNetworkSiteRequestRequestTypeDef(
     _RequiredUpdateNetworkSiteRequestRequestTypeDef, _OptionalUpdateNetworkSiteRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PingResponseTypeDef = TypedDict(
-    "PingResponseTypeDef",
-    {
-        "status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ActivateDeviceIdentifierResponseTypeDef = TypedDict(
     "ActivateDeviceIdentifierResponseTypeDef",
     {
         "deviceIdentifier": DeviceIdentifierTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeactivateDeviceIdentifierResponseTypeDef = TypedDict(
     "DeactivateDeviceIdentifierResponseTypeDef",
     {
         "deviceIdentifier": DeviceIdentifierTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeviceIdentifierResponseTypeDef = TypedDict(
     "GetDeviceIdentifierResponseTypeDef",
     {
         "deviceIdentifier": DeviceIdentifierTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeviceIdentifiersResponseTypeDef = TypedDict(
     "ListDeviceIdentifiersResponseTypeDef",
     {
         "deviceIdentifiers": List[DeviceIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ReturnInformationTypeDef = TypedDict(
+    "ReturnInformationTypeDef",
+    {
+        "replacementOrderArn": str,
+        "returnReason": str,
+        "shippingAddress": AddressTypeDef,
+        "shippingLabel": str,
+    },
+    total=False,
+)
+
 _RequiredActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredActivateNetworkSiteRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "shippingAddress": AddressTypeDef,
     },
 )
 _OptionalActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_OptionalActivateNetworkSiteRequestRequestTypeDef",
     {
         "clientToken": str,
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ActivateNetworkSiteRequestRequestTypeDef(
     _RequiredActivateNetworkSiteRequestRequestTypeDef,
     _OptionalActivateNetworkSiteRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCommitmentInformationTypeDef = TypedDict(
+    "_RequiredCommitmentInformationTypeDef",
+    {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+    },
+)
+_OptionalCommitmentInformationTypeDef = TypedDict(
+    "_OptionalCommitmentInformationTypeDef",
+    {
+        "expiresOn": datetime,
+        "startAt": datetime,
+    },
+    total=False,
+)
 
-ReturnInformationTypeDef = TypedDict(
-    "ReturnInformationTypeDef",
+class CommitmentInformationTypeDef(
+    _RequiredCommitmentInformationTypeDef, _OptionalCommitmentInformationTypeDef
+):
+    pass
+
+_RequiredOrderedResourceDefinitionTypeDef = TypedDict(
+    "_RequiredOrderedResourceDefinitionTypeDef",
     {
-        "replacementOrderArn": str,
-        "returnReason": str,
-        "shippingAddress": AddressTypeDef,
-        "shippingLabel": str,
+        "count": int,
+        "type": NetworkResourceDefinitionTypeType,
+    },
+)
+_OptionalOrderedResourceDefinitionTypeDef = TypedDict(
+    "_OptionalOrderedResourceDefinitionTypeDef",
+    {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
     total=False,
 )
 
+class OrderedResourceDefinitionTypeDef(
+    _RequiredOrderedResourceDefinitionTypeDef, _OptionalOrderedResourceDefinitionTypeDef
+):
+    pass
+
 _RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
     "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
     {
         "networkResourceArn": str,
         "updateType": UpdateTypeType,
     },
 )
 _OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
     "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
     {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
         "returnReason": str,
         "shippingAddress": AddressTypeDef,
     },
     total=False,
 )
 
-
 class StartNetworkResourceUpdateRequestRequestTypeDef(
     _RequiredStartNetworkResourceUpdateRequestRequestTypeDef,
     _OptionalStartNetworkResourceUpdateRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredConfigureAccessPointRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAccessPointRequestRequestTypeDef",
     {
         "accessPointArn": str,
     },
 )
 _OptionalConfigureAccessPointRequestRequestTypeDef = TypedDict(
@@ -659,158 +776,55 @@
         "cpiUserPassword": str,
         "cpiUsername": str,
         "position": PositionTypeDef,
     },
     total=False,
 )
 
-
 class ConfigureAccessPointRequestRequestTypeDef(
     _RequiredConfigureAccessPointRequestRequestTypeDef,
     _OptionalConfigureAccessPointRequestRequestTypeDef,
 ):
     pass
 
-
 CreateNetworkResponseTypeDef = TypedDict(
     "CreateNetworkResponseTypeDef",
     {
         "network": NetworkTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteNetworkResponseTypeDef = TypedDict(
     "DeleteNetworkResponseTypeDef",
     {
         "network": NetworkTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNetworkResponseTypeDef = TypedDict(
     "GetNetworkResponseTypeDef",
     {
         "network": NetworkTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNetworksResponseTypeDef = TypedDict(
     "ListNetworksResponseTypeDef",
     {
         "networks": List[NetworkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
-    {
-        "filters": Mapping[DeviceIdentifierFilterKeysType, Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef(
-    _RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-    _OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
-    {
-        "filters": Mapping[NetworkResourceFilterKeysType, Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef(
-    _RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-    _OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
-    "_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
-    "_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
-    {
-        "filters": Mapping[Literal["STATUS"], Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListNetworkSitesRequestListNetworkSitesPaginateTypeDef(
-    _RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-    _OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-):
-    pass
-
-
-ListNetworksRequestListNetworksPaginateTypeDef = TypedDict(
-    "ListNetworksRequestListNetworksPaginateTypeDef",
-    {
-        "filters": Mapping[Literal["STATUS"], Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
-    "_RequiredListOrdersRequestListOrdersPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
-    "_OptionalListOrdersRequestListOrdersPaginateTypeDef",
-    {
-        "filters": Mapping[OrderFilterKeysType, Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListOrdersRequestListOrdersPaginateTypeDef(
-    _RequiredListOrdersRequestListOrdersPaginateTypeDef,
-    _OptionalListOrdersRequestListOrdersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredNetworkResourceDefinitionTypeDef = TypedDict(
     "_RequiredNetworkResourceDefinitionTypeDef",
     {
         "count": int,
         "type": NetworkResourceDefinitionTypeType,
     },
 )
@@ -818,39 +832,24 @@
     "_OptionalNetworkResourceDefinitionTypeDef",
     {
         "options": List[NameValuePairTypeDef],
     },
     total=False,
 )
 
-
 class NetworkResourceDefinitionTypeDef(
     _RequiredNetworkResourceDefinitionTypeDef, _OptionalNetworkResourceDefinitionTypeDef
 ):
     pass
 
-
-OrderTypeDef = TypedDict(
-    "OrderTypeDef",
-    {
-        "acknowledgmentStatus": AcknowledgmentStatusType,
-        "createdAt": datetime,
-        "networkArn": str,
-        "networkSiteArn": str,
-        "orderArn": str,
-        "shippingAddress": AddressTypeDef,
-        "trackingInformation": List[TrackingInformationTypeDef],
-    },
-    total=False,
-)
-
 NetworkResourceTypeDef = TypedDict(
     "NetworkResourceTypeDef",
     {
         "attributes": List[NameValuePairTypeDef],
+        "commitmentInformation": CommitmentInformationTypeDef,
         "createdAt": datetime,
         "description": str,
         "health": HealthStatusType,
         "model": str,
         "networkArn": str,
         "networkResourceArn": str,
         "networkSiteArn": str,
@@ -862,80 +861,95 @@
         "statusReason": str,
         "type": Literal["RADIO_UNIT"],
         "vendor": str,
     },
     total=False,
 )
 
-SitePlanTypeDef = TypedDict(
-    "SitePlanTypeDef",
+OrderTypeDef = TypedDict(
+    "OrderTypeDef",
     {
-        "options": List[NameValuePairTypeDef],
-        "resourceDefinitions": List[NetworkResourceDefinitionTypeDef],
+        "acknowledgmentStatus": AcknowledgmentStatusType,
+        "createdAt": datetime,
+        "networkArn": str,
+        "networkSiteArn": str,
+        "orderArn": str,
+        "orderedResources": List[OrderedResourceDefinitionTypeDef],
+        "shippingAddress": AddressTypeDef,
+        "trackingInformation": List[TrackingInformationTypeDef],
     },
     total=False,
 )
 
-AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
-    "AcknowledgeOrderReceiptResponseTypeDef",
-    {
-        "order": OrderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetOrderResponseTypeDef = TypedDict(
-    "GetOrderResponseTypeDef",
-    {
-        "order": OrderTypeDef,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListOrdersResponseTypeDef = TypedDict(
-    "ListOrdersResponseTypeDef",
+SitePlanTypeDef = TypedDict(
+    "SitePlanTypeDef",
     {
-        "nextToken": str,
-        "orders": List[OrderTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "options": List[NameValuePairTypeDef],
+        "resourceDefinitions": List[NetworkResourceDefinitionTypeDef],
     },
+    total=False,
 )
 
 ConfigureAccessPointResponseTypeDef = TypedDict(
     "ConfigureAccessPointResponseTypeDef",
     {
         "accessPoint": NetworkResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNetworkResourceResponseTypeDef = TypedDict(
     "GetNetworkResourceResponseTypeDef",
     {
         "networkResource": NetworkResourceTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNetworkResourcesResponseTypeDef = TypedDict(
     "ListNetworkResourcesResponseTypeDef",
     {
         "networkResources": List[NetworkResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartNetworkResourceUpdateResponseTypeDef = TypedDict(
     "StartNetworkResourceUpdateResponseTypeDef",
     {
         "networkResource": NetworkResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
+    "AcknowledgeOrderReceiptResponseTypeDef",
+    {
+        "order": OrderTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetOrderResponseTypeDef = TypedDict(
+    "GetOrderResponseTypeDef",
+    {
+        "order": OrderTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListOrdersResponseTypeDef = TypedDict(
+    "ListOrdersResponseTypeDef",
+    {
+        "nextToken": str,
+        "orders": List[OrderTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkSiteRequestRequestTypeDef",
     {
         "networkArn": str,
@@ -951,21 +965,19 @@
         "description": str,
         "pendingPlan": SitePlanTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateNetworkSiteRequestRequestTypeDef(
     _RequiredCreateNetworkSiteRequestRequestTypeDef, _OptionalCreateNetworkSiteRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredNetworkSiteTypeDef = TypedDict(
     "_RequiredNetworkSiteTypeDef",
     {
         "networkArn": str,
         "networkSiteArn": str,
         "networkSiteName": str,
         "status": NetworkSiteStatusType,
@@ -981,19 +993,17 @@
         "description": str,
         "pendingPlan": SitePlanTypeDef,
         "statusReason": str,
     },
     total=False,
 )
 
-
 class NetworkSiteTypeDef(_RequiredNetworkSiteTypeDef, _OptionalNetworkSiteTypeDef):
     pass
 
-
 _RequiredUpdateNetworkSitePlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkSitePlanRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "pendingPlan": SitePlanTypeDef,
     },
 )
@@ -1001,66 +1011,64 @@
     "_OptionalUpdateNetworkSitePlanRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateNetworkSitePlanRequestRequestTypeDef(
     _RequiredUpdateNetworkSitePlanRequestRequestTypeDef,
     _OptionalUpdateNetworkSitePlanRequestRequestTypeDef,
 ):
     pass
 
-
 ActivateNetworkSiteResponseTypeDef = TypedDict(
     "ActivateNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateNetworkSiteResponseTypeDef = TypedDict(
     "CreateNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteNetworkSiteResponseTypeDef = TypedDict(
     "DeleteNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNetworkSiteResponseTypeDef = TypedDict(
     "GetNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNetworkSitesResponseTypeDef = TypedDict(
     "ListNetworkSitesResponseTypeDef",
     {
         "networkSites": List[NetworkSiteTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNetworkSiteResponseTypeDef = TypedDict(
     "UpdateNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/type_defs.pyi` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AcknowledgmentStatusType,
+    CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
     HealthStatusType,
     NetworkResourceDefinitionTypeType,
     NetworkResourceFilterKeysType,
     NetworkResourceStatusType,
@@ -35,73 +36,77 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ActivateDeviceIdentifierRequestRequestTypeDef",
     "DeviceIdentifierTypeDef",
     "AddressTypeDef",
+    "CommitmentConfigurationTypeDef",
     "PositionTypeDef",
     "CreateNetworkRequestRequestTypeDef",
     "NetworkTypeDef",
     "DeactivateDeviceIdentifierRequestRequestTypeDef",
     "DeleteNetworkRequestRequestTypeDef",
     "DeleteNetworkSiteRequestRequestTypeDef",
     "GetDeviceIdentifierRequestRequestTypeDef",
     "GetNetworkRequestRequestTypeDef",
     "GetNetworkResourceRequestRequestTypeDef",
     "GetNetworkSiteRequestRequestTypeDef",
     "GetOrderRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
     "ListDeviceIdentifiersRequestRequestTypeDef",
+    "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
     "ListNetworkResourcesRequestRequestTypeDef",
+    "ListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
     "ListNetworkSitesRequestRequestTypeDef",
+    "ListNetworksRequestListNetworksPaginateTypeDef",
     "ListNetworksRequestRequestTypeDef",
+    "ListOrdersRequestListOrdersPaginateTypeDef",
     "ListOrdersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "NameValuePairTypeDef",
     "TrackingInformationTypeDef",
+    "PaginatorConfigTypeDef",
+    "PingResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateNetworkSiteRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PingResponseTypeDef",
     "ActivateDeviceIdentifierResponseTypeDef",
     "DeactivateDeviceIdentifierResponseTypeDef",
     "GetDeviceIdentifierResponseTypeDef",
     "ListDeviceIdentifiersResponseTypeDef",
-    "ActivateNetworkSiteRequestRequestTypeDef",
     "ReturnInformationTypeDef",
+    "ActivateNetworkSiteRequestRequestTypeDef",
+    "CommitmentInformationTypeDef",
+    "OrderedResourceDefinitionTypeDef",
     "StartNetworkResourceUpdateRequestRequestTypeDef",
     "ConfigureAccessPointRequestRequestTypeDef",
     "CreateNetworkResponseTypeDef",
     "DeleteNetworkResponseTypeDef",
     "GetNetworkResponseTypeDef",
     "ListNetworksResponseTypeDef",
-    "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
-    "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
-    "ListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
-    "ListNetworksRequestListNetworksPaginateTypeDef",
-    "ListOrdersRequestListOrdersPaginateTypeDef",
     "NetworkResourceDefinitionTypeDef",
-    "OrderTypeDef",
     "NetworkResourceTypeDef",
+    "OrderTypeDef",
     "SitePlanTypeDef",
-    "AcknowledgeOrderReceiptResponseTypeDef",
-    "GetOrderResponseTypeDef",
-    "ListOrdersResponseTypeDef",
     "ConfigureAccessPointResponseTypeDef",
     "GetNetworkResourceResponseTypeDef",
     "ListNetworkResourcesResponseTypeDef",
     "StartNetworkResourceUpdateResponseTypeDef",
+    "AcknowledgeOrderReceiptResponseTypeDef",
+    "GetOrderResponseTypeDef",
+    "ListOrdersResponseTypeDef",
     "CreateNetworkSiteRequestRequestTypeDef",
     "NetworkSiteTypeDef",
     "UpdateNetworkSitePlanRequestRequestTypeDef",
     "ActivateNetworkSiteResponseTypeDef",
     "CreateNetworkSiteResponseTypeDef",
     "DeleteNetworkSiteResponseTypeDef",
     "GetNetworkSiteResponseTypeDef",
@@ -112,45 +117,36 @@
 AcknowledgeOrderReceiptRequestRequestTypeDef = TypedDict(
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
     {
         "orderArn": str,
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
 _RequiredActivateDeviceIdentifierRequestRequestTypeDef = TypedDict(
     "_RequiredActivateDeviceIdentifierRequestRequestTypeDef",
     {
         "deviceIdentifierArn": str,
     },
 )
 _OptionalActivateDeviceIdentifierRequestRequestTypeDef = TypedDict(
     "_OptionalActivateDeviceIdentifierRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class ActivateDeviceIdentifierRequestRequestTypeDef(
     _RequiredActivateDeviceIdentifierRequestRequestTypeDef,
     _OptionalActivateDeviceIdentifierRequestRequestTypeDef,
 ):
     pass
 
+
 DeviceIdentifierTypeDef = TypedDict(
     "DeviceIdentifierTypeDef",
     {
         "createdAt": datetime,
         "deviceIdentifierArn": str,
         "iccid": str,
         "imsi": str,
@@ -174,24 +170,35 @@
         "street1": str,
     },
 )
 _OptionalAddressTypeDef = TypedDict(
     "_OptionalAddressTypeDef",
     {
         "company": str,
+        "emailAddress": str,
         "phoneNumber": str,
         "street2": str,
         "street3": str,
     },
     total=False,
 )
 
+
 class AddressTypeDef(_RequiredAddressTypeDef, _OptionalAddressTypeDef):
     pass
 
+
+CommitmentConfigurationTypeDef = TypedDict(
+    "CommitmentConfigurationTypeDef",
+    {
+        "automaticRenewal": bool,
+        "commitmentLength": CommitmentLengthType,
+    },
+)
+
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "elevation": float,
         "elevationReference": ElevationReferenceType,
         "elevationUnit": Literal["FEET"],
         "latitude": float,
@@ -212,19 +219,21 @@
         "clientToken": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateNetworkRequestRequestTypeDef(
     _RequiredCreateNetworkRequestRequestTypeDef, _OptionalCreateNetworkRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredNetworkTypeDef = TypedDict(
     "_RequiredNetworkTypeDef",
     {
         "networkArn": str,
         "networkName": str,
         "status": NetworkStatusType,
     },
@@ -235,75 +244,83 @@
         "createdAt": datetime,
         "description": str,
         "statusReason": str,
     },
     total=False,
 )
 
+
 class NetworkTypeDef(_RequiredNetworkTypeDef, _OptionalNetworkTypeDef):
     pass
 
+
 _RequiredDeactivateDeviceIdentifierRequestRequestTypeDef = TypedDict(
     "_RequiredDeactivateDeviceIdentifierRequestRequestTypeDef",
     {
         "deviceIdentifierArn": str,
     },
 )
 _OptionalDeactivateDeviceIdentifierRequestRequestTypeDef = TypedDict(
     "_OptionalDeactivateDeviceIdentifierRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeactivateDeviceIdentifierRequestRequestTypeDef(
     _RequiredDeactivateDeviceIdentifierRequestRequestTypeDef,
     _OptionalDeactivateDeviceIdentifierRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteNetworkRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalDeleteNetworkRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteNetworkRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteNetworkRequestRequestTypeDef(
     _RequiredDeleteNetworkRequestRequestTypeDef, _OptionalDeleteNetworkRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteNetworkSiteRequestRequestTypeDef",
     {
         "networkSiteArn": str,
     },
 )
 _OptionalDeleteNetworkSiteRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteNetworkSiteRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteNetworkSiteRequestRequestTypeDef(
     _RequiredDeleteNetworkSiteRequestRequestTypeDef, _OptionalDeleteNetworkSiteRequestRequestTypeDef
 ):
     pass
 
+
 GetDeviceIdentifierRequestRequestTypeDef = TypedDict(
     "GetDeviceIdentifierRequestRequestTypeDef",
     {
         "deviceIdentifierArn": str,
     },
 )
 
@@ -331,24 +348,37 @@
 GetOrderRequestRequestTypeDef = TypedDict(
     "GetOrderRequestRequestTypeDef",
     {
         "orderArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "networkArn": str,
+    },
+)
+_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
+    {
+        "filters": Mapping[DeviceIdentifierFilterKeysType, Sequence[str]],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef(
+    _RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+    _OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDeviceIdentifiersRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceIdentifiersRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListDeviceIdentifiersRequestRequestTypeDef = TypedDict(
@@ -357,20 +387,45 @@
         "filters": Mapping[DeviceIdentifierFilterKeysType, Sequence[str]],
         "maxResults": int,
         "startToken": str,
     },
     total=False,
 )
 
+
 class ListDeviceIdentifiersRequestRequestTypeDef(
     _RequiredListDeviceIdentifiersRequestRequestTypeDef,
     _OptionalListDeviceIdentifiersRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
+    {
+        "filters": Mapping[NetworkResourceFilterKeysType, Sequence[str]],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef(
+    _RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
+    _OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListNetworkResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListNetworkResourcesRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListNetworkResourcesRequestRequestTypeDef = TypedDict(
@@ -379,20 +434,45 @@
         "filters": Mapping[NetworkResourceFilterKeysType, Sequence[str]],
         "maxResults": int,
         "startToken": str,
     },
     total=False,
 )
 
+
 class ListNetworkResourcesRequestRequestTypeDef(
     _RequiredListNetworkResourcesRequestRequestTypeDef,
     _OptionalListNetworkResourcesRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
+    "_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
+    "_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
+    {
+        "filters": Mapping[Literal["STATUS"], Sequence[str]],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListNetworkSitesRequestListNetworkSitesPaginateTypeDef(
+    _RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
+    _OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListNetworkSitesRequestRequestTypeDef = TypedDict(
     "_RequiredListNetworkSitesRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListNetworkSitesRequestRequestTypeDef = TypedDict(
@@ -401,29 +481,63 @@
         "filters": Mapping[Literal["STATUS"], Sequence[str]],
         "maxResults": int,
         "startToken": str,
     },
     total=False,
 )
 
+
 class ListNetworkSitesRequestRequestTypeDef(
     _RequiredListNetworkSitesRequestRequestTypeDef, _OptionalListNetworkSitesRequestRequestTypeDef
 ):
     pass
 
+
+ListNetworksRequestListNetworksPaginateTypeDef = TypedDict(
+    "ListNetworksRequestListNetworksPaginateTypeDef",
+    {
+        "filters": Mapping[Literal["STATUS"], Sequence[str]],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListNetworksRequestRequestTypeDef = TypedDict(
     "ListNetworksRequestRequestTypeDef",
     {
         "filters": Mapping[Literal["STATUS"], Sequence[str]],
         "maxResults": int,
         "startToken": str,
     },
     total=False,
 )
 
+_RequiredListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
+    "_RequiredListOrdersRequestListOrdersPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
+    "_OptionalListOrdersRequestListOrdersPaginateTypeDef",
+    {
+        "filters": Mapping[OrderFilterKeysType, Sequence[str]],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListOrdersRequestListOrdersPaginateTypeDef(
+    _RequiredListOrdersRequestListOrdersPaginateTypeDef,
+    _OptionalListOrdersRequestListOrdersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListOrdersRequestRequestTypeDef = TypedDict(
     "_RequiredListOrdersRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListOrdersRequestRequestTypeDef = TypedDict(
@@ -432,51 +546,92 @@
         "filters": Mapping[OrderFilterKeysType, Sequence[str]],
         "maxResults": int,
         "startToken": str,
     },
     total=False,
 )
 
+
 class ListOrdersRequestRequestTypeDef(
     _RequiredListOrdersRequestRequestTypeDef, _OptionalListOrdersRequestRequestTypeDef
 ):
     pass
 
+
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
 _RequiredNameValuePairTypeDef = TypedDict(
     "_RequiredNameValuePairTypeDef",
     {
         "name": str,
     },
 )
 _OptionalNameValuePairTypeDef = TypedDict(
     "_OptionalNameValuePairTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class NameValuePairTypeDef(_RequiredNameValuePairTypeDef, _OptionalNameValuePairTypeDef):
     pass
 
+
 TrackingInformationTypeDef = TypedDict(
     "TrackingInformationTypeDef",
     {
         "trackingNumber": str,
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
+PingResponseTypeDef = TypedDict(
+    "PingResponseTypeDef",
+    {
+        "status": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -500,124 +655,160 @@
     {
         "clientToken": str,
         "description": str,
     },
     total=False,
 )
 
+
 class UpdateNetworkSiteRequestRequestTypeDef(
     _RequiredUpdateNetworkSiteRequestRequestTypeDef, _OptionalUpdateNetworkSiteRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PingResponseTypeDef = TypedDict(
-    "PingResponseTypeDef",
-    {
-        "status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 ActivateDeviceIdentifierResponseTypeDef = TypedDict(
     "ActivateDeviceIdentifierResponseTypeDef",
     {
         "deviceIdentifier": DeviceIdentifierTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeactivateDeviceIdentifierResponseTypeDef = TypedDict(
     "DeactivateDeviceIdentifierResponseTypeDef",
     {
         "deviceIdentifier": DeviceIdentifierTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeviceIdentifierResponseTypeDef = TypedDict(
     "GetDeviceIdentifierResponseTypeDef",
     {
         "deviceIdentifier": DeviceIdentifierTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeviceIdentifiersResponseTypeDef = TypedDict(
     "ListDeviceIdentifiersResponseTypeDef",
     {
         "deviceIdentifiers": List[DeviceIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ReturnInformationTypeDef = TypedDict(
+    "ReturnInformationTypeDef",
+    {
+        "replacementOrderArn": str,
+        "returnReason": str,
+        "shippingAddress": AddressTypeDef,
+        "shippingLabel": str,
+    },
+    total=False,
+)
+
 _RequiredActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredActivateNetworkSiteRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "shippingAddress": AddressTypeDef,
     },
 )
 _OptionalActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_OptionalActivateNetworkSiteRequestRequestTypeDef",
     {
         "clientToken": str,
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ActivateNetworkSiteRequestRequestTypeDef(
     _RequiredActivateNetworkSiteRequestRequestTypeDef,
     _OptionalActivateNetworkSiteRequestRequestTypeDef,
 ):
     pass
 
-ReturnInformationTypeDef = TypedDict(
-    "ReturnInformationTypeDef",
+
+_RequiredCommitmentInformationTypeDef = TypedDict(
+    "_RequiredCommitmentInformationTypeDef",
     {
-        "replacementOrderArn": str,
-        "returnReason": str,
-        "shippingAddress": AddressTypeDef,
-        "shippingLabel": str,
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+    },
+)
+_OptionalCommitmentInformationTypeDef = TypedDict(
+    "_OptionalCommitmentInformationTypeDef",
+    {
+        "expiresOn": datetime,
+        "startAt": datetime,
+    },
+    total=False,
+)
+
+
+class CommitmentInformationTypeDef(
+    _RequiredCommitmentInformationTypeDef, _OptionalCommitmentInformationTypeDef
+):
+    pass
+
+
+_RequiredOrderedResourceDefinitionTypeDef = TypedDict(
+    "_RequiredOrderedResourceDefinitionTypeDef",
+    {
+        "count": int,
+        "type": NetworkResourceDefinitionTypeType,
+    },
+)
+_OptionalOrderedResourceDefinitionTypeDef = TypedDict(
+    "_OptionalOrderedResourceDefinitionTypeDef",
+    {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
     total=False,
 )
 
+
+class OrderedResourceDefinitionTypeDef(
+    _RequiredOrderedResourceDefinitionTypeDef, _OptionalOrderedResourceDefinitionTypeDef
+):
+    pass
+
+
 _RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
     "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
     {
         "networkResourceArn": str,
         "updateType": UpdateTypeType,
     },
 )
 _OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
     "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
     {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
         "returnReason": str,
         "shippingAddress": AddressTypeDef,
     },
     total=False,
 )
 
+
 class StartNetworkResourceUpdateRequestRequestTypeDef(
     _RequiredStartNetworkResourceUpdateRequestRequestTypeDef,
     _OptionalStartNetworkResourceUpdateRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredConfigureAccessPointRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAccessPointRequestRequestTypeDef",
     {
         "accessPointArn": str,
     },
 )
 _OptionalConfigureAccessPointRequestRequestTypeDef = TypedDict(
@@ -628,148 +819,57 @@
         "cpiUserPassword": str,
         "cpiUsername": str,
         "position": PositionTypeDef,
     },
     total=False,
 )
 
+
 class ConfigureAccessPointRequestRequestTypeDef(
     _RequiredConfigureAccessPointRequestRequestTypeDef,
     _OptionalConfigureAccessPointRequestRequestTypeDef,
 ):
     pass
 
+
 CreateNetworkResponseTypeDef = TypedDict(
     "CreateNetworkResponseTypeDef",
     {
         "network": NetworkTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteNetworkResponseTypeDef = TypedDict(
     "DeleteNetworkResponseTypeDef",
     {
         "network": NetworkTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNetworkResponseTypeDef = TypedDict(
     "GetNetworkResponseTypeDef",
     {
         "network": NetworkTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNetworksResponseTypeDef = TypedDict(
     "ListNetworksResponseTypeDef",
     {
         "networks": List[NetworkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
-    {
-        "filters": Mapping[DeviceIdentifierFilterKeysType, Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef(
-    _RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-    _OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-):
-    pass
-
-_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
-    {
-        "filters": Mapping[NetworkResourceFilterKeysType, Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef(
-    _RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-    _OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-):
-    pass
-
-_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
-    "_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
-    "_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
-    {
-        "filters": Mapping[Literal["STATUS"], Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListNetworkSitesRequestListNetworkSitesPaginateTypeDef(
-    _RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-    _OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-):
-    pass
-
-ListNetworksRequestListNetworksPaginateTypeDef = TypedDict(
-    "ListNetworksRequestListNetworksPaginateTypeDef",
-    {
-        "filters": Mapping[Literal["STATUS"], Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
-    "_RequiredListOrdersRequestListOrdersPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
-    "_OptionalListOrdersRequestListOrdersPaginateTypeDef",
-    {
-        "filters": Mapping[OrderFilterKeysType, Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListOrdersRequestListOrdersPaginateTypeDef(
-    _RequiredListOrdersRequestListOrdersPaginateTypeDef,
-    _OptionalListOrdersRequestListOrdersPaginateTypeDef,
-):
-    pass
-
 _RequiredNetworkResourceDefinitionTypeDef = TypedDict(
     "_RequiredNetworkResourceDefinitionTypeDef",
     {
         "count": int,
         "type": NetworkResourceDefinitionTypeType,
     },
 )
@@ -777,37 +877,26 @@
     "_OptionalNetworkResourceDefinitionTypeDef",
     {
         "options": List[NameValuePairTypeDef],
     },
     total=False,
 )
 
+
 class NetworkResourceDefinitionTypeDef(
     _RequiredNetworkResourceDefinitionTypeDef, _OptionalNetworkResourceDefinitionTypeDef
 ):
     pass
 
-OrderTypeDef = TypedDict(
-    "OrderTypeDef",
-    {
-        "acknowledgmentStatus": AcknowledgmentStatusType,
-        "createdAt": datetime,
-        "networkArn": str,
-        "networkSiteArn": str,
-        "orderArn": str,
-        "shippingAddress": AddressTypeDef,
-        "trackingInformation": List[TrackingInformationTypeDef],
-    },
-    total=False,
-)
 
 NetworkResourceTypeDef = TypedDict(
     "NetworkResourceTypeDef",
     {
         "attributes": List[NameValuePairTypeDef],
+        "commitmentInformation": CommitmentInformationTypeDef,
         "createdAt": datetime,
         "description": str,
         "health": HealthStatusType,
         "model": str,
         "networkArn": str,
         "networkResourceArn": str,
         "networkSiteArn": str,
@@ -819,80 +908,95 @@
         "statusReason": str,
         "type": Literal["RADIO_UNIT"],
         "vendor": str,
     },
     total=False,
 )
 
-SitePlanTypeDef = TypedDict(
-    "SitePlanTypeDef",
+OrderTypeDef = TypedDict(
+    "OrderTypeDef",
     {
-        "options": List[NameValuePairTypeDef],
-        "resourceDefinitions": List[NetworkResourceDefinitionTypeDef],
+        "acknowledgmentStatus": AcknowledgmentStatusType,
+        "createdAt": datetime,
+        "networkArn": str,
+        "networkSiteArn": str,
+        "orderArn": str,
+        "orderedResources": List[OrderedResourceDefinitionTypeDef],
+        "shippingAddress": AddressTypeDef,
+        "trackingInformation": List[TrackingInformationTypeDef],
     },
     total=False,
 )
 
-AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
-    "AcknowledgeOrderReceiptResponseTypeDef",
-    {
-        "order": OrderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetOrderResponseTypeDef = TypedDict(
-    "GetOrderResponseTypeDef",
-    {
-        "order": OrderTypeDef,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListOrdersResponseTypeDef = TypedDict(
-    "ListOrdersResponseTypeDef",
+SitePlanTypeDef = TypedDict(
+    "SitePlanTypeDef",
     {
-        "nextToken": str,
-        "orders": List[OrderTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "options": List[NameValuePairTypeDef],
+        "resourceDefinitions": List[NetworkResourceDefinitionTypeDef],
     },
+    total=False,
 )
 
 ConfigureAccessPointResponseTypeDef = TypedDict(
     "ConfigureAccessPointResponseTypeDef",
     {
         "accessPoint": NetworkResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNetworkResourceResponseTypeDef = TypedDict(
     "GetNetworkResourceResponseTypeDef",
     {
         "networkResource": NetworkResourceTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNetworkResourcesResponseTypeDef = TypedDict(
     "ListNetworkResourcesResponseTypeDef",
     {
         "networkResources": List[NetworkResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartNetworkResourceUpdateResponseTypeDef = TypedDict(
     "StartNetworkResourceUpdateResponseTypeDef",
     {
         "networkResource": NetworkResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
+    "AcknowledgeOrderReceiptResponseTypeDef",
+    {
+        "order": OrderTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetOrderResponseTypeDef = TypedDict(
+    "GetOrderResponseTypeDef",
+    {
+        "order": OrderTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListOrdersResponseTypeDef = TypedDict(
+    "ListOrdersResponseTypeDef",
+    {
+        "nextToken": str,
+        "orders": List[OrderTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkSiteRequestRequestTypeDef",
     {
         "networkArn": str,
@@ -908,19 +1012,21 @@
         "description": str,
         "pendingPlan": SitePlanTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateNetworkSiteRequestRequestTypeDef(
     _RequiredCreateNetworkSiteRequestRequestTypeDef, _OptionalCreateNetworkSiteRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredNetworkSiteTypeDef = TypedDict(
     "_RequiredNetworkSiteTypeDef",
     {
         "networkArn": str,
         "networkSiteArn": str,
         "networkSiteName": str,
         "status": NetworkSiteStatusType,
@@ -936,17 +1042,19 @@
         "description": str,
         "pendingPlan": SitePlanTypeDef,
         "statusReason": str,
     },
     total=False,
 )
 
+
 class NetworkSiteTypeDef(_RequiredNetworkSiteTypeDef, _OptionalNetworkSiteTypeDef):
     pass
 
+
 _RequiredUpdateNetworkSitePlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkSitePlanRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "pendingPlan": SitePlanTypeDef,
     },
 )
@@ -954,64 +1062,66 @@
     "_OptionalUpdateNetworkSitePlanRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateNetworkSitePlanRequestRequestTypeDef(
     _RequiredUpdateNetworkSitePlanRequestRequestTypeDef,
     _OptionalUpdateNetworkSitePlanRequestRequestTypeDef,
 ):
     pass
 
+
 ActivateNetworkSiteResponseTypeDef = TypedDict(
     "ActivateNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateNetworkSiteResponseTypeDef = TypedDict(
     "CreateNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteNetworkSiteResponseTypeDef = TypedDict(
     "DeleteNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNetworkSiteResponseTypeDef = TypedDict(
     "GetNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNetworkSitesResponseTypeDef = TypedDict(
     "ListNetworkSitesResponseTypeDef",
     {
         "networkSites": List[NetworkSiteTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNetworkSiteResponseTypeDef = TypedDict(
     "UpdateNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/PKG-INFO` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-privatenetworks
-Version: 1.26.72
-Summary: Type annotations for boto3.Private5G 1.26.72 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Private5G 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-privatenetworks"></a>
 
 # mypy-boto3-privatenetworks
 
 [![PyPI - mypy-boto3-privatenetworks](https://img.shields.io/pypi/v/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-privatenetworks?color=blue)](https://pypistats.org/packages/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,14 +312,15 @@
 
 `mypy_boto3_privatenetworks.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_privatenetworks.literals import (
     AcknowledgmentStatusType,
+    CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
     ElevationUnitType,
     HealthStatusType,
     ListDeviceIdentifiersPaginatorName,
     ListNetworkResourcesPaginatorName,
@@ -353,71 +354,74 @@
 
 `mypy_boto3_privatenetworks.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
     AddressTypeDef,
+    CommitmentConfigurationTypeDef,
     PositionTypeDef,
     CreateNetworkRequestRequestTypeDef,
     NetworkTypeDef,
     DeactivateDeviceIdentifierRequestRequestTypeDef,
     DeleteNetworkRequestRequestTypeDef,
     DeleteNetworkSiteRequestRequestTypeDef,
     GetDeviceIdentifierRequestRequestTypeDef,
     GetNetworkRequestRequestTypeDef,
     GetNetworkResourceRequestRequestTypeDef,
     GetNetworkSiteRequestRequestTypeDef,
     GetOrderRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
     ListDeviceIdentifiersRequestRequestTypeDef,
+    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
     ListNetworkResourcesRequestRequestTypeDef,
+    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
     ListNetworkSitesRequestRequestTypeDef,
+    ListNetworksRequestListNetworksPaginateTypeDef,
     ListNetworksRequestRequestTypeDef,
+    ListOrdersRequestListOrdersPaginateTypeDef,
     ListOrdersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NameValuePairTypeDef,
     TrackingInformationTypeDef,
+    PaginatorConfigTypeDef,
+    PingResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateNetworkSiteRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PingResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
     ListDeviceIdentifiersResponseTypeDef,
-    ActivateNetworkSiteRequestRequestTypeDef,
     ReturnInformationTypeDef,
+    ActivateNetworkSiteRequestRequestTypeDef,
+    CommitmentInformationTypeDef,
+    OrderedResourceDefinitionTypeDef,
     StartNetworkResourceUpdateRequestRequestTypeDef,
     ConfigureAccessPointRequestRequestTypeDef,
     CreateNetworkResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     GetNetworkResponseTypeDef,
     ListNetworksResponseTypeDef,
-    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-    ListNetworksRequestListNetworksPaginateTypeDef,
-    ListOrdersRequestListOrdersPaginateTypeDef,
     NetworkResourceDefinitionTypeDef,
-    OrderTypeDef,
     NetworkResourceTypeDef,
+    OrderTypeDef,
     SitePlanTypeDef,
-    AcknowledgeOrderReceiptResponseTypeDef,
-    GetOrderResponseTypeDef,
-    ListOrdersResponseTypeDef,
     ConfigureAccessPointResponseTypeDef,
     GetNetworkResourceResponseTypeDef,
     ListNetworkResourcesResponseTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
+    AcknowledgeOrderReceiptResponseTypeDef,
+    GetOrderResponseTypeDef,
+    ListOrdersResponseTypeDef,
     CreateNetworkSiteRequestRequestTypeDef,
     NetworkSiteTypeDef,
     UpdateNetworkSitePlanRequestRequestTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetNetworkSiteResponseTypeDef,
@@ -433,42 +437,42 @@
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

### Comparing `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/SOURCES.txt` & `mypy-boto3-privatenetworks-1.27.0/mypy_boto3_privatenetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.26.72/setup.py` & `mypy-boto3-privatenetworks-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-privatenetworks.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-privatenetworks",
-    version="1.26.72",
+    version="1.27.0",
     packages=["mypy_boto3_privatenetworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Private5G 1.26.72 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Private5G 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/",
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


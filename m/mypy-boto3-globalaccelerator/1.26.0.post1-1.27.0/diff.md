# Comparing `tmp/mypy-boto3-globalaccelerator-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-globalaccelerator-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-globalaccelerator-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:28 2022, max compression
+gzip compressed data, was "mypy-boto3-globalaccelerator-1.27.0.tar", last modified: Mon Jul  3 19:50:49 2023, max compression
```

## Comparing `mypy-boto3-globalaccelerator-1.26.0.post1.tar` & `mypy-boto3-globalaccelerator-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:28.604831 mypy-boto3-globalaccelerator-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:35:07.000000 mypy-boto3-globalaccelerator-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    20469 2022-11-01 21:43:28.600831 mypy-boto3-globalaccelerator-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18988 2022-11-01 21:35:07.000000 mypy-boto3-globalaccelerator-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:28.600831 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/
--rw-r--r--   0 runner    (1001) docker     (121)     2490 2022-11-01 21:35:07.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-11-01 21:35:07.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-11-01 21:35:07.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    41374 2022-11-01 21:35:08.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    41310 2022-11-01 21:35:08.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9356 2022-11-01 21:35:08.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9354 2022-11-01 21:35:08.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10618 2022-11-01 21:35:08.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    10608 2022-11-01 21:35:08.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:35:07.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    44638 2022-11-01 21:35:09.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    44589 2022-11-01 21:35:08.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:35:07.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:28.600831 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    20469 2022-11-01 21:43:28.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-11-01 21:43:28.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:28.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:28.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:28.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-01 21:43:28.000000 mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:28.604831 mypy-boto3-globalaccelerator-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-11-01 21:35:07.000000 mypy-boto3-globalaccelerator-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:49.227319 mypy-boto3-globalaccelerator-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-03 19:50:49.227319 mypy-boto3-globalaccelerator-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:49.227319 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41373 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41309 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44730 2023-07-03 19:38:19.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44681 2023-07-03 19:38:19.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:49.227319 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-03 19:50:49.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 19:50:49.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:49.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:49.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:49.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:50:49.000000 mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:49.227319 mypy-boto3-globalaccelerator-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-03 19:38:18.000000 mypy-boto3-globalaccelerator-1.27.0/setup.py
```

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/LICENSE` & `mypy-boto3-globalaccelerator-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/PKG-INFO` & `mypy-boto3-globalaccelerator-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-globalaccelerator
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.GlobalAccelerator 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.GlobalAccelerator 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/
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
 
 <a id="mypy-boto3-globalaccelerator"></a>
 
 # mypy-boto3-globalaccelerator
 
 [![PyPI - mypy-boto3-globalaccelerator](https://img.shields.io/pypi/v/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-globalaccelerator?color=blue)](https://pypistats.org/packages/mypy-boto3-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlobalAccelerator 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[boto3.GlobalAccelerator 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
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
 [mypy-boto3-globalaccelerator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,15 +368,14 @@
 ```python
 from mypy_boto3_globalaccelerator.type_defs import (
     AcceleratorAttributesTypeDef,
     AcceleratorEventTypeDef,
     IpSetTypeDef,
     CustomRoutingEndpointConfigurationTypeDef,
     CustomRoutingEndpointDescriptionTypeDef,
-    ResponseMetadataTypeDef,
     EndpointConfigurationTypeDef,
     EndpointDescriptionTypeDef,
     AdvertiseByoipCidrRequestRequestTypeDef,
     AllowCustomRoutingTrafficRequestRequestTypeDef,
     ByoipCidrEventTypeDef,
     CidrAuthorizationContextTypeDef,
     TagTypeDef,
@@ -397,40 +397,49 @@
     DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorRequestRequestTypeDef,
     DescribeCustomRoutingEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingListenerRequestRequestTypeDef,
     DescribeEndpointGroupRequestRequestTypeDef,
     DescribeListenerRequestRequestTypeDef,
     SocketAddressTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointIdentifierTypeDef,
-    PaginatorConfigTypeDef,
+    ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
     ListAcceleratorsRequestRequestTypeDef,
+    ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
     ListByoipCidrsRequestRequestTypeDef,
+    ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
     ListCustomRoutingAcceleratorsRequestRequestTypeDef,
     ListCustomRoutingEndpointGroupsRequestRequestTypeDef,
+    ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
     ListCustomRoutingListenersRequestRequestTypeDef,
+    ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
     ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
+    ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
     ListCustomRoutingPortMappingsRequestRequestTypeDef,
+    ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
     ListEndpointGroupsRequestRequestTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     RemoveCustomRoutingEndpointsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAcceleratorAttributesRequestRequestTypeDef,
     UpdateAcceleratorRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorRequestRequestTypeDef,
     WithdrawByoipCidrRequestRequestTypeDef,
+    DescribeAcceleratorAttributesResponseTypeDef,
+    UpdateAcceleratorAttributesResponseTypeDef,
     AcceleratorTypeDef,
     CustomRoutingAcceleratorTypeDef,
     AddCustomRoutingEndpointsRequestRequestTypeDef,
     AddCustomRoutingEndpointsResponseTypeDef,
-    DescribeAcceleratorAttributesResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    UpdateAcceleratorAttributesResponseTypeDef,
     AddEndpointsRequestRequestTypeDef,
     AddEndpointsResponseTypeDef,
     ByoipCidrTypeDef,
     ProvisionByoipCidrRequestRequestTypeDef,
     CreateAcceleratorRequestRequestTypeDef,
     CreateCustomRoutingAcceleratorRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -447,22 +456,14 @@
     UpdateEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorAttributesResponseTypeDef,
     UpdateCustomRoutingAcceleratorAttributesResponseTypeDef,
     CustomRoutingEndpointGroupTypeDef,
     DestinationPortMappingTypeDef,
     PortMappingTypeDef,
     RemoveEndpointsRequestRequestTypeDef,
-    ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
-    ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
-    ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
-    ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
-    ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
-    ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
-    ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
     CreateAcceleratorResponseTypeDef,
     DescribeAcceleratorResponseTypeDef,
     ListAcceleratorsResponseTypeDef,
     UpdateAcceleratorResponseTypeDef,
     CreateCustomRoutingAcceleratorResponseTypeDef,
     DescribeCustomRoutingAcceleratorResponseTypeDef,
     ListCustomRoutingAcceleratorsResponseTypeDef,
@@ -499,42 +500,42 @@
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

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/README.md` & `mypy-boto3-globalaccelerator-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-globalaccelerator"></a>
 
 # mypy-boto3-globalaccelerator
 
 [![PyPI - mypy-boto3-globalaccelerator](https://img.shields.io/pypi/v/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-globalaccelerator?color=blue)](https://pypistats.org/packages/mypy-boto3-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlobalAccelerator 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[boto3.GlobalAccelerator 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
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
 [mypy-boto3-globalaccelerator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,15 +336,14 @@
 ```python
 from mypy_boto3_globalaccelerator.type_defs import (
     AcceleratorAttributesTypeDef,
     AcceleratorEventTypeDef,
     IpSetTypeDef,
     CustomRoutingEndpointConfigurationTypeDef,
     CustomRoutingEndpointDescriptionTypeDef,
-    ResponseMetadataTypeDef,
     EndpointConfigurationTypeDef,
     EndpointDescriptionTypeDef,
     AdvertiseByoipCidrRequestRequestTypeDef,
     AllowCustomRoutingTrafficRequestRequestTypeDef,
     ByoipCidrEventTypeDef,
     CidrAuthorizationContextTypeDef,
     TagTypeDef,
@@ -366,40 +365,49 @@
     DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorRequestRequestTypeDef,
     DescribeCustomRoutingEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingListenerRequestRequestTypeDef,
     DescribeEndpointGroupRequestRequestTypeDef,
     DescribeListenerRequestRequestTypeDef,
     SocketAddressTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointIdentifierTypeDef,
-    PaginatorConfigTypeDef,
+    ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
     ListAcceleratorsRequestRequestTypeDef,
+    ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
     ListByoipCidrsRequestRequestTypeDef,
+    ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
     ListCustomRoutingAcceleratorsRequestRequestTypeDef,
     ListCustomRoutingEndpointGroupsRequestRequestTypeDef,
+    ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
     ListCustomRoutingListenersRequestRequestTypeDef,
+    ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
     ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
+    ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
     ListCustomRoutingPortMappingsRequestRequestTypeDef,
+    ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
     ListEndpointGroupsRequestRequestTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     RemoveCustomRoutingEndpointsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAcceleratorAttributesRequestRequestTypeDef,
     UpdateAcceleratorRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorRequestRequestTypeDef,
     WithdrawByoipCidrRequestRequestTypeDef,
+    DescribeAcceleratorAttributesResponseTypeDef,
+    UpdateAcceleratorAttributesResponseTypeDef,
     AcceleratorTypeDef,
     CustomRoutingAcceleratorTypeDef,
     AddCustomRoutingEndpointsRequestRequestTypeDef,
     AddCustomRoutingEndpointsResponseTypeDef,
-    DescribeAcceleratorAttributesResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    UpdateAcceleratorAttributesResponseTypeDef,
     AddEndpointsRequestRequestTypeDef,
     AddEndpointsResponseTypeDef,
     ByoipCidrTypeDef,
     ProvisionByoipCidrRequestRequestTypeDef,
     CreateAcceleratorRequestRequestTypeDef,
     CreateCustomRoutingAcceleratorRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -416,22 +424,14 @@
     UpdateEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorAttributesResponseTypeDef,
     UpdateCustomRoutingAcceleratorAttributesResponseTypeDef,
     CustomRoutingEndpointGroupTypeDef,
     DestinationPortMappingTypeDef,
     PortMappingTypeDef,
     RemoveEndpointsRequestRequestTypeDef,
-    ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
-    ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
-    ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
-    ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
-    ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
-    ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
-    ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
     CreateAcceleratorResponseTypeDef,
     DescribeAcceleratorResponseTypeDef,
     ListAcceleratorsResponseTypeDef,
     UpdateAcceleratorResponseTypeDef,
     CreateCustomRoutingAcceleratorResponseTypeDef,
     DescribeCustomRoutingAcceleratorResponseTypeDef,
     ListCustomRoutingAcceleratorsResponseTypeDef,
@@ -468,42 +468,42 @@
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

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/__init__.py` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/__init__.pyi` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/__main__.py` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GlobalAccelerator 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.GlobalAccelerator 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator\nOther"
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

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/client.py` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,15 +484,15 @@
 
     def list_byoip_cidrs(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListByoipCidrsResponseTypeDef:
         """
         Lists the IP address ranges that were specified in calls to
         [ProvisionByoipCidr](https://docs.aws.amazon.com/global-
-        accelerator/latest/api/ProvisionByoipCidr.html)_ , including the current state
+        accelerator/latest/api/ProvisionByoipCidr.html)_, including the current state
         and a history of state changes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.list_byoip_cidrs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/client/#list_byoip_cidrs)
         """
 
     def list_custom_routing_accelerators(
```

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/client.pyi` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
         """
     def list_byoip_cidrs(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListByoipCidrsResponseTypeDef:
         """
         Lists the IP address ranges that were specified in calls to
         [ProvisionByoipCidr](https://docs.aws.amazon.com/global-
-        accelerator/latest/api/ProvisionByoipCidr.html)_ , including the current state
+        accelerator/latest/api/ProvisionByoipCidr.html)_, including the current state
         and a history of state changes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Client.list_byoip_cidrs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/client/#list_byoip_cidrs)
         """
     def list_custom_routing_accelerators(
         self, *, MaxResults: int = ..., NextToken: str = ...
```

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/literals.py` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AcceleratorStatusType",
     "ByoipCidrStateType",
     "ClientAffinityType",
     "CustomRoutingAcceleratorStatusType",
     "CustomRoutingDestinationTrafficStateType",
     "CustomRoutingProtocolType",
@@ -41,15 +40,14 @@
     "ProtocolType",
     "GlobalAcceleratorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AcceleratorStatusType = Literal["DEPLOYED", "IN_PROGRESS"]
 ByoipCidrStateType = Literal[
     "ADVERTISING",
     "DEPROVISIONED",
     "FAILED_ADVERTISING",
     "FAILED_DEPROVISION",
     "FAILED_PROVISION",
@@ -91,23 +89,25 @@
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
@@ -117,30 +117,35 @@
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
@@ -166,14 +171,15 @@
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
@@ -218,51 +224,57 @@
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
@@ -275,14 +287,15 @@
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
@@ -294,28 +307,35 @@
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
@@ -324,14 +344,15 @@
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
@@ -342,55 +363,64 @@
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

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/literals.pyi` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/literals.py`

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
     "AcceleratorStatusType",
     "ByoipCidrStateType",
     "ClientAffinityType",
     "CustomRoutingAcceleratorStatusType",
     "CustomRoutingDestinationTrafficStateType",
     "CustomRoutingProtocolType",
@@ -40,14 +41,15 @@
     "ProtocolType",
     "GlobalAcceleratorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 AcceleratorStatusType = Literal["DEPLOYED", "IN_PROGRESS"]
 ByoipCidrStateType = Literal[
     "ADVERTISING",
     "DEPROVISIONED",
     "FAILED_ADVERTISING",
     "FAILED_DEPROVISION",
     "FAILED_PROVISION",
@@ -89,23 +91,25 @@
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
@@ -115,30 +119,35 @@
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
@@ -164,14 +173,15 @@
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
@@ -216,51 +226,57 @@
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
@@ -273,14 +289,15 @@
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
@@ -292,28 +309,35 @@
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
@@ -322,14 +346,15 @@
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
@@ -340,55 +365,64 @@
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

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/paginator.py` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -56,144 +56,134 @@
     "ListCustomRoutingListenersPaginator",
     "ListCustomRoutingPortMappingsPaginator",
     "ListCustomRoutingPortMappingsByDestinationPaginator",
     "ListEndpointGroupsPaginator",
     "ListListenersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAcceleratorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListAccelerators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listacceleratorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListAccelerators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listacceleratorspaginator)
         """
 
-
 class ListByoipCidrsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListByoipCidrs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listbyoipcidrspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListByoipCidrsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListByoipCidrs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listbyoipcidrspaginator)
         """
 
-
 class ListCustomRoutingAcceleratorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingAccelerators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingacceleratorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomRoutingAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingAccelerators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingacceleratorspaginator)
         """
 
-
 class ListCustomRoutingListenersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingListeners)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutinglistenerspaginator)
     """
 
     def paginate(
-        self, *, AcceleratorArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AcceleratorArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomRoutingListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutinglistenerspaginator)
         """
 
-
 class ListCustomRoutingPortMappingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingportmappingspaginator)
     """
 
     def paginate(
         self,
         *,
         AcceleratorArn: str,
         EndpointGroupArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomRoutingPortMappingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingportmappingspaginator)
         """
 
-
 class ListCustomRoutingPortMappingsByDestinationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappingsByDestination)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingportmappingsbydestinationpaginator)
     """
 
     def paginate(
         self,
         *,
         EndpointId: str,
         DestinationAddress: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomRoutingPortMappingsByDestinationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappingsByDestination.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingportmappingsbydestinationpaginator)
         """
 
-
 class ListEndpointGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListEndpointGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listendpointgroupspaginator)
     """
 
     def paginate(
-        self, *, ListenerArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ListenerArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEndpointGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListEndpointGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listendpointgroupspaginator)
         """
 
-
 class ListListenersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListListeners)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listlistenerspaginator)
     """
 
     def paginate(
-        self, *, AcceleratorArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AcceleratorArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listlistenerspaginator)
         """
```

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/paginator.pyi` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,134 +56,144 @@
     "ListCustomRoutingListenersPaginator",
     "ListCustomRoutingPortMappingsPaginator",
     "ListCustomRoutingPortMappingsByDestinationPaginator",
     "ListEndpointGroupsPaginator",
     "ListListenersPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAcceleratorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListAccelerators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listacceleratorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListAccelerators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listacceleratorspaginator)
         """
 
+
 class ListByoipCidrsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListByoipCidrs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listbyoipcidrspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListByoipCidrsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListByoipCidrs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listbyoipcidrspaginator)
         """
 
+
 class ListCustomRoutingAcceleratorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingAccelerators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingacceleratorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomRoutingAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingAccelerators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingacceleratorspaginator)
         """
 
+
 class ListCustomRoutingListenersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingListeners)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutinglistenerspaginator)
     """
 
     def paginate(
-        self, *, AcceleratorArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AcceleratorArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomRoutingListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutinglistenerspaginator)
         """
 
+
 class ListCustomRoutingPortMappingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingportmappingspaginator)
     """
 
     def paginate(
         self,
         *,
         AcceleratorArn: str,
         EndpointGroupArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomRoutingPortMappingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingportmappingspaginator)
         """
 
+
 class ListCustomRoutingPortMappingsByDestinationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappingsByDestination)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingportmappingsbydestinationpaginator)
     """
 
     def paginate(
         self,
         *,
         EndpointId: str,
         DestinationAddress: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomRoutingPortMappingsByDestinationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappingsByDestination.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingportmappingsbydestinationpaginator)
         """
 
+
 class ListEndpointGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListEndpointGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listendpointgroupspaginator)
     """
 
     def paginate(
-        self, *, ListenerArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ListenerArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEndpointGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListEndpointGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listendpointgroupspaginator)
         """
 
+
 class ListListenersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListListeners)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listlistenerspaginator)
     """
 
     def paginate(
-        self, *, AcceleratorArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AcceleratorArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listlistenerspaginator)
         """
```

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/type_defs.py` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
 __all__ = (
     "AcceleratorAttributesTypeDef",
     "AcceleratorEventTypeDef",
     "IpSetTypeDef",
     "CustomRoutingEndpointConfigurationTypeDef",
     "CustomRoutingEndpointDescriptionTypeDef",
-    "ResponseMetadataTypeDef",
     "EndpointConfigurationTypeDef",
     "EndpointDescriptionTypeDef",
     "AdvertiseByoipCidrRequestRequestTypeDef",
     "AllowCustomRoutingTrafficRequestRequestTypeDef",
     "ByoipCidrEventTypeDef",
     "CidrAuthorizationContextTypeDef",
     "TagTypeDef",
@@ -67,40 +66,49 @@
     "DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef",
     "DescribeCustomRoutingAcceleratorRequestRequestTypeDef",
     "DescribeCustomRoutingEndpointGroupRequestRequestTypeDef",
     "DescribeCustomRoutingListenerRequestRequestTypeDef",
     "DescribeEndpointGroupRequestRequestTypeDef",
     "DescribeListenerRequestRequestTypeDef",
     "SocketAddressTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EndpointIdentifierTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
     "ListAcceleratorsRequestRequestTypeDef",
+    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
     "ListByoipCidrsRequestRequestTypeDef",
+    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
     "ListCustomRoutingAcceleratorsRequestRequestTypeDef",
     "ListCustomRoutingEndpointGroupsRequestRequestTypeDef",
+    "ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
     "ListCustomRoutingListenersRequestRequestTypeDef",
+    "ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
     "ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef",
+    "ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
     "ListCustomRoutingPortMappingsRequestRequestTypeDef",
+    "ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
     "ListEndpointGroupsRequestRequestTypeDef",
+    "ListListenersRequestListListenersPaginateTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "RemoveCustomRoutingEndpointsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAcceleratorAttributesRequestRequestTypeDef",
     "UpdateAcceleratorRequestRequestTypeDef",
     "UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef",
     "UpdateCustomRoutingAcceleratorRequestRequestTypeDef",
     "WithdrawByoipCidrRequestRequestTypeDef",
+    "DescribeAcceleratorAttributesResponseTypeDef",
+    "UpdateAcceleratorAttributesResponseTypeDef",
     "AcceleratorTypeDef",
     "CustomRoutingAcceleratorTypeDef",
     "AddCustomRoutingEndpointsRequestRequestTypeDef",
     "AddCustomRoutingEndpointsResponseTypeDef",
-    "DescribeAcceleratorAttributesResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "UpdateAcceleratorAttributesResponseTypeDef",
     "AddEndpointsRequestRequestTypeDef",
     "AddEndpointsResponseTypeDef",
     "ByoipCidrTypeDef",
     "ProvisionByoipCidrRequestRequestTypeDef",
     "CreateAcceleratorRequestRequestTypeDef",
     "CreateCustomRoutingAcceleratorRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
@@ -117,22 +125,14 @@
     "UpdateEndpointGroupRequestRequestTypeDef",
     "DescribeCustomRoutingAcceleratorAttributesResponseTypeDef",
     "UpdateCustomRoutingAcceleratorAttributesResponseTypeDef",
     "CustomRoutingEndpointGroupTypeDef",
     "DestinationPortMappingTypeDef",
     "PortMappingTypeDef",
     "RemoveEndpointsRequestRequestTypeDef",
-    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
-    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
-    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
-    "ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
-    "ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
-    "ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
-    "ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
-    "ListListenersRequestListListenersPaginateTypeDef",
     "CreateAcceleratorResponseTypeDef",
     "DescribeAcceleratorResponseTypeDef",
     "ListAcceleratorsResponseTypeDef",
     "UpdateAcceleratorResponseTypeDef",
     "CreateCustomRoutingAcceleratorResponseTypeDef",
     "DescribeCustomRoutingAcceleratorResponseTypeDef",
     "ListCustomRoutingAcceleratorsResponseTypeDef",
@@ -202,25 +202,14 @@
     "CustomRoutingEndpointDescriptionTypeDef",
     {
         "EndpointId": str,
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
 EndpointConfigurationTypeDef = TypedDict(
     "EndpointConfigurationTypeDef",
     {
         "EndpointId": str,
         "Weight": int,
         "ClientIPPreservationEnabled": bool,
     },
@@ -478,14 +467,21 @@
     {
         "IpAddress": str,
         "Port": int,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEndpointIdentifierTypeDef = TypedDict(
     "_RequiredEndpointIdentifierTypeDef",
     {
         "EndpointId": str,
     },
 )
 _OptionalEndpointIdentifierTypeDef = TypedDict(
@@ -499,42 +495,56 @@
 
 class EndpointIdentifierTypeDef(
     _RequiredEndpointIdentifierTypeDef, _OptionalEndpointIdentifierTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAcceleratorsRequestListAcceleratorsPaginateTypeDef = TypedDict(
+    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAcceleratorsRequestRequestTypeDef = TypedDict(
     "ListAcceleratorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListByoipCidrsRequestListByoipCidrsPaginateTypeDef = TypedDict(
+    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListByoipCidrsRequestRequestTypeDef = TypedDict(
     "ListByoipCidrsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef = TypedDict(
+    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCustomRoutingAcceleratorsRequestRequestTypeDef = TypedDict(
     "ListCustomRoutingAcceleratorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -559,14 +569,36 @@
 class ListCustomRoutingEndpointGroupsRequestRequestTypeDef(
     _RequiredListCustomRoutingEndpointGroupsRequestRequestTypeDef,
     _OptionalListCustomRoutingEndpointGroupsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
+    "_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
+    {
+        "AcceleratorArn": str,
+    },
+)
+_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
+    "_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef(
+    _RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
+    _OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListCustomRoutingListenersRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomRoutingListenersRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 _OptionalListCustomRoutingListenersRequestRequestTypeDef = TypedDict(
@@ -582,14 +614,37 @@
 class ListCustomRoutingListenersRequestRequestTypeDef(
     _RequiredListCustomRoutingListenersRequestRequestTypeDef,
     _OptionalListCustomRoutingListenersRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
+    "_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
+    {
+        "EndpointId": str,
+        "DestinationAddress": str,
+    },
+)
+_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
+    "_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef(
+    _RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
+    _OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef",
     {
         "EndpointId": str,
         "DestinationAddress": str,
     },
 )
@@ -606,14 +661,41 @@
 class ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef(
     _RequiredListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
     _OptionalListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
+        {
+            "AcceleratorArn": str,
+        },
+    )
+)
+_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
+        {
+            "EndpointGroupArn": str,
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
+
+class ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef(
+    _RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
+    _OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListCustomRoutingPortMappingsRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomRoutingPortMappingsRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 _OptionalListCustomRoutingPortMappingsRequestRequestTypeDef = TypedDict(
@@ -630,14 +712,36 @@
 class ListCustomRoutingPortMappingsRequestRequestTypeDef(
     _RequiredListCustomRoutingPortMappingsRequestRequestTypeDef,
     _OptionalListCustomRoutingPortMappingsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
+    {
+        "ListenerArn": str,
+    },
+)
+_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef(
+    _RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
+    _OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEndpointGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListEndpointGroupsRequestRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalListEndpointGroupsRequestRequestTypeDef = TypedDict(
@@ -653,14 +757,36 @@
 class ListEndpointGroupsRequestRequestTypeDef(
     _RequiredListEndpointGroupsRequestRequestTypeDef,
     _OptionalListEndpointGroupsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_RequiredListListenersRequestListListenersPaginateTypeDef",
+    {
+        "AcceleratorArn": str,
+    },
+)
+_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_OptionalListListenersRequestListListenersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListListenersRequestListListenersPaginateTypeDef(
+    _RequiredListListenersRequestListListenersPaginateTypeDef,
+    _OptionalListListenersRequestListListenersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListListenersRequestRequestTypeDef = TypedDict(
     "_RequiredListListenersRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 _OptionalListListenersRequestRequestTypeDef = TypedDict(
@@ -682,22 +808,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 RemoveCustomRoutingEndpointsRequestRequestTypeDef = TypedDict(
     "RemoveCustomRoutingEndpointsRequestRequestTypeDef",
     {
         "EndpointIds": Sequence[str],
         "EndpointGroupArn": str,
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
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -800,14 +947,30 @@
 WithdrawByoipCidrRequestRequestTypeDef = TypedDict(
     "WithdrawByoipCidrRequestRequestTypeDef",
     {
         "Cidr": str,
     },
 )
 
+DescribeAcceleratorAttributesResponseTypeDef = TypedDict(
+    "DescribeAcceleratorAttributesResponseTypeDef",
+    {
+        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAcceleratorAttributesResponseTypeDef = TypedDict(
+    "UpdateAcceleratorAttributesResponseTypeDef",
+    {
+        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AcceleratorTypeDef = TypedDict(
     "AcceleratorTypeDef",
     {
         "AcceleratorArn": str,
         "Name": str,
         "IpAddressType": IpAddressTypeType,
         "Enabled": bool,
@@ -847,38 +1010,15 @@
 )
 
 AddCustomRoutingEndpointsResponseTypeDef = TypedDict(
     "AddCustomRoutingEndpointsResponseTypeDef",
     {
         "EndpointDescriptions": List[CustomRoutingEndpointDescriptionTypeDef],
         "EndpointGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAcceleratorAttributesResponseTypeDef = TypedDict(
-    "DescribeAcceleratorAttributesResponseTypeDef",
-    {
-        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
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
-UpdateAcceleratorAttributesResponseTypeDef = TypedDict(
-    "UpdateAcceleratorAttributesResponseTypeDef",
-    {
-        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddEndpointsRequestRequestTypeDef = TypedDict(
     "AddEndpointsRequestRequestTypeDef",
     {
         "EndpointConfigurations": Sequence[EndpointConfigurationTypeDef],
@@ -887,15 +1027,15 @@
 )
 
 AddEndpointsResponseTypeDef = TypedDict(
     "AddEndpointsResponseTypeDef",
     {
         "EndpointDescriptions": List[EndpointDescriptionTypeDef],
         "EndpointGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ByoipCidrTypeDef = TypedDict(
     "ByoipCidrTypeDef",
     {
         "Cidr": str,
@@ -964,15 +1104,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1151,23 +1291,23 @@
     pass
 
 
 DescribeCustomRoutingAcceleratorAttributesResponseTypeDef = TypedDict(
     "DescribeCustomRoutingAcceleratorAttributesResponseTypeDef",
     {
         "AcceleratorAttributes": CustomRoutingAcceleratorAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCustomRoutingAcceleratorAttributesResponseTypeDef = TypedDict(
     "UpdateCustomRoutingAcceleratorAttributesResponseTypeDef",
     {
         "AcceleratorAttributes": CustomRoutingAcceleratorAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CustomRoutingEndpointGroupTypeDef = TypedDict(
     "CustomRoutingEndpointGroupTypeDef",
     {
         "EndpointGroupArn": str,
@@ -1210,395 +1350,255 @@
     "RemoveEndpointsRequestRequestTypeDef",
     {
         "EndpointIdentifiers": Sequence[EndpointIdentifierTypeDef],
         "EndpointGroupArn": str,
     },
 )
 
-ListAcceleratorsRequestListAcceleratorsPaginateTypeDef = TypedDict(
-    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListByoipCidrsRequestListByoipCidrsPaginateTypeDef = TypedDict(
-    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef = TypedDict(
-    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
-    "_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
-    {
-        "AcceleratorArn": str,
-    },
-)
-_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
-    "_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef(
-    _RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
-    _OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
-    "_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
-    {
-        "EndpointId": str,
-        "DestinationAddress": str,
-    },
-)
-_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
-    "_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef(
-    _RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
-    _OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
-        {
-            "AcceleratorArn": str,
-        },
-    )
-)
-_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
-        {
-            "EndpointGroupArn": str,
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-
-class ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef(
-    _RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
-    _OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
-    {
-        "ListenerArn": str,
-    },
-)
-_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef(
-    _RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
-    _OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_RequiredListListenersRequestListListenersPaginateTypeDef",
-    {
-        "AcceleratorArn": str,
-    },
-)
-_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_OptionalListListenersRequestListListenersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListListenersRequestListListenersPaginateTypeDef(
-    _RequiredListListenersRequestListListenersPaginateTypeDef,
-    _OptionalListListenersRequestListListenersPaginateTypeDef,
-):
-    pass
-
-
 CreateAcceleratorResponseTypeDef = TypedDict(
     "CreateAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAcceleratorResponseTypeDef = TypedDict(
     "DescribeAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAcceleratorsResponseTypeDef = TypedDict(
     "ListAcceleratorsResponseTypeDef",
     {
         "Accelerators": List[AcceleratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAcceleratorResponseTypeDef = TypedDict(
     "UpdateAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCustomRoutingAcceleratorResponseTypeDef = TypedDict(
     "CreateCustomRoutingAcceleratorResponseTypeDef",
     {
         "Accelerator": CustomRoutingAcceleratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCustomRoutingAcceleratorResponseTypeDef = TypedDict(
     "DescribeCustomRoutingAcceleratorResponseTypeDef",
     {
         "Accelerator": CustomRoutingAcceleratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomRoutingAcceleratorsResponseTypeDef = TypedDict(
     "ListCustomRoutingAcceleratorsResponseTypeDef",
     {
         "Accelerators": List[CustomRoutingAcceleratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCustomRoutingAcceleratorResponseTypeDef = TypedDict(
     "UpdateCustomRoutingAcceleratorResponseTypeDef",
     {
         "Accelerator": CustomRoutingAcceleratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdvertiseByoipCidrResponseTypeDef = TypedDict(
     "AdvertiseByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeprovisionByoipCidrResponseTypeDef = TypedDict(
     "DeprovisionByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListByoipCidrsResponseTypeDef = TypedDict(
     "ListByoipCidrsResponseTypeDef",
     {
         "ByoipCidrs": List[ByoipCidrTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProvisionByoipCidrResponseTypeDef = TypedDict(
     "ProvisionByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WithdrawByoipCidrResponseTypeDef = TypedDict(
     "WithdrawByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCustomRoutingListenerResponseTypeDef = TypedDict(
     "CreateCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCustomRoutingListenerResponseTypeDef = TypedDict(
     "DescribeCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomRoutingListenersResponseTypeDef = TypedDict(
     "ListCustomRoutingListenersResponseTypeDef",
     {
         "Listeners": List[CustomRoutingListenerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCustomRoutingListenerResponseTypeDef = TypedDict(
     "UpdateCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateListenerResponseTypeDef = TypedDict(
     "CreateListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeListenerResponseTypeDef = TypedDict(
     "DescribeListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListListenersResponseTypeDef = TypedDict(
     "ListListenersResponseTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateListenerResponseTypeDef = TypedDict(
     "UpdateListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEndpointGroupResponseTypeDef = TypedDict(
     "CreateEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointGroupResponseTypeDef = TypedDict(
     "DescribeEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEndpointGroupsResponseTypeDef = TypedDict(
     "ListEndpointGroupsResponseTypeDef",
     {
         "EndpointGroups": List[EndpointGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointGroupResponseTypeDef = TypedDict(
     "UpdateEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
     "CreateCustomRoutingEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
     "DescribeCustomRoutingEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomRoutingEndpointGroupsResponseTypeDef = TypedDict(
     "ListCustomRoutingEndpointGroupsResponseTypeDef",
     {
         "EndpointGroups": List[CustomRoutingEndpointGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomRoutingPortMappingsByDestinationResponseTypeDef = TypedDict(
     "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
     {
         "DestinationPortMappings": List[DestinationPortMappingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomRoutingPortMappingsResponseTypeDef = TypedDict(
     "ListCustomRoutingPortMappingsResponseTypeDef",
     {
         "PortMappings": List[PortMappingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator/type_defs.pyi` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 
 __all__ = (
     "AcceleratorAttributesTypeDef",
     "AcceleratorEventTypeDef",
     "IpSetTypeDef",
     "CustomRoutingEndpointConfigurationTypeDef",
     "CustomRoutingEndpointDescriptionTypeDef",
-    "ResponseMetadataTypeDef",
     "EndpointConfigurationTypeDef",
     "EndpointDescriptionTypeDef",
     "AdvertiseByoipCidrRequestRequestTypeDef",
     "AllowCustomRoutingTrafficRequestRequestTypeDef",
     "ByoipCidrEventTypeDef",
     "CidrAuthorizationContextTypeDef",
     "TagTypeDef",
@@ -66,40 +65,49 @@
     "DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef",
     "DescribeCustomRoutingAcceleratorRequestRequestTypeDef",
     "DescribeCustomRoutingEndpointGroupRequestRequestTypeDef",
     "DescribeCustomRoutingListenerRequestRequestTypeDef",
     "DescribeEndpointGroupRequestRequestTypeDef",
     "DescribeListenerRequestRequestTypeDef",
     "SocketAddressTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EndpointIdentifierTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
     "ListAcceleratorsRequestRequestTypeDef",
+    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
     "ListByoipCidrsRequestRequestTypeDef",
+    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
     "ListCustomRoutingAcceleratorsRequestRequestTypeDef",
     "ListCustomRoutingEndpointGroupsRequestRequestTypeDef",
+    "ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
     "ListCustomRoutingListenersRequestRequestTypeDef",
+    "ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
     "ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef",
+    "ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
     "ListCustomRoutingPortMappingsRequestRequestTypeDef",
+    "ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
     "ListEndpointGroupsRequestRequestTypeDef",
+    "ListListenersRequestListListenersPaginateTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "RemoveCustomRoutingEndpointsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAcceleratorAttributesRequestRequestTypeDef",
     "UpdateAcceleratorRequestRequestTypeDef",
     "UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef",
     "UpdateCustomRoutingAcceleratorRequestRequestTypeDef",
     "WithdrawByoipCidrRequestRequestTypeDef",
+    "DescribeAcceleratorAttributesResponseTypeDef",
+    "UpdateAcceleratorAttributesResponseTypeDef",
     "AcceleratorTypeDef",
     "CustomRoutingAcceleratorTypeDef",
     "AddCustomRoutingEndpointsRequestRequestTypeDef",
     "AddCustomRoutingEndpointsResponseTypeDef",
-    "DescribeAcceleratorAttributesResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "UpdateAcceleratorAttributesResponseTypeDef",
     "AddEndpointsRequestRequestTypeDef",
     "AddEndpointsResponseTypeDef",
     "ByoipCidrTypeDef",
     "ProvisionByoipCidrRequestRequestTypeDef",
     "CreateAcceleratorRequestRequestTypeDef",
     "CreateCustomRoutingAcceleratorRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
@@ -116,22 +124,14 @@
     "UpdateEndpointGroupRequestRequestTypeDef",
     "DescribeCustomRoutingAcceleratorAttributesResponseTypeDef",
     "UpdateCustomRoutingAcceleratorAttributesResponseTypeDef",
     "CustomRoutingEndpointGroupTypeDef",
     "DestinationPortMappingTypeDef",
     "PortMappingTypeDef",
     "RemoveEndpointsRequestRequestTypeDef",
-    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
-    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
-    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
-    "ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
-    "ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
-    "ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
-    "ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
-    "ListListenersRequestListListenersPaginateTypeDef",
     "CreateAcceleratorResponseTypeDef",
     "DescribeAcceleratorResponseTypeDef",
     "ListAcceleratorsResponseTypeDef",
     "UpdateAcceleratorResponseTypeDef",
     "CreateCustomRoutingAcceleratorResponseTypeDef",
     "DescribeCustomRoutingAcceleratorResponseTypeDef",
     "ListCustomRoutingAcceleratorsResponseTypeDef",
@@ -201,25 +201,14 @@
     "CustomRoutingEndpointDescriptionTypeDef",
     {
         "EndpointId": str,
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
 EndpointConfigurationTypeDef = TypedDict(
     "EndpointConfigurationTypeDef",
     {
         "EndpointId": str,
         "Weight": int,
         "ClientIPPreservationEnabled": bool,
     },
@@ -473,14 +462,21 @@
     {
         "IpAddress": str,
         "Port": int,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEndpointIdentifierTypeDef = TypedDict(
     "_RequiredEndpointIdentifierTypeDef",
     {
         "EndpointId": str,
     },
 )
 _OptionalEndpointIdentifierTypeDef = TypedDict(
@@ -492,42 +488,56 @@
 )
 
 class EndpointIdentifierTypeDef(
     _RequiredEndpointIdentifierTypeDef, _OptionalEndpointIdentifierTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAcceleratorsRequestListAcceleratorsPaginateTypeDef = TypedDict(
+    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAcceleratorsRequestRequestTypeDef = TypedDict(
     "ListAcceleratorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListByoipCidrsRequestListByoipCidrsPaginateTypeDef = TypedDict(
+    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListByoipCidrsRequestRequestTypeDef = TypedDict(
     "ListByoipCidrsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef = TypedDict(
+    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCustomRoutingAcceleratorsRequestRequestTypeDef = TypedDict(
     "ListCustomRoutingAcceleratorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -550,14 +560,34 @@
 
 class ListCustomRoutingEndpointGroupsRequestRequestTypeDef(
     _RequiredListCustomRoutingEndpointGroupsRequestRequestTypeDef,
     _OptionalListCustomRoutingEndpointGroupsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
+    "_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
+    {
+        "AcceleratorArn": str,
+    },
+)
+_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
+    "_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef(
+    _RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
+    _OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
+):
+    pass
+
 _RequiredListCustomRoutingListenersRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomRoutingListenersRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 _OptionalListCustomRoutingListenersRequestRequestTypeDef = TypedDict(
@@ -571,14 +601,35 @@
 
 class ListCustomRoutingListenersRequestRequestTypeDef(
     _RequiredListCustomRoutingListenersRequestRequestTypeDef,
     _OptionalListCustomRoutingListenersRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
+    "_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
+    {
+        "EndpointId": str,
+        "DestinationAddress": str,
+    },
+)
+_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
+    "_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef(
+    _RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
+    _OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
+):
+    pass
+
 _RequiredListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef",
     {
         "EndpointId": str,
         "DestinationAddress": str,
     },
 )
@@ -593,14 +644,39 @@
 
 class ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef(
     _RequiredListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
     _OptionalListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
+        {
+            "AcceleratorArn": str,
+        },
+    )
+)
+_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
+        {
+            "EndpointGroupArn": str,
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
+class ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef(
+    _RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
+    _OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
+):
+    pass
+
 _RequiredListCustomRoutingPortMappingsRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomRoutingPortMappingsRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 _OptionalListCustomRoutingPortMappingsRequestRequestTypeDef = TypedDict(
@@ -615,14 +691,34 @@
 
 class ListCustomRoutingPortMappingsRequestRequestTypeDef(
     _RequiredListCustomRoutingPortMappingsRequestRequestTypeDef,
     _OptionalListCustomRoutingPortMappingsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
+    {
+        "ListenerArn": str,
+    },
+)
+_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef(
+    _RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
+    _OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
+):
+    pass
+
 _RequiredListEndpointGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListEndpointGroupsRequestRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalListEndpointGroupsRequestRequestTypeDef = TypedDict(
@@ -636,14 +732,34 @@
 
 class ListEndpointGroupsRequestRequestTypeDef(
     _RequiredListEndpointGroupsRequestRequestTypeDef,
     _OptionalListEndpointGroupsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_RequiredListListenersRequestListListenersPaginateTypeDef",
+    {
+        "AcceleratorArn": str,
+    },
+)
+_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_OptionalListListenersRequestListListenersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListListenersRequestListListenersPaginateTypeDef(
+    _RequiredListListenersRequestListListenersPaginateTypeDef,
+    _OptionalListListenersRequestListListenersPaginateTypeDef,
+):
+    pass
+
 _RequiredListListenersRequestRequestTypeDef = TypedDict(
     "_RequiredListListenersRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 _OptionalListListenersRequestRequestTypeDef = TypedDict(
@@ -663,22 +779,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 RemoveCustomRoutingEndpointsRequestRequestTypeDef = TypedDict(
     "RemoveCustomRoutingEndpointsRequestRequestTypeDef",
     {
         "EndpointIds": Sequence[str],
         "EndpointGroupArn": str,
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
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -773,14 +910,30 @@
 WithdrawByoipCidrRequestRequestTypeDef = TypedDict(
     "WithdrawByoipCidrRequestRequestTypeDef",
     {
         "Cidr": str,
     },
 )
 
+DescribeAcceleratorAttributesResponseTypeDef = TypedDict(
+    "DescribeAcceleratorAttributesResponseTypeDef",
+    {
+        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAcceleratorAttributesResponseTypeDef = TypedDict(
+    "UpdateAcceleratorAttributesResponseTypeDef",
+    {
+        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AcceleratorTypeDef = TypedDict(
     "AcceleratorTypeDef",
     {
         "AcceleratorArn": str,
         "Name": str,
         "IpAddressType": IpAddressTypeType,
         "Enabled": bool,
@@ -820,38 +973,15 @@
 )
 
 AddCustomRoutingEndpointsResponseTypeDef = TypedDict(
     "AddCustomRoutingEndpointsResponseTypeDef",
     {
         "EndpointDescriptions": List[CustomRoutingEndpointDescriptionTypeDef],
         "EndpointGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAcceleratorAttributesResponseTypeDef = TypedDict(
-    "DescribeAcceleratorAttributesResponseTypeDef",
-    {
-        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
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
-UpdateAcceleratorAttributesResponseTypeDef = TypedDict(
-    "UpdateAcceleratorAttributesResponseTypeDef",
-    {
-        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddEndpointsRequestRequestTypeDef = TypedDict(
     "AddEndpointsRequestRequestTypeDef",
     {
         "EndpointConfigurations": Sequence[EndpointConfigurationTypeDef],
@@ -860,15 +990,15 @@
 )
 
 AddEndpointsResponseTypeDef = TypedDict(
     "AddEndpointsResponseTypeDef",
     {
         "EndpointDescriptions": List[EndpointDescriptionTypeDef],
         "EndpointGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ByoipCidrTypeDef = TypedDict(
     "ByoipCidrTypeDef",
     {
         "Cidr": str,
@@ -933,15 +1063,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1112,23 +1242,23 @@
 ):
     pass
 
 DescribeCustomRoutingAcceleratorAttributesResponseTypeDef = TypedDict(
     "DescribeCustomRoutingAcceleratorAttributesResponseTypeDef",
     {
         "AcceleratorAttributes": CustomRoutingAcceleratorAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCustomRoutingAcceleratorAttributesResponseTypeDef = TypedDict(
     "UpdateCustomRoutingAcceleratorAttributesResponseTypeDef",
     {
         "AcceleratorAttributes": CustomRoutingAcceleratorAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CustomRoutingEndpointGroupTypeDef = TypedDict(
     "CustomRoutingEndpointGroupTypeDef",
     {
         "EndpointGroupArn": str,
@@ -1171,385 +1301,255 @@
     "RemoveEndpointsRequestRequestTypeDef",
     {
         "EndpointIdentifiers": Sequence[EndpointIdentifierTypeDef],
         "EndpointGroupArn": str,
     },
 )
 
-ListAcceleratorsRequestListAcceleratorsPaginateTypeDef = TypedDict(
-    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListByoipCidrsRequestListByoipCidrsPaginateTypeDef = TypedDict(
-    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef = TypedDict(
-    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
-    "_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
-    {
-        "AcceleratorArn": str,
-    },
-)
-_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
-    "_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef(
-    _RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
-    _OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
-):
-    pass
-
-_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
-    "_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
-    {
-        "EndpointId": str,
-        "DestinationAddress": str,
-    },
-)
-_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
-    "_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef(
-    _RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
-    _OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
-):
-    pass
-
-_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
-        {
-            "AcceleratorArn": str,
-        },
-    )
-)
-_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
-        {
-            "EndpointGroupArn": str,
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-class ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef(
-    _RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
-    _OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
-):
-    pass
-
-_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
-    {
-        "ListenerArn": str,
-    },
-)
-_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef(
-    _RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
-    _OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
-):
-    pass
-
-_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_RequiredListListenersRequestListListenersPaginateTypeDef",
-    {
-        "AcceleratorArn": str,
-    },
-)
-_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_OptionalListListenersRequestListListenersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListListenersRequestListListenersPaginateTypeDef(
-    _RequiredListListenersRequestListListenersPaginateTypeDef,
-    _OptionalListListenersRequestListListenersPaginateTypeDef,
-):
-    pass
-
 CreateAcceleratorResponseTypeDef = TypedDict(
     "CreateAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAcceleratorResponseTypeDef = TypedDict(
     "DescribeAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAcceleratorsResponseTypeDef = TypedDict(
     "ListAcceleratorsResponseTypeDef",
     {
         "Accelerators": List[AcceleratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAcceleratorResponseTypeDef = TypedDict(
     "UpdateAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCustomRoutingAcceleratorResponseTypeDef = TypedDict(
     "CreateCustomRoutingAcceleratorResponseTypeDef",
     {
         "Accelerator": CustomRoutingAcceleratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCustomRoutingAcceleratorResponseTypeDef = TypedDict(
     "DescribeCustomRoutingAcceleratorResponseTypeDef",
     {
         "Accelerator": CustomRoutingAcceleratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomRoutingAcceleratorsResponseTypeDef = TypedDict(
     "ListCustomRoutingAcceleratorsResponseTypeDef",
     {
         "Accelerators": List[CustomRoutingAcceleratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCustomRoutingAcceleratorResponseTypeDef = TypedDict(
     "UpdateCustomRoutingAcceleratorResponseTypeDef",
     {
         "Accelerator": CustomRoutingAcceleratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdvertiseByoipCidrResponseTypeDef = TypedDict(
     "AdvertiseByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeprovisionByoipCidrResponseTypeDef = TypedDict(
     "DeprovisionByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListByoipCidrsResponseTypeDef = TypedDict(
     "ListByoipCidrsResponseTypeDef",
     {
         "ByoipCidrs": List[ByoipCidrTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProvisionByoipCidrResponseTypeDef = TypedDict(
     "ProvisionByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WithdrawByoipCidrResponseTypeDef = TypedDict(
     "WithdrawByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCustomRoutingListenerResponseTypeDef = TypedDict(
     "CreateCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCustomRoutingListenerResponseTypeDef = TypedDict(
     "DescribeCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomRoutingListenersResponseTypeDef = TypedDict(
     "ListCustomRoutingListenersResponseTypeDef",
     {
         "Listeners": List[CustomRoutingListenerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCustomRoutingListenerResponseTypeDef = TypedDict(
     "UpdateCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateListenerResponseTypeDef = TypedDict(
     "CreateListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeListenerResponseTypeDef = TypedDict(
     "DescribeListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListListenersResponseTypeDef = TypedDict(
     "ListListenersResponseTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateListenerResponseTypeDef = TypedDict(
     "UpdateListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEndpointGroupResponseTypeDef = TypedDict(
     "CreateEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointGroupResponseTypeDef = TypedDict(
     "DescribeEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEndpointGroupsResponseTypeDef = TypedDict(
     "ListEndpointGroupsResponseTypeDef",
     {
         "EndpointGroups": List[EndpointGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointGroupResponseTypeDef = TypedDict(
     "UpdateEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
     "CreateCustomRoutingEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
     "DescribeCustomRoutingEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomRoutingEndpointGroupsResponseTypeDef = TypedDict(
     "ListCustomRoutingEndpointGroupsResponseTypeDef",
     {
         "EndpointGroups": List[CustomRoutingEndpointGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomRoutingPortMappingsByDestinationResponseTypeDef = TypedDict(
     "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
     {
         "DestinationPortMappings": List[DestinationPortMappingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomRoutingPortMappingsResponseTypeDef = TypedDict(
     "ListCustomRoutingPortMappingsResponseTypeDef",
     {
         "PortMappings": List[PortMappingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator.egg-info/PKG-INFO` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-globalaccelerator
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.GlobalAccelerator 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.GlobalAccelerator 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/
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
 
 <a id="mypy-boto3-globalaccelerator"></a>
 
 # mypy-boto3-globalaccelerator
 
 [![PyPI - mypy-boto3-globalaccelerator](https://img.shields.io/pypi/v/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-globalaccelerator?color=blue)](https://pypistats.org/packages/mypy-boto3-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlobalAccelerator 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[boto3.GlobalAccelerator 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
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
 [mypy-boto3-globalaccelerator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,15 +368,14 @@
 ```python
 from mypy_boto3_globalaccelerator.type_defs import (
     AcceleratorAttributesTypeDef,
     AcceleratorEventTypeDef,
     IpSetTypeDef,
     CustomRoutingEndpointConfigurationTypeDef,
     CustomRoutingEndpointDescriptionTypeDef,
-    ResponseMetadataTypeDef,
     EndpointConfigurationTypeDef,
     EndpointDescriptionTypeDef,
     AdvertiseByoipCidrRequestRequestTypeDef,
     AllowCustomRoutingTrafficRequestRequestTypeDef,
     ByoipCidrEventTypeDef,
     CidrAuthorizationContextTypeDef,
     TagTypeDef,
@@ -397,40 +397,49 @@
     DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorRequestRequestTypeDef,
     DescribeCustomRoutingEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingListenerRequestRequestTypeDef,
     DescribeEndpointGroupRequestRequestTypeDef,
     DescribeListenerRequestRequestTypeDef,
     SocketAddressTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointIdentifierTypeDef,
-    PaginatorConfigTypeDef,
+    ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
     ListAcceleratorsRequestRequestTypeDef,
+    ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
     ListByoipCidrsRequestRequestTypeDef,
+    ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
     ListCustomRoutingAcceleratorsRequestRequestTypeDef,
     ListCustomRoutingEndpointGroupsRequestRequestTypeDef,
+    ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
     ListCustomRoutingListenersRequestRequestTypeDef,
+    ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
     ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
+    ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
     ListCustomRoutingPortMappingsRequestRequestTypeDef,
+    ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
     ListEndpointGroupsRequestRequestTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     RemoveCustomRoutingEndpointsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAcceleratorAttributesRequestRequestTypeDef,
     UpdateAcceleratorRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorRequestRequestTypeDef,
     WithdrawByoipCidrRequestRequestTypeDef,
+    DescribeAcceleratorAttributesResponseTypeDef,
+    UpdateAcceleratorAttributesResponseTypeDef,
     AcceleratorTypeDef,
     CustomRoutingAcceleratorTypeDef,
     AddCustomRoutingEndpointsRequestRequestTypeDef,
     AddCustomRoutingEndpointsResponseTypeDef,
-    DescribeAcceleratorAttributesResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    UpdateAcceleratorAttributesResponseTypeDef,
     AddEndpointsRequestRequestTypeDef,
     AddEndpointsResponseTypeDef,
     ByoipCidrTypeDef,
     ProvisionByoipCidrRequestRequestTypeDef,
     CreateAcceleratorRequestRequestTypeDef,
     CreateCustomRoutingAcceleratorRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -447,22 +456,14 @@
     UpdateEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorAttributesResponseTypeDef,
     UpdateCustomRoutingAcceleratorAttributesResponseTypeDef,
     CustomRoutingEndpointGroupTypeDef,
     DestinationPortMappingTypeDef,
     PortMappingTypeDef,
     RemoveEndpointsRequestRequestTypeDef,
-    ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
-    ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
-    ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
-    ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
-    ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
-    ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
-    ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
     CreateAcceleratorResponseTypeDef,
     DescribeAcceleratorResponseTypeDef,
     ListAcceleratorsResponseTypeDef,
     UpdateAcceleratorResponseTypeDef,
     CreateCustomRoutingAcceleratorResponseTypeDef,
     DescribeCustomRoutingAcceleratorResponseTypeDef,
     ListCustomRoutingAcceleratorsResponseTypeDef,
@@ -499,42 +500,42 @@
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

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/mypy_boto3_globalaccelerator.egg-info/SOURCES.txt` & `mypy-boto3-globalaccelerator-1.27.0/mypy_boto3_globalaccelerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.26.0.post1/setup.py` & `mypy-boto3-globalaccelerator-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-globalaccelerator.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-globalaccelerator",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_globalaccelerator"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GlobalAccelerator 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.GlobalAccelerator 1.27.0 service generated with"
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
     keywords="boto3 globalaccelerator type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_globalaccelerator": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_globalaccelerator": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/",
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


# Comparing `tmp/mypy-boto3-directconnect-1.26.91.tar.gz` & `tmp/mypy-boto3-directconnect-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-directconnect-1.26.91.tar", last modified: Tue Mar 14 19:48:00 2023, max compression
+gzip compressed data, was "mypy-boto3-directconnect-1.27.0.tar", last modified: Mon Jul  3 19:50:38 2023, max compression
```

## Comparing `mypy-boto3-directconnect-1.26.91.tar` & `mypy-boto3-directconnect-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.333218 mypy-boto3-directconnect-1.26.91/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20297 2023-03-14 19:48:00.333218 mypy-boto3-directconnect-1.26.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18786 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.333218 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47262 2023-03-14 19:46:56.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47189 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10617 2023-03-14 19:46:56.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-03-14 19:46:56.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-03-14 19:46:56.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-03-14 19:46:56.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54933 2023-03-14 19:46:57.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54886 2023-03-14 19:46:56.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.333218 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20297 2023-03-14 19:48:00.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-14 19:48:00.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:48:00.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:48:00.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-14 19:48:00.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-14 19:48:00.000000 mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 19:48:00.333218 mypy-boto3-directconnect-1.26.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-14 19:46:55.000000 mypy-boto3-directconnect-1.26.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.891113 mypy-boto3-directconnect-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20279 2023-07-03 19:50:38.891113 mypy-boto3-directconnect-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18770 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.887113 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47262 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47189 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-07-03 19:35:35.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55029 2023-07-03 19:35:36.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54982 2023-07-03 19:35:35.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.891113 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20279 2023-07-03 19:50:38.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 19:50:38.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:38.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:38.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:38.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:50:38.000000 mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:38.891113 mypy-boto3-directconnect-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 19:35:34.000000 mypy-boto3-directconnect-1.27.0/setup.py
```

### Comparing `mypy-boto3-directconnect-1.26.91/LICENSE` & `mypy-boto3-directconnect-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-directconnect-1.26.91/PKG-INFO` & `mypy-boto3-directconnect-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-directconnect
-Version: 1.26.91
-Summary: Type annotations for boto3.DirectConnect 1.26.91 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.DirectConnect 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-directconnect"></a>
 
 # mypy-boto3-directconnect
 
 [![PyPI - mypy-boto3-directconnect](https://img.shields.io/pypi/v/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-directconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectConnect 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[boto3.DirectConnect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-directconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,85 +350,88 @@
 
 `mypy_boto3_directconnect.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_directconnect.type_defs import (
     RouteFilterPrefixTypeDef,
-    ResponseMetadataTypeDef,
     AllocateConnectionOnInterconnectRequestRequestTypeDef,
     TagTypeDef,
     AssociateConnectionWithLagRequestRequestTypeDef,
     AssociateHostedConnectionRequestRequestTypeDef,
     AssociateMacSecKeyRequestRequestTypeDef,
     MacSecKeyTypeDef,
     AssociateVirtualInterfaceRequestRequestTypeDef,
     AssociatedGatewayTypeDef,
     BGPPeerTypeDef,
     ConfirmConnectionRequestRequestTypeDef,
+    ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementRequestRequestTypeDef,
+    ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
+    ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceRequestRequestTypeDef,
+    ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceRequestRequestTypeDef,
+    ConfirmTransitVirtualInterfaceResponseTypeDef,
     NewBGPPeerTypeDef,
     CreateDirectConnectGatewayRequestRequestTypeDef,
     DirectConnectGatewayTypeDef,
     CustomerAgreementTypeDef,
     DeleteBGPPeerRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationRequestRequestTypeDef,
     DeleteDirectConnectGatewayRequestRequestTypeDef,
     DeleteInterconnectRequestRequestTypeDef,
+    DeleteInterconnectResponseTypeDef,
     DeleteLagRequestRequestTypeDef,
     DeleteVirtualInterfaceRequestRequestTypeDef,
+    DeleteVirtualInterfaceResponseTypeDef,
     DescribeConnectionLoaRequestRequestTypeDef,
     LoaTypeDef,
     DescribeConnectionsOnInterconnectRequestRequestTypeDef,
     DescribeConnectionsRequestRequestTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
     DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef,
+    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef,
     DirectConnectGatewayAttachmentTypeDef,
+    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewaysRequestRequestTypeDef,
     DescribeHostedConnectionsRequestRequestTypeDef,
     DescribeInterconnectLoaRequestRequestTypeDef,
     DescribeInterconnectsRequestRequestTypeDef,
     DescribeLagsRequestRequestTypeDef,
     DescribeLoaRequestRequestTypeDef,
     DescribeRouterConfigurationRequestRequestTypeDef,
     RouterTypeTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DescribeVirtualInterfacesRequestRequestTypeDef,
     DisassociateConnectionFromLagRequestRequestTypeDef,
     DisassociateMacSecKeyRequestRequestTypeDef,
     ListVirtualInterfaceTestHistoryRequestRequestTypeDef,
     VirtualInterfaceTestHistoryTypeDef,
+    LoaResponseMetadataTypeDef,
     LocationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartBgpFailoverTestRequestRequestTypeDef,
     StopBgpFailoverTestRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     UpdateDirectConnectGatewayRequestRequestTypeDef,
     UpdateLagRequestRequestTypeDef,
     UpdateVirtualInterfaceAttributesRequestRequestTypeDef,
     VirtualGatewayTypeDef,
     AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     UpdateDirectConnectGatewayAssociationRequestRequestTypeDef,
-    ConfirmConnectionResponseTypeDef,
-    ConfirmCustomerAgreementResponseTypeDef,
-    ConfirmPrivateVirtualInterfaceResponseTypeDef,
-    ConfirmPublicVirtualInterfaceResponseTypeDef,
-    ConfirmTransitVirtualInterfaceResponseTypeDef,
-    DeleteInterconnectResponseTypeDef,
-    DeleteVirtualInterfaceResponseTypeDef,
-    LoaResponseMetadataTypeDef,
     AllocateHostedConnectionRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateInterconnectRequestRequestTypeDef,
     CreateLagRequestRequestTypeDef,
     InterconnectResponseMetadataTypeDef,
     InterconnectTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
@@ -451,17 +454,14 @@
     CreateDirectConnectGatewayResultTypeDef,
     DeleteDirectConnectGatewayResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     DescribeCustomerMetadataResponseTypeDef,
     DescribeConnectionLoaResponseTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
-    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
-    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
-    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     LocationsTypeDef,
     VirtualGatewaysTypeDef,
@@ -500,42 +500,42 @@
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

### Comparing `mypy-boto3-directconnect-1.26.91/README.md` & `mypy-boto3-directconnect-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-directconnect"></a>
 
 # mypy-boto3-directconnect
 
 [![PyPI - mypy-boto3-directconnect](https://img.shields.io/pypi/v/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-directconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectConnect 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[boto3.DirectConnect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-directconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,85 +318,88 @@
 
 `mypy_boto3_directconnect.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_directconnect.type_defs import (
     RouteFilterPrefixTypeDef,
-    ResponseMetadataTypeDef,
     AllocateConnectionOnInterconnectRequestRequestTypeDef,
     TagTypeDef,
     AssociateConnectionWithLagRequestRequestTypeDef,
     AssociateHostedConnectionRequestRequestTypeDef,
     AssociateMacSecKeyRequestRequestTypeDef,
     MacSecKeyTypeDef,
     AssociateVirtualInterfaceRequestRequestTypeDef,
     AssociatedGatewayTypeDef,
     BGPPeerTypeDef,
     ConfirmConnectionRequestRequestTypeDef,
+    ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementRequestRequestTypeDef,
+    ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
+    ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceRequestRequestTypeDef,
+    ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceRequestRequestTypeDef,
+    ConfirmTransitVirtualInterfaceResponseTypeDef,
     NewBGPPeerTypeDef,
     CreateDirectConnectGatewayRequestRequestTypeDef,
     DirectConnectGatewayTypeDef,
     CustomerAgreementTypeDef,
     DeleteBGPPeerRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationRequestRequestTypeDef,
     DeleteDirectConnectGatewayRequestRequestTypeDef,
     DeleteInterconnectRequestRequestTypeDef,
+    DeleteInterconnectResponseTypeDef,
     DeleteLagRequestRequestTypeDef,
     DeleteVirtualInterfaceRequestRequestTypeDef,
+    DeleteVirtualInterfaceResponseTypeDef,
     DescribeConnectionLoaRequestRequestTypeDef,
     LoaTypeDef,
     DescribeConnectionsOnInterconnectRequestRequestTypeDef,
     DescribeConnectionsRequestRequestTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
     DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef,
+    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef,
     DirectConnectGatewayAttachmentTypeDef,
+    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewaysRequestRequestTypeDef,
     DescribeHostedConnectionsRequestRequestTypeDef,
     DescribeInterconnectLoaRequestRequestTypeDef,
     DescribeInterconnectsRequestRequestTypeDef,
     DescribeLagsRequestRequestTypeDef,
     DescribeLoaRequestRequestTypeDef,
     DescribeRouterConfigurationRequestRequestTypeDef,
     RouterTypeTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DescribeVirtualInterfacesRequestRequestTypeDef,
     DisassociateConnectionFromLagRequestRequestTypeDef,
     DisassociateMacSecKeyRequestRequestTypeDef,
     ListVirtualInterfaceTestHistoryRequestRequestTypeDef,
     VirtualInterfaceTestHistoryTypeDef,
+    LoaResponseMetadataTypeDef,
     LocationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartBgpFailoverTestRequestRequestTypeDef,
     StopBgpFailoverTestRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     UpdateDirectConnectGatewayRequestRequestTypeDef,
     UpdateLagRequestRequestTypeDef,
     UpdateVirtualInterfaceAttributesRequestRequestTypeDef,
     VirtualGatewayTypeDef,
     AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     UpdateDirectConnectGatewayAssociationRequestRequestTypeDef,
-    ConfirmConnectionResponseTypeDef,
-    ConfirmCustomerAgreementResponseTypeDef,
-    ConfirmPrivateVirtualInterfaceResponseTypeDef,
-    ConfirmPublicVirtualInterfaceResponseTypeDef,
-    ConfirmTransitVirtualInterfaceResponseTypeDef,
-    DeleteInterconnectResponseTypeDef,
-    DeleteVirtualInterfaceResponseTypeDef,
-    LoaResponseMetadataTypeDef,
     AllocateHostedConnectionRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateInterconnectRequestRequestTypeDef,
     CreateLagRequestRequestTypeDef,
     InterconnectResponseMetadataTypeDef,
     InterconnectTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
@@ -419,17 +422,14 @@
     CreateDirectConnectGatewayResultTypeDef,
     DeleteDirectConnectGatewayResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     DescribeCustomerMetadataResponseTypeDef,
     DescribeConnectionLoaResponseTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
-    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
-    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
-    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     LocationsTypeDef,
     VirtualGatewaysTypeDef,
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

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/__init__.py` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/__init__.pyi` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/__main__.py` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DirectConnect 1.26.91\nVersion:         1.26.91\nBuilder"
-        " version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.DirectConnect 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.91")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/client.py` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/client.pyi` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/literals.py` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
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
@@ -157,14 +158,15 @@
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
@@ -262,14 +264,15 @@
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
@@ -305,14 +308,15 @@
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
@@ -331,16 +335,19 @@
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
@@ -424,15 +431,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
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

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/literals.pyi` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
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
@@ -155,14 +156,15 @@
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
@@ -260,14 +262,15 @@
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
@@ -303,14 +306,15 @@
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
@@ -329,16 +333,19 @@
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
@@ -422,15 +429,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
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

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/paginator.py` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     def paginate(
         self,
         *,
         associationId: str = ...,
         associatedGatewayId: str = ...,
         directConnectGatewayId: str = ...,
         virtualGatewayId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDirectConnectGatewayAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayassociationspaginator)
         """
 
 
@@ -79,28 +79,28 @@
     """
 
     def paginate(
         self,
         *,
         directConnectGatewayId: str = ...,
         virtualInterfaceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDirectConnectGatewayAttachmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayattachmentspaginator)
         """
 
 
 class DescribeDirectConnectGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayspaginator)
     """
 
     def paginate(
-        self, *, directConnectGatewayId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, directConnectGatewayId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDirectConnectGatewaysResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayspaginator)
         """
```

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/paginator.pyi` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     def paginate(
         self,
         *,
         associationId: str = ...,
         associatedGatewayId: str = ...,
         directConnectGatewayId: str = ...,
         virtualGatewayId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDirectConnectGatewayAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayassociationspaginator)
         """
 
 class DescribeDirectConnectGatewayAttachmentsPaginator(Paginator):
@@ -75,27 +75,27 @@
     """
 
     def paginate(
         self,
         *,
         directConnectGatewayId: str = ...,
         virtualInterfaceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDirectConnectGatewayAttachmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayattachmentspaginator)
         """
 
 class DescribeDirectConnectGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayspaginator)
     """
 
     def paginate(
-        self, *, directConnectGatewayId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, directConnectGatewayId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDirectConnectGatewaysResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayspaginator)
         """
```

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/type_defs.py` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,88 +38,90 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "RouteFilterPrefixTypeDef",
-    "ResponseMetadataTypeDef",
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     "TagTypeDef",
     "AssociateConnectionWithLagRequestRequestTypeDef",
     "AssociateHostedConnectionRequestRequestTypeDef",
     "AssociateMacSecKeyRequestRequestTypeDef",
     "MacSecKeyTypeDef",
     "AssociateVirtualInterfaceRequestRequestTypeDef",
     "AssociatedGatewayTypeDef",
     "BGPPeerTypeDef",
     "ConfirmConnectionRequestRequestTypeDef",
+    "ConfirmConnectionResponseTypeDef",
     "ConfirmCustomerAgreementRequestRequestTypeDef",
+    "ConfirmCustomerAgreementResponseTypeDef",
     "ConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
+    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
+    "ConfirmPublicVirtualInterfaceResponseTypeDef",
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
+    "ConfirmTransitVirtualInterfaceResponseTypeDef",
     "NewBGPPeerTypeDef",
     "CreateDirectConnectGatewayRequestRequestTypeDef",
     "DirectConnectGatewayTypeDef",
     "CustomerAgreementTypeDef",
     "DeleteBGPPeerRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationRequestRequestTypeDef",
     "DeleteDirectConnectGatewayRequestRequestTypeDef",
     "DeleteInterconnectRequestRequestTypeDef",
+    "DeleteInterconnectResponseTypeDef",
     "DeleteLagRequestRequestTypeDef",
     "DeleteVirtualInterfaceRequestRequestTypeDef",
+    "DeleteVirtualInterfaceResponseTypeDef",
     "DescribeConnectionLoaRequestRequestTypeDef",
     "LoaTypeDef",
     "DescribeConnectionsOnInterconnectRequestRequestTypeDef",
     "DescribeConnectionsRequestRequestTypeDef",
     "DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
     "DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef",
+    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
     "DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef",
     "DirectConnectGatewayAttachmentTypeDef",
+    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     "DescribeDirectConnectGatewaysRequestRequestTypeDef",
     "DescribeHostedConnectionsRequestRequestTypeDef",
     "DescribeInterconnectLoaRequestRequestTypeDef",
     "DescribeInterconnectsRequestRequestTypeDef",
     "DescribeLagsRequestRequestTypeDef",
     "DescribeLoaRequestRequestTypeDef",
     "DescribeRouterConfigurationRequestRequestTypeDef",
     "RouterTypeTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DescribeVirtualInterfacesRequestRequestTypeDef",
     "DisassociateConnectionFromLagRequestRequestTypeDef",
     "DisassociateMacSecKeyRequestRequestTypeDef",
     "ListVirtualInterfaceTestHistoryRequestRequestTypeDef",
     "VirtualInterfaceTestHistoryTypeDef",
+    "LoaResponseMetadataTypeDef",
     "LocationTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartBgpFailoverTestRequestRequestTypeDef",
     "StopBgpFailoverTestRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "UpdateDirectConnectGatewayRequestRequestTypeDef",
     "UpdateLagRequestRequestTypeDef",
     "UpdateVirtualInterfaceAttributesRequestRequestTypeDef",
     "VirtualGatewayTypeDef",
     "AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationRequestRequestTypeDef",
     "UpdateDirectConnectGatewayAssociationRequestRequestTypeDef",
-    "ConfirmConnectionResponseTypeDef",
-    "ConfirmCustomerAgreementResponseTypeDef",
-    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
-    "ConfirmPublicVirtualInterfaceResponseTypeDef",
-    "ConfirmTransitVirtualInterfaceResponseTypeDef",
-    "DeleteInterconnectResponseTypeDef",
-    "DeleteVirtualInterfaceResponseTypeDef",
-    "LoaResponseMetadataTypeDef",
     "AllocateHostedConnectionRequestRequestTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "CreateInterconnectRequestRequestTypeDef",
     "CreateLagRequestRequestTypeDef",
     "InterconnectResponseMetadataTypeDef",
     "InterconnectTypeDef",
     "NewPrivateVirtualInterfaceAllocationTypeDef",
@@ -142,17 +144,14 @@
     "CreateDirectConnectGatewayResultTypeDef",
     "DeleteDirectConnectGatewayResultTypeDef",
     "DescribeDirectConnectGatewaysResultTypeDef",
     "UpdateDirectConnectGatewayResponseTypeDef",
     "DescribeCustomerMetadataResponseTypeDef",
     "DescribeConnectionLoaResponseTypeDef",
     "DescribeInterconnectLoaResponseTypeDef",
-    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
-    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
-    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     "DescribeRouterConfigurationResponseTypeDef",
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     "StartBgpFailoverTestResponseTypeDef",
     "StopBgpFailoverTestResponseTypeDef",
     "LocationsTypeDef",
     "VirtualGatewaysTypeDef",
@@ -187,25 +186,14 @@
     "RouteFilterPrefixTypeDef",
     {
         "cidr": str,
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
 AllocateConnectionOnInterconnectRequestRequestTypeDef = TypedDict(
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     {
         "bandwidth": str,
         "connectionName": str,
         "ownerAccount": str,
         "interconnectId": str,
@@ -223,19 +211,17 @@
     "_OptionalTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 AssociateConnectionWithLagRequestRequestTypeDef = TypedDict(
     "AssociateConnectionWithLagRequestRequestTypeDef",
     {
         "connectionId": str,
         "lagId": str,
     },
 )
@@ -260,22 +246,20 @@
         "secretARN": str,
         "ckn": str,
         "cak": str,
     },
     total=False,
 )
 
-
 class AssociateMacSecKeyRequestRequestTypeDef(
     _RequiredAssociateMacSecKeyRequestRequestTypeDef,
     _OptionalAssociateMacSecKeyRequestRequestTypeDef,
 ):
     pass
 
-
 MacSecKeyTypeDef = TypedDict(
     "MacSecKeyTypeDef",
     {
         "secretARN": str,
         "ckn": str,
         "state": str,
         "startOn": str,
@@ -322,22 +306,38 @@
 ConfirmConnectionRequestRequestTypeDef = TypedDict(
     "ConfirmConnectionRequestRequestTypeDef",
     {
         "connectionId": str,
     },
 )
 
+ConfirmConnectionResponseTypeDef = TypedDict(
+    "ConfirmConnectionResponseTypeDef",
+    {
+        "connectionState": ConnectionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConfirmCustomerAgreementRequestRequestTypeDef = TypedDict(
     "ConfirmCustomerAgreementRequestRequestTypeDef",
     {
         "agreementName": str,
     },
     total=False,
 )
 
+ConfirmCustomerAgreementResponseTypeDef = TypedDict(
+    "ConfirmCustomerAgreementResponseTypeDef",
+    {
+        "status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalConfirmPrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
@@ -345,37 +345,59 @@
     {
         "virtualGatewayId": str,
         "directConnectGatewayId": str,
     },
     total=False,
 )
 
-
 class ConfirmPrivateVirtualInterfaceRequestRequestTypeDef(
     _RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
     _OptionalConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
 ):
     pass
 
+ConfirmPrivateVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ConfirmPublicVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
+ConfirmPublicVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmPublicVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConfirmTransitVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
         "directConnectGatewayId": str,
     },
 )
 
+ConfirmTransitVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmTransitVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NewBGPPeerTypeDef = TypedDict(
     "NewBGPPeerTypeDef",
     {
         "asn": int,
         "authKey": str,
         "addressFamily": AddressFamilyType,
         "amazonAddress": str,
@@ -394,22 +416,20 @@
     "_OptionalCreateDirectConnectGatewayRequestRequestTypeDef",
     {
         "amazonSideAsn": int,
     },
     total=False,
 )
 
-
 class CreateDirectConnectGatewayRequestRequestTypeDef(
     _RequiredCreateDirectConnectGatewayRequestRequestTypeDef,
     _OptionalCreateDirectConnectGatewayRequestRequestTypeDef,
 ):
     pass
 
-
 DirectConnectGatewayTypeDef = TypedDict(
     "DirectConnectGatewayTypeDef",
     {
         "directConnectGatewayId": str,
         "directConnectGatewayName": str,
         "amazonSideAsn": int,
         "ownerAccount": str,
@@ -473,28 +493,44 @@
 DeleteInterconnectRequestRequestTypeDef = TypedDict(
     "DeleteInterconnectRequestRequestTypeDef",
     {
         "interconnectId": str,
     },
 )
 
+DeleteInterconnectResponseTypeDef = TypedDict(
+    "DeleteInterconnectResponseTypeDef",
+    {
+        "interconnectState": InterconnectStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteLagRequestRequestTypeDef = TypedDict(
     "DeleteLagRequestRequestTypeDef",
     {
         "lagId": str,
     },
 )
 
 DeleteVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "DeleteVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
+DeleteVirtualInterfaceResponseTypeDef = TypedDict(
+    "DeleteVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeConnectionLoaRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConnectionLoaRequestRequestTypeDef",
     {
         "connectionId": str,
     },
 )
 _OptionalDescribeConnectionLoaRequestRequestTypeDef = TypedDict(
@@ -502,22 +538,20 @@
     {
         "providerName": str,
         "loaContentType": Literal["application/pdf"],
     },
     total=False,
 )
 
-
 class DescribeConnectionLoaRequestRequestTypeDef(
     _RequiredDescribeConnectionLoaRequestRequestTypeDef,
     _OptionalDescribeConnectionLoaRequestRequestTypeDef,
 ):
     pass
 
-
 LoaTypeDef = TypedDict(
     "LoaTypeDef",
     {
         "loaContent": bytes,
         "loaContentType": Literal["application/pdf"],
     },
     total=False,
@@ -546,20 +580,22 @@
         "associatedGatewayId": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "associationId": str,
+        "associatedGatewayId": str,
+        "directConnectGatewayId": str,
+        "virtualGatewayId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef",
     {
@@ -569,14 +605,24 @@
         "maxResults": int,
         "nextToken": str,
         "virtualGatewayId": str,
     },
     total=False,
 )
 
+DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
+    {
+        "directConnectGatewayId": str,
+        "virtualInterfaceId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "virtualInterfaceId": str,
         "maxResults": int,
         "nextToken": str,
@@ -594,14 +640,23 @@
         "attachmentState": DirectConnectGatewayAttachmentStateType,
         "attachmentType": DirectConnectGatewayAttachmentTypeType,
         "stateChangeError": str,
     },
     total=False,
 )
 
+DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
+    {
+        "directConnectGatewayId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDirectConnectGatewaysRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewaysRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -626,22 +681,20 @@
     {
         "providerName": str,
         "loaContentType": Literal["application/pdf"],
     },
     total=False,
 )
 
-
 class DescribeInterconnectLoaRequestRequestTypeDef(
     _RequiredDescribeInterconnectLoaRequestRequestTypeDef,
     _OptionalDescribeInterconnectLoaRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeInterconnectsRequestRequestTypeDef = TypedDict(
     "DescribeInterconnectsRequestRequestTypeDef",
     {
         "interconnectId": str,
     },
     total=False,
 )
@@ -665,43 +718,39 @@
     {
         "providerName": str,
         "loaContentType": Literal["application/pdf"],
     },
     total=False,
 )
 
-
 class DescribeLoaRequestRequestTypeDef(
     _RequiredDescribeLoaRequestRequestTypeDef, _OptionalDescribeLoaRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeRouterConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRouterConfigurationRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalDescribeRouterConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeRouterConfigurationRequestRequestTypeDef",
     {
         "routerTypeIdentifier": str,
     },
     total=False,
 )
 
-
 class DescribeRouterConfigurationRequestRequestTypeDef(
     _RequiredDescribeRouterConfigurationRequestRequestTypeDef,
     _OptionalDescribeRouterConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 RouterTypeTypeDef = TypedDict(
     "RouterTypeTypeDef",
     {
         "vendor": str,
         "platform": str,
         "software": str,
         "xsltTemplateName": str,
@@ -767,27 +816,57 @@
         "testDurationInMinutes": int,
         "startTime": datetime,
         "endTime": datetime,
     },
     total=False,
 )
 
+LoaResponseMetadataTypeDef = TypedDict(
+    "LoaResponseMetadataTypeDef",
+    {
+        "loaContent": bytes,
+        "loaContentType": Literal["application/pdf"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "locationCode": str,
         "locationName": str,
         "region": str,
         "availablePortSpeeds": List[str],
         "availableProviders": List[str],
         "availableMacSecPortSpeeds": List[str],
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
 _RequiredStartBgpFailoverTestRequestRequestTypeDef = TypedDict(
     "_RequiredStartBgpFailoverTestRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalStartBgpFailoverTestRequestRequestTypeDef = TypedDict(
@@ -795,22 +874,20 @@
     {
         "bgpPeers": Sequence[str],
         "testDurationInMinutes": int,
     },
     total=False,
 )
 
-
 class StartBgpFailoverTestRequestRequestTypeDef(
     _RequiredStartBgpFailoverTestRequestRequestTypeDef,
     _OptionalStartBgpFailoverTestRequestRequestTypeDef,
 ):
     pass
 
-
 StopBgpFailoverTestRequestRequestTypeDef = TypedDict(
     "StopBgpFailoverTestRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
@@ -833,21 +910,19 @@
     {
         "connectionName": str,
         "encryptionMode": str,
     },
     total=False,
 )
 
-
 class UpdateConnectionRequestRequestTypeDef(
     _RequiredUpdateConnectionRequestRequestTypeDef, _OptionalUpdateConnectionRequestRequestTypeDef
 ):
     pass
 
-
 UpdateDirectConnectGatewayRequestRequestTypeDef = TypedDict(
     "UpdateDirectConnectGatewayRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "newDirectConnectGatewayName": str,
     },
 )
@@ -864,21 +939,19 @@
         "lagName": str,
         "minimumLinks": int,
         "encryptionMode": str,
     },
     total=False,
 )
 
-
 class UpdateLagRequestRequestTypeDef(
     _RequiredUpdateLagRequestRequestTypeDef, _OptionalUpdateLagRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateVirtualInterfaceAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualInterfaceAttributesRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalUpdateVirtualInterfaceAttributesRequestRequestTypeDef = TypedDict(
@@ -887,22 +960,20 @@
         "mtu": int,
         "enableSiteLink": bool,
         "virtualInterfaceName": str,
     },
     total=False,
 )
 
-
 class UpdateVirtualInterfaceAttributesRequestRequestTypeDef(
     _RequiredUpdateVirtualInterfaceAttributesRequestRequestTypeDef,
     _OptionalUpdateVirtualInterfaceAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 VirtualGatewayTypeDef = TypedDict(
     "VirtualGatewayTypeDef",
     {
         "virtualGatewayId": str,
         "virtualGatewayState": str,
     },
     total=False,
@@ -920,22 +991,20 @@
     "_OptionalAcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     {
         "overrideAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
     },
     total=False,
 )
 
-
 class AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef(
     _RequiredAcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     _OptionalAcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "directConnectGatewayOwnerAccount": str,
         "gatewayId": str,
     },
@@ -945,22 +1014,20 @@
     {
         "addAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
         "removeAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
     },
     total=False,
 )
 
-
 class CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef(
     _RequiredCreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     _OptionalCreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDirectConnectGatewayAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDirectConnectGatewayAssociationRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
     },
 )
 _OptionalCreateDirectConnectGatewayAssociationRequestRequestTypeDef = TypedDict(
@@ -969,97 +1036,30 @@
         "gatewayId": str,
         "addAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
         "virtualGatewayId": str,
     },
     total=False,
 )
 
-
 class CreateDirectConnectGatewayAssociationRequestRequestTypeDef(
     _RequiredCreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     _OptionalCreateDirectConnectGatewayAssociationRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateDirectConnectGatewayAssociationRequestRequestTypeDef = TypedDict(
     "UpdateDirectConnectGatewayAssociationRequestRequestTypeDef",
     {
         "associationId": str,
         "addAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
         "removeAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
     },
     total=False,
 )
 
-ConfirmConnectionResponseTypeDef = TypedDict(
-    "ConfirmConnectionResponseTypeDef",
-    {
-        "connectionState": ConnectionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfirmCustomerAgreementResponseTypeDef = TypedDict(
-    "ConfirmCustomerAgreementResponseTypeDef",
-    {
-        "status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfirmPrivateVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfirmPublicVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmPublicVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfirmTransitVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmTransitVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteInterconnectResponseTypeDef = TypedDict(
-    "DeleteInterconnectResponseTypeDef",
-    {
-        "interconnectState": InterconnectStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteVirtualInterfaceResponseTypeDef = TypedDict(
-    "DeleteVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LoaResponseMetadataTypeDef = TypedDict(
-    "LoaResponseMetadataTypeDef",
-    {
-        "loaContent": bytes,
-        "loaContentType": Literal["application/pdf"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredAllocateHostedConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAllocateHostedConnectionRequestRequestTypeDef",
     {
         "connectionId": str,
         "ownerAccount": str,
         "bandwidth": str,
         "connectionName": str,
@@ -1070,22 +1070,20 @@
     "_OptionalAllocateHostedConnectionRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class AllocateHostedConnectionRequestRequestTypeDef(
     _RequiredAllocateHostedConnectionRequestRequestTypeDef,
     _OptionalAllocateHostedConnectionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "location": str,
         "bandwidth": str,
         "connectionName": str,
     },
@@ -1097,21 +1095,19 @@
         "tags": Sequence[TagTypeDef],
         "providerName": str,
         "requestMACSec": bool,
     },
     total=False,
 )
 
-
 class CreateConnectionRequestRequestTypeDef(
     _RequiredCreateConnectionRequestRequestTypeDef, _OptionalCreateConnectionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateInterconnectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInterconnectRequestRequestTypeDef",
     {
         "interconnectName": str,
         "bandwidth": str,
         "location": str,
     },
@@ -1122,22 +1118,20 @@
         "lagId": str,
         "tags": Sequence[TagTypeDef],
         "providerName": str,
     },
     total=False,
 )
 
-
 class CreateInterconnectRequestRequestTypeDef(
     _RequiredCreateInterconnectRequestRequestTypeDef,
     _OptionalCreateInterconnectRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateLagRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLagRequestRequestTypeDef",
     {
         "numberOfConnections": int,
         "location": str,
         "connectionsBandwidth": str,
         "lagName": str,
@@ -1151,21 +1145,19 @@
         "childConnectionTags": Sequence[TagTypeDef],
         "providerName": str,
         "requestMACSec": bool,
     },
     total=False,
 )
 
-
 class CreateLagRequestRequestTypeDef(
     _RequiredCreateLagRequestRequestTypeDef, _OptionalCreateLagRequestRequestTypeDef
 ):
     pass
 
-
 InterconnectResponseMetadataTypeDef = TypedDict(
     "InterconnectResponseMetadataTypeDef",
     {
         "interconnectId": str,
         "interconnectName": str,
         "interconnectState": InterconnectStateType,
         "region": str,
@@ -1176,15 +1168,15 @@
         "awsDevice": str,
         "jumboFrameCapable": bool,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
         "tags": List[TagTypeDef],
         "providerName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InterconnectTypeDef = TypedDict(
     "InterconnectTypeDef",
     {
         "interconnectId": str,
@@ -1223,22 +1215,20 @@
         "addressFamily": AddressFamilyType,
         "customerAddress": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class NewPrivateVirtualInterfaceAllocationTypeDef(
     _RequiredNewPrivateVirtualInterfaceAllocationTypeDef,
     _OptionalNewPrivateVirtualInterfaceAllocationTypeDef,
 ):
     pass
 
-
 _RequiredNewPrivateVirtualInterfaceTypeDef = TypedDict(
     "_RequiredNewPrivateVirtualInterfaceTypeDef",
     {
         "virtualInterfaceName": str,
         "vlan": int,
         "asn": int,
     },
@@ -1255,21 +1245,19 @@
         "directConnectGatewayId": str,
         "tags": Sequence[TagTypeDef],
         "enableSiteLink": bool,
     },
     total=False,
 )
 
-
 class NewPrivateVirtualInterfaceTypeDef(
     _RequiredNewPrivateVirtualInterfaceTypeDef, _OptionalNewPrivateVirtualInterfaceTypeDef
 ):
     pass
 
-
 _RequiredNewPublicVirtualInterfaceAllocationTypeDef = TypedDict(
     "_RequiredNewPublicVirtualInterfaceAllocationTypeDef",
     {
         "virtualInterfaceName": str,
         "vlan": int,
         "asn": int,
     },
@@ -1283,22 +1271,20 @@
         "addressFamily": AddressFamilyType,
         "routeFilterPrefixes": Sequence[RouteFilterPrefixTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class NewPublicVirtualInterfaceAllocationTypeDef(
     _RequiredNewPublicVirtualInterfaceAllocationTypeDef,
     _OptionalNewPublicVirtualInterfaceAllocationTypeDef,
 ):
     pass
 
-
 _RequiredNewPublicVirtualInterfaceTypeDef = TypedDict(
     "_RequiredNewPublicVirtualInterfaceTypeDef",
     {
         "virtualInterfaceName": str,
         "vlan": int,
         "asn": int,
     },
@@ -1312,21 +1298,19 @@
         "addressFamily": AddressFamilyType,
         "routeFilterPrefixes": Sequence[RouteFilterPrefixTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class NewPublicVirtualInterfaceTypeDef(
     _RequiredNewPublicVirtualInterfaceTypeDef, _OptionalNewPublicVirtualInterfaceTypeDef
 ):
     pass
 
-
 NewTransitVirtualInterfaceAllocationTypeDef = TypedDict(
     "NewTransitVirtualInterfaceAllocationTypeDef",
     {
         "virtualInterfaceName": str,
         "vlan": int,
         "asn": int,
         "mtu": int,
@@ -1375,15 +1359,15 @@
 )
 
 AssociateMacSecKeyResponseTypeDef = TypedDict(
     "AssociateMacSecKeyResponseTypeDef",
     {
         "connectionId": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConnectionResponseMetadataTypeDef = TypedDict(
     "ConnectionResponseMetadataTypeDef",
     {
         "ownerAccount": str,
@@ -1404,15 +1388,15 @@
         "hasLogicalRedundancy": HasLogicalRedundancyType,
         "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "portEncryptionStatus": str,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ownerAccount": str,
@@ -1442,15 +1426,15 @@
 )
 
 DisassociateMacSecKeyResponseTypeDef = TypedDict(
     "DisassociateMacSecKeyResponseTypeDef",
     {
         "connectionId": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DirectConnectGatewayAssociationProposalTypeDef = TypedDict(
     "DirectConnectGatewayAssociationProposalTypeDef",
     {
         "proposalId": str,
@@ -1506,15 +1490,15 @@
         "routeFilterPrefixes": List[RouteFilterPrefixTypeDef],
         "bgpPeers": List[BGPPeerTypeDef],
         "region": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "tags": List[TagTypeDef],
         "siteLinkEnabled": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VirtualInterfaceTypeDef = TypedDict(
     "VirtualInterfaceTypeDef",
     {
         "ownerAccount": str,
@@ -1556,165 +1540,134 @@
     total=False,
 )
 
 CreateDirectConnectGatewayResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayResultTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDirectConnectGatewayResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayResultTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDirectConnectGatewaysResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewaysResultTypeDef",
     {
         "directConnectGateways": List[DirectConnectGatewayTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDirectConnectGatewayResponseTypeDef = TypedDict(
     "UpdateDirectConnectGatewayResponseTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCustomerMetadataResponseTypeDef = TypedDict(
     "DescribeCustomerMetadataResponseTypeDef",
     {
         "agreements": List[CustomerAgreementTypeDef],
         "nniPartnerType": NniPartnerTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectionLoaResponseTypeDef = TypedDict(
     "DescribeConnectionLoaResponseTypeDef",
     {
         "loa": LoaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInterconnectLoaResponseTypeDef = TypedDict(
     "DescribeInterconnectLoaResponseTypeDef",
     {
         "loa": LoaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
-    {
-        "associationId": str,
-        "associatedGatewayId": str,
-        "directConnectGatewayId": str,
-        "virtualGatewayId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "virtualInterfaceId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 DescribeDirectConnectGatewayAttachmentsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     {
         "directConnectGatewayAttachments": List[DirectConnectGatewayAttachmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRouterConfigurationResponseTypeDef = TypedDict(
     "DescribeRouterConfigurationResponseTypeDef",
     {
         "customerRouterConfig": str,
         "router": RouterTypeTypeDef,
         "virtualInterfaceId": str,
         "virtualInterfaceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVirtualInterfaceTestHistoryResponseTypeDef = TypedDict(
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     {
         "virtualInterfaceTestHistory": List[VirtualInterfaceTestHistoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartBgpFailoverTestResponseTypeDef = TypedDict(
     "StartBgpFailoverTestResponseTypeDef",
     {
         "virtualInterfaceTest": VirtualInterfaceTestHistoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopBgpFailoverTestResponseTypeDef = TypedDict(
     "StopBgpFailoverTestResponseTypeDef",
     {
         "virtualInterfaceTest": VirtualInterfaceTestHistoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LocationsTypeDef = TypedDict(
     "LocationsTypeDef",
     {
         "locations": List[LocationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VirtualGatewaysTypeDef = TypedDict(
     "VirtualGatewaysTypeDef",
     {
         "virtualGateways": List[VirtualGatewayTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InterconnectsTypeDef = TypedDict(
     "InterconnectsTypeDef",
     {
         "interconnects": List[InterconnectTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AllocatePrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "AllocatePrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "connectionId": str,
@@ -1765,23 +1718,23 @@
     },
 )
 
 DescribeTagsResponseTypeDef = TypedDict(
     "DescribeTagsResponseTypeDef",
     {
         "resourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConnectionsTypeDef = TypedDict(
     "ConnectionsTypeDef",
     {
         "connections": List[ConnectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LagResponseMetadataTypeDef = TypedDict(
     "LagResponseMetadataTypeDef",
     {
         "connectionsBandwidth": str,
@@ -1801,15 +1754,15 @@
         "jumboFrameCapable": bool,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
         "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LagTypeDef = TypedDict(
     "LagTypeDef",
     {
         "connectionsBandwidth": str,
@@ -1837,118 +1790,118 @@
     total=False,
 )
 
 CreateDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDirectConnectGatewayAssociationProposalsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationProposalsResultTypeDef",
     {
         "directConnectGatewayAssociationProposals": List[
             DirectConnectGatewayAssociationProposalTypeDef
         ],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AcceptDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "AcceptDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDirectConnectGatewayAssociationsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationsResultTypeDef",
     {
         "directConnectGatewayAssociations": List[DirectConnectGatewayAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "UpdateDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AllocateTransitVirtualInterfaceResultTypeDef = TypedDict(
     "AllocateTransitVirtualInterfaceResultTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBGPPeerResponseTypeDef = TypedDict(
     "CreateBGPPeerResponseTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTransitVirtualInterfaceResultTypeDef = TypedDict(
     "CreateTransitVirtualInterfaceResultTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteBGPPeerResponseTypeDef = TypedDict(
     "DeleteBGPPeerResponseTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VirtualInterfacesTypeDef = TypedDict(
     "VirtualInterfacesTypeDef",
     {
         "virtualInterfaces": List[VirtualInterfaceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LagsTypeDef = TypedDict(
     "LagsTypeDef",
     {
         "lags": List[LagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect/type_defs.pyi` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,87 +38,91 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "RouteFilterPrefixTypeDef",
-    "ResponseMetadataTypeDef",
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     "TagTypeDef",
     "AssociateConnectionWithLagRequestRequestTypeDef",
     "AssociateHostedConnectionRequestRequestTypeDef",
     "AssociateMacSecKeyRequestRequestTypeDef",
     "MacSecKeyTypeDef",
     "AssociateVirtualInterfaceRequestRequestTypeDef",
     "AssociatedGatewayTypeDef",
     "BGPPeerTypeDef",
     "ConfirmConnectionRequestRequestTypeDef",
+    "ConfirmConnectionResponseTypeDef",
     "ConfirmCustomerAgreementRequestRequestTypeDef",
+    "ConfirmCustomerAgreementResponseTypeDef",
     "ConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
+    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
+    "ConfirmPublicVirtualInterfaceResponseTypeDef",
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
+    "ConfirmTransitVirtualInterfaceResponseTypeDef",
     "NewBGPPeerTypeDef",
     "CreateDirectConnectGatewayRequestRequestTypeDef",
     "DirectConnectGatewayTypeDef",
     "CustomerAgreementTypeDef",
     "DeleteBGPPeerRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationRequestRequestTypeDef",
     "DeleteDirectConnectGatewayRequestRequestTypeDef",
     "DeleteInterconnectRequestRequestTypeDef",
+    "DeleteInterconnectResponseTypeDef",
     "DeleteLagRequestRequestTypeDef",
     "DeleteVirtualInterfaceRequestRequestTypeDef",
+    "DeleteVirtualInterfaceResponseTypeDef",
     "DescribeConnectionLoaRequestRequestTypeDef",
     "LoaTypeDef",
     "DescribeConnectionsOnInterconnectRequestRequestTypeDef",
     "DescribeConnectionsRequestRequestTypeDef",
     "DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
     "DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef",
+    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
     "DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef",
     "DirectConnectGatewayAttachmentTypeDef",
+    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     "DescribeDirectConnectGatewaysRequestRequestTypeDef",
     "DescribeHostedConnectionsRequestRequestTypeDef",
     "DescribeInterconnectLoaRequestRequestTypeDef",
     "DescribeInterconnectsRequestRequestTypeDef",
     "DescribeLagsRequestRequestTypeDef",
     "DescribeLoaRequestRequestTypeDef",
     "DescribeRouterConfigurationRequestRequestTypeDef",
     "RouterTypeTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DescribeVirtualInterfacesRequestRequestTypeDef",
     "DisassociateConnectionFromLagRequestRequestTypeDef",
     "DisassociateMacSecKeyRequestRequestTypeDef",
     "ListVirtualInterfaceTestHistoryRequestRequestTypeDef",
     "VirtualInterfaceTestHistoryTypeDef",
+    "LoaResponseMetadataTypeDef",
     "LocationTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartBgpFailoverTestRequestRequestTypeDef",
     "StopBgpFailoverTestRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "UpdateDirectConnectGatewayRequestRequestTypeDef",
     "UpdateLagRequestRequestTypeDef",
     "UpdateVirtualInterfaceAttributesRequestRequestTypeDef",
     "VirtualGatewayTypeDef",
     "AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationRequestRequestTypeDef",
     "UpdateDirectConnectGatewayAssociationRequestRequestTypeDef",
-    "ConfirmConnectionResponseTypeDef",
-    "ConfirmCustomerAgreementResponseTypeDef",
-    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
-    "ConfirmPublicVirtualInterfaceResponseTypeDef",
-    "ConfirmTransitVirtualInterfaceResponseTypeDef",
-    "DeleteInterconnectResponseTypeDef",
-    "DeleteVirtualInterfaceResponseTypeDef",
-    "LoaResponseMetadataTypeDef",
     "AllocateHostedConnectionRequestRequestTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "CreateInterconnectRequestRequestTypeDef",
     "CreateLagRequestRequestTypeDef",
     "InterconnectResponseMetadataTypeDef",
     "InterconnectTypeDef",
     "NewPrivateVirtualInterfaceAllocationTypeDef",
@@ -141,17 +145,14 @@
     "CreateDirectConnectGatewayResultTypeDef",
     "DeleteDirectConnectGatewayResultTypeDef",
     "DescribeDirectConnectGatewaysResultTypeDef",
     "UpdateDirectConnectGatewayResponseTypeDef",
     "DescribeCustomerMetadataResponseTypeDef",
     "DescribeConnectionLoaResponseTypeDef",
     "DescribeInterconnectLoaResponseTypeDef",
-    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
-    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
-    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     "DescribeRouterConfigurationResponseTypeDef",
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     "StartBgpFailoverTestResponseTypeDef",
     "StopBgpFailoverTestResponseTypeDef",
     "LocationsTypeDef",
     "VirtualGatewaysTypeDef",
@@ -186,25 +187,14 @@
     "RouteFilterPrefixTypeDef",
     {
         "cidr": str,
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
 AllocateConnectionOnInterconnectRequestRequestTypeDef = TypedDict(
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     {
         "bandwidth": str,
         "connectionName": str,
         "ownerAccount": str,
         "interconnectId": str,
@@ -222,17 +212,19 @@
     "_OptionalTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 AssociateConnectionWithLagRequestRequestTypeDef = TypedDict(
     "AssociateConnectionWithLagRequestRequestTypeDef",
     {
         "connectionId": str,
         "lagId": str,
     },
 )
@@ -257,20 +249,22 @@
         "secretARN": str,
         "ckn": str,
         "cak": str,
     },
     total=False,
 )
 
+
 class AssociateMacSecKeyRequestRequestTypeDef(
     _RequiredAssociateMacSecKeyRequestRequestTypeDef,
     _OptionalAssociateMacSecKeyRequestRequestTypeDef,
 ):
     pass
 
+
 MacSecKeyTypeDef = TypedDict(
     "MacSecKeyTypeDef",
     {
         "secretARN": str,
         "ckn": str,
         "state": str,
         "startOn": str,
@@ -317,22 +311,38 @@
 ConfirmConnectionRequestRequestTypeDef = TypedDict(
     "ConfirmConnectionRequestRequestTypeDef",
     {
         "connectionId": str,
     },
 )
 
+ConfirmConnectionResponseTypeDef = TypedDict(
+    "ConfirmConnectionResponseTypeDef",
+    {
+        "connectionState": ConnectionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConfirmCustomerAgreementRequestRequestTypeDef = TypedDict(
     "ConfirmCustomerAgreementRequestRequestTypeDef",
     {
         "agreementName": str,
     },
     total=False,
 )
 
+ConfirmCustomerAgreementResponseTypeDef = TypedDict(
+    "ConfirmCustomerAgreementResponseTypeDef",
+    {
+        "status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalConfirmPrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
@@ -340,35 +350,61 @@
     {
         "virtualGatewayId": str,
         "directConnectGatewayId": str,
     },
     total=False,
 )
 
+
 class ConfirmPrivateVirtualInterfaceRequestRequestTypeDef(
     _RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
     _OptionalConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
 ):
     pass
 
+
+ConfirmPrivateVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConfirmPublicVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
+ConfirmPublicVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmPublicVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConfirmTransitVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
         "directConnectGatewayId": str,
     },
 )
 
+ConfirmTransitVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmTransitVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NewBGPPeerTypeDef = TypedDict(
     "NewBGPPeerTypeDef",
     {
         "asn": int,
         "authKey": str,
         "addressFamily": AddressFamilyType,
         "amazonAddress": str,
@@ -387,20 +423,22 @@
     "_OptionalCreateDirectConnectGatewayRequestRequestTypeDef",
     {
         "amazonSideAsn": int,
     },
     total=False,
 )
 
+
 class CreateDirectConnectGatewayRequestRequestTypeDef(
     _RequiredCreateDirectConnectGatewayRequestRequestTypeDef,
     _OptionalCreateDirectConnectGatewayRequestRequestTypeDef,
 ):
     pass
 
+
 DirectConnectGatewayTypeDef = TypedDict(
     "DirectConnectGatewayTypeDef",
     {
         "directConnectGatewayId": str,
         "directConnectGatewayName": str,
         "amazonSideAsn": int,
         "ownerAccount": str,
@@ -464,28 +502,44 @@
 DeleteInterconnectRequestRequestTypeDef = TypedDict(
     "DeleteInterconnectRequestRequestTypeDef",
     {
         "interconnectId": str,
     },
 )
 
+DeleteInterconnectResponseTypeDef = TypedDict(
+    "DeleteInterconnectResponseTypeDef",
+    {
+        "interconnectState": InterconnectStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteLagRequestRequestTypeDef = TypedDict(
     "DeleteLagRequestRequestTypeDef",
     {
         "lagId": str,
     },
 )
 
 DeleteVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "DeleteVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
+DeleteVirtualInterfaceResponseTypeDef = TypedDict(
+    "DeleteVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeConnectionLoaRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConnectionLoaRequestRequestTypeDef",
     {
         "connectionId": str,
     },
 )
 _OptionalDescribeConnectionLoaRequestRequestTypeDef = TypedDict(
@@ -493,20 +547,22 @@
     {
         "providerName": str,
         "loaContentType": Literal["application/pdf"],
     },
     total=False,
 )
 
+
 class DescribeConnectionLoaRequestRequestTypeDef(
     _RequiredDescribeConnectionLoaRequestRequestTypeDef,
     _OptionalDescribeConnectionLoaRequestRequestTypeDef,
 ):
     pass
 
+
 LoaTypeDef = TypedDict(
     "LoaTypeDef",
     {
         "loaContent": bytes,
         "loaContentType": Literal["application/pdf"],
     },
     total=False,
@@ -535,20 +591,22 @@
         "associatedGatewayId": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "associationId": str,
+        "associatedGatewayId": str,
+        "directConnectGatewayId": str,
+        "virtualGatewayId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef",
     {
@@ -558,14 +616,24 @@
         "maxResults": int,
         "nextToken": str,
         "virtualGatewayId": str,
     },
     total=False,
 )
 
+DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
+    {
+        "directConnectGatewayId": str,
+        "virtualInterfaceId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "virtualInterfaceId": str,
         "maxResults": int,
         "nextToken": str,
@@ -583,14 +651,23 @@
         "attachmentState": DirectConnectGatewayAttachmentStateType,
         "attachmentType": DirectConnectGatewayAttachmentTypeType,
         "stateChangeError": str,
     },
     total=False,
 )
 
+DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
+    {
+        "directConnectGatewayId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDirectConnectGatewaysRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewaysRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -615,20 +692,22 @@
     {
         "providerName": str,
         "loaContentType": Literal["application/pdf"],
     },
     total=False,
 )
 
+
 class DescribeInterconnectLoaRequestRequestTypeDef(
     _RequiredDescribeInterconnectLoaRequestRequestTypeDef,
     _OptionalDescribeInterconnectLoaRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeInterconnectsRequestRequestTypeDef = TypedDict(
     "DescribeInterconnectsRequestRequestTypeDef",
     {
         "interconnectId": str,
     },
     total=False,
 )
@@ -652,39 +731,43 @@
     {
         "providerName": str,
         "loaContentType": Literal["application/pdf"],
     },
     total=False,
 )
 
+
 class DescribeLoaRequestRequestTypeDef(
     _RequiredDescribeLoaRequestRequestTypeDef, _OptionalDescribeLoaRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeRouterConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRouterConfigurationRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalDescribeRouterConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeRouterConfigurationRequestRequestTypeDef",
     {
         "routerTypeIdentifier": str,
     },
     total=False,
 )
 
+
 class DescribeRouterConfigurationRequestRequestTypeDef(
     _RequiredDescribeRouterConfigurationRequestRequestTypeDef,
     _OptionalDescribeRouterConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 RouterTypeTypeDef = TypedDict(
     "RouterTypeTypeDef",
     {
         "vendor": str,
         "platform": str,
         "software": str,
         "xsltTemplateName": str,
@@ -750,27 +833,57 @@
         "testDurationInMinutes": int,
         "startTime": datetime,
         "endTime": datetime,
     },
     total=False,
 )
 
+LoaResponseMetadataTypeDef = TypedDict(
+    "LoaResponseMetadataTypeDef",
+    {
+        "loaContent": bytes,
+        "loaContentType": Literal["application/pdf"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "locationCode": str,
         "locationName": str,
         "region": str,
         "availablePortSpeeds": List[str],
         "availableProviders": List[str],
         "availableMacSecPortSpeeds": List[str],
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
 _RequiredStartBgpFailoverTestRequestRequestTypeDef = TypedDict(
     "_RequiredStartBgpFailoverTestRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalStartBgpFailoverTestRequestRequestTypeDef = TypedDict(
@@ -778,20 +891,22 @@
     {
         "bgpPeers": Sequence[str],
         "testDurationInMinutes": int,
     },
     total=False,
 )
 
+
 class StartBgpFailoverTestRequestRequestTypeDef(
     _RequiredStartBgpFailoverTestRequestRequestTypeDef,
     _OptionalStartBgpFailoverTestRequestRequestTypeDef,
 ):
     pass
 
+
 StopBgpFailoverTestRequestRequestTypeDef = TypedDict(
     "StopBgpFailoverTestRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
@@ -814,19 +929,21 @@
     {
         "connectionName": str,
         "encryptionMode": str,
     },
     total=False,
 )
 
+
 class UpdateConnectionRequestRequestTypeDef(
     _RequiredUpdateConnectionRequestRequestTypeDef, _OptionalUpdateConnectionRequestRequestTypeDef
 ):
     pass
 
+
 UpdateDirectConnectGatewayRequestRequestTypeDef = TypedDict(
     "UpdateDirectConnectGatewayRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "newDirectConnectGatewayName": str,
     },
 )
@@ -843,19 +960,21 @@
         "lagName": str,
         "minimumLinks": int,
         "encryptionMode": str,
     },
     total=False,
 )
 
+
 class UpdateLagRequestRequestTypeDef(
     _RequiredUpdateLagRequestRequestTypeDef, _OptionalUpdateLagRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateVirtualInterfaceAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualInterfaceAttributesRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalUpdateVirtualInterfaceAttributesRequestRequestTypeDef = TypedDict(
@@ -864,20 +983,22 @@
         "mtu": int,
         "enableSiteLink": bool,
         "virtualInterfaceName": str,
     },
     total=False,
 )
 
+
 class UpdateVirtualInterfaceAttributesRequestRequestTypeDef(
     _RequiredUpdateVirtualInterfaceAttributesRequestRequestTypeDef,
     _OptionalUpdateVirtualInterfaceAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 VirtualGatewayTypeDef = TypedDict(
     "VirtualGatewayTypeDef",
     {
         "virtualGatewayId": str,
         "virtualGatewayState": str,
     },
     total=False,
@@ -895,20 +1016,22 @@
     "_OptionalAcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     {
         "overrideAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
     },
     total=False,
 )
 
+
 class AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef(
     _RequiredAcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     _OptionalAcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "directConnectGatewayOwnerAccount": str,
         "gatewayId": str,
     },
@@ -918,20 +1041,22 @@
     {
         "addAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
         "removeAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
     },
     total=False,
 )
 
+
 class CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef(
     _RequiredCreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     _OptionalCreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDirectConnectGatewayAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDirectConnectGatewayAssociationRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
     },
 )
 _OptionalCreateDirectConnectGatewayAssociationRequestRequestTypeDef = TypedDict(
@@ -940,95 +1065,32 @@
         "gatewayId": str,
         "addAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
         "virtualGatewayId": str,
     },
     total=False,
 )
 
+
 class CreateDirectConnectGatewayAssociationRequestRequestTypeDef(
     _RequiredCreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     _OptionalCreateDirectConnectGatewayAssociationRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateDirectConnectGatewayAssociationRequestRequestTypeDef = TypedDict(
     "UpdateDirectConnectGatewayAssociationRequestRequestTypeDef",
     {
         "associationId": str,
         "addAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
         "removeAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
     },
     total=False,
 )
 
-ConfirmConnectionResponseTypeDef = TypedDict(
-    "ConfirmConnectionResponseTypeDef",
-    {
-        "connectionState": ConnectionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfirmCustomerAgreementResponseTypeDef = TypedDict(
-    "ConfirmCustomerAgreementResponseTypeDef",
-    {
-        "status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfirmPrivateVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfirmPublicVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmPublicVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfirmTransitVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmTransitVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteInterconnectResponseTypeDef = TypedDict(
-    "DeleteInterconnectResponseTypeDef",
-    {
-        "interconnectState": InterconnectStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteVirtualInterfaceResponseTypeDef = TypedDict(
-    "DeleteVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LoaResponseMetadataTypeDef = TypedDict(
-    "LoaResponseMetadataTypeDef",
-    {
-        "loaContent": bytes,
-        "loaContentType": Literal["application/pdf"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredAllocateHostedConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAllocateHostedConnectionRequestRequestTypeDef",
     {
         "connectionId": str,
         "ownerAccount": str,
         "bandwidth": str,
         "connectionName": str,
@@ -1039,20 +1101,22 @@
     "_OptionalAllocateHostedConnectionRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class AllocateHostedConnectionRequestRequestTypeDef(
     _RequiredAllocateHostedConnectionRequestRequestTypeDef,
     _OptionalAllocateHostedConnectionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "location": str,
         "bandwidth": str,
         "connectionName": str,
     },
@@ -1064,19 +1128,21 @@
         "tags": Sequence[TagTypeDef],
         "providerName": str,
         "requestMACSec": bool,
     },
     total=False,
 )
 
+
 class CreateConnectionRequestRequestTypeDef(
     _RequiredCreateConnectionRequestRequestTypeDef, _OptionalCreateConnectionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateInterconnectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInterconnectRequestRequestTypeDef",
     {
         "interconnectName": str,
         "bandwidth": str,
         "location": str,
     },
@@ -1087,20 +1153,22 @@
         "lagId": str,
         "tags": Sequence[TagTypeDef],
         "providerName": str,
     },
     total=False,
 )
 
+
 class CreateInterconnectRequestRequestTypeDef(
     _RequiredCreateInterconnectRequestRequestTypeDef,
     _OptionalCreateInterconnectRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateLagRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLagRequestRequestTypeDef",
     {
         "numberOfConnections": int,
         "location": str,
         "connectionsBandwidth": str,
         "lagName": str,
@@ -1114,19 +1182,21 @@
         "childConnectionTags": Sequence[TagTypeDef],
         "providerName": str,
         "requestMACSec": bool,
     },
     total=False,
 )
 
+
 class CreateLagRequestRequestTypeDef(
     _RequiredCreateLagRequestRequestTypeDef, _OptionalCreateLagRequestRequestTypeDef
 ):
     pass
 
+
 InterconnectResponseMetadataTypeDef = TypedDict(
     "InterconnectResponseMetadataTypeDef",
     {
         "interconnectId": str,
         "interconnectName": str,
         "interconnectState": InterconnectStateType,
         "region": str,
@@ -1137,15 +1207,15 @@
         "awsDevice": str,
         "jumboFrameCapable": bool,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
         "tags": List[TagTypeDef],
         "providerName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InterconnectTypeDef = TypedDict(
     "InterconnectTypeDef",
     {
         "interconnectId": str,
@@ -1184,20 +1254,22 @@
         "addressFamily": AddressFamilyType,
         "customerAddress": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class NewPrivateVirtualInterfaceAllocationTypeDef(
     _RequiredNewPrivateVirtualInterfaceAllocationTypeDef,
     _OptionalNewPrivateVirtualInterfaceAllocationTypeDef,
 ):
     pass
 
+
 _RequiredNewPrivateVirtualInterfaceTypeDef = TypedDict(
     "_RequiredNewPrivateVirtualInterfaceTypeDef",
     {
         "virtualInterfaceName": str,
         "vlan": int,
         "asn": int,
     },
@@ -1214,19 +1286,21 @@
         "directConnectGatewayId": str,
         "tags": Sequence[TagTypeDef],
         "enableSiteLink": bool,
     },
     total=False,
 )
 
+
 class NewPrivateVirtualInterfaceTypeDef(
     _RequiredNewPrivateVirtualInterfaceTypeDef, _OptionalNewPrivateVirtualInterfaceTypeDef
 ):
     pass
 
+
 _RequiredNewPublicVirtualInterfaceAllocationTypeDef = TypedDict(
     "_RequiredNewPublicVirtualInterfaceAllocationTypeDef",
     {
         "virtualInterfaceName": str,
         "vlan": int,
         "asn": int,
     },
@@ -1240,20 +1314,22 @@
         "addressFamily": AddressFamilyType,
         "routeFilterPrefixes": Sequence[RouteFilterPrefixTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class NewPublicVirtualInterfaceAllocationTypeDef(
     _RequiredNewPublicVirtualInterfaceAllocationTypeDef,
     _OptionalNewPublicVirtualInterfaceAllocationTypeDef,
 ):
     pass
 
+
 _RequiredNewPublicVirtualInterfaceTypeDef = TypedDict(
     "_RequiredNewPublicVirtualInterfaceTypeDef",
     {
         "virtualInterfaceName": str,
         "vlan": int,
         "asn": int,
     },
@@ -1267,19 +1343,21 @@
         "addressFamily": AddressFamilyType,
         "routeFilterPrefixes": Sequence[RouteFilterPrefixTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class NewPublicVirtualInterfaceTypeDef(
     _RequiredNewPublicVirtualInterfaceTypeDef, _OptionalNewPublicVirtualInterfaceTypeDef
 ):
     pass
 
+
 NewTransitVirtualInterfaceAllocationTypeDef = TypedDict(
     "NewTransitVirtualInterfaceAllocationTypeDef",
     {
         "virtualInterfaceName": str,
         "vlan": int,
         "asn": int,
         "mtu": int,
@@ -1328,15 +1406,15 @@
 )
 
 AssociateMacSecKeyResponseTypeDef = TypedDict(
     "AssociateMacSecKeyResponseTypeDef",
     {
         "connectionId": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConnectionResponseMetadataTypeDef = TypedDict(
     "ConnectionResponseMetadataTypeDef",
     {
         "ownerAccount": str,
@@ -1357,15 +1435,15 @@
         "hasLogicalRedundancy": HasLogicalRedundancyType,
         "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "portEncryptionStatus": str,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ownerAccount": str,
@@ -1395,15 +1473,15 @@
 )
 
 DisassociateMacSecKeyResponseTypeDef = TypedDict(
     "DisassociateMacSecKeyResponseTypeDef",
     {
         "connectionId": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DirectConnectGatewayAssociationProposalTypeDef = TypedDict(
     "DirectConnectGatewayAssociationProposalTypeDef",
     {
         "proposalId": str,
@@ -1459,15 +1537,15 @@
         "routeFilterPrefixes": List[RouteFilterPrefixTypeDef],
         "bgpPeers": List[BGPPeerTypeDef],
         "region": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "tags": List[TagTypeDef],
         "siteLinkEnabled": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VirtualInterfaceTypeDef = TypedDict(
     "VirtualInterfaceTypeDef",
     {
         "ownerAccount": str,
@@ -1509,165 +1587,134 @@
     total=False,
 )
 
 CreateDirectConnectGatewayResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayResultTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDirectConnectGatewayResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayResultTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDirectConnectGatewaysResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewaysResultTypeDef",
     {
         "directConnectGateways": List[DirectConnectGatewayTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDirectConnectGatewayResponseTypeDef = TypedDict(
     "UpdateDirectConnectGatewayResponseTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCustomerMetadataResponseTypeDef = TypedDict(
     "DescribeCustomerMetadataResponseTypeDef",
     {
         "agreements": List[CustomerAgreementTypeDef],
         "nniPartnerType": NniPartnerTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectionLoaResponseTypeDef = TypedDict(
     "DescribeConnectionLoaResponseTypeDef",
     {
         "loa": LoaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInterconnectLoaResponseTypeDef = TypedDict(
     "DescribeInterconnectLoaResponseTypeDef",
     {
         "loa": LoaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
-    {
-        "associationId": str,
-        "associatedGatewayId": str,
-        "directConnectGatewayId": str,
-        "virtualGatewayId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "virtualInterfaceId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 DescribeDirectConnectGatewayAttachmentsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     {
         "directConnectGatewayAttachments": List[DirectConnectGatewayAttachmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRouterConfigurationResponseTypeDef = TypedDict(
     "DescribeRouterConfigurationResponseTypeDef",
     {
         "customerRouterConfig": str,
         "router": RouterTypeTypeDef,
         "virtualInterfaceId": str,
         "virtualInterfaceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVirtualInterfaceTestHistoryResponseTypeDef = TypedDict(
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     {
         "virtualInterfaceTestHistory": List[VirtualInterfaceTestHistoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartBgpFailoverTestResponseTypeDef = TypedDict(
     "StartBgpFailoverTestResponseTypeDef",
     {
         "virtualInterfaceTest": VirtualInterfaceTestHistoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopBgpFailoverTestResponseTypeDef = TypedDict(
     "StopBgpFailoverTestResponseTypeDef",
     {
         "virtualInterfaceTest": VirtualInterfaceTestHistoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LocationsTypeDef = TypedDict(
     "LocationsTypeDef",
     {
         "locations": List[LocationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VirtualGatewaysTypeDef = TypedDict(
     "VirtualGatewaysTypeDef",
     {
         "virtualGateways": List[VirtualGatewayTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InterconnectsTypeDef = TypedDict(
     "InterconnectsTypeDef",
     {
         "interconnects": List[InterconnectTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AllocatePrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "AllocatePrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "connectionId": str,
@@ -1718,23 +1765,23 @@
     },
 )
 
 DescribeTagsResponseTypeDef = TypedDict(
     "DescribeTagsResponseTypeDef",
     {
         "resourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConnectionsTypeDef = TypedDict(
     "ConnectionsTypeDef",
     {
         "connections": List[ConnectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LagResponseMetadataTypeDef = TypedDict(
     "LagResponseMetadataTypeDef",
     {
         "connectionsBandwidth": str,
@@ -1754,15 +1801,15 @@
         "jumboFrameCapable": bool,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
         "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LagTypeDef = TypedDict(
     "LagTypeDef",
     {
         "connectionsBandwidth": str,
@@ -1790,118 +1837,118 @@
     total=False,
 )
 
 CreateDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDirectConnectGatewayAssociationProposalsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationProposalsResultTypeDef",
     {
         "directConnectGatewayAssociationProposals": List[
             DirectConnectGatewayAssociationProposalTypeDef
         ],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AcceptDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "AcceptDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDirectConnectGatewayAssociationsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationsResultTypeDef",
     {
         "directConnectGatewayAssociations": List[DirectConnectGatewayAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "UpdateDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AllocateTransitVirtualInterfaceResultTypeDef = TypedDict(
     "AllocateTransitVirtualInterfaceResultTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBGPPeerResponseTypeDef = TypedDict(
     "CreateBGPPeerResponseTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTransitVirtualInterfaceResultTypeDef = TypedDict(
     "CreateTransitVirtualInterfaceResultTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteBGPPeerResponseTypeDef = TypedDict(
     "DeleteBGPPeerResponseTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VirtualInterfacesTypeDef = TypedDict(
     "VirtualInterfacesTypeDef",
     {
         "virtualInterfaces": List[VirtualInterfaceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LagsTypeDef = TypedDict(
     "LagsTypeDef",
     {
         "lags": List[LagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/PKG-INFO` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-directconnect
-Version: 1.26.91
-Summary: Type annotations for boto3.DirectConnect 1.26.91 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.DirectConnect 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-directconnect"></a>
 
 # mypy-boto3-directconnect
 
 [![PyPI - mypy-boto3-directconnect](https://img.shields.io/pypi/v/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-directconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectConnect 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[boto3.DirectConnect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-directconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,85 +350,88 @@
 
 `mypy_boto3_directconnect.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_directconnect.type_defs import (
     RouteFilterPrefixTypeDef,
-    ResponseMetadataTypeDef,
     AllocateConnectionOnInterconnectRequestRequestTypeDef,
     TagTypeDef,
     AssociateConnectionWithLagRequestRequestTypeDef,
     AssociateHostedConnectionRequestRequestTypeDef,
     AssociateMacSecKeyRequestRequestTypeDef,
     MacSecKeyTypeDef,
     AssociateVirtualInterfaceRequestRequestTypeDef,
     AssociatedGatewayTypeDef,
     BGPPeerTypeDef,
     ConfirmConnectionRequestRequestTypeDef,
+    ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementRequestRequestTypeDef,
+    ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
+    ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceRequestRequestTypeDef,
+    ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceRequestRequestTypeDef,
+    ConfirmTransitVirtualInterfaceResponseTypeDef,
     NewBGPPeerTypeDef,
     CreateDirectConnectGatewayRequestRequestTypeDef,
     DirectConnectGatewayTypeDef,
     CustomerAgreementTypeDef,
     DeleteBGPPeerRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationRequestRequestTypeDef,
     DeleteDirectConnectGatewayRequestRequestTypeDef,
     DeleteInterconnectRequestRequestTypeDef,
+    DeleteInterconnectResponseTypeDef,
     DeleteLagRequestRequestTypeDef,
     DeleteVirtualInterfaceRequestRequestTypeDef,
+    DeleteVirtualInterfaceResponseTypeDef,
     DescribeConnectionLoaRequestRequestTypeDef,
     LoaTypeDef,
     DescribeConnectionsOnInterconnectRequestRequestTypeDef,
     DescribeConnectionsRequestRequestTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
     DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef,
+    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef,
     DirectConnectGatewayAttachmentTypeDef,
+    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewaysRequestRequestTypeDef,
     DescribeHostedConnectionsRequestRequestTypeDef,
     DescribeInterconnectLoaRequestRequestTypeDef,
     DescribeInterconnectsRequestRequestTypeDef,
     DescribeLagsRequestRequestTypeDef,
     DescribeLoaRequestRequestTypeDef,
     DescribeRouterConfigurationRequestRequestTypeDef,
     RouterTypeTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DescribeVirtualInterfacesRequestRequestTypeDef,
     DisassociateConnectionFromLagRequestRequestTypeDef,
     DisassociateMacSecKeyRequestRequestTypeDef,
     ListVirtualInterfaceTestHistoryRequestRequestTypeDef,
     VirtualInterfaceTestHistoryTypeDef,
+    LoaResponseMetadataTypeDef,
     LocationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartBgpFailoverTestRequestRequestTypeDef,
     StopBgpFailoverTestRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     UpdateDirectConnectGatewayRequestRequestTypeDef,
     UpdateLagRequestRequestTypeDef,
     UpdateVirtualInterfaceAttributesRequestRequestTypeDef,
     VirtualGatewayTypeDef,
     AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     UpdateDirectConnectGatewayAssociationRequestRequestTypeDef,
-    ConfirmConnectionResponseTypeDef,
-    ConfirmCustomerAgreementResponseTypeDef,
-    ConfirmPrivateVirtualInterfaceResponseTypeDef,
-    ConfirmPublicVirtualInterfaceResponseTypeDef,
-    ConfirmTransitVirtualInterfaceResponseTypeDef,
-    DeleteInterconnectResponseTypeDef,
-    DeleteVirtualInterfaceResponseTypeDef,
-    LoaResponseMetadataTypeDef,
     AllocateHostedConnectionRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateInterconnectRequestRequestTypeDef,
     CreateLagRequestRequestTypeDef,
     InterconnectResponseMetadataTypeDef,
     InterconnectTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
@@ -451,17 +454,14 @@
     CreateDirectConnectGatewayResultTypeDef,
     DeleteDirectConnectGatewayResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     DescribeCustomerMetadataResponseTypeDef,
     DescribeConnectionLoaResponseTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
-    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
-    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
-    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     LocationsTypeDef,
     VirtualGatewaysTypeDef,
@@ -500,42 +500,42 @@
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

### Comparing `mypy-boto3-directconnect-1.26.91/mypy_boto3_directconnect.egg-info/SOURCES.txt` & `mypy-boto3-directconnect-1.27.0/mypy_boto3_directconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.26.91/setup.py` & `mypy-boto3-directconnect-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-directconnect.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-directconnect",
-    version="1.26.91",
+    version="1.27.0",
     packages=["mypy_boto3_directconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DirectConnect 1.26.91 service generated with mypy-boto3-builder"
-        " 7.13.0"
+        "Type annotations for boto3.DirectConnect 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/",
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


# Comparing `tmp/mypy-boto3-mediaconnect-1.26.113.tar.gz` & `tmp/mypy-boto3-mediaconnect-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediaconnect-1.26.113.tar", last modified: Thu Apr 13 19:32:29 2023, max compression
+gzip compressed data, was "mypy-boto3-mediaconnect-1.27.0.tar", last modified: Mon Jul  3 19:51:05 2023, max compression
```

## Comparing `mypy-boto3-mediaconnect-1.26.113.tar` & `mypy-boto3-mediaconnect-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:32:29.140819 mypy-boto3-mediaconnect-1.26.113/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22062 2023-04-13 19:32:29.140819 mypy-boto3-mediaconnect-1.26.113/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:32:29.140819 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40299 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11652 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64946 2023-04-13 19:32:18.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64855 2023-04-13 19:32:17.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:32:29.140819 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22062 2023-04-13 19:32:29.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-13 19:32:29.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:32:29.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:32:29.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 19:32:29.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 19:32:29.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:32:29.140819 mypy-boto3-mediaconnect-1.26.113/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:05.967639 mypy-boto3-mediaconnect-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:39.000000 mypy-boto3-mediaconnect-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22056 2023-07-03 19:51:05.963639 mypy-boto3-mediaconnect-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20551 2023-07-03 19:41:39.000000 mypy-boto3-mediaconnect-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:05.955639 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-03 19:41:39.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-03 19:41:39.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:41:40.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-07-03 19:41:40.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40299 2023-07-03 19:41:40.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:40.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65058 2023-07-03 19:41:42.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64967 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:39.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:05.963639 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22056 2023-07-03 19:51:05.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 19:51:05.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:05.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:05.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:05.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:51:05.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:05.967639 mypy-boto3-mediaconnect-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:41:39.000000 mypy-boto3-mediaconnect-1.27.0/setup.py
```

### Comparing `mypy-boto3-mediaconnect-1.26.113/LICENSE` & `mypy-boto3-mediaconnect-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.26.113/PKG-INFO` & `mypy-boto3-mediaconnect-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconnect
-Version: 1.26.113
-Summary: Type annotations for boto3.MediaConnect 1.26.113 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.MediaConnect 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConnect 1.26.113](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[boto3.MediaConnect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -398,107 +398,114 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconnect.type_defs import (
     VpcInterfaceAttachmentTypeDef,
     AddBridgeNetworkOutputRequestTypeDef,
     AddBridgeNetworkSourceRequestTypeDef,
-    ResponseMetadataTypeDef,
     AddEgressGatewayBridgeRequestTypeDef,
     VpcInterfaceRequestTypeDef,
     VpcInterfaceTypeDef,
     AddIngressGatewayBridgeRequestTypeDef,
     AddMaintenanceTypeDef,
     EncryptionTypeDef,
     BridgeFlowOutputTypeDef,
     BridgeNetworkOutputTypeDef,
     BridgeNetworkSourceTypeDef,
     EgressGatewayBridgeTypeDef,
     IngressGatewayBridgeTypeDef,
     MessageDetailTypeDef,
     GatewayNetworkTypeDef,
     DeleteBridgeRequestRequestTypeDef,
+    DeleteBridgeResponseTypeDef,
     DeleteFlowRequestRequestTypeDef,
+    DeleteFlowResponseTypeDef,
     DeleteGatewayRequestRequestTypeDef,
+    DeleteGatewayResponseTypeDef,
     DeregisterGatewayInstanceRequestRequestTypeDef,
+    DeregisterGatewayInstanceResponseTypeDef,
     DescribeBridgeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeFlowRequestRequestTypeDef,
     MessagesTypeDef,
     DescribeGatewayInstanceRequestRequestTypeDef,
     DescribeGatewayRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
     InterfaceRequestTypeDef,
     InterfaceTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncodingParametersRequestTypeDef,
     EncodingParametersTypeDef,
     SourcePriorityTypeDef,
     MaintenanceTypeDef,
     FmtpRequestTypeDef,
     FmtpTypeDef,
-    PaginatorConfigTypeDef,
+    ListBridgesRequestListBridgesPaginateTypeDef,
     ListBridgesRequestRequestTypeDef,
     ListedBridgeTypeDef,
+    ListEntitlementsRequestListEntitlementsPaginateTypeDef,
     ListEntitlementsRequestRequestTypeDef,
     ListedEntitlementTypeDef,
+    ListFlowsRequestListFlowsPaginateTypeDef,
     ListFlowsRequestRequestTypeDef,
+    ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef,
     ListGatewayInstancesRequestRequestTypeDef,
     ListedGatewayInstanceTypeDef,
+    ListGatewaysRequestListGatewaysPaginateTypeDef,
     ListGatewaysRequestRequestTypeDef,
     ListedGatewayTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ResourceSpecificationTypeDef,
     TransportTypeDef,
+    PaginatorConfigTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
     RemoveBridgeOutputRequestRequestTypeDef,
+    RemoveBridgeOutputResponseTypeDef,
     RemoveBridgeSourceRequestRequestTypeDef,
+    RemoveBridgeSourceResponseTypeDef,
     RemoveFlowMediaStreamRequestRequestTypeDef,
+    RemoveFlowMediaStreamResponseTypeDef,
     RemoveFlowOutputRequestRequestTypeDef,
+    RemoveFlowOutputResponseTypeDef,
     RemoveFlowSourceRequestRequestTypeDef,
+    RemoveFlowSourceResponseTypeDef,
     RemoveFlowVpcInterfaceRequestRequestTypeDef,
+    RemoveFlowVpcInterfaceResponseTypeDef,
+    ResponseMetadataTypeDef,
     RevokeFlowEntitlementRequestRequestTypeDef,
+    RevokeFlowEntitlementResponseTypeDef,
     StartFlowRequestRequestTypeDef,
+    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
+    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBridgeNetworkOutputRequestTypeDef,
     UpdateBridgeNetworkSourceRequestTypeDef,
     UpdateEgressGatewayBridgeRequestTypeDef,
     UpdateIngressGatewayBridgeRequestTypeDef,
     UpdateBridgeStateRequestRequestTypeDef,
+    UpdateBridgeStateResponseTypeDef,
     UpdateEncryptionTypeDef,
     UpdateMaintenanceTypeDef,
     UpdateGatewayInstanceRequestRequestTypeDef,
+    UpdateGatewayInstanceResponseTypeDef,
     AddBridgeFlowSourceRequestTypeDef,
     BridgeFlowSourceTypeDef,
     GatewayBridgeSourceTypeDef,
     SetGatewayBridgeSourceRequestTypeDef,
     UpdateBridgeFlowSourceRequestTypeDef,
     UpdateGatewayBridgeSourceRequestTypeDef,
     AddBridgeOutputRequestTypeDef,
-    DeleteBridgeResponseTypeDef,
-    DeleteFlowResponseTypeDef,
-    DeleteGatewayResponseTypeDef,
-    DeregisterGatewayInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RemoveBridgeOutputResponseTypeDef,
-    RemoveBridgeSourceResponseTypeDef,
-    RemoveFlowMediaStreamResponseTypeDef,
-    RemoveFlowOutputResponseTypeDef,
-    RemoveFlowSourceResponseTypeDef,
-    RemoveFlowVpcInterfaceResponseTypeDef,
-    RevokeFlowEntitlementResponseTypeDef,
-    StartFlowResponseTypeDef,
-    StopFlowResponseTypeDef,
-    UpdateBridgeStateResponseTypeDef,
-    UpdateGatewayInstanceResponseTypeDef,
     AddFlowVpcInterfacesRequestRequestTypeDef,
     AddFlowVpcInterfacesResponseTypeDef,
     EntitlementTypeDef,
     GrantEntitlementRequestTypeDef,
     BridgeOutputTypeDef,
     GatewayInstanceTypeDef,
     CreateGatewayRequestRequestTypeDef,
@@ -511,21 +518,14 @@
     DestinationConfigurationTypeDef,
     InputConfigurationTypeDef,
     FailoverConfigTypeDef,
     UpdateFailoverConfigTypeDef,
     ListedFlowTypeDef,
     MediaStreamAttributesRequestTypeDef,
     MediaStreamAttributesTypeDef,
-    ListBridgesRequestListBridgesPaginateTypeDef,
-    ListEntitlementsRequestListEntitlementsPaginateTypeDef,
-    ListFlowsRequestListFlowsPaginateTypeDef,
-    ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef,
-    ListGatewaysRequestListGatewaysPaginateTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
     ListBridgesResponseTypeDef,
     ListEntitlementsResponseTypeDef,
     ListGatewayInstancesResponseTypeDef,
     ListGatewaysResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     UpdateBridgeOutputRequestRequestTypeDef,
```

### Comparing `mypy-boto3-mediaconnect-1.26.113/README.md` & `mypy-boto3-mediaconnect-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConnect 1.26.113](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[boto3.MediaConnect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -366,107 +366,114 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconnect.type_defs import (
     VpcInterfaceAttachmentTypeDef,
     AddBridgeNetworkOutputRequestTypeDef,
     AddBridgeNetworkSourceRequestTypeDef,
-    ResponseMetadataTypeDef,
     AddEgressGatewayBridgeRequestTypeDef,
     VpcInterfaceRequestTypeDef,
     VpcInterfaceTypeDef,
     AddIngressGatewayBridgeRequestTypeDef,
     AddMaintenanceTypeDef,
     EncryptionTypeDef,
     BridgeFlowOutputTypeDef,
     BridgeNetworkOutputTypeDef,
     BridgeNetworkSourceTypeDef,
     EgressGatewayBridgeTypeDef,
     IngressGatewayBridgeTypeDef,
     MessageDetailTypeDef,
     GatewayNetworkTypeDef,
     DeleteBridgeRequestRequestTypeDef,
+    DeleteBridgeResponseTypeDef,
     DeleteFlowRequestRequestTypeDef,
+    DeleteFlowResponseTypeDef,
     DeleteGatewayRequestRequestTypeDef,
+    DeleteGatewayResponseTypeDef,
     DeregisterGatewayInstanceRequestRequestTypeDef,
+    DeregisterGatewayInstanceResponseTypeDef,
     DescribeBridgeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeFlowRequestRequestTypeDef,
     MessagesTypeDef,
     DescribeGatewayInstanceRequestRequestTypeDef,
     DescribeGatewayRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
     InterfaceRequestTypeDef,
     InterfaceTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncodingParametersRequestTypeDef,
     EncodingParametersTypeDef,
     SourcePriorityTypeDef,
     MaintenanceTypeDef,
     FmtpRequestTypeDef,
     FmtpTypeDef,
-    PaginatorConfigTypeDef,
+    ListBridgesRequestListBridgesPaginateTypeDef,
     ListBridgesRequestRequestTypeDef,
     ListedBridgeTypeDef,
+    ListEntitlementsRequestListEntitlementsPaginateTypeDef,
     ListEntitlementsRequestRequestTypeDef,
     ListedEntitlementTypeDef,
+    ListFlowsRequestListFlowsPaginateTypeDef,
     ListFlowsRequestRequestTypeDef,
+    ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef,
     ListGatewayInstancesRequestRequestTypeDef,
     ListedGatewayInstanceTypeDef,
+    ListGatewaysRequestListGatewaysPaginateTypeDef,
     ListGatewaysRequestRequestTypeDef,
     ListedGatewayTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ResourceSpecificationTypeDef,
     TransportTypeDef,
+    PaginatorConfigTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
     RemoveBridgeOutputRequestRequestTypeDef,
+    RemoveBridgeOutputResponseTypeDef,
     RemoveBridgeSourceRequestRequestTypeDef,
+    RemoveBridgeSourceResponseTypeDef,
     RemoveFlowMediaStreamRequestRequestTypeDef,
+    RemoveFlowMediaStreamResponseTypeDef,
     RemoveFlowOutputRequestRequestTypeDef,
+    RemoveFlowOutputResponseTypeDef,
     RemoveFlowSourceRequestRequestTypeDef,
+    RemoveFlowSourceResponseTypeDef,
     RemoveFlowVpcInterfaceRequestRequestTypeDef,
+    RemoveFlowVpcInterfaceResponseTypeDef,
+    ResponseMetadataTypeDef,
     RevokeFlowEntitlementRequestRequestTypeDef,
+    RevokeFlowEntitlementResponseTypeDef,
     StartFlowRequestRequestTypeDef,
+    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
+    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBridgeNetworkOutputRequestTypeDef,
     UpdateBridgeNetworkSourceRequestTypeDef,
     UpdateEgressGatewayBridgeRequestTypeDef,
     UpdateIngressGatewayBridgeRequestTypeDef,
     UpdateBridgeStateRequestRequestTypeDef,
+    UpdateBridgeStateResponseTypeDef,
     UpdateEncryptionTypeDef,
     UpdateMaintenanceTypeDef,
     UpdateGatewayInstanceRequestRequestTypeDef,
+    UpdateGatewayInstanceResponseTypeDef,
     AddBridgeFlowSourceRequestTypeDef,
     BridgeFlowSourceTypeDef,
     GatewayBridgeSourceTypeDef,
     SetGatewayBridgeSourceRequestTypeDef,
     UpdateBridgeFlowSourceRequestTypeDef,
     UpdateGatewayBridgeSourceRequestTypeDef,
     AddBridgeOutputRequestTypeDef,
-    DeleteBridgeResponseTypeDef,
-    DeleteFlowResponseTypeDef,
-    DeleteGatewayResponseTypeDef,
-    DeregisterGatewayInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RemoveBridgeOutputResponseTypeDef,
-    RemoveBridgeSourceResponseTypeDef,
-    RemoveFlowMediaStreamResponseTypeDef,
-    RemoveFlowOutputResponseTypeDef,
-    RemoveFlowSourceResponseTypeDef,
-    RemoveFlowVpcInterfaceResponseTypeDef,
-    RevokeFlowEntitlementResponseTypeDef,
-    StartFlowResponseTypeDef,
-    StopFlowResponseTypeDef,
-    UpdateBridgeStateResponseTypeDef,
-    UpdateGatewayInstanceResponseTypeDef,
     AddFlowVpcInterfacesRequestRequestTypeDef,
     AddFlowVpcInterfacesResponseTypeDef,
     EntitlementTypeDef,
     GrantEntitlementRequestTypeDef,
     BridgeOutputTypeDef,
     GatewayInstanceTypeDef,
     CreateGatewayRequestRequestTypeDef,
@@ -479,21 +486,14 @@
     DestinationConfigurationTypeDef,
     InputConfigurationTypeDef,
     FailoverConfigTypeDef,
     UpdateFailoverConfigTypeDef,
     ListedFlowTypeDef,
     MediaStreamAttributesRequestTypeDef,
     MediaStreamAttributesTypeDef,
-    ListBridgesRequestListBridgesPaginateTypeDef,
-    ListEntitlementsRequestListEntitlementsPaginateTypeDef,
-    ListFlowsRequestListFlowsPaginateTypeDef,
-    ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef,
-    ListGatewaysRequestListGatewaysPaginateTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
     ListBridgesResponseTypeDef,
     ListEntitlementsResponseTypeDef,
     ListGatewayInstancesResponseTypeDef,
     ListGatewaysResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     UpdateBridgeOutputRequestRequestTypeDef,
```

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/__init__.py` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/__init__.pyi` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/__main__.py` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaConnect 1.26.113\nVersion:         1.26.113\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.MediaConnect 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.113")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/client.py` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/client.pyi` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/literals.py` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
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
@@ -198,14 +199,15 @@
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
@@ -347,14 +349,15 @@
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
@@ -373,16 +376,19 @@
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
@@ -466,14 +472,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
```

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/literals.pyi` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
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
@@ -196,14 +197,15 @@
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
@@ -345,14 +347,15 @@
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
@@ -371,16 +374,19 @@
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
@@ -464,14 +470,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
```

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/paginator.py` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -52,121 +52,112 @@
     "ListFlowsPaginator",
     "ListGatewayInstancesPaginator",
     "ListGatewaysPaginator",
     "ListOfferingsPaginator",
     "ListReservationsPaginator",
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
 class ListBridgesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListBridges)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listbridgespaginator)
     """
 
     def paginate(
-        self, *, FilterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FilterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBridgesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListBridges.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listbridgespaginator)
         """
 
-
 class ListEntitlementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListEntitlements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listentitlementspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEntitlementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListEntitlements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listentitlementspaginator)
         """
 
-
 class ListFlowsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListFlows)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listflowspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFlowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListFlows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listflowspaginator)
         """
 
-
 class ListGatewayInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGatewayInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayinstancespaginator)
     """
 
     def paginate(
-        self, *, FilterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FilterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGatewayInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGatewayInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayinstancespaginator)
         """
 
-
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGatewaysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayspaginator)
         """
 
-
 class ListOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listofferingspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listofferingspaginator)
         """
 
-
 class ListReservationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListReservations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listreservationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListReservations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listreservationspaginator)
         """
```

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/paginator.pyi` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,112 +52,121 @@
     "ListFlowsPaginator",
     "ListGatewayInstancesPaginator",
     "ListGatewaysPaginator",
     "ListOfferingsPaginator",
     "ListReservationsPaginator",
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
 class ListBridgesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListBridges)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listbridgespaginator)
     """
 
     def paginate(
-        self, *, FilterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FilterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBridgesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListBridges.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listbridgespaginator)
         """
 
+
 class ListEntitlementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListEntitlements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listentitlementspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEntitlementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListEntitlements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listentitlementspaginator)
         """
 
+
 class ListFlowsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListFlows)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listflowspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFlowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListFlows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listflowspaginator)
         """
 
+
 class ListGatewayInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGatewayInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayinstancespaginator)
     """
 
     def paginate(
-        self, *, FilterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FilterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGatewayInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGatewayInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayinstancespaginator)
         """
 
+
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGatewaysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayspaginator)
         """
 
+
 class ListOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listofferingspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listofferingspaginator)
         """
 
+
 class ListReservationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListReservations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listreservationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListReservations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listreservationspaginator)
         """
```

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/type_defs.py` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,107 +51,114 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "VpcInterfaceAttachmentTypeDef",
     "AddBridgeNetworkOutputRequestTypeDef",
     "AddBridgeNetworkSourceRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AddEgressGatewayBridgeRequestTypeDef",
     "VpcInterfaceRequestTypeDef",
     "VpcInterfaceTypeDef",
     "AddIngressGatewayBridgeRequestTypeDef",
     "AddMaintenanceTypeDef",
     "EncryptionTypeDef",
     "BridgeFlowOutputTypeDef",
     "BridgeNetworkOutputTypeDef",
     "BridgeNetworkSourceTypeDef",
     "EgressGatewayBridgeTypeDef",
     "IngressGatewayBridgeTypeDef",
     "MessageDetailTypeDef",
     "GatewayNetworkTypeDef",
     "DeleteBridgeRequestRequestTypeDef",
+    "DeleteBridgeResponseTypeDef",
     "DeleteFlowRequestRequestTypeDef",
+    "DeleteFlowResponseTypeDef",
     "DeleteGatewayRequestRequestTypeDef",
+    "DeleteGatewayResponseTypeDef",
     "DeregisterGatewayInstanceRequestRequestTypeDef",
+    "DeregisterGatewayInstanceResponseTypeDef",
     "DescribeBridgeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeFlowRequestRequestTypeDef",
     "MessagesTypeDef",
     "DescribeGatewayInstanceRequestRequestTypeDef",
     "DescribeGatewayRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
     "InterfaceRequestTypeDef",
     "InterfaceTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncodingParametersRequestTypeDef",
     "EncodingParametersTypeDef",
     "SourcePriorityTypeDef",
     "MaintenanceTypeDef",
     "FmtpRequestTypeDef",
     "FmtpTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListBridgesRequestListBridgesPaginateTypeDef",
     "ListBridgesRequestRequestTypeDef",
     "ListedBridgeTypeDef",
+    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
     "ListEntitlementsRequestRequestTypeDef",
     "ListedEntitlementTypeDef",
+    "ListFlowsRequestListFlowsPaginateTypeDef",
     "ListFlowsRequestRequestTypeDef",
+    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
     "ListGatewayInstancesRequestRequestTypeDef",
     "ListedGatewayInstanceTypeDef",
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
     "ListGatewaysRequestRequestTypeDef",
     "ListedGatewayTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
+    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ResourceSpecificationTypeDef",
     "TransportTypeDef",
+    "PaginatorConfigTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
     "RemoveBridgeOutputRequestRequestTypeDef",
+    "RemoveBridgeOutputResponseTypeDef",
     "RemoveBridgeSourceRequestRequestTypeDef",
+    "RemoveBridgeSourceResponseTypeDef",
     "RemoveFlowMediaStreamRequestRequestTypeDef",
+    "RemoveFlowMediaStreamResponseTypeDef",
     "RemoveFlowOutputRequestRequestTypeDef",
+    "RemoveFlowOutputResponseTypeDef",
     "RemoveFlowSourceRequestRequestTypeDef",
+    "RemoveFlowSourceResponseTypeDef",
     "RemoveFlowVpcInterfaceRequestRequestTypeDef",
+    "RemoveFlowVpcInterfaceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeFlowEntitlementRequestRequestTypeDef",
+    "RevokeFlowEntitlementResponseTypeDef",
     "StartFlowRequestRequestTypeDef",
+    "StartFlowResponseTypeDef",
     "StopFlowRequestRequestTypeDef",
+    "StopFlowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBridgeNetworkOutputRequestTypeDef",
     "UpdateBridgeNetworkSourceRequestTypeDef",
     "UpdateEgressGatewayBridgeRequestTypeDef",
     "UpdateIngressGatewayBridgeRequestTypeDef",
     "UpdateBridgeStateRequestRequestTypeDef",
+    "UpdateBridgeStateResponseTypeDef",
     "UpdateEncryptionTypeDef",
     "UpdateMaintenanceTypeDef",
     "UpdateGatewayInstanceRequestRequestTypeDef",
+    "UpdateGatewayInstanceResponseTypeDef",
     "AddBridgeFlowSourceRequestTypeDef",
     "BridgeFlowSourceTypeDef",
     "GatewayBridgeSourceTypeDef",
     "SetGatewayBridgeSourceRequestTypeDef",
     "UpdateBridgeFlowSourceRequestTypeDef",
     "UpdateGatewayBridgeSourceRequestTypeDef",
     "AddBridgeOutputRequestTypeDef",
-    "DeleteBridgeResponseTypeDef",
-    "DeleteFlowResponseTypeDef",
-    "DeleteGatewayResponseTypeDef",
-    "DeregisterGatewayInstanceResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RemoveBridgeOutputResponseTypeDef",
-    "RemoveBridgeSourceResponseTypeDef",
-    "RemoveFlowMediaStreamResponseTypeDef",
-    "RemoveFlowOutputResponseTypeDef",
-    "RemoveFlowSourceResponseTypeDef",
-    "RemoveFlowVpcInterfaceResponseTypeDef",
-    "RevokeFlowEntitlementResponseTypeDef",
-    "StartFlowResponseTypeDef",
-    "StopFlowResponseTypeDef",
-    "UpdateBridgeStateResponseTypeDef",
-    "UpdateGatewayInstanceResponseTypeDef",
     "AddFlowVpcInterfacesRequestRequestTypeDef",
     "AddFlowVpcInterfacesResponseTypeDef",
     "EntitlementTypeDef",
     "GrantEntitlementRequestTypeDef",
     "BridgeOutputTypeDef",
     "GatewayInstanceTypeDef",
     "CreateGatewayRequestRequestTypeDef",
@@ -164,21 +171,14 @@
     "DestinationConfigurationTypeDef",
     "InputConfigurationTypeDef",
     "FailoverConfigTypeDef",
     "UpdateFailoverConfigTypeDef",
     "ListedFlowTypeDef",
     "MediaStreamAttributesRequestTypeDef",
     "MediaStreamAttributesTypeDef",
-    "ListBridgesRequestListBridgesPaginateTypeDef",
-    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
-    "ListFlowsRequestListFlowsPaginateTypeDef",
-    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
-    "ListGatewaysRequestListGatewaysPaginateTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListBridgesResponseTypeDef",
     "ListEntitlementsResponseTypeDef",
     "ListGatewayInstancesResponseTypeDef",
     "ListGatewaysResponseTypeDef",
     "OfferingTypeDef",
     "ReservationTypeDef",
     "UpdateBridgeOutputRequestRequestTypeDef",
@@ -267,25 +267,14 @@
         "Name": str,
         "NetworkName": str,
         "Port": int,
         "Protocol": ProtocolType,
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
 AddEgressGatewayBridgeRequestTypeDef = TypedDict(
     "AddEgressGatewayBridgeRequestTypeDef",
     {
         "MaxBitrate": int,
     },
 )
 
@@ -473,28 +462,53 @@
 DeleteBridgeRequestRequestTypeDef = TypedDict(
     "DeleteBridgeRequestRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 
+DeleteBridgeResponseTypeDef = TypedDict(
+    "DeleteBridgeResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteFlowRequestRequestTypeDef = TypedDict(
     "DeleteFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
+DeleteFlowResponseTypeDef = TypedDict(
+    "DeleteFlowResponseTypeDef",
+    {
+        "FlowArn": str,
+        "Status": StatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteGatewayRequestRequestTypeDef = TypedDict(
     "DeleteGatewayRequestRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
+DeleteGatewayResponseTypeDef = TypedDict(
+    "DeleteGatewayResponseTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeregisterGatewayInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterGatewayInstanceRequestRequestTypeDef",
     {
         "GatewayInstanceArn": str,
     },
 )
 _OptionalDeregisterGatewayInstanceRequestRequestTypeDef = TypedDict(
@@ -509,14 +523,23 @@
 class DeregisterGatewayInstanceRequestRequestTypeDef(
     _RequiredDeregisterGatewayInstanceRequestRequestTypeDef,
     _OptionalDeregisterGatewayInstanceRequestRequestTypeDef,
 ):
     pass
 
 
+DeregisterGatewayInstanceResponseTypeDef = TypedDict(
+    "DeregisterGatewayInstanceResponseTypeDef",
+    {
+        "GatewayInstanceArn": str,
+        "InstanceState": InstanceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeBridgeRequestRequestTypeDef = TypedDict(
     "DescribeBridgeRequestRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 
@@ -581,14 +604,21 @@
 InterfaceTypeDef = TypedDict(
     "InterfaceTypeDef",
     {
         "Name": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncodingParametersRequestTypeDef = TypedDict(
     "EncodingParametersRequestTypeDef",
     {
         "CompressionFactor": float,
         "EncoderProfile": EncoderProfileType,
     },
 )
@@ -644,20 +674,19 @@
         "Range": RangeType,
         "ScanMode": ScanModeType,
         "Tcs": TcsType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListBridgesRequestListBridgesPaginateTypeDef = TypedDict(
+    "ListBridgesRequestListBridgesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "FilterArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBridgesRequestRequestTypeDef = TypedDict(
     "ListBridgesRequestRequestTypeDef",
     {
@@ -675,14 +704,22 @@
         "BridgeState": BridgeStateType,
         "BridgeType": str,
         "Name": str,
         "PlacementArn": str,
     },
 )
 
+ListEntitlementsRequestListEntitlementsPaginateTypeDef = TypedDict(
+    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEntitlementsRequestRequestTypeDef = TypedDict(
     "ListEntitlementsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -706,23 +743,40 @@
 
 class ListedEntitlementTypeDef(
     _RequiredListedEntitlementTypeDef, _OptionalListedEntitlementTypeDef
 ):
     pass
 
 
+ListFlowsRequestListFlowsPaginateTypeDef = TypedDict(
+    "ListFlowsRequestListFlowsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFlowsRequestRequestTypeDef = TypedDict(
     "ListFlowsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef = TypedDict(
+    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
+    {
+        "FilterArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGatewayInstancesRequestRequestTypeDef = TypedDict(
     "ListGatewayInstancesRequestRequestTypeDef",
     {
         "FilterArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -748,14 +802,22 @@
 
 class ListedGatewayInstanceTypeDef(
     _RequiredListedGatewayInstanceTypeDef, _OptionalListedGatewayInstanceTypeDef
 ):
     pass
 
 
+ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGatewaysRequestRequestTypeDef = TypedDict(
     "ListGatewaysRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -766,23 +828,39 @@
     {
         "GatewayArn": str,
         "GatewayState": GatewayStateType,
         "Name": str,
     },
 )
 
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
+    "ListReservationsRequestListReservationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReservationsRequestRequestTypeDef = TypedDict(
     "ListReservationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -791,14 +869,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredResourceSpecificationTypeDef = TypedDict(
     "_RequiredResourceSpecificationTypeDef",
     {
         "ResourceType": Literal["Mbps_Outbound_Bandwidth"],
     },
 )
 _OptionalResourceSpecificationTypeDef = TypedDict(
@@ -842,14 +928,24 @@
 )
 
 
 class TransportTypeDef(_RequiredTransportTypeDef, _OptionalTransportTypeDef):
     pass
 
 
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
 PurchaseOfferingRequestRequestTypeDef = TypedDict(
     "PurchaseOfferingRequestRequestTypeDef",
     {
         "OfferingArn": str,
         "ReservationName": str,
         "Start": str,
     },
@@ -859,76 +955,169 @@
     "RemoveBridgeOutputRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "OutputName": str,
     },
 )
 
+RemoveBridgeOutputResponseTypeDef = TypedDict(
+    "RemoveBridgeOutputResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "OutputName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveBridgeSourceRequestRequestTypeDef = TypedDict(
     "RemoveBridgeSourceRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "SourceName": str,
     },
 )
 
+RemoveBridgeSourceResponseTypeDef = TypedDict(
+    "RemoveBridgeSourceResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "SourceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveFlowMediaStreamRequestRequestTypeDef = TypedDict(
     "RemoveFlowMediaStreamRequestRequestTypeDef",
     {
         "FlowArn": str,
         "MediaStreamName": str,
     },
 )
 
+RemoveFlowMediaStreamResponseTypeDef = TypedDict(
+    "RemoveFlowMediaStreamResponseTypeDef",
+    {
+        "FlowArn": str,
+        "MediaStreamName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveFlowOutputRequestRequestTypeDef = TypedDict(
     "RemoveFlowOutputRequestRequestTypeDef",
     {
         "FlowArn": str,
         "OutputArn": str,
     },
 )
 
+RemoveFlowOutputResponseTypeDef = TypedDict(
+    "RemoveFlowOutputResponseTypeDef",
+    {
+        "FlowArn": str,
+        "OutputArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveFlowSourceRequestRequestTypeDef = TypedDict(
     "RemoveFlowSourceRequestRequestTypeDef",
     {
         "FlowArn": str,
         "SourceArn": str,
     },
 )
 
+RemoveFlowSourceResponseTypeDef = TypedDict(
+    "RemoveFlowSourceResponseTypeDef",
+    {
+        "FlowArn": str,
+        "SourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveFlowVpcInterfaceRequestRequestTypeDef = TypedDict(
     "RemoveFlowVpcInterfaceRequestRequestTypeDef",
     {
         "FlowArn": str,
         "VpcInterfaceName": str,
     },
 )
 
+RemoveFlowVpcInterfaceResponseTypeDef = TypedDict(
+    "RemoveFlowVpcInterfaceResponseTypeDef",
+    {
+        "FlowArn": str,
+        "NonDeletedNetworkInterfaceIds": List[str],
+        "VpcInterfaceName": str,
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
 RevokeFlowEntitlementRequestRequestTypeDef = TypedDict(
     "RevokeFlowEntitlementRequestRequestTypeDef",
     {
         "EntitlementArn": str,
         "FlowArn": str,
     },
 )
 
+RevokeFlowEntitlementResponseTypeDef = TypedDict(
+    "RevokeFlowEntitlementResponseTypeDef",
+    {
+        "EntitlementArn": str,
+        "FlowArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartFlowRequestRequestTypeDef = TypedDict(
     "StartFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
+StartFlowResponseTypeDef = TypedDict(
+    "StartFlowResponseTypeDef",
+    {
+        "FlowArn": str,
+        "Status": StatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopFlowRequestRequestTypeDef = TypedDict(
     "StopFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
+StopFlowResponseTypeDef = TypedDict(
+    "StopFlowResponseTypeDef",
+    {
+        "FlowArn": str,
+        "Status": StatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -985,14 +1174,23 @@
     "UpdateBridgeStateRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "DesiredState": DesiredStateType,
     },
 )
 
+UpdateBridgeStateResponseTypeDef = TypedDict(
+    "UpdateBridgeStateResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "DesiredState": DesiredStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateEncryptionTypeDef = TypedDict(
     "UpdateEncryptionTypeDef",
     {
         "Algorithm": AlgorithmType,
         "ConstantInitializationVector": str,
         "DeviceId": str,
         "KeyType": KeyTypeType,
@@ -1033,14 +1231,23 @@
 class UpdateGatewayInstanceRequestRequestTypeDef(
     _RequiredUpdateGatewayInstanceRequestRequestTypeDef,
     _OptionalUpdateGatewayInstanceRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateGatewayInstanceResponseTypeDef = TypedDict(
+    "UpdateGatewayInstanceResponseTypeDef",
+    {
+        "BridgePlacement": BridgePlacementType,
+        "GatewayInstanceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAddBridgeFlowSourceRequestTypeDef = TypedDict(
     "_RequiredAddBridgeFlowSourceRequestTypeDef",
     {
         "FlowArn": str,
         "Name": str,
     },
 )
@@ -1144,177 +1351,28 @@
     "AddBridgeOutputRequestTypeDef",
     {
         "NetworkOutput": AddBridgeNetworkOutputRequestTypeDef,
     },
     total=False,
 )
 
-DeleteBridgeResponseTypeDef = TypedDict(
-    "DeleteBridgeResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFlowResponseTypeDef = TypedDict(
-    "DeleteFlowResponseTypeDef",
-    {
-        "FlowArn": str,
-        "Status": StatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteGatewayResponseTypeDef = TypedDict(
-    "DeleteGatewayResponseTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeregisterGatewayInstanceResponseTypeDef = TypedDict(
-    "DeregisterGatewayInstanceResponseTypeDef",
-    {
-        "GatewayInstanceArn": str,
-        "InstanceState": InstanceStateType,
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
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveBridgeOutputResponseTypeDef = TypedDict(
-    "RemoveBridgeOutputResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "OutputName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveBridgeSourceResponseTypeDef = TypedDict(
-    "RemoveBridgeSourceResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "SourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveFlowMediaStreamResponseTypeDef = TypedDict(
-    "RemoveFlowMediaStreamResponseTypeDef",
-    {
-        "FlowArn": str,
-        "MediaStreamName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveFlowOutputResponseTypeDef = TypedDict(
-    "RemoveFlowOutputResponseTypeDef",
-    {
-        "FlowArn": str,
-        "OutputArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveFlowSourceResponseTypeDef = TypedDict(
-    "RemoveFlowSourceResponseTypeDef",
-    {
-        "FlowArn": str,
-        "SourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveFlowVpcInterfaceResponseTypeDef = TypedDict(
-    "RemoveFlowVpcInterfaceResponseTypeDef",
-    {
-        "FlowArn": str,
-        "NonDeletedNetworkInterfaceIds": List[str],
-        "VpcInterfaceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RevokeFlowEntitlementResponseTypeDef = TypedDict(
-    "RevokeFlowEntitlementResponseTypeDef",
-    {
-        "EntitlementArn": str,
-        "FlowArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartFlowResponseTypeDef = TypedDict(
-    "StartFlowResponseTypeDef",
-    {
-        "FlowArn": str,
-        "Status": StatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopFlowResponseTypeDef = TypedDict(
-    "StopFlowResponseTypeDef",
-    {
-        "FlowArn": str,
-        "Status": StatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateBridgeStateResponseTypeDef = TypedDict(
-    "UpdateBridgeStateResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "DesiredState": DesiredStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGatewayInstanceResponseTypeDef = TypedDict(
-    "UpdateGatewayInstanceResponseTypeDef",
-    {
-        "BridgePlacement": BridgePlacementType,
-        "GatewayInstanceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AddFlowVpcInterfacesRequestRequestTypeDef = TypedDict(
     "AddFlowVpcInterfacesRequestRequestTypeDef",
     {
         "FlowArn": str,
         "VpcInterfaces": Sequence[VpcInterfaceRequestTypeDef],
     },
 )
 
 AddFlowVpcInterfacesResponseTypeDef = TypedDict(
     "AddFlowVpcInterfacesResponseTypeDef",
     {
         "FlowArn": str,
         "VpcInterfaces": List[VpcInterfaceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEntitlementTypeDef = TypedDict(
     "_RequiredEntitlementTypeDef",
     {
         "EntitlementArn": str,
@@ -1603,105 +1661,47 @@
 
 class MediaStreamAttributesTypeDef(
     _RequiredMediaStreamAttributesTypeDef, _OptionalMediaStreamAttributesTypeDef
 ):
     pass
 
 
-ListBridgesRequestListBridgesPaginateTypeDef = TypedDict(
-    "ListBridgesRequestListBridgesPaginateTypeDef",
-    {
-        "FilterArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEntitlementsRequestListEntitlementsPaginateTypeDef = TypedDict(
-    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFlowsRequestListFlowsPaginateTypeDef = TypedDict(
-    "ListFlowsRequestListFlowsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef = TypedDict(
-    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
-    {
-        "FilterArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysRequestListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
-    "ListReservationsRequestListReservationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListBridgesResponseTypeDef = TypedDict(
     "ListBridgesResponseTypeDef",
     {
         "Bridges": List[ListedBridgeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEntitlementsResponseTypeDef = TypedDict(
     "ListEntitlementsResponseTypeDef",
     {
         "Entitlements": List[ListedEntitlementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGatewayInstancesResponseTypeDef = TypedDict(
     "ListGatewayInstancesResponseTypeDef",
     {
         "Instances": List[ListedGatewayInstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGatewaysResponseTypeDef = TypedDict(
     "ListGatewaysResponseTypeDef",
     {
         "Gateways": List[ListedGatewayTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "CurrencyCode": str,
@@ -1834,24 +1834,24 @@
 )
 
 GrantFlowEntitlementsResponseTypeDef = TypedDict(
     "GrantFlowEntitlementsResponseTypeDef",
     {
         "Entitlements": List[EntitlementTypeDef],
         "FlowArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFlowEntitlementResponseTypeDef = TypedDict(
     "UpdateFlowEntitlementResponseTypeDef",
     {
         "Entitlement": EntitlementTypeDef,
         "FlowArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GrantFlowEntitlementsRequestRequestTypeDef = TypedDict(
     "GrantFlowEntitlementsRequestRequestTypeDef",
     {
         "Entitlements": Sequence[GrantEntitlementRequestTypeDef],
@@ -1860,48 +1860,48 @@
 )
 
 AddBridgeOutputsResponseTypeDef = TypedDict(
     "AddBridgeOutputsResponseTypeDef",
     {
         "BridgeArn": str,
         "Outputs": List[BridgeOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBridgeOutputResponseTypeDef = TypedDict(
     "UpdateBridgeOutputResponseTypeDef",
     {
         "BridgeArn": str,
         "Output": BridgeOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGatewayInstanceResponseTypeDef = TypedDict(
     "DescribeGatewayInstanceResponseTypeDef",
     {
         "GatewayInstance": GatewayInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateGatewayResponseTypeDef = TypedDict(
     "CreateGatewayResponseTypeDef",
     {
         "Gateway": GatewayTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGatewayResponseTypeDef = TypedDict(
     "DescribeGatewayResponseTypeDef",
     {
         "Gateway": GatewayTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMediaStreamOutputConfigurationRequestTypeDef = TypedDict(
     "_RequiredMediaStreamOutputConfigurationRequestTypeDef",
     {
         "EncodingName": EncodingNameType,
@@ -2039,15 +2039,15 @@
 
 
 ListFlowsResponseTypeDef = TypedDict(
     "ListFlowsResponseTypeDef",
     {
         "Flows": List[ListedFlowTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAddMediaStreamRequestTypeDef = TypedDict(
     "_RequiredAddMediaStreamRequestTypeDef",
     {
         "MediaStreamId": int,
@@ -2125,49 +2125,49 @@
     pass
 
 
 DescribeOfferingResponseTypeDef = TypedDict(
     "DescribeOfferingResponseTypeDef",
     {
         "Offering": OfferingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOfferingsResponseTypeDef = TypedDict(
     "ListOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "Offerings": List[OfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservationResponseTypeDef = TypedDict(
     "DescribeReservationResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReservationsResponseTypeDef = TypedDict(
     "ListReservationsResponseTypeDef",
     {
         "NextToken": str,
         "Reservations": List[ReservationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PurchaseOfferingResponseTypeDef = TypedDict(
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddBridgeSourcesRequestRequestTypeDef = TypedDict(
     "AddBridgeSourcesRequestRequestTypeDef",
     {
         "BridgeArn": str,
@@ -2202,15 +2202,15 @@
 
 
 AddBridgeSourcesResponseTypeDef = TypedDict(
     "AddBridgeSourcesResponseTypeDef",
     {
         "BridgeArn": str,
         "Sources": List[BridgeSourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBridgeTypeDef = TypedDict(
     "_RequiredBridgeTypeDef",
     {
         "BridgeArn": str,
@@ -2238,15 +2238,15 @@
 
 
 UpdateBridgeSourceResponseTypeDef = TypedDict(
     "UpdateBridgeSourceResponseTypeDef",
     {
         "BridgeArn": str,
         "Source": BridgeSourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAddOutputRequestTypeDef = TypedDict(
     "_RequiredAddOutputRequestTypeDef",
     {
         "Protocol": ProtocolType,
@@ -2452,48 +2452,48 @@
 )
 
 AddFlowMediaStreamsResponseTypeDef = TypedDict(
     "AddFlowMediaStreamsResponseTypeDef",
     {
         "FlowArn": str,
         "MediaStreams": List[MediaStreamTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFlowMediaStreamResponseTypeDef = TypedDict(
     "UpdateFlowMediaStreamResponseTypeDef",
     {
         "FlowArn": str,
         "MediaStream": MediaStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBridgeResponseTypeDef = TypedDict(
     "CreateBridgeResponseTypeDef",
     {
         "Bridge": BridgeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBridgeResponseTypeDef = TypedDict(
     "DescribeBridgeResponseTypeDef",
     {
         "Bridge": BridgeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBridgeResponseTypeDef = TypedDict(
     "UpdateBridgeResponseTypeDef",
     {
         "Bridge": BridgeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddFlowOutputsRequestRequestTypeDef = TypedDict(
     "AddFlowOutputsRequestRequestTypeDef",
     {
         "FlowArn": str,
@@ -2539,33 +2539,33 @@
 
 
 AddFlowOutputsResponseTypeDef = TypedDict(
     "AddFlowOutputsResponseTypeDef",
     {
         "FlowArn": str,
         "Outputs": List[OutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFlowOutputResponseTypeDef = TypedDict(
     "UpdateFlowOutputResponseTypeDef",
     {
         "FlowArn": str,
         "Output": OutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddFlowSourcesResponseTypeDef = TypedDict(
     "AddFlowSourcesResponseTypeDef",
     {
         "FlowArn": str,
         "Sources": List[SourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFlowTypeDef = TypedDict(
     "_RequiredFlowTypeDef",
     {
         "AvailabilityZone": str,
@@ -2597,35 +2597,35 @@
 
 
 UpdateFlowSourceResponseTypeDef = TypedDict(
     "UpdateFlowSourceResponseTypeDef",
     {
         "FlowArn": str,
         "Source": SourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFlowResponseTypeDef = TypedDict(
     "CreateFlowResponseTypeDef",
     {
         "Flow": FlowTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFlowResponseTypeDef = TypedDict(
     "DescribeFlowResponseTypeDef",
     {
         "Flow": FlowTypeDef,
         "Messages": MessagesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFlowResponseTypeDef = TypedDict(
     "UpdateFlowResponseTypeDef",
     {
         "Flow": FlowTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/type_defs.pyi` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -50,107 +50,114 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "VpcInterfaceAttachmentTypeDef",
     "AddBridgeNetworkOutputRequestTypeDef",
     "AddBridgeNetworkSourceRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AddEgressGatewayBridgeRequestTypeDef",
     "VpcInterfaceRequestTypeDef",
     "VpcInterfaceTypeDef",
     "AddIngressGatewayBridgeRequestTypeDef",
     "AddMaintenanceTypeDef",
     "EncryptionTypeDef",
     "BridgeFlowOutputTypeDef",
     "BridgeNetworkOutputTypeDef",
     "BridgeNetworkSourceTypeDef",
     "EgressGatewayBridgeTypeDef",
     "IngressGatewayBridgeTypeDef",
     "MessageDetailTypeDef",
     "GatewayNetworkTypeDef",
     "DeleteBridgeRequestRequestTypeDef",
+    "DeleteBridgeResponseTypeDef",
     "DeleteFlowRequestRequestTypeDef",
+    "DeleteFlowResponseTypeDef",
     "DeleteGatewayRequestRequestTypeDef",
+    "DeleteGatewayResponseTypeDef",
     "DeregisterGatewayInstanceRequestRequestTypeDef",
+    "DeregisterGatewayInstanceResponseTypeDef",
     "DescribeBridgeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeFlowRequestRequestTypeDef",
     "MessagesTypeDef",
     "DescribeGatewayInstanceRequestRequestTypeDef",
     "DescribeGatewayRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
     "InterfaceRequestTypeDef",
     "InterfaceTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncodingParametersRequestTypeDef",
     "EncodingParametersTypeDef",
     "SourcePriorityTypeDef",
     "MaintenanceTypeDef",
     "FmtpRequestTypeDef",
     "FmtpTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListBridgesRequestListBridgesPaginateTypeDef",
     "ListBridgesRequestRequestTypeDef",
     "ListedBridgeTypeDef",
+    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
     "ListEntitlementsRequestRequestTypeDef",
     "ListedEntitlementTypeDef",
+    "ListFlowsRequestListFlowsPaginateTypeDef",
     "ListFlowsRequestRequestTypeDef",
+    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
     "ListGatewayInstancesRequestRequestTypeDef",
     "ListedGatewayInstanceTypeDef",
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
     "ListGatewaysRequestRequestTypeDef",
     "ListedGatewayTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
+    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ResourceSpecificationTypeDef",
     "TransportTypeDef",
+    "PaginatorConfigTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
     "RemoveBridgeOutputRequestRequestTypeDef",
+    "RemoveBridgeOutputResponseTypeDef",
     "RemoveBridgeSourceRequestRequestTypeDef",
+    "RemoveBridgeSourceResponseTypeDef",
     "RemoveFlowMediaStreamRequestRequestTypeDef",
+    "RemoveFlowMediaStreamResponseTypeDef",
     "RemoveFlowOutputRequestRequestTypeDef",
+    "RemoveFlowOutputResponseTypeDef",
     "RemoveFlowSourceRequestRequestTypeDef",
+    "RemoveFlowSourceResponseTypeDef",
     "RemoveFlowVpcInterfaceRequestRequestTypeDef",
+    "RemoveFlowVpcInterfaceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeFlowEntitlementRequestRequestTypeDef",
+    "RevokeFlowEntitlementResponseTypeDef",
     "StartFlowRequestRequestTypeDef",
+    "StartFlowResponseTypeDef",
     "StopFlowRequestRequestTypeDef",
+    "StopFlowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBridgeNetworkOutputRequestTypeDef",
     "UpdateBridgeNetworkSourceRequestTypeDef",
     "UpdateEgressGatewayBridgeRequestTypeDef",
     "UpdateIngressGatewayBridgeRequestTypeDef",
     "UpdateBridgeStateRequestRequestTypeDef",
+    "UpdateBridgeStateResponseTypeDef",
     "UpdateEncryptionTypeDef",
     "UpdateMaintenanceTypeDef",
     "UpdateGatewayInstanceRequestRequestTypeDef",
+    "UpdateGatewayInstanceResponseTypeDef",
     "AddBridgeFlowSourceRequestTypeDef",
     "BridgeFlowSourceTypeDef",
     "GatewayBridgeSourceTypeDef",
     "SetGatewayBridgeSourceRequestTypeDef",
     "UpdateBridgeFlowSourceRequestTypeDef",
     "UpdateGatewayBridgeSourceRequestTypeDef",
     "AddBridgeOutputRequestTypeDef",
-    "DeleteBridgeResponseTypeDef",
-    "DeleteFlowResponseTypeDef",
-    "DeleteGatewayResponseTypeDef",
-    "DeregisterGatewayInstanceResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RemoveBridgeOutputResponseTypeDef",
-    "RemoveBridgeSourceResponseTypeDef",
-    "RemoveFlowMediaStreamResponseTypeDef",
-    "RemoveFlowOutputResponseTypeDef",
-    "RemoveFlowSourceResponseTypeDef",
-    "RemoveFlowVpcInterfaceResponseTypeDef",
-    "RevokeFlowEntitlementResponseTypeDef",
-    "StartFlowResponseTypeDef",
-    "StopFlowResponseTypeDef",
-    "UpdateBridgeStateResponseTypeDef",
-    "UpdateGatewayInstanceResponseTypeDef",
     "AddFlowVpcInterfacesRequestRequestTypeDef",
     "AddFlowVpcInterfacesResponseTypeDef",
     "EntitlementTypeDef",
     "GrantEntitlementRequestTypeDef",
     "BridgeOutputTypeDef",
     "GatewayInstanceTypeDef",
     "CreateGatewayRequestRequestTypeDef",
@@ -163,21 +170,14 @@
     "DestinationConfigurationTypeDef",
     "InputConfigurationTypeDef",
     "FailoverConfigTypeDef",
     "UpdateFailoverConfigTypeDef",
     "ListedFlowTypeDef",
     "MediaStreamAttributesRequestTypeDef",
     "MediaStreamAttributesTypeDef",
-    "ListBridgesRequestListBridgesPaginateTypeDef",
-    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
-    "ListFlowsRequestListFlowsPaginateTypeDef",
-    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
-    "ListGatewaysRequestListGatewaysPaginateTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListBridgesResponseTypeDef",
     "ListEntitlementsResponseTypeDef",
     "ListGatewayInstancesResponseTypeDef",
     "ListGatewaysResponseTypeDef",
     "OfferingTypeDef",
     "ReservationTypeDef",
     "UpdateBridgeOutputRequestRequestTypeDef",
@@ -266,25 +266,14 @@
         "Name": str,
         "NetworkName": str,
         "Port": int,
         "Protocol": ProtocolType,
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
 AddEgressGatewayBridgeRequestTypeDef = TypedDict(
     "AddEgressGatewayBridgeRequestTypeDef",
     {
         "MaxBitrate": int,
     },
 )
 
@@ -462,28 +451,53 @@
 DeleteBridgeRequestRequestTypeDef = TypedDict(
     "DeleteBridgeRequestRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 
+DeleteBridgeResponseTypeDef = TypedDict(
+    "DeleteBridgeResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteFlowRequestRequestTypeDef = TypedDict(
     "DeleteFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
+DeleteFlowResponseTypeDef = TypedDict(
+    "DeleteFlowResponseTypeDef",
+    {
+        "FlowArn": str,
+        "Status": StatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteGatewayRequestRequestTypeDef = TypedDict(
     "DeleteGatewayRequestRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
+DeleteGatewayResponseTypeDef = TypedDict(
+    "DeleteGatewayResponseTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeregisterGatewayInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterGatewayInstanceRequestRequestTypeDef",
     {
         "GatewayInstanceArn": str,
     },
 )
 _OptionalDeregisterGatewayInstanceRequestRequestTypeDef = TypedDict(
@@ -496,14 +510,23 @@
 
 class DeregisterGatewayInstanceRequestRequestTypeDef(
     _RequiredDeregisterGatewayInstanceRequestRequestTypeDef,
     _OptionalDeregisterGatewayInstanceRequestRequestTypeDef,
 ):
     pass
 
+DeregisterGatewayInstanceResponseTypeDef = TypedDict(
+    "DeregisterGatewayInstanceResponseTypeDef",
+    {
+        "GatewayInstanceArn": str,
+        "InstanceState": InstanceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeBridgeRequestRequestTypeDef = TypedDict(
     "DescribeBridgeRequestRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 
@@ -568,14 +591,21 @@
 InterfaceTypeDef = TypedDict(
     "InterfaceTypeDef",
     {
         "Name": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncodingParametersRequestTypeDef = TypedDict(
     "EncodingParametersRequestTypeDef",
     {
         "CompressionFactor": float,
         "EncoderProfile": EncoderProfileType,
     },
 )
@@ -631,20 +661,19 @@
         "Range": RangeType,
         "ScanMode": ScanModeType,
         "Tcs": TcsType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListBridgesRequestListBridgesPaginateTypeDef = TypedDict(
+    "ListBridgesRequestListBridgesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "FilterArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBridgesRequestRequestTypeDef = TypedDict(
     "ListBridgesRequestRequestTypeDef",
     {
@@ -662,14 +691,22 @@
         "BridgeState": BridgeStateType,
         "BridgeType": str,
         "Name": str,
         "PlacementArn": str,
     },
 )
 
+ListEntitlementsRequestListEntitlementsPaginateTypeDef = TypedDict(
+    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEntitlementsRequestRequestTypeDef = TypedDict(
     "ListEntitlementsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -691,23 +728,40 @@
 )
 
 class ListedEntitlementTypeDef(
     _RequiredListedEntitlementTypeDef, _OptionalListedEntitlementTypeDef
 ):
     pass
 
+ListFlowsRequestListFlowsPaginateTypeDef = TypedDict(
+    "ListFlowsRequestListFlowsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFlowsRequestRequestTypeDef = TypedDict(
     "ListFlowsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef = TypedDict(
+    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
+    {
+        "FilterArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGatewayInstancesRequestRequestTypeDef = TypedDict(
     "ListGatewayInstancesRequestRequestTypeDef",
     {
         "FilterArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -731,14 +785,22 @@
 )
 
 class ListedGatewayInstanceTypeDef(
     _RequiredListedGatewayInstanceTypeDef, _OptionalListedGatewayInstanceTypeDef
 ):
     pass
 
+ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGatewaysRequestRequestTypeDef = TypedDict(
     "ListGatewaysRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -749,23 +811,39 @@
     {
         "GatewayArn": str,
         "GatewayState": GatewayStateType,
         "Name": str,
     },
 )
 
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
+    "ListReservationsRequestListReservationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReservationsRequestRequestTypeDef = TypedDict(
     "ListReservationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -774,14 +852,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredResourceSpecificationTypeDef = TypedDict(
     "_RequiredResourceSpecificationTypeDef",
     {
         "ResourceType": Literal["Mbps_Outbound_Bandwidth"],
     },
 )
 _OptionalResourceSpecificationTypeDef = TypedDict(
@@ -821,14 +907,24 @@
     },
     total=False,
 )
 
 class TransportTypeDef(_RequiredTransportTypeDef, _OptionalTransportTypeDef):
     pass
 
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
 PurchaseOfferingRequestRequestTypeDef = TypedDict(
     "PurchaseOfferingRequestRequestTypeDef",
     {
         "OfferingArn": str,
         "ReservationName": str,
         "Start": str,
     },
@@ -838,76 +934,169 @@
     "RemoveBridgeOutputRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "OutputName": str,
     },
 )
 
+RemoveBridgeOutputResponseTypeDef = TypedDict(
+    "RemoveBridgeOutputResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "OutputName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveBridgeSourceRequestRequestTypeDef = TypedDict(
     "RemoveBridgeSourceRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "SourceName": str,
     },
 )
 
+RemoveBridgeSourceResponseTypeDef = TypedDict(
+    "RemoveBridgeSourceResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "SourceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveFlowMediaStreamRequestRequestTypeDef = TypedDict(
     "RemoveFlowMediaStreamRequestRequestTypeDef",
     {
         "FlowArn": str,
         "MediaStreamName": str,
     },
 )
 
+RemoveFlowMediaStreamResponseTypeDef = TypedDict(
+    "RemoveFlowMediaStreamResponseTypeDef",
+    {
+        "FlowArn": str,
+        "MediaStreamName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveFlowOutputRequestRequestTypeDef = TypedDict(
     "RemoveFlowOutputRequestRequestTypeDef",
     {
         "FlowArn": str,
         "OutputArn": str,
     },
 )
 
+RemoveFlowOutputResponseTypeDef = TypedDict(
+    "RemoveFlowOutputResponseTypeDef",
+    {
+        "FlowArn": str,
+        "OutputArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveFlowSourceRequestRequestTypeDef = TypedDict(
     "RemoveFlowSourceRequestRequestTypeDef",
     {
         "FlowArn": str,
         "SourceArn": str,
     },
 )
 
+RemoveFlowSourceResponseTypeDef = TypedDict(
+    "RemoveFlowSourceResponseTypeDef",
+    {
+        "FlowArn": str,
+        "SourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveFlowVpcInterfaceRequestRequestTypeDef = TypedDict(
     "RemoveFlowVpcInterfaceRequestRequestTypeDef",
     {
         "FlowArn": str,
         "VpcInterfaceName": str,
     },
 )
 
+RemoveFlowVpcInterfaceResponseTypeDef = TypedDict(
+    "RemoveFlowVpcInterfaceResponseTypeDef",
+    {
+        "FlowArn": str,
+        "NonDeletedNetworkInterfaceIds": List[str],
+        "VpcInterfaceName": str,
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
 RevokeFlowEntitlementRequestRequestTypeDef = TypedDict(
     "RevokeFlowEntitlementRequestRequestTypeDef",
     {
         "EntitlementArn": str,
         "FlowArn": str,
     },
 )
 
+RevokeFlowEntitlementResponseTypeDef = TypedDict(
+    "RevokeFlowEntitlementResponseTypeDef",
+    {
+        "EntitlementArn": str,
+        "FlowArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartFlowRequestRequestTypeDef = TypedDict(
     "StartFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
+StartFlowResponseTypeDef = TypedDict(
+    "StartFlowResponseTypeDef",
+    {
+        "FlowArn": str,
+        "Status": StatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopFlowRequestRequestTypeDef = TypedDict(
     "StopFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
+StopFlowResponseTypeDef = TypedDict(
+    "StopFlowResponseTypeDef",
+    {
+        "FlowArn": str,
+        "Status": StatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -964,14 +1153,23 @@
     "UpdateBridgeStateRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "DesiredState": DesiredStateType,
     },
 )
 
+UpdateBridgeStateResponseTypeDef = TypedDict(
+    "UpdateBridgeStateResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "DesiredState": DesiredStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateEncryptionTypeDef = TypedDict(
     "UpdateEncryptionTypeDef",
     {
         "Algorithm": AlgorithmType,
         "ConstantInitializationVector": str,
         "DeviceId": str,
         "KeyType": KeyTypeType,
@@ -1010,14 +1208,23 @@
 
 class UpdateGatewayInstanceRequestRequestTypeDef(
     _RequiredUpdateGatewayInstanceRequestRequestTypeDef,
     _OptionalUpdateGatewayInstanceRequestRequestTypeDef,
 ):
     pass
 
+UpdateGatewayInstanceResponseTypeDef = TypedDict(
+    "UpdateGatewayInstanceResponseTypeDef",
+    {
+        "BridgePlacement": BridgePlacementType,
+        "GatewayInstanceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAddBridgeFlowSourceRequestTypeDef = TypedDict(
     "_RequiredAddBridgeFlowSourceRequestTypeDef",
     {
         "FlowArn": str,
         "Name": str,
     },
 )
@@ -1113,177 +1320,28 @@
     "AddBridgeOutputRequestTypeDef",
     {
         "NetworkOutput": AddBridgeNetworkOutputRequestTypeDef,
     },
     total=False,
 )
 
-DeleteBridgeResponseTypeDef = TypedDict(
-    "DeleteBridgeResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFlowResponseTypeDef = TypedDict(
-    "DeleteFlowResponseTypeDef",
-    {
-        "FlowArn": str,
-        "Status": StatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteGatewayResponseTypeDef = TypedDict(
-    "DeleteGatewayResponseTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeregisterGatewayInstanceResponseTypeDef = TypedDict(
-    "DeregisterGatewayInstanceResponseTypeDef",
-    {
-        "GatewayInstanceArn": str,
-        "InstanceState": InstanceStateType,
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
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveBridgeOutputResponseTypeDef = TypedDict(
-    "RemoveBridgeOutputResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "OutputName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveBridgeSourceResponseTypeDef = TypedDict(
-    "RemoveBridgeSourceResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "SourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveFlowMediaStreamResponseTypeDef = TypedDict(
-    "RemoveFlowMediaStreamResponseTypeDef",
-    {
-        "FlowArn": str,
-        "MediaStreamName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveFlowOutputResponseTypeDef = TypedDict(
-    "RemoveFlowOutputResponseTypeDef",
-    {
-        "FlowArn": str,
-        "OutputArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveFlowSourceResponseTypeDef = TypedDict(
-    "RemoveFlowSourceResponseTypeDef",
-    {
-        "FlowArn": str,
-        "SourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveFlowVpcInterfaceResponseTypeDef = TypedDict(
-    "RemoveFlowVpcInterfaceResponseTypeDef",
-    {
-        "FlowArn": str,
-        "NonDeletedNetworkInterfaceIds": List[str],
-        "VpcInterfaceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RevokeFlowEntitlementResponseTypeDef = TypedDict(
-    "RevokeFlowEntitlementResponseTypeDef",
-    {
-        "EntitlementArn": str,
-        "FlowArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartFlowResponseTypeDef = TypedDict(
-    "StartFlowResponseTypeDef",
-    {
-        "FlowArn": str,
-        "Status": StatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopFlowResponseTypeDef = TypedDict(
-    "StopFlowResponseTypeDef",
-    {
-        "FlowArn": str,
-        "Status": StatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateBridgeStateResponseTypeDef = TypedDict(
-    "UpdateBridgeStateResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "DesiredState": DesiredStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGatewayInstanceResponseTypeDef = TypedDict(
-    "UpdateGatewayInstanceResponseTypeDef",
-    {
-        "BridgePlacement": BridgePlacementType,
-        "GatewayInstanceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AddFlowVpcInterfacesRequestRequestTypeDef = TypedDict(
     "AddFlowVpcInterfacesRequestRequestTypeDef",
     {
         "FlowArn": str,
         "VpcInterfaces": Sequence[VpcInterfaceRequestTypeDef],
     },
 )
 
 AddFlowVpcInterfacesResponseTypeDef = TypedDict(
     "AddFlowVpcInterfacesResponseTypeDef",
     {
         "FlowArn": str,
         "VpcInterfaces": List[VpcInterfaceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEntitlementTypeDef = TypedDict(
     "_RequiredEntitlementTypeDef",
     {
         "EntitlementArn": str,
@@ -1554,105 +1612,47 @@
 )
 
 class MediaStreamAttributesTypeDef(
     _RequiredMediaStreamAttributesTypeDef, _OptionalMediaStreamAttributesTypeDef
 ):
     pass
 
-ListBridgesRequestListBridgesPaginateTypeDef = TypedDict(
-    "ListBridgesRequestListBridgesPaginateTypeDef",
-    {
-        "FilterArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEntitlementsRequestListEntitlementsPaginateTypeDef = TypedDict(
-    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFlowsRequestListFlowsPaginateTypeDef = TypedDict(
-    "ListFlowsRequestListFlowsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef = TypedDict(
-    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
-    {
-        "FilterArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysRequestListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
-    "ListReservationsRequestListReservationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListBridgesResponseTypeDef = TypedDict(
     "ListBridgesResponseTypeDef",
     {
         "Bridges": List[ListedBridgeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEntitlementsResponseTypeDef = TypedDict(
     "ListEntitlementsResponseTypeDef",
     {
         "Entitlements": List[ListedEntitlementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGatewayInstancesResponseTypeDef = TypedDict(
     "ListGatewayInstancesResponseTypeDef",
     {
         "Instances": List[ListedGatewayInstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGatewaysResponseTypeDef = TypedDict(
     "ListGatewaysResponseTypeDef",
     {
         "Gateways": List[ListedGatewayTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "CurrencyCode": str,
@@ -1779,24 +1779,24 @@
 )
 
 GrantFlowEntitlementsResponseTypeDef = TypedDict(
     "GrantFlowEntitlementsResponseTypeDef",
     {
         "Entitlements": List[EntitlementTypeDef],
         "FlowArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFlowEntitlementResponseTypeDef = TypedDict(
     "UpdateFlowEntitlementResponseTypeDef",
     {
         "Entitlement": EntitlementTypeDef,
         "FlowArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GrantFlowEntitlementsRequestRequestTypeDef = TypedDict(
     "GrantFlowEntitlementsRequestRequestTypeDef",
     {
         "Entitlements": Sequence[GrantEntitlementRequestTypeDef],
@@ -1805,48 +1805,48 @@
 )
 
 AddBridgeOutputsResponseTypeDef = TypedDict(
     "AddBridgeOutputsResponseTypeDef",
     {
         "BridgeArn": str,
         "Outputs": List[BridgeOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBridgeOutputResponseTypeDef = TypedDict(
     "UpdateBridgeOutputResponseTypeDef",
     {
         "BridgeArn": str,
         "Output": BridgeOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGatewayInstanceResponseTypeDef = TypedDict(
     "DescribeGatewayInstanceResponseTypeDef",
     {
         "GatewayInstance": GatewayInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateGatewayResponseTypeDef = TypedDict(
     "CreateGatewayResponseTypeDef",
     {
         "Gateway": GatewayTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGatewayResponseTypeDef = TypedDict(
     "DescribeGatewayResponseTypeDef",
     {
         "Gateway": GatewayTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMediaStreamOutputConfigurationRequestTypeDef = TypedDict(
     "_RequiredMediaStreamOutputConfigurationRequestTypeDef",
     {
         "EncodingName": EncodingNameType,
@@ -1972,15 +1972,15 @@
     pass
 
 ListFlowsResponseTypeDef = TypedDict(
     "ListFlowsResponseTypeDef",
     {
         "Flows": List[ListedFlowTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAddMediaStreamRequestTypeDef = TypedDict(
     "_RequiredAddMediaStreamRequestTypeDef",
     {
         "MediaStreamId": int,
@@ -2052,49 +2052,49 @@
 class MediaStreamTypeDef(_RequiredMediaStreamTypeDef, _OptionalMediaStreamTypeDef):
     pass
 
 DescribeOfferingResponseTypeDef = TypedDict(
     "DescribeOfferingResponseTypeDef",
     {
         "Offering": OfferingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOfferingsResponseTypeDef = TypedDict(
     "ListOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "Offerings": List[OfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservationResponseTypeDef = TypedDict(
     "DescribeReservationResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReservationsResponseTypeDef = TypedDict(
     "ListReservationsResponseTypeDef",
     {
         "NextToken": str,
         "Reservations": List[ReservationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PurchaseOfferingResponseTypeDef = TypedDict(
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddBridgeSourcesRequestRequestTypeDef = TypedDict(
     "AddBridgeSourcesRequestRequestTypeDef",
     {
         "BridgeArn": str,
@@ -2127,15 +2127,15 @@
     pass
 
 AddBridgeSourcesResponseTypeDef = TypedDict(
     "AddBridgeSourcesResponseTypeDef",
     {
         "BridgeArn": str,
         "Sources": List[BridgeSourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBridgeTypeDef = TypedDict(
     "_RequiredBridgeTypeDef",
     {
         "BridgeArn": str,
@@ -2161,15 +2161,15 @@
     pass
 
 UpdateBridgeSourceResponseTypeDef = TypedDict(
     "UpdateBridgeSourceResponseTypeDef",
     {
         "BridgeArn": str,
         "Source": BridgeSourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAddOutputRequestTypeDef = TypedDict(
     "_RequiredAddOutputRequestTypeDef",
     {
         "Protocol": ProtocolType,
@@ -2365,48 +2365,48 @@
 )
 
 AddFlowMediaStreamsResponseTypeDef = TypedDict(
     "AddFlowMediaStreamsResponseTypeDef",
     {
         "FlowArn": str,
         "MediaStreams": List[MediaStreamTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFlowMediaStreamResponseTypeDef = TypedDict(
     "UpdateFlowMediaStreamResponseTypeDef",
     {
         "FlowArn": str,
         "MediaStream": MediaStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBridgeResponseTypeDef = TypedDict(
     "CreateBridgeResponseTypeDef",
     {
         "Bridge": BridgeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBridgeResponseTypeDef = TypedDict(
     "DescribeBridgeResponseTypeDef",
     {
         "Bridge": BridgeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBridgeResponseTypeDef = TypedDict(
     "UpdateBridgeResponseTypeDef",
     {
         "Bridge": BridgeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddFlowOutputsRequestRequestTypeDef = TypedDict(
     "AddFlowOutputsRequestRequestTypeDef",
     {
         "FlowArn": str,
@@ -2450,33 +2450,33 @@
     pass
 
 AddFlowOutputsResponseTypeDef = TypedDict(
     "AddFlowOutputsResponseTypeDef",
     {
         "FlowArn": str,
         "Outputs": List[OutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFlowOutputResponseTypeDef = TypedDict(
     "UpdateFlowOutputResponseTypeDef",
     {
         "FlowArn": str,
         "Output": OutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddFlowSourcesResponseTypeDef = TypedDict(
     "AddFlowSourcesResponseTypeDef",
     {
         "FlowArn": str,
         "Sources": List[SourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFlowTypeDef = TypedDict(
     "_RequiredFlowTypeDef",
     {
         "AvailabilityZone": str,
@@ -2506,35 +2506,35 @@
     pass
 
 UpdateFlowSourceResponseTypeDef = TypedDict(
     "UpdateFlowSourceResponseTypeDef",
     {
         "FlowArn": str,
         "Source": SourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFlowResponseTypeDef = TypedDict(
     "CreateFlowResponseTypeDef",
     {
         "Flow": FlowTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFlowResponseTypeDef = TypedDict(
     "DescribeFlowResponseTypeDef",
     {
         "Flow": FlowTypeDef,
         "Messages": MessagesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFlowResponseTypeDef = TypedDict(
     "UpdateFlowResponseTypeDef",
     {
         "Flow": FlowTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/waiter.py` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/waiter.pyi` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/PKG-INFO` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconnect
-Version: 1.26.113
-Summary: Type annotations for boto3.MediaConnect 1.26.113 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.MediaConnect 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConnect 1.26.113](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[boto3.MediaConnect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -398,107 +398,114 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconnect.type_defs import (
     VpcInterfaceAttachmentTypeDef,
     AddBridgeNetworkOutputRequestTypeDef,
     AddBridgeNetworkSourceRequestTypeDef,
-    ResponseMetadataTypeDef,
     AddEgressGatewayBridgeRequestTypeDef,
     VpcInterfaceRequestTypeDef,
     VpcInterfaceTypeDef,
     AddIngressGatewayBridgeRequestTypeDef,
     AddMaintenanceTypeDef,
     EncryptionTypeDef,
     BridgeFlowOutputTypeDef,
     BridgeNetworkOutputTypeDef,
     BridgeNetworkSourceTypeDef,
     EgressGatewayBridgeTypeDef,
     IngressGatewayBridgeTypeDef,
     MessageDetailTypeDef,
     GatewayNetworkTypeDef,
     DeleteBridgeRequestRequestTypeDef,
+    DeleteBridgeResponseTypeDef,
     DeleteFlowRequestRequestTypeDef,
+    DeleteFlowResponseTypeDef,
     DeleteGatewayRequestRequestTypeDef,
+    DeleteGatewayResponseTypeDef,
     DeregisterGatewayInstanceRequestRequestTypeDef,
+    DeregisterGatewayInstanceResponseTypeDef,
     DescribeBridgeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeFlowRequestRequestTypeDef,
     MessagesTypeDef,
     DescribeGatewayInstanceRequestRequestTypeDef,
     DescribeGatewayRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
     InterfaceRequestTypeDef,
     InterfaceTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncodingParametersRequestTypeDef,
     EncodingParametersTypeDef,
     SourcePriorityTypeDef,
     MaintenanceTypeDef,
     FmtpRequestTypeDef,
     FmtpTypeDef,
-    PaginatorConfigTypeDef,
+    ListBridgesRequestListBridgesPaginateTypeDef,
     ListBridgesRequestRequestTypeDef,
     ListedBridgeTypeDef,
+    ListEntitlementsRequestListEntitlementsPaginateTypeDef,
     ListEntitlementsRequestRequestTypeDef,
     ListedEntitlementTypeDef,
+    ListFlowsRequestListFlowsPaginateTypeDef,
     ListFlowsRequestRequestTypeDef,
+    ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef,
     ListGatewayInstancesRequestRequestTypeDef,
     ListedGatewayInstanceTypeDef,
+    ListGatewaysRequestListGatewaysPaginateTypeDef,
     ListGatewaysRequestRequestTypeDef,
     ListedGatewayTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ResourceSpecificationTypeDef,
     TransportTypeDef,
+    PaginatorConfigTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
     RemoveBridgeOutputRequestRequestTypeDef,
+    RemoveBridgeOutputResponseTypeDef,
     RemoveBridgeSourceRequestRequestTypeDef,
+    RemoveBridgeSourceResponseTypeDef,
     RemoveFlowMediaStreamRequestRequestTypeDef,
+    RemoveFlowMediaStreamResponseTypeDef,
     RemoveFlowOutputRequestRequestTypeDef,
+    RemoveFlowOutputResponseTypeDef,
     RemoveFlowSourceRequestRequestTypeDef,
+    RemoveFlowSourceResponseTypeDef,
     RemoveFlowVpcInterfaceRequestRequestTypeDef,
+    RemoveFlowVpcInterfaceResponseTypeDef,
+    ResponseMetadataTypeDef,
     RevokeFlowEntitlementRequestRequestTypeDef,
+    RevokeFlowEntitlementResponseTypeDef,
     StartFlowRequestRequestTypeDef,
+    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
+    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBridgeNetworkOutputRequestTypeDef,
     UpdateBridgeNetworkSourceRequestTypeDef,
     UpdateEgressGatewayBridgeRequestTypeDef,
     UpdateIngressGatewayBridgeRequestTypeDef,
     UpdateBridgeStateRequestRequestTypeDef,
+    UpdateBridgeStateResponseTypeDef,
     UpdateEncryptionTypeDef,
     UpdateMaintenanceTypeDef,
     UpdateGatewayInstanceRequestRequestTypeDef,
+    UpdateGatewayInstanceResponseTypeDef,
     AddBridgeFlowSourceRequestTypeDef,
     BridgeFlowSourceTypeDef,
     GatewayBridgeSourceTypeDef,
     SetGatewayBridgeSourceRequestTypeDef,
     UpdateBridgeFlowSourceRequestTypeDef,
     UpdateGatewayBridgeSourceRequestTypeDef,
     AddBridgeOutputRequestTypeDef,
-    DeleteBridgeResponseTypeDef,
-    DeleteFlowResponseTypeDef,
-    DeleteGatewayResponseTypeDef,
-    DeregisterGatewayInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RemoveBridgeOutputResponseTypeDef,
-    RemoveBridgeSourceResponseTypeDef,
-    RemoveFlowMediaStreamResponseTypeDef,
-    RemoveFlowOutputResponseTypeDef,
-    RemoveFlowSourceResponseTypeDef,
-    RemoveFlowVpcInterfaceResponseTypeDef,
-    RevokeFlowEntitlementResponseTypeDef,
-    StartFlowResponseTypeDef,
-    StopFlowResponseTypeDef,
-    UpdateBridgeStateResponseTypeDef,
-    UpdateGatewayInstanceResponseTypeDef,
     AddFlowVpcInterfacesRequestRequestTypeDef,
     AddFlowVpcInterfacesResponseTypeDef,
     EntitlementTypeDef,
     GrantEntitlementRequestTypeDef,
     BridgeOutputTypeDef,
     GatewayInstanceTypeDef,
     CreateGatewayRequestRequestTypeDef,
@@ -511,21 +518,14 @@
     DestinationConfigurationTypeDef,
     InputConfigurationTypeDef,
     FailoverConfigTypeDef,
     UpdateFailoverConfigTypeDef,
     ListedFlowTypeDef,
     MediaStreamAttributesRequestTypeDef,
     MediaStreamAttributesTypeDef,
-    ListBridgesRequestListBridgesPaginateTypeDef,
-    ListEntitlementsRequestListEntitlementsPaginateTypeDef,
-    ListFlowsRequestListFlowsPaginateTypeDef,
-    ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef,
-    ListGatewaysRequestListGatewaysPaginateTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
     ListBridgesResponseTypeDef,
     ListEntitlementsResponseTypeDef,
     ListGatewayInstancesResponseTypeDef,
     ListGatewaysResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     UpdateBridgeOutputRequestRequestTypeDef,
```

### Comparing `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/SOURCES.txt` & `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.26.113/setup.py` & `mypy-boto3-mediaconnect-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediaconnect",
-    version="1.26.113",
+    version="1.27.0",
     packages=["mypy_boto3_mediaconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaConnect 1.26.113 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.MediaConnect 1.27.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


# Comparing `tmp/mypy-boto3-vpc-lattice-1.26.107.tar.gz` & `tmp/mypy-boto3-vpc-lattice-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-vpc-lattice-1.26.107.tar", last modified: Wed Apr  5 20:26:20 2023, max compression
+gzip compressed data, was "mypy-boto3-vpc-lattice-1.27.0.tar", last modified: Mon Jul  3 19:51:35 2023, max compression
```

## Comparing `mypy-boto3-vpc-lattice-1.26.107.tar` & `mypy-boto3-vpc-lattice-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:26:20.402390 mypy-boto3-vpc-lattice-1.26.107/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-05 20:26:06.000000 mypy-boto3-vpc-lattice-1.26.107/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20224 2023-04-05 20:26:20.390389 mypy-boto3-vpc-lattice-1.26.107/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-04-05 20:26:06.000000 mypy-boto3-vpc-lattice-1.26.107/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:26:20.390389 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-05 20:26:06.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-05 20:26:06.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-05 20:26:06.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38846 2023-04-05 20:26:07.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38778 2023-04-05 20:26:06.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-04-05 20:26:07.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-04-05 20:26:07.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-04-05 20:26:07.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-04-05 20:26:07.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 20:26:06.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48577 2023-04-05 20:26:08.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48528 2023-04-05 20:26:08.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-05 20:26:06.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:26:20.390389 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20224 2023-04-05 20:26:20.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-05 20:26:20.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 20:26:20.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 20:26:20.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-05 20:26:20.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-05 20:26:20.000000 mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 20:26:20.402390 mypy-boto3-vpc-lattice-1.26.107/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-05 20:26:06.000000 mypy-boto3-vpc-lattice-1.26.107/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.512131 mypy-boto3-vpc-lattice-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:20.000000 mypy-boto3-vpc-lattice-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20218 2023-07-03 19:51:35.512131 mypy-boto3-vpc-lattice-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-07-03 19:49:20.000000 mypy-boto3-vpc-lattice-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.504131 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-03 19:49:20.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-03 19:49:20.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-03 19:49:20.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38846 2023-07-03 19:49:23.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38778 2023-07-03 19:49:20.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-07-03 19:49:23.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-07-03 19:49:23.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-07-03 19:49:23.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-07-03 19:49:23.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:20.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48681 2023-07-03 19:49:24.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48632 2023-07-03 19:49:23.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:20.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.512131 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20218 2023-07-03 19:51:35.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-03 19:51:35.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:35.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 19:51:35.000000 mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:35.512131 mypy-boto3-vpc-lattice-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-03 19:49:20.000000 mypy-boto3-vpc-lattice-1.27.0/setup.py
```

### Comparing `mypy-boto3-vpc-lattice-1.26.107/LICENSE` & `mypy-boto3-vpc-lattice-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.26.107/PKG-INFO` & `mypy-boto3-vpc-lattice-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-vpc-lattice
-Version: 1.26.107
-Summary: Type annotations for boto3.VPCLattice 1.26.107 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.VPCLattice 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-vpc-lattice?color=blue)](https://pypistats.org/packages/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.26.107](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -366,115 +366,115 @@
 
 `mypy_boto3_vpc_lattice.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_vpc_lattice.type_defs import (
     AccessLogSubscriptionSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RuleUpdateFailureTypeDef,
     CreateAccessLogSubscriptionRequestRequestTypeDef,
+    CreateAccessLogSubscriptionResponseTypeDef,
     CreateServiceNetworkRequestRequestTypeDef,
+    CreateServiceNetworkResponseTypeDef,
     CreateServiceNetworkServiceAssociationRequestRequestTypeDef,
     DnsEntryTypeDef,
     CreateServiceNetworkVpcAssociationRequestRequestTypeDef,
+    CreateServiceNetworkVpcAssociationResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     DeleteAccessLogSubscriptionRequestRequestTypeDef,
     DeleteAuthPolicyRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteServiceNetworkRequestRequestTypeDef,
     DeleteServiceNetworkServiceAssociationRequestRequestTypeDef,
+    DeleteServiceNetworkServiceAssociationResponseTypeDef,
     DeleteServiceNetworkVpcAssociationRequestRequestTypeDef,
+    DeleteServiceNetworkVpcAssociationResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
+    DeleteServiceResponseTypeDef,
     DeleteTargetGroupRequestRequestTypeDef,
+    DeleteTargetGroupResponseTypeDef,
     TargetTypeDef,
     TargetFailureTypeDef,
     FixedResponseActionTypeDef,
     WeightedTargetGroupTypeDef,
     GetAccessLogSubscriptionRequestRequestTypeDef,
+    GetAccessLogSubscriptionResponseTypeDef,
     GetAuthPolicyRequestRequestTypeDef,
+    GetAuthPolicyResponseTypeDef,
     GetListenerRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetRuleRequestRequestTypeDef,
     GetServiceNetworkRequestRequestTypeDef,
+    GetServiceNetworkResponseTypeDef,
     GetServiceNetworkServiceAssociationRequestRequestTypeDef,
     GetServiceNetworkVpcAssociationRequestRequestTypeDef,
+    GetServiceNetworkVpcAssociationResponseTypeDef,
     GetServiceRequestRequestTypeDef,
     GetTargetGroupRequestRequestTypeDef,
     HeaderMatchTypeTypeDef,
     MatcherTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
     ListAccessLogSubscriptionsRequestRequestTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListenerSummaryTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
+    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
     ListServiceNetworkServiceAssociationsRequestRequestTypeDef,
+    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
     ListServiceNetworkVpcAssociationsRequestRequestTypeDef,
     ServiceNetworkVpcAssociationSummaryTypeDef,
+    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
     ListServiceNetworksRequestRequestTypeDef,
     ServiceNetworkSummaryTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
     ListTargetGroupsRequestRequestTypeDef,
     TargetGroupSummaryTypeDef,
     TargetSummaryTypeDef,
+    PaginatorConfigTypeDef,
     PathMatchTypeTypeDef,
     PutAuthPolicyRequestRequestTypeDef,
+    PutAuthPolicyResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessLogSubscriptionRequestRequestTypeDef,
-    UpdateServiceNetworkRequestRequestTypeDef,
-    UpdateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    UpdateServiceRequestRequestTypeDef,
-    CreateAccessLogSubscriptionResponseTypeDef,
-    CreateServiceNetworkResponseTypeDef,
-    CreateServiceNetworkVpcAssociationResponseTypeDef,
-    DeleteServiceNetworkServiceAssociationResponseTypeDef,
-    DeleteServiceNetworkVpcAssociationResponseTypeDef,
-    DeleteServiceResponseTypeDef,
-    DeleteTargetGroupResponseTypeDef,
-    GetAccessLogSubscriptionResponseTypeDef,
-    GetAuthPolicyResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetServiceNetworkResponseTypeDef,
-    GetServiceNetworkVpcAssociationResponseTypeDef,
-    ListAccessLogSubscriptionsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutAuthPolicyResponseTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
+    UpdateServiceNetworkRequestRequestTypeDef,
     UpdateServiceNetworkResponseTypeDef,
+    UpdateServiceNetworkVpcAssociationRequestRequestTypeDef,
     UpdateServiceNetworkVpcAssociationResponseTypeDef,
+    UpdateServiceRequestRequestTypeDef,
     UpdateServiceResponseTypeDef,
+    ListAccessLogSubscriptionsResponseTypeDef,
     CreateServiceNetworkServiceAssociationResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceNetworkServiceAssociationResponseTypeDef,
     GetServiceResponseTypeDef,
     ServiceNetworkServiceAssociationSummaryTypeDef,
     ServiceSummaryTypeDef,
     DeregisterTargetsRequestRequestTypeDef,
+    ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
     RegisterTargetsRequestRequestTypeDef,
     DeregisterTargetsResponseTypeDef,
     RegisterTargetsResponseTypeDef,
     ForwardActionTypeDef,
     HeaderMatchTypeDef,
     HealthCheckConfigTypeDef,
-    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
-    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
-    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
-    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
-    ListTargetsRequestListTargetsPaginateTypeDef,
     ListListenersResponseTypeDef,
     ListRulesResponseTypeDef,
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServiceNetworksResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PathMatchTypeDef,
```

### Comparing `mypy-boto3-vpc-lattice-1.26.107/README.md` & `mypy-boto3-vpc-lattice-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-vpc-lattice?color=blue)](https://pypistats.org/packages/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.26.107](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -334,115 +334,115 @@
 
 `mypy_boto3_vpc_lattice.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_vpc_lattice.type_defs import (
     AccessLogSubscriptionSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RuleUpdateFailureTypeDef,
     CreateAccessLogSubscriptionRequestRequestTypeDef,
+    CreateAccessLogSubscriptionResponseTypeDef,
     CreateServiceNetworkRequestRequestTypeDef,
+    CreateServiceNetworkResponseTypeDef,
     CreateServiceNetworkServiceAssociationRequestRequestTypeDef,
     DnsEntryTypeDef,
     CreateServiceNetworkVpcAssociationRequestRequestTypeDef,
+    CreateServiceNetworkVpcAssociationResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     DeleteAccessLogSubscriptionRequestRequestTypeDef,
     DeleteAuthPolicyRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteServiceNetworkRequestRequestTypeDef,
     DeleteServiceNetworkServiceAssociationRequestRequestTypeDef,
+    DeleteServiceNetworkServiceAssociationResponseTypeDef,
     DeleteServiceNetworkVpcAssociationRequestRequestTypeDef,
+    DeleteServiceNetworkVpcAssociationResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
+    DeleteServiceResponseTypeDef,
     DeleteTargetGroupRequestRequestTypeDef,
+    DeleteTargetGroupResponseTypeDef,
     TargetTypeDef,
     TargetFailureTypeDef,
     FixedResponseActionTypeDef,
     WeightedTargetGroupTypeDef,
     GetAccessLogSubscriptionRequestRequestTypeDef,
+    GetAccessLogSubscriptionResponseTypeDef,
     GetAuthPolicyRequestRequestTypeDef,
+    GetAuthPolicyResponseTypeDef,
     GetListenerRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetRuleRequestRequestTypeDef,
     GetServiceNetworkRequestRequestTypeDef,
+    GetServiceNetworkResponseTypeDef,
     GetServiceNetworkServiceAssociationRequestRequestTypeDef,
     GetServiceNetworkVpcAssociationRequestRequestTypeDef,
+    GetServiceNetworkVpcAssociationResponseTypeDef,
     GetServiceRequestRequestTypeDef,
     GetTargetGroupRequestRequestTypeDef,
     HeaderMatchTypeTypeDef,
     MatcherTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
     ListAccessLogSubscriptionsRequestRequestTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListenerSummaryTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
+    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
     ListServiceNetworkServiceAssociationsRequestRequestTypeDef,
+    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
     ListServiceNetworkVpcAssociationsRequestRequestTypeDef,
     ServiceNetworkVpcAssociationSummaryTypeDef,
+    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
     ListServiceNetworksRequestRequestTypeDef,
     ServiceNetworkSummaryTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
     ListTargetGroupsRequestRequestTypeDef,
     TargetGroupSummaryTypeDef,
     TargetSummaryTypeDef,
+    PaginatorConfigTypeDef,
     PathMatchTypeTypeDef,
     PutAuthPolicyRequestRequestTypeDef,
+    PutAuthPolicyResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessLogSubscriptionRequestRequestTypeDef,
-    UpdateServiceNetworkRequestRequestTypeDef,
-    UpdateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    UpdateServiceRequestRequestTypeDef,
-    CreateAccessLogSubscriptionResponseTypeDef,
-    CreateServiceNetworkResponseTypeDef,
-    CreateServiceNetworkVpcAssociationResponseTypeDef,
-    DeleteServiceNetworkServiceAssociationResponseTypeDef,
-    DeleteServiceNetworkVpcAssociationResponseTypeDef,
-    DeleteServiceResponseTypeDef,
-    DeleteTargetGroupResponseTypeDef,
-    GetAccessLogSubscriptionResponseTypeDef,
-    GetAuthPolicyResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetServiceNetworkResponseTypeDef,
-    GetServiceNetworkVpcAssociationResponseTypeDef,
-    ListAccessLogSubscriptionsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutAuthPolicyResponseTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
+    UpdateServiceNetworkRequestRequestTypeDef,
     UpdateServiceNetworkResponseTypeDef,
+    UpdateServiceNetworkVpcAssociationRequestRequestTypeDef,
     UpdateServiceNetworkVpcAssociationResponseTypeDef,
+    UpdateServiceRequestRequestTypeDef,
     UpdateServiceResponseTypeDef,
+    ListAccessLogSubscriptionsResponseTypeDef,
     CreateServiceNetworkServiceAssociationResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceNetworkServiceAssociationResponseTypeDef,
     GetServiceResponseTypeDef,
     ServiceNetworkServiceAssociationSummaryTypeDef,
     ServiceSummaryTypeDef,
     DeregisterTargetsRequestRequestTypeDef,
+    ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
     RegisterTargetsRequestRequestTypeDef,
     DeregisterTargetsResponseTypeDef,
     RegisterTargetsResponseTypeDef,
     ForwardActionTypeDef,
     HeaderMatchTypeDef,
     HealthCheckConfigTypeDef,
-    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
-    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
-    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
-    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
-    ListTargetsRequestListTargetsPaginateTypeDef,
     ListListenersResponseTypeDef,
     ListRulesResponseTypeDef,
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServiceNetworksResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PathMatchTypeDef,
```

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/__init__.py` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/__init__.pyi` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/__main__.py` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VPCLattice 1.26.107\nVersion:         1.26.107\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.VPCLattice 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.107")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/client.py` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/client.pyi` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/literals.py` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
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
@@ -147,14 +148,15 @@
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
@@ -296,14 +298,15 @@
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
@@ -322,16 +325,19 @@
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
@@ -415,14 +421,15 @@
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

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/literals.pyi` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
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
@@ -145,14 +146,15 @@
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
@@ -294,14 +296,15 @@
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
@@ -320,16 +323,19 @@
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
@@ -413,14 +419,15 @@
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

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/paginator.py` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,30 +80,30 @@
 class ListAccessLogSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListAccessLogSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listaccesslogsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, resourceIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccessLogSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListAccessLogSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listaccesslogsubscriptionspaginator)
         """
 
 
 class ListListenersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListListeners)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listlistenerspaginator)
     """
 
     def paginate(
-        self, *, serviceIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, serviceIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listlistenerspaginator)
         """
 
 
@@ -114,15 +114,15 @@
     """
 
     def paginate(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listrulespaginator)
         """
 
 
@@ -133,15 +133,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceIdentifier: str = ...,
         serviceNetworkIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceNetworkServiceAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkServiceAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkserviceassociationspaginator)
         """
 
 
@@ -152,45 +152,45 @@
     """
 
     def paginate(
         self,
         *,
         serviceNetworkIdentifier: str = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceNetworkVpcAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkVpcAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkvpcassociationspaginator)
         """
 
 
 class ListServiceNetworksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkspaginator)
         """
 
 
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicespaginator)
         """
 
 
@@ -201,15 +201,15 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupType: TargetGroupTypeType = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listtargetgroupspaginator)
         """
 
 
@@ -220,13 +220,13 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupIdentifier: str,
         targets: Sequence[TargetTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listtargetspaginator)
         """
```

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/paginator.pyi` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -77,29 +77,29 @@
 class ListAccessLogSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListAccessLogSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listaccesslogsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, resourceIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccessLogSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListAccessLogSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listaccesslogsubscriptionspaginator)
         """
 
 class ListListenersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListListeners)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listlistenerspaginator)
     """
 
     def paginate(
-        self, *, serviceIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, serviceIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listlistenerspaginator)
         """
 
 class ListRulesPaginator(Paginator):
@@ -109,15 +109,15 @@
     """
 
     def paginate(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listrulespaginator)
         """
 
 class ListServiceNetworkServiceAssociationsPaginator(Paginator):
@@ -127,15 +127,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceIdentifier: str = ...,
         serviceNetworkIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceNetworkServiceAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkServiceAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkserviceassociationspaginator)
         """
 
 class ListServiceNetworkVpcAssociationsPaginator(Paginator):
@@ -145,43 +145,43 @@
     """
 
     def paginate(
         self,
         *,
         serviceNetworkIdentifier: str = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceNetworkVpcAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkVpcAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkvpcassociationspaginator)
         """
 
 class ListServiceNetworksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkspaginator)
         """
 
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicespaginator)
         """
 
 class ListTargetGroupsPaginator(Paginator):
@@ -191,15 +191,15 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupType: TargetGroupTypeType = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listtargetgroupspaginator)
         """
 
 class ListTargetsPaginator(Paginator):
@@ -209,13 +209,13 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupIdentifier: str,
         targets: Sequence[TargetTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listtargetspaginator)
         """
```

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/type_defs.py` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,115 +35,115 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessLogSubscriptionSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "RuleUpdateFailureTypeDef",
     "CreateAccessLogSubscriptionRequestRequestTypeDef",
+    "CreateAccessLogSubscriptionResponseTypeDef",
     "CreateServiceNetworkRequestRequestTypeDef",
+    "CreateServiceNetworkResponseTypeDef",
     "CreateServiceNetworkServiceAssociationRequestRequestTypeDef",
     "DnsEntryTypeDef",
     "CreateServiceNetworkVpcAssociationRequestRequestTypeDef",
+    "CreateServiceNetworkVpcAssociationResponseTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "DeleteAccessLogSubscriptionRequestRequestTypeDef",
     "DeleteAuthPolicyRequestRequestTypeDef",
     "DeleteListenerRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteServiceNetworkRequestRequestTypeDef",
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
+    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
+    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
+    "DeleteServiceResponseTypeDef",
     "DeleteTargetGroupRequestRequestTypeDef",
+    "DeleteTargetGroupResponseTypeDef",
     "TargetTypeDef",
     "TargetFailureTypeDef",
     "FixedResponseActionTypeDef",
     "WeightedTargetGroupTypeDef",
     "GetAccessLogSubscriptionRequestRequestTypeDef",
+    "GetAccessLogSubscriptionResponseTypeDef",
     "GetAuthPolicyRequestRequestTypeDef",
+    "GetAuthPolicyResponseTypeDef",
     "GetListenerRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "GetRuleRequestRequestTypeDef",
     "GetServiceNetworkRequestRequestTypeDef",
+    "GetServiceNetworkResponseTypeDef",
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
+    "GetServiceNetworkVpcAssociationResponseTypeDef",
     "GetServiceRequestRequestTypeDef",
     "GetTargetGroupRequestRequestTypeDef",
     "HeaderMatchTypeTypeDef",
     "MatcherTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
     "ListAccessLogSubscriptionsRequestRequestTypeDef",
+    "ListListenersRequestListListenersPaginateTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListenerSummaryTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
+    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
     "ListServiceNetworkServiceAssociationsRequestRequestTypeDef",
+    "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
     "ListServiceNetworkVpcAssociationsRequestRequestTypeDef",
     "ServiceNetworkVpcAssociationSummaryTypeDef",
+    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
     "ListServiceNetworksRequestRequestTypeDef",
     "ServiceNetworkSummaryTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
     "ListTargetGroupsRequestRequestTypeDef",
     "TargetGroupSummaryTypeDef",
     "TargetSummaryTypeDef",
+    "PaginatorConfigTypeDef",
     "PathMatchTypeTypeDef",
     "PutAuthPolicyRequestRequestTypeDef",
+    "PutAuthPolicyResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
-    "UpdateServiceNetworkRequestRequestTypeDef",
-    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "UpdateServiceRequestRequestTypeDef",
-    "CreateAccessLogSubscriptionResponseTypeDef",
-    "CreateServiceNetworkResponseTypeDef",
-    "CreateServiceNetworkVpcAssociationResponseTypeDef",
-    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
-    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
-    "DeleteServiceResponseTypeDef",
-    "DeleteTargetGroupResponseTypeDef",
-    "GetAccessLogSubscriptionResponseTypeDef",
-    "GetAuthPolicyResponseTypeDef",
-    "GetResourcePolicyResponseTypeDef",
-    "GetServiceNetworkResponseTypeDef",
-    "GetServiceNetworkVpcAssociationResponseTypeDef",
-    "ListAccessLogSubscriptionsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutAuthPolicyResponseTypeDef",
     "UpdateAccessLogSubscriptionResponseTypeDef",
+    "UpdateServiceNetworkRequestRequestTypeDef",
     "UpdateServiceNetworkResponseTypeDef",
+    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
     "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+    "UpdateServiceRequestRequestTypeDef",
     "UpdateServiceResponseTypeDef",
+    "ListAccessLogSubscriptionsResponseTypeDef",
     "CreateServiceNetworkServiceAssociationResponseTypeDef",
     "CreateServiceResponseTypeDef",
     "GetServiceNetworkServiceAssociationResponseTypeDef",
     "GetServiceResponseTypeDef",
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     "ServiceSummaryTypeDef",
     "DeregisterTargetsRequestRequestTypeDef",
+    "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListTargetsRequestRequestTypeDef",
     "RegisterTargetsRequestRequestTypeDef",
     "DeregisterTargetsResponseTypeDef",
     "RegisterTargetsResponseTypeDef",
     "ForwardActionTypeDef",
     "HeaderMatchTypeDef",
     "HealthCheckConfigTypeDef",
-    "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
-    "ListListenersRequestListListenersPaginateTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
-    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
-    "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
-    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
-    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
-    "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListListenersResponseTypeDef",
     "ListRulesResponseTypeDef",
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     "ListServiceNetworksResponseTypeDef",
     "ListTargetGroupsResponseTypeDef",
     "ListTargetsResponseTypeDef",
     "PathMatchTypeDef",
@@ -183,25 +183,14 @@
         "id": str,
         "lastUpdatedAt": datetime,
         "resourceArn": str,
         "resourceId": str,
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
 RuleUpdateFailureTypeDef = TypedDict(
     "RuleUpdateFailureTypeDef",
     {
         "failureCode": str,
         "failureMessage": str,
         "ruleIdentifier": str,
     },
@@ -228,14 +217,26 @@
 class CreateAccessLogSubscriptionRequestRequestTypeDef(
     _RequiredCreateAccessLogSubscriptionRequestRequestTypeDef,
     _OptionalCreateAccessLogSubscriptionRequestRequestTypeDef,
 ):
     pass
 
 
+CreateAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "CreateAccessLogSubscriptionResponseTypeDef",
+    {
+        "arn": str,
+        "destinationArn": str,
+        "id": str,
+        "resourceArn": str,
+        "resourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateServiceNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceNetworkRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceNetworkRequestRequestTypeDef = TypedDict(
@@ -252,14 +253,25 @@
 class CreateServiceNetworkRequestRequestTypeDef(
     _RequiredCreateServiceNetworkRequestRequestTypeDef,
     _OptionalCreateServiceNetworkRequestRequestTypeDef,
 ):
     pass
 
 
+CreateServiceNetworkResponseTypeDef = TypedDict(
+    "CreateServiceNetworkResponseTypeDef",
+    {
+        "arn": str,
+        "authType": AuthTypeType,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
         "serviceNetworkIdentifier": str,
     },
 )
@@ -310,14 +322,26 @@
 class CreateServiceNetworkVpcAssociationRequestRequestTypeDef(
     _RequiredCreateServiceNetworkVpcAssociationRequestRequestTypeDef,
     _OptionalCreateServiceNetworkVpcAssociationRequestRequestTypeDef,
 ):
     pass
 
 
+CreateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "CreateServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "createdBy": str,
+        "id": str,
+        "securityGroupIds": List[str],
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceRequestRequestTypeDef = TypedDict(
@@ -387,35 +411,76 @@
 DeleteServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceNetworkServiceAssociationIdentifier": str,
     },
 )
 
+DeleteServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
+    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": ServiceNetworkServiceAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
         "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
+DeleteServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 
+DeleteServiceResponseTypeDef = TypedDict(
+    "DeleteServiceResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "status": ServiceStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTargetGroupRequestRequestTypeDef = TypedDict(
     "DeleteTargetGroupRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 
+DeleteTargetGroupResponseTypeDef = TypedDict(
+    "DeleteTargetGroupResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": TargetGroupStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "id": str,
     },
 )
 _OptionalTargetTypeDef = TypedDict(
@@ -473,21 +538,46 @@
 GetAccessLogSubscriptionRequestRequestTypeDef = TypedDict(
     "GetAccessLogSubscriptionRequestRequestTypeDef",
     {
         "accessLogSubscriptionIdentifier": str,
     },
 )
 
+GetAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "GetAccessLogSubscriptionResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "destinationArn": str,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "resourceArn": str,
+        "resourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAuthPolicyRequestRequestTypeDef = TypedDict(
     "GetAuthPolicyRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
 )
 
+GetAuthPolicyResponseTypeDef = TypedDict(
+    "GetAuthPolicyResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "policy": str,
+        "state": AuthPolicyStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetListenerRequestRequestTypeDef = TypedDict(
     "GetListenerRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
@@ -495,14 +585,22 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "ruleIdentifier": str,
         "serviceIdentifier": str,
     },
@@ -511,28 +609,63 @@
 GetServiceNetworkRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkRequestRequestTypeDef",
     {
         "serviceNetworkIdentifier": str,
     },
 )
 
+GetServiceNetworkResponseTypeDef = TypedDict(
+    "GetServiceNetworkResponseTypeDef",
+    {
+        "arn": str,
+        "authType": AuthTypeType,
+        "createdAt": datetime,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "name": str,
+        "numberOfAssociatedServices": int,
+        "numberOfAssociatedVPCs": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceNetworkServiceAssociationIdentifier": str,
     },
 )
 
 GetServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
         "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
+GetServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "GetServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "createdBy": str,
+        "failureCode": str,
+        "failureMessage": str,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "securityGroupIds": List[str],
+        "serviceNetworkArn": str,
+        "serviceNetworkId": str,
+        "serviceNetworkName": str,
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "vpcId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetServiceRequestRequestTypeDef = TypedDict(
     "GetServiceRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 
@@ -557,24 +690,36 @@
     "MatcherTypeDef",
     {
         "httpCode": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
+    "_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "resourceIdentifier": str,
+    },
+)
+_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
+    "_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(
+    _RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    _OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAccessLogSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessLogSubscriptionsRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
 )
 _OptionalListAccessLogSubscriptionsRequestRequestTypeDef = TypedDict(
@@ -590,14 +735,36 @@
 class ListAccessLogSubscriptionsRequestRequestTypeDef(
     _RequiredListAccessLogSubscriptionsRequestRequestTypeDef,
     _OptionalListAccessLogSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_RequiredListListenersRequestListListenersPaginateTypeDef",
+    {
+        "serviceIdentifier": str,
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
         "serviceIdentifier": str,
     },
 )
 _OptionalListListenersRequestRequestTypeDef = TypedDict(
@@ -626,14 +793,37 @@
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
     },
     total=False,
 )
 
+_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_RequiredListRulesRequestListRulesPaginateTypeDef",
+    {
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_OptionalListRulesRequestListRulesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRulesRequestListRulesPaginateTypeDef(
+    _RequiredListRulesRequestListRulesPaginateTypeDef,
+    _OptionalListRulesRequestListRulesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListRulesRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
@@ -663,25 +853,47 @@
         "lastUpdatedAt": datetime,
         "name": str,
         "priority": int,
     },
     total=False,
 )
 
+ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef = TypedDict(
+    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
+    {
+        "serviceIdentifier": str,
+        "serviceNetworkIdentifier": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServiceNetworkServiceAssociationsRequestRequestTypeDef = TypedDict(
     "ListServiceNetworkServiceAssociationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "serviceIdentifier": str,
         "serviceNetworkIdentifier": str,
     },
     total=False,
 )
 
+ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef = (
+    TypedDict(
+        "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
+        {
+            "serviceNetworkIdentifier": str,
+            "vpcIdentifier": str,
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
 ListServiceNetworkVpcAssociationsRequestRequestTypeDef = TypedDict(
     "ListServiceNetworkVpcAssociationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "serviceNetworkIdentifier": str,
         "vpcIdentifier": str,
@@ -702,14 +914,22 @@
         "serviceNetworkName": str,
         "status": ServiceNetworkVpcAssociationStatusType,
         "vpcId": str,
     },
     total=False,
 )
 
+ListServiceNetworksRequestListServiceNetworksPaginateTypeDef = TypedDict(
+    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServiceNetworksRequestRequestTypeDef = TypedDict(
     "ListServiceNetworksRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -725,14 +945,22 @@
         "name": str,
         "numberOfAssociatedServices": int,
         "numberOfAssociatedVPCs": int,
     },
     total=False,
 )
 
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -741,14 +969,32 @@
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
+ListTargetGroupsRequestListTargetGroupsPaginateTypeDef = TypedDict(
+    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
+    {
+        "targetGroupType": TargetGroupTypeType,
+        "vpcIdentifier": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTargetGroupsRequestRequestTypeDef = TypedDict(
     "ListTargetGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "targetGroupType": TargetGroupTypeType,
         "vpcIdentifier": str,
@@ -782,14 +1028,24 @@
         "port": int,
         "reasonCode": str,
         "status": TargetStatusType,
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
 PathMatchTypeTypeDef = TypedDict(
     "PathMatchTypeTypeDef",
     {
         "exact": str,
         "prefix": str,
     },
     total=False,
@@ -799,22 +1055,42 @@
     "PutAuthPolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceIdentifier": str,
     },
 )
 
+PutAuthPolicyResponseTypeDef = TypedDict(
+    "PutAuthPolicyResponseTypeDef",
+    {
+        "policy": str,
+        "state": AuthPolicyStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -831,295 +1107,134 @@
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
     {
         "accessLogSubscriptionIdentifier": str,
         "destinationArn": str,
     },
 )
 
-UpdateServiceNetworkRequestRequestTypeDef = TypedDict(
-    "UpdateServiceNetworkRequestRequestTypeDef",
-    {
-        "authType": AuthTypeType,
-        "serviceNetworkIdentifier": str,
-    },
-)
-
-UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
-    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
-    {
-        "securityGroupIds": Sequence[str],
-        "serviceNetworkVpcAssociationIdentifier": str,
-    },
-)
-
-_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateServiceRequestRequestTypeDef",
-    {
-        "serviceIdentifier": str,
-    },
-)
-_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateServiceRequestRequestTypeDef",
-    {
-        "authType": AuthTypeType,
-        "certificateArn": str,
-    },
-    total=False,
-)
-
-
-class UpdateServiceRequestRequestTypeDef(
-    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
-):
-    pass
-
-
-CreateAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "CreateAccessLogSubscriptionResponseTypeDef",
+UpdateAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "UpdateAccessLogSubscriptionResponseTypeDef",
     {
         "arn": str,
         "destinationArn": str,
         "id": str,
         "resourceArn": str,
         "resourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceNetworkResponseTypeDef = TypedDict(
-    "CreateServiceNetworkResponseTypeDef",
+UpdateServiceNetworkRequestRequestTypeDef = TypedDict(
+    "UpdateServiceNetworkRequestRequestTypeDef",
     {
-        "arn": str,
         "authType": AuthTypeType,
-        "id": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "serviceNetworkIdentifier": str,
     },
 )
 
-CreateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "CreateServiceNetworkVpcAssociationResponseTypeDef",
+UpdateServiceNetworkResponseTypeDef = TypedDict(
+    "UpdateServiceNetworkResponseTypeDef",
     {
         "arn": str,
-        "createdBy": str,
+        "authType": AuthTypeType,
         "id": str,
-        "securityGroupIds": List[str],
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
-    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
+UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
+    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "securityGroupIds": Sequence[str],
+        "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
-DeleteServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
+UpdateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
     {
         "arn": str,
+        "createdBy": str,
         "id": str,
+        "securityGroupIds": List[str],
         "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceResponseTypeDef = TypedDict(
-    "DeleteServiceResponseTypeDef",
+_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateServiceRequestRequestTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "status": ServiceStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "serviceIdentifier": str,
     },
 )
-
-DeleteTargetGroupResponseTypeDef = TypedDict(
-    "DeleteTargetGroupResponseTypeDef",
+_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateServiceRequestRequestTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "status": TargetGroupStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "authType": AuthTypeType,
+        "certificateArn": str,
     },
+    total=False,
 )
 
-GetAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "GetAccessLogSubscriptionResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "destinationArn": str,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "resourceArn": str,
-        "resourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-GetAuthPolicyResponseTypeDef = TypedDict(
-    "GetAuthPolicyResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "policy": str,
-        "state": AuthPolicyStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateServiceRequestRequestTypeDef(
+    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
+):
+    pass
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-GetServiceNetworkResponseTypeDef = TypedDict(
-    "GetServiceNetworkResponseTypeDef",
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
     {
         "arn": str,
         "authType": AuthTypeType,
-        "createdAt": datetime,
+        "certificateArn": str,
+        "customDomainName": str,
         "id": str,
-        "lastUpdatedAt": datetime,
         "name": str,
-        "numberOfAssociatedServices": int,
-        "numberOfAssociatedVPCs": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "GetServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "createdBy": str,
-        "failureCode": str,
-        "failureMessage": str,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "securityGroupIds": List[str],
-        "serviceNetworkArn": str,
-        "serviceNetworkId": str,
-        "serviceNetworkName": str,
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "vpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccessLogSubscriptionsResponseTypeDef = TypedDict(
     "ListAccessLogSubscriptionsResponseTypeDef",
     {
         "items": List[AccessLogSubscriptionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutAuthPolicyResponseTypeDef = TypedDict(
-    "PutAuthPolicyResponseTypeDef",
-    {
-        "policy": str,
-        "state": AuthPolicyStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "UpdateAccessLogSubscriptionResponseTypeDef",
-    {
-        "arn": str,
-        "destinationArn": str,
-        "id": str,
-        "resourceArn": str,
-        "resourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateServiceNetworkResponseTypeDef = TypedDict(
-    "UpdateServiceNetworkResponseTypeDef",
-    {
-        "arn": str,
-        "authType": AuthTypeType,
-        "id": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "createdBy": str,
-        "id": str,
-        "securityGroupIds": List[str],
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
-    {
-        "arn": str,
-        "authType": AuthTypeType,
-        "certificateArn": str,
-        "customDomainName": str,
-        "id": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
     "CreateServiceNetworkServiceAssociationResponseTypeDef",
     {
         "arn": str,
         "createdBy": str,
         "customDomainName": str,
         "dnsEntry": DnsEntryTypeDef,
         "id": str,
         "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "arn": str,
         "authType": AuthTypeType,
         "certificateArn": str,
         "customDomainName": str,
         "dnsEntry": DnsEntryTypeDef,
         "id": str,
         "name": str,
         "status": ServiceStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
     "GetServiceNetworkServiceAssociationResponseTypeDef",
     {
         "arn": str,
@@ -1133,15 +1248,15 @@
         "serviceArn": str,
         "serviceId": str,
         "serviceName": str,
         "serviceNetworkArn": str,
         "serviceNetworkId": str,
         "serviceNetworkName": str,
         "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "arn": str,
@@ -1152,15 +1267,15 @@
         "dnsEntry": DnsEntryTypeDef,
         "failureCode": str,
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "status": ServiceStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServiceNetworkServiceAssociationSummaryTypeDef = TypedDict(
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     {
         "arn": str,
@@ -1199,14 +1314,37 @@
     "DeregisterTargetsRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
         "targets": Sequence[TargetTypeDef],
     },
 )
 
+_RequiredListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
+    "_RequiredListTargetsRequestListTargetsPaginateTypeDef",
+    {
+        "targetGroupIdentifier": str,
+    },
+)
+_OptionalListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
+    "_OptionalListTargetsRequestListTargetsPaginateTypeDef",
+    {
+        "targets": Sequence[TargetTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTargetsRequestListTargetsPaginateTypeDef(
+    _RequiredListTargetsRequestListTargetsPaginateTypeDef,
+    _OptionalListTargetsRequestListTargetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 _OptionalListTargetsRequestRequestTypeDef = TypedDict(
@@ -1235,24 +1373,24 @@
 )
 
 DeregisterTargetsResponseTypeDef = TypedDict(
     "DeregisterTargetsResponseTypeDef",
     {
         "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterTargetsResponseTypeDef = TypedDict(
     "RegisterTargetsResponseTypeDef",
     {
         "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ForwardActionTypeDef = TypedDict(
     "ForwardActionTypeDef",
     {
         "targetGroups": Sequence[WeightedTargetGroupTypeDef],
@@ -1292,203 +1430,65 @@
         "protocol": TargetGroupProtocolType,
         "protocolVersion": HealthCheckProtocolVersionType,
         "unhealthyThresholdCount": int,
     },
     total=False,
 )
 
-_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
-    "_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
-    {
-        "resourceIdentifier": str,
-    },
-)
-_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
-    "_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(
-    _RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-    _OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_RequiredListListenersRequestListListenersPaginateTypeDef",
-    {
-        "serviceIdentifier": str,
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
-_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_RequiredListRulesRequestListRulesPaginateTypeDef",
-    {
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_OptionalListRulesRequestListRulesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRulesRequestListRulesPaginateTypeDef(
-    _RequiredListRulesRequestListRulesPaginateTypeDef,
-    _OptionalListRulesRequestListRulesPaginateTypeDef,
-):
-    pass
-
-
-ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef = TypedDict(
-    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
-    {
-        "serviceIdentifier": str,
-        "serviceNetworkIdentifier": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef = (
-    TypedDict(
-        "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
-        {
-            "serviceNetworkIdentifier": str,
-            "vpcIdentifier": str,
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-ListServiceNetworksRequestListServiceNetworksPaginateTypeDef = TypedDict(
-    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTargetGroupsRequestListTargetGroupsPaginateTypeDef = TypedDict(
-    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
-    {
-        "targetGroupType": TargetGroupTypeType,
-        "vpcIdentifier": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
-    "_RequiredListTargetsRequestListTargetsPaginateTypeDef",
-    {
-        "targetGroupIdentifier": str,
-    },
-)
-_OptionalListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
-    "_OptionalListTargetsRequestListTargetsPaginateTypeDef",
-    {
-        "targets": Sequence[TargetTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTargetsRequestListTargetsPaginateTypeDef(
-    _RequiredListTargetsRequestListTargetsPaginateTypeDef,
-    _OptionalListTargetsRequestListTargetsPaginateTypeDef,
-):
-    pass
-
-
 ListListenersResponseTypeDef = TypedDict(
     "ListListenersResponseTypeDef",
     {
         "items": List[ListenerSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "items": List[RuleSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceNetworkVpcAssociationsResponseTypeDef = TypedDict(
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     {
         "items": List[ServiceNetworkVpcAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceNetworksResponseTypeDef = TypedDict(
     "ListServiceNetworksResponseTypeDef",
     {
         "items": List[ServiceNetworkSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTargetGroupsResponseTypeDef = TypedDict(
     "ListTargetGroupsResponseTypeDef",
     {
         "items": List[TargetGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTargetsResponseTypeDef = TypedDict(
     "ListTargetsResponseTypeDef",
     {
         "items": List[TargetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPathMatchTypeDef = TypedDict(
     "_RequiredPathMatchTypeDef",
     {
         "match": PathMatchTypeTypeDef,
@@ -1508,24 +1508,24 @@
 
 
 ListServiceNetworkServiceAssociationsResponseTypeDef = TypedDict(
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     {
         "items": List[ServiceNetworkServiceAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "items": List[ServiceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "fixedResponse": FixedResponseActionTypeDef,
@@ -1610,15 +1610,15 @@
         "defaultAction": RuleActionTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetListenerResponseTypeDef = TypedDict(
     "GetListenerResponseTypeDef",
     {
         "arn": str,
@@ -1627,15 +1627,15 @@
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateListenerRequestRequestTypeDef = TypedDict(
     "UpdateListenerRequestRequestTypeDef",
     {
         "defaultAction": RuleActionTypeDef,
@@ -1651,15 +1651,15 @@
         "defaultAction": RuleActionTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTargetGroupRequestRequestTypeDef",
     {
         "name": str,
@@ -1688,15 +1688,15 @@
     {
         "arn": str,
         "config": TargetGroupConfigTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTargetGroupResponseTypeDef = TypedDict(
     "GetTargetGroupResponseTypeDef",
     {
         "arn": str,
@@ -1706,28 +1706,28 @@
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "serviceArns": List[str],
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTargetGroupResponseTypeDef = TypedDict(
     "UpdateTargetGroupResponseTypeDef",
     {
         "arn": str,
         "config": TargetGroupConfigTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleMatchTypeDef = TypedDict(
     "RuleMatchTypeDef",
     {
         "httpMatch": HttpMatchTypeDef,
@@ -1767,15 +1767,15 @@
     {
         "action": RuleActionTypeDef,
         "arn": str,
         "id": str,
         "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "action": RuleActionTypeDef,
@@ -1783,15 +1783,15 @@
         "createdAt": datetime,
         "id": str,
         "isDefault": bool,
         "lastUpdatedAt": datetime,
         "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleUpdateSuccessTypeDef = TypedDict(
     "RuleUpdateSuccessTypeDef",
     {
         "action": RuleActionTypeDef,
@@ -1857,24 +1857,24 @@
         "action": RuleActionTypeDef,
         "arn": str,
         "id": str,
         "isDefault": bool,
         "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateRuleResponseTypeDef = TypedDict(
     "BatchUpdateRuleResponseTypeDef",
     {
         "successful": List[RuleUpdateSuccessTypeDef],
         "unsuccessful": List[RuleUpdateFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateRuleRequestRequestTypeDef = TypedDict(
     "BatchUpdateRuleRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
```

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice/type_defs.pyi` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,115 +34,115 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessLogSubscriptionSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "RuleUpdateFailureTypeDef",
     "CreateAccessLogSubscriptionRequestRequestTypeDef",
+    "CreateAccessLogSubscriptionResponseTypeDef",
     "CreateServiceNetworkRequestRequestTypeDef",
+    "CreateServiceNetworkResponseTypeDef",
     "CreateServiceNetworkServiceAssociationRequestRequestTypeDef",
     "DnsEntryTypeDef",
     "CreateServiceNetworkVpcAssociationRequestRequestTypeDef",
+    "CreateServiceNetworkVpcAssociationResponseTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "DeleteAccessLogSubscriptionRequestRequestTypeDef",
     "DeleteAuthPolicyRequestRequestTypeDef",
     "DeleteListenerRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteServiceNetworkRequestRequestTypeDef",
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
+    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
+    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
+    "DeleteServiceResponseTypeDef",
     "DeleteTargetGroupRequestRequestTypeDef",
+    "DeleteTargetGroupResponseTypeDef",
     "TargetTypeDef",
     "TargetFailureTypeDef",
     "FixedResponseActionTypeDef",
     "WeightedTargetGroupTypeDef",
     "GetAccessLogSubscriptionRequestRequestTypeDef",
+    "GetAccessLogSubscriptionResponseTypeDef",
     "GetAuthPolicyRequestRequestTypeDef",
+    "GetAuthPolicyResponseTypeDef",
     "GetListenerRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "GetRuleRequestRequestTypeDef",
     "GetServiceNetworkRequestRequestTypeDef",
+    "GetServiceNetworkResponseTypeDef",
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
+    "GetServiceNetworkVpcAssociationResponseTypeDef",
     "GetServiceRequestRequestTypeDef",
     "GetTargetGroupRequestRequestTypeDef",
     "HeaderMatchTypeTypeDef",
     "MatcherTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
     "ListAccessLogSubscriptionsRequestRequestTypeDef",
+    "ListListenersRequestListListenersPaginateTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListenerSummaryTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
+    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
     "ListServiceNetworkServiceAssociationsRequestRequestTypeDef",
+    "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
     "ListServiceNetworkVpcAssociationsRequestRequestTypeDef",
     "ServiceNetworkVpcAssociationSummaryTypeDef",
+    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
     "ListServiceNetworksRequestRequestTypeDef",
     "ServiceNetworkSummaryTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
     "ListTargetGroupsRequestRequestTypeDef",
     "TargetGroupSummaryTypeDef",
     "TargetSummaryTypeDef",
+    "PaginatorConfigTypeDef",
     "PathMatchTypeTypeDef",
     "PutAuthPolicyRequestRequestTypeDef",
+    "PutAuthPolicyResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
-    "UpdateServiceNetworkRequestRequestTypeDef",
-    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "UpdateServiceRequestRequestTypeDef",
-    "CreateAccessLogSubscriptionResponseTypeDef",
-    "CreateServiceNetworkResponseTypeDef",
-    "CreateServiceNetworkVpcAssociationResponseTypeDef",
-    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
-    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
-    "DeleteServiceResponseTypeDef",
-    "DeleteTargetGroupResponseTypeDef",
-    "GetAccessLogSubscriptionResponseTypeDef",
-    "GetAuthPolicyResponseTypeDef",
-    "GetResourcePolicyResponseTypeDef",
-    "GetServiceNetworkResponseTypeDef",
-    "GetServiceNetworkVpcAssociationResponseTypeDef",
-    "ListAccessLogSubscriptionsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutAuthPolicyResponseTypeDef",
     "UpdateAccessLogSubscriptionResponseTypeDef",
+    "UpdateServiceNetworkRequestRequestTypeDef",
     "UpdateServiceNetworkResponseTypeDef",
+    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
     "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+    "UpdateServiceRequestRequestTypeDef",
     "UpdateServiceResponseTypeDef",
+    "ListAccessLogSubscriptionsResponseTypeDef",
     "CreateServiceNetworkServiceAssociationResponseTypeDef",
     "CreateServiceResponseTypeDef",
     "GetServiceNetworkServiceAssociationResponseTypeDef",
     "GetServiceResponseTypeDef",
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     "ServiceSummaryTypeDef",
     "DeregisterTargetsRequestRequestTypeDef",
+    "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListTargetsRequestRequestTypeDef",
     "RegisterTargetsRequestRequestTypeDef",
     "DeregisterTargetsResponseTypeDef",
     "RegisterTargetsResponseTypeDef",
     "ForwardActionTypeDef",
     "HeaderMatchTypeDef",
     "HealthCheckConfigTypeDef",
-    "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
-    "ListListenersRequestListListenersPaginateTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
-    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
-    "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
-    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
-    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
-    "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListListenersResponseTypeDef",
     "ListRulesResponseTypeDef",
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     "ListServiceNetworksResponseTypeDef",
     "ListTargetGroupsResponseTypeDef",
     "ListTargetsResponseTypeDef",
     "PathMatchTypeDef",
@@ -182,25 +182,14 @@
         "id": str,
         "lastUpdatedAt": datetime,
         "resourceArn": str,
         "resourceId": str,
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
 RuleUpdateFailureTypeDef = TypedDict(
     "RuleUpdateFailureTypeDef",
     {
         "failureCode": str,
         "failureMessage": str,
         "ruleIdentifier": str,
     },
@@ -225,14 +214,26 @@
 
 class CreateAccessLogSubscriptionRequestRequestTypeDef(
     _RequiredCreateAccessLogSubscriptionRequestRequestTypeDef,
     _OptionalCreateAccessLogSubscriptionRequestRequestTypeDef,
 ):
     pass
 
+CreateAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "CreateAccessLogSubscriptionResponseTypeDef",
+    {
+        "arn": str,
+        "destinationArn": str,
+        "id": str,
+        "resourceArn": str,
+        "resourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateServiceNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceNetworkRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceNetworkRequestRequestTypeDef = TypedDict(
@@ -247,14 +248,25 @@
 
 class CreateServiceNetworkRequestRequestTypeDef(
     _RequiredCreateServiceNetworkRequestRequestTypeDef,
     _OptionalCreateServiceNetworkRequestRequestTypeDef,
 ):
     pass
 
+CreateServiceNetworkResponseTypeDef = TypedDict(
+    "CreateServiceNetworkResponseTypeDef",
+    {
+        "arn": str,
+        "authType": AuthTypeType,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
         "serviceNetworkIdentifier": str,
     },
 )
@@ -301,14 +313,26 @@
 
 class CreateServiceNetworkVpcAssociationRequestRequestTypeDef(
     _RequiredCreateServiceNetworkVpcAssociationRequestRequestTypeDef,
     _OptionalCreateServiceNetworkVpcAssociationRequestRequestTypeDef,
 ):
     pass
 
+CreateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "CreateServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "createdBy": str,
+        "id": str,
+        "securityGroupIds": List[str],
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceRequestRequestTypeDef = TypedDict(
@@ -376,35 +400,76 @@
 DeleteServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceNetworkServiceAssociationIdentifier": str,
     },
 )
 
+DeleteServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
+    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": ServiceNetworkServiceAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
         "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
+DeleteServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 
+DeleteServiceResponseTypeDef = TypedDict(
+    "DeleteServiceResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "status": ServiceStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTargetGroupRequestRequestTypeDef = TypedDict(
     "DeleteTargetGroupRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 
+DeleteTargetGroupResponseTypeDef = TypedDict(
+    "DeleteTargetGroupResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": TargetGroupStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "id": str,
     },
 )
 _OptionalTargetTypeDef = TypedDict(
@@ -458,21 +523,46 @@
 GetAccessLogSubscriptionRequestRequestTypeDef = TypedDict(
     "GetAccessLogSubscriptionRequestRequestTypeDef",
     {
         "accessLogSubscriptionIdentifier": str,
     },
 )
 
+GetAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "GetAccessLogSubscriptionResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "destinationArn": str,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "resourceArn": str,
+        "resourceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAuthPolicyRequestRequestTypeDef = TypedDict(
     "GetAuthPolicyRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
 )
 
+GetAuthPolicyResponseTypeDef = TypedDict(
+    "GetAuthPolicyResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "policy": str,
+        "state": AuthPolicyStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetListenerRequestRequestTypeDef = TypedDict(
     "GetListenerRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
@@ -480,14 +570,22 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "ruleIdentifier": str,
         "serviceIdentifier": str,
     },
@@ -496,28 +594,63 @@
 GetServiceNetworkRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkRequestRequestTypeDef",
     {
         "serviceNetworkIdentifier": str,
     },
 )
 
+GetServiceNetworkResponseTypeDef = TypedDict(
+    "GetServiceNetworkResponseTypeDef",
+    {
+        "arn": str,
+        "authType": AuthTypeType,
+        "createdAt": datetime,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "name": str,
+        "numberOfAssociatedServices": int,
+        "numberOfAssociatedVPCs": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceNetworkServiceAssociationIdentifier": str,
     },
 )
 
 GetServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
         "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
+GetServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "GetServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "createdBy": str,
+        "failureCode": str,
+        "failureMessage": str,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "securityGroupIds": List[str],
+        "serviceNetworkArn": str,
+        "serviceNetworkId": str,
+        "serviceNetworkName": str,
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "vpcId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetServiceRequestRequestTypeDef = TypedDict(
     "GetServiceRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 
@@ -542,24 +675,34 @@
     "MatcherTypeDef",
     {
         "httpCode": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
+    "_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "resourceIdentifier": str,
+    },
+)
+_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
+    "_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(
+    _RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    _OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAccessLogSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessLogSubscriptionsRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
 )
 _OptionalListAccessLogSubscriptionsRequestRequestTypeDef = TypedDict(
@@ -573,14 +716,34 @@
 
 class ListAccessLogSubscriptionsRequestRequestTypeDef(
     _RequiredListAccessLogSubscriptionsRequestRequestTypeDef,
     _OptionalListAccessLogSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_RequiredListListenersRequestListListenersPaginateTypeDef",
+    {
+        "serviceIdentifier": str,
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
         "serviceIdentifier": str,
     },
 )
 _OptionalListListenersRequestRequestTypeDef = TypedDict(
@@ -607,14 +770,35 @@
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
     },
     total=False,
 )
 
+_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_RequiredListRulesRequestListRulesPaginateTypeDef",
+    {
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_OptionalListRulesRequestListRulesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRulesRequestListRulesPaginateTypeDef(
+    _RequiredListRulesRequestListRulesPaginateTypeDef,
+    _OptionalListRulesRequestListRulesPaginateTypeDef,
+):
+    pass
+
 _RequiredListRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListRulesRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
@@ -642,25 +826,47 @@
         "lastUpdatedAt": datetime,
         "name": str,
         "priority": int,
     },
     total=False,
 )
 
+ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef = TypedDict(
+    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
+    {
+        "serviceIdentifier": str,
+        "serviceNetworkIdentifier": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServiceNetworkServiceAssociationsRequestRequestTypeDef = TypedDict(
     "ListServiceNetworkServiceAssociationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "serviceIdentifier": str,
         "serviceNetworkIdentifier": str,
     },
     total=False,
 )
 
+ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef = (
+    TypedDict(
+        "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
+        {
+            "serviceNetworkIdentifier": str,
+            "vpcIdentifier": str,
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
 ListServiceNetworkVpcAssociationsRequestRequestTypeDef = TypedDict(
     "ListServiceNetworkVpcAssociationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "serviceNetworkIdentifier": str,
         "vpcIdentifier": str,
@@ -681,14 +887,22 @@
         "serviceNetworkName": str,
         "status": ServiceNetworkVpcAssociationStatusType,
         "vpcId": str,
     },
     total=False,
 )
 
+ListServiceNetworksRequestListServiceNetworksPaginateTypeDef = TypedDict(
+    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServiceNetworksRequestRequestTypeDef = TypedDict(
     "ListServiceNetworksRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -704,14 +918,22 @@
         "name": str,
         "numberOfAssociatedServices": int,
         "numberOfAssociatedVPCs": int,
     },
     total=False,
 )
 
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -720,14 +942,32 @@
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
+ListTargetGroupsRequestListTargetGroupsPaginateTypeDef = TypedDict(
+    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
+    {
+        "targetGroupType": TargetGroupTypeType,
+        "vpcIdentifier": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTargetGroupsRequestRequestTypeDef = TypedDict(
     "ListTargetGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "targetGroupType": TargetGroupTypeType,
         "vpcIdentifier": str,
@@ -761,14 +1001,24 @@
         "port": int,
         "reasonCode": str,
         "status": TargetStatusType,
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
 PathMatchTypeTypeDef = TypedDict(
     "PathMatchTypeTypeDef",
     {
         "exact": str,
         "prefix": str,
     },
     total=False,
@@ -778,22 +1028,42 @@
     "PutAuthPolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceIdentifier": str,
     },
 )
 
+PutAuthPolicyResponseTypeDef = TypedDict(
+    "PutAuthPolicyResponseTypeDef",
+    {
+        "policy": str,
+        "state": AuthPolicyStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -810,293 +1080,132 @@
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
     {
         "accessLogSubscriptionIdentifier": str,
         "destinationArn": str,
     },
 )
 
-UpdateServiceNetworkRequestRequestTypeDef = TypedDict(
-    "UpdateServiceNetworkRequestRequestTypeDef",
-    {
-        "authType": AuthTypeType,
-        "serviceNetworkIdentifier": str,
-    },
-)
-
-UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
-    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
-    {
-        "securityGroupIds": Sequence[str],
-        "serviceNetworkVpcAssociationIdentifier": str,
-    },
-)
-
-_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateServiceRequestRequestTypeDef",
-    {
-        "serviceIdentifier": str,
-    },
-)
-_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateServiceRequestRequestTypeDef",
-    {
-        "authType": AuthTypeType,
-        "certificateArn": str,
-    },
-    total=False,
-)
-
-class UpdateServiceRequestRequestTypeDef(
-    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
-):
-    pass
-
-CreateAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "CreateAccessLogSubscriptionResponseTypeDef",
+UpdateAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "UpdateAccessLogSubscriptionResponseTypeDef",
     {
         "arn": str,
         "destinationArn": str,
         "id": str,
         "resourceArn": str,
         "resourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceNetworkResponseTypeDef = TypedDict(
-    "CreateServiceNetworkResponseTypeDef",
+UpdateServiceNetworkRequestRequestTypeDef = TypedDict(
+    "UpdateServiceNetworkRequestRequestTypeDef",
     {
-        "arn": str,
         "authType": AuthTypeType,
-        "id": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "CreateServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "createdBy": str,
-        "id": str,
-        "securityGroupIds": List[str],
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
-    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "serviceNetworkIdentifier": str,
     },
 )
 
-DeleteServiceResponseTypeDef = TypedDict(
-    "DeleteServiceResponseTypeDef",
+UpdateServiceNetworkResponseTypeDef = TypedDict(
+    "UpdateServiceNetworkResponseTypeDef",
     {
         "arn": str,
+        "authType": AuthTypeType,
         "id": str,
         "name": str,
-        "status": ServiceStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteTargetGroupResponseTypeDef = TypedDict(
-    "DeleteTargetGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": TargetGroupStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "GetAccessLogSubscriptionResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "destinationArn": str,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "resourceArn": str,
-        "resourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAuthPolicyResponseTypeDef = TypedDict(
-    "GetAuthPolicyResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "policy": str,
-        "state": AuthPolicyStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetServiceNetworkResponseTypeDef = TypedDict(
-    "GetServiceNetworkResponseTypeDef",
+UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
+    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
-        "arn": str,
-        "authType": AuthTypeType,
-        "createdAt": datetime,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "name": str,
-        "numberOfAssociatedServices": int,
-        "numberOfAssociatedVPCs": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "securityGroupIds": Sequence[str],
+        "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
-GetServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "GetServiceNetworkVpcAssociationResponseTypeDef",
+UpdateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
     {
         "arn": str,
-        "createdAt": datetime,
         "createdBy": str,
-        "failureCode": str,
-        "failureMessage": str,
         "id": str,
-        "lastUpdatedAt": datetime,
         "securityGroupIds": List[str],
-        "serviceNetworkArn": str,
-        "serviceNetworkId": str,
-        "serviceNetworkName": str,
         "status": ServiceNetworkVpcAssociationStatusType,
-        "vpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAccessLogSubscriptionsResponseTypeDef = TypedDict(
-    "ListAccessLogSubscriptionsResponseTypeDef",
-    {
-        "items": List[AccessLogSubscriptionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutAuthPolicyResponseTypeDef = TypedDict(
-    "PutAuthPolicyResponseTypeDef",
-    {
-        "policy": str,
-        "state": AuthPolicyStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "UpdateAccessLogSubscriptionResponseTypeDef",
+_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateServiceRequestRequestTypeDef",
     {
-        "arn": str,
-        "destinationArn": str,
-        "id": str,
-        "resourceArn": str,
-        "resourceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "serviceIdentifier": str,
     },
 )
-
-UpdateServiceNetworkResponseTypeDef = TypedDict(
-    "UpdateServiceNetworkResponseTypeDef",
+_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateServiceRequestRequestTypeDef",
     {
-        "arn": str,
         "authType": AuthTypeType,
-        "id": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "certificateArn": str,
     },
+    total=False,
 )
 
-UpdateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "createdBy": str,
-        "id": str,
-        "securityGroupIds": List[str],
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateServiceRequestRequestTypeDef(
+    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
+):
+    pass
 
 UpdateServiceResponseTypeDef = TypedDict(
     "UpdateServiceResponseTypeDef",
     {
         "arn": str,
         "authType": AuthTypeType,
         "certificateArn": str,
         "customDomainName": str,
         "id": str,
         "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAccessLogSubscriptionsResponseTypeDef = TypedDict(
+    "ListAccessLogSubscriptionsResponseTypeDef",
+    {
+        "items": List[AccessLogSubscriptionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
     "CreateServiceNetworkServiceAssociationResponseTypeDef",
     {
         "arn": str,
         "createdBy": str,
         "customDomainName": str,
         "dnsEntry": DnsEntryTypeDef,
         "id": str,
         "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "arn": str,
         "authType": AuthTypeType,
         "certificateArn": str,
         "customDomainName": str,
         "dnsEntry": DnsEntryTypeDef,
         "id": str,
         "name": str,
         "status": ServiceStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
     "GetServiceNetworkServiceAssociationResponseTypeDef",
     {
         "arn": str,
@@ -1110,15 +1219,15 @@
         "serviceArn": str,
         "serviceId": str,
         "serviceName": str,
         "serviceNetworkArn": str,
         "serviceNetworkId": str,
         "serviceNetworkName": str,
         "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "arn": str,
@@ -1129,15 +1238,15 @@
         "dnsEntry": DnsEntryTypeDef,
         "failureCode": str,
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "status": ServiceStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServiceNetworkServiceAssociationSummaryTypeDef = TypedDict(
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     {
         "arn": str,
@@ -1176,14 +1285,35 @@
     "DeregisterTargetsRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
         "targets": Sequence[TargetTypeDef],
     },
 )
 
+_RequiredListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
+    "_RequiredListTargetsRequestListTargetsPaginateTypeDef",
+    {
+        "targetGroupIdentifier": str,
+    },
+)
+_OptionalListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
+    "_OptionalListTargetsRequestListTargetsPaginateTypeDef",
+    {
+        "targets": Sequence[TargetTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTargetsRequestListTargetsPaginateTypeDef(
+    _RequiredListTargetsRequestListTargetsPaginateTypeDef,
+    _OptionalListTargetsRequestListTargetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 _OptionalListTargetsRequestRequestTypeDef = TypedDict(
@@ -1210,24 +1340,24 @@
 )
 
 DeregisterTargetsResponseTypeDef = TypedDict(
     "DeregisterTargetsResponseTypeDef",
     {
         "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterTargetsResponseTypeDef = TypedDict(
     "RegisterTargetsResponseTypeDef",
     {
         "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ForwardActionTypeDef = TypedDict(
     "ForwardActionTypeDef",
     {
         "targetGroups": Sequence[WeightedTargetGroupTypeDef],
@@ -1265,195 +1395,65 @@
         "protocol": TargetGroupProtocolType,
         "protocolVersion": HealthCheckProtocolVersionType,
         "unhealthyThresholdCount": int,
     },
     total=False,
 )
 
-_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
-    "_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
-    {
-        "resourceIdentifier": str,
-    },
-)
-_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
-    "_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(
-    _RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-    _OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_RequiredListListenersRequestListListenersPaginateTypeDef",
-    {
-        "serviceIdentifier": str,
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
-_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_RequiredListRulesRequestListRulesPaginateTypeDef",
-    {
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_OptionalListRulesRequestListRulesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRulesRequestListRulesPaginateTypeDef(
-    _RequiredListRulesRequestListRulesPaginateTypeDef,
-    _OptionalListRulesRequestListRulesPaginateTypeDef,
-):
-    pass
-
-ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef = TypedDict(
-    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
-    {
-        "serviceIdentifier": str,
-        "serviceNetworkIdentifier": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef = (
-    TypedDict(
-        "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
-        {
-            "serviceNetworkIdentifier": str,
-            "vpcIdentifier": str,
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-ListServiceNetworksRequestListServiceNetworksPaginateTypeDef = TypedDict(
-    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTargetGroupsRequestListTargetGroupsPaginateTypeDef = TypedDict(
-    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
-    {
-        "targetGroupType": TargetGroupTypeType,
-        "vpcIdentifier": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
-    "_RequiredListTargetsRequestListTargetsPaginateTypeDef",
-    {
-        "targetGroupIdentifier": str,
-    },
-)
-_OptionalListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
-    "_OptionalListTargetsRequestListTargetsPaginateTypeDef",
-    {
-        "targets": Sequence[TargetTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTargetsRequestListTargetsPaginateTypeDef(
-    _RequiredListTargetsRequestListTargetsPaginateTypeDef,
-    _OptionalListTargetsRequestListTargetsPaginateTypeDef,
-):
-    pass
-
 ListListenersResponseTypeDef = TypedDict(
     "ListListenersResponseTypeDef",
     {
         "items": List[ListenerSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "items": List[RuleSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceNetworkVpcAssociationsResponseTypeDef = TypedDict(
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     {
         "items": List[ServiceNetworkVpcAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceNetworksResponseTypeDef = TypedDict(
     "ListServiceNetworksResponseTypeDef",
     {
         "items": List[ServiceNetworkSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTargetGroupsResponseTypeDef = TypedDict(
     "ListTargetGroupsResponseTypeDef",
     {
         "items": List[TargetGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTargetsResponseTypeDef = TypedDict(
     "ListTargetsResponseTypeDef",
     {
         "items": List[TargetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPathMatchTypeDef = TypedDict(
     "_RequiredPathMatchTypeDef",
     {
         "match": PathMatchTypeTypeDef,
@@ -1471,24 +1471,24 @@
     pass
 
 ListServiceNetworkServiceAssociationsResponseTypeDef = TypedDict(
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     {
         "items": List[ServiceNetworkServiceAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "items": List[ServiceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "fixedResponse": FixedResponseActionTypeDef,
@@ -1569,15 +1569,15 @@
         "defaultAction": RuleActionTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetListenerResponseTypeDef = TypedDict(
     "GetListenerResponseTypeDef",
     {
         "arn": str,
@@ -1586,15 +1586,15 @@
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateListenerRequestRequestTypeDef = TypedDict(
     "UpdateListenerRequestRequestTypeDef",
     {
         "defaultAction": RuleActionTypeDef,
@@ -1610,15 +1610,15 @@
         "defaultAction": RuleActionTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTargetGroupRequestRequestTypeDef",
     {
         "name": str,
@@ -1645,15 +1645,15 @@
     {
         "arn": str,
         "config": TargetGroupConfigTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTargetGroupResponseTypeDef = TypedDict(
     "GetTargetGroupResponseTypeDef",
     {
         "arn": str,
@@ -1663,28 +1663,28 @@
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "serviceArns": List[str],
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTargetGroupResponseTypeDef = TypedDict(
     "UpdateTargetGroupResponseTypeDef",
     {
         "arn": str,
         "config": TargetGroupConfigTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleMatchTypeDef = TypedDict(
     "RuleMatchTypeDef",
     {
         "httpMatch": HttpMatchTypeDef,
@@ -1722,15 +1722,15 @@
     {
         "action": RuleActionTypeDef,
         "arn": str,
         "id": str,
         "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "action": RuleActionTypeDef,
@@ -1738,15 +1738,15 @@
         "createdAt": datetime,
         "id": str,
         "isDefault": bool,
         "lastUpdatedAt": datetime,
         "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleUpdateSuccessTypeDef = TypedDict(
     "RuleUpdateSuccessTypeDef",
     {
         "action": RuleActionTypeDef,
@@ -1808,24 +1808,24 @@
         "action": RuleActionTypeDef,
         "arn": str,
         "id": str,
         "isDefault": bool,
         "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateRuleResponseTypeDef = TypedDict(
     "BatchUpdateRuleResponseTypeDef",
     {
         "successful": List[RuleUpdateSuccessTypeDef],
         "unsuccessful": List[RuleUpdateFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateRuleRequestRequestTypeDef = TypedDict(
     "BatchUpdateRuleRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
```

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice.egg-info/PKG-INFO` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-vpc-lattice
-Version: 1.26.107
-Summary: Type annotations for boto3.VPCLattice 1.26.107 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.VPCLattice 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-vpc-lattice?color=blue)](https://pypistats.org/packages/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.26.107](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -366,115 +366,115 @@
 
 `mypy_boto3_vpc_lattice.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_vpc_lattice.type_defs import (
     AccessLogSubscriptionSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RuleUpdateFailureTypeDef,
     CreateAccessLogSubscriptionRequestRequestTypeDef,
+    CreateAccessLogSubscriptionResponseTypeDef,
     CreateServiceNetworkRequestRequestTypeDef,
+    CreateServiceNetworkResponseTypeDef,
     CreateServiceNetworkServiceAssociationRequestRequestTypeDef,
     DnsEntryTypeDef,
     CreateServiceNetworkVpcAssociationRequestRequestTypeDef,
+    CreateServiceNetworkVpcAssociationResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     DeleteAccessLogSubscriptionRequestRequestTypeDef,
     DeleteAuthPolicyRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteServiceNetworkRequestRequestTypeDef,
     DeleteServiceNetworkServiceAssociationRequestRequestTypeDef,
+    DeleteServiceNetworkServiceAssociationResponseTypeDef,
     DeleteServiceNetworkVpcAssociationRequestRequestTypeDef,
+    DeleteServiceNetworkVpcAssociationResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
+    DeleteServiceResponseTypeDef,
     DeleteTargetGroupRequestRequestTypeDef,
+    DeleteTargetGroupResponseTypeDef,
     TargetTypeDef,
     TargetFailureTypeDef,
     FixedResponseActionTypeDef,
     WeightedTargetGroupTypeDef,
     GetAccessLogSubscriptionRequestRequestTypeDef,
+    GetAccessLogSubscriptionResponseTypeDef,
     GetAuthPolicyRequestRequestTypeDef,
+    GetAuthPolicyResponseTypeDef,
     GetListenerRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetRuleRequestRequestTypeDef,
     GetServiceNetworkRequestRequestTypeDef,
+    GetServiceNetworkResponseTypeDef,
     GetServiceNetworkServiceAssociationRequestRequestTypeDef,
     GetServiceNetworkVpcAssociationRequestRequestTypeDef,
+    GetServiceNetworkVpcAssociationResponseTypeDef,
     GetServiceRequestRequestTypeDef,
     GetTargetGroupRequestRequestTypeDef,
     HeaderMatchTypeTypeDef,
     MatcherTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
     ListAccessLogSubscriptionsRequestRequestTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListenerSummaryTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
+    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
     ListServiceNetworkServiceAssociationsRequestRequestTypeDef,
+    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
     ListServiceNetworkVpcAssociationsRequestRequestTypeDef,
     ServiceNetworkVpcAssociationSummaryTypeDef,
+    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
     ListServiceNetworksRequestRequestTypeDef,
     ServiceNetworkSummaryTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
     ListTargetGroupsRequestRequestTypeDef,
     TargetGroupSummaryTypeDef,
     TargetSummaryTypeDef,
+    PaginatorConfigTypeDef,
     PathMatchTypeTypeDef,
     PutAuthPolicyRequestRequestTypeDef,
+    PutAuthPolicyResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessLogSubscriptionRequestRequestTypeDef,
-    UpdateServiceNetworkRequestRequestTypeDef,
-    UpdateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    UpdateServiceRequestRequestTypeDef,
-    CreateAccessLogSubscriptionResponseTypeDef,
-    CreateServiceNetworkResponseTypeDef,
-    CreateServiceNetworkVpcAssociationResponseTypeDef,
-    DeleteServiceNetworkServiceAssociationResponseTypeDef,
-    DeleteServiceNetworkVpcAssociationResponseTypeDef,
-    DeleteServiceResponseTypeDef,
-    DeleteTargetGroupResponseTypeDef,
-    GetAccessLogSubscriptionResponseTypeDef,
-    GetAuthPolicyResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetServiceNetworkResponseTypeDef,
-    GetServiceNetworkVpcAssociationResponseTypeDef,
-    ListAccessLogSubscriptionsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutAuthPolicyResponseTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
+    UpdateServiceNetworkRequestRequestTypeDef,
     UpdateServiceNetworkResponseTypeDef,
+    UpdateServiceNetworkVpcAssociationRequestRequestTypeDef,
     UpdateServiceNetworkVpcAssociationResponseTypeDef,
+    UpdateServiceRequestRequestTypeDef,
     UpdateServiceResponseTypeDef,
+    ListAccessLogSubscriptionsResponseTypeDef,
     CreateServiceNetworkServiceAssociationResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceNetworkServiceAssociationResponseTypeDef,
     GetServiceResponseTypeDef,
     ServiceNetworkServiceAssociationSummaryTypeDef,
     ServiceSummaryTypeDef,
     DeregisterTargetsRequestRequestTypeDef,
+    ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
     RegisterTargetsRequestRequestTypeDef,
     DeregisterTargetsResponseTypeDef,
     RegisterTargetsResponseTypeDef,
     ForwardActionTypeDef,
     HeaderMatchTypeDef,
     HealthCheckConfigTypeDef,
-    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
-    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
-    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
-    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
-    ListTargetsRequestListTargetsPaginateTypeDef,
     ListListenersResponseTypeDef,
     ListRulesResponseTypeDef,
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServiceNetworksResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PathMatchTypeDef,
```

### Comparing `mypy-boto3-vpc-lattice-1.26.107/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt` & `mypy-boto3-vpc-lattice-1.27.0/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.26.107/setup.py` & `mypy-boto3-vpc-lattice-1.27.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-vpc-lattice",
-    version="1.26.107",
+    version="1.27.0",
     packages=["mypy_boto3_vpc_lattice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VPCLattice 1.26.107 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.VPCLattice 1.27.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


# Comparing `tmp/mypy-boto3-route53-1.26.56.tar.gz` & `tmp/mypy-boto3-route53-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-1.26.56.tar", last modified: Tue Jan 24 20:25:10 2023, max compression
+gzip compressed data, was "mypy-boto3-route53-1.27.0.tar", last modified: Mon Jul  3 19:51:21 2023, max compression
```

## Comparing `mypy-boto3-route53-1.26.56.tar` & `mypy-boto3-route53-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:25:10.916532 mypy-boto3-route53-1.26.56/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-24 20:24:58.000000 mypy-boto3-route53-1.26.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22614 2023-01-24 20:25:10.904532 mypy-boto3-route53-1.26.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21127 2023-01-24 20:24:58.000000 mypy-boto3-route53-1.26.56/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:25:10.904532 mypy-boto3-route53-1.26.56/mypy_boto3_route53/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-01-24 20:24:58.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-01-24 20:24:58.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-24 20:24:58.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55440 2023-01-24 20:24:59.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    55354 2023-01-24 20:24:59.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-01-24 20:24:59.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-01-24 20:24:59.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-01-24 20:24:59.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-01-24 20:24:59.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:24:58.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61049 2023-01-24 20:25:00.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60982 2023-01-24 20:25:00.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-24 20:24:58.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-01-24 20:24:59.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-01-24 20:24:59.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:25:10.904532 mypy-boto3-route53-1.26.56/mypy_boto3_route53.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22614 2023-01-24 20:25:10.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-01-24 20:25:10.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 20:25:10.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 20:25:10.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-24 20:25:10.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-24 20:25:10.000000 mypy-boto3-route53-1.26.56/mypy_boto3_route53.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 20:25:10.916532 mypy-boto3-route53-1.26.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-01-24 20:24:58.000000 mypy-boto3-route53-1.26.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.311899 mypy-boto3-route53-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:27.000000 mypy-boto3-route53-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22590 2023-07-03 19:51:21.307899 mypy-boto3-route53-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-07-03 19:46:27.000000 mypy-boto3-route53-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.299899 mypy-boto3-route53-1.27.0/mypy_boto3_route53/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-03 19:46:27.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-03 19:46:27.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:46:27.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55440 2023-07-03 19:46:30.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55354 2023-07-03 19:46:27.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-03 19:46:30.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-07-03 19:46:30.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-03 19:46:30.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-07-03 19:46:30.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:27.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    61189 2023-07-03 19:46:31.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-07-03 19:46:31.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:27.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-03 19:46:30.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-03 19:46:30.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.307899 mypy-boto3-route53-1.27.0/mypy_boto3_route53.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22590 2023-07-03 19:51:21.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-03 19:51:21.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:21.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:21.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:21.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:51:21.000000 mypy-boto3-route53-1.27.0/mypy_boto3_route53.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:21.311899 mypy-boto3-route53-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:46:27.000000 mypy-boto3-route53-1.27.0/setup.py
```

### Comparing `mypy-boto3-route53-1.26.56/LICENSE` & `mypy-boto3-route53-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-route53-1.26.56/PKG-INFO` & `mypy-boto3-route53-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53
-Version: 1.26.56
-Summary: Type annotations for boto3.Route53 1.26.56 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Route53 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-route53"></a>
 
 # mypy-boto3-route53
 
 [![PyPI - mypy-boto3-route53](https://img.shields.io/pypi/v/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53?color=blue)](https://pypistats.org/packages/mypy-boto3-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53 1.26.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[boto3.Route53 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [mypy-boto3-route53 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/).
 
 See how it helps to find and fix potential bugs:
 
@@ -395,19 +395,19 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53.type_defs import (
     AccountLimitTypeDef,
     ActivateKeySigningKeyRequestRequestTypeDef,
     ChangeInfoTypeDef,
-    ResponseMetadataTypeDef,
     AlarmIdentifierTypeDef,
     AliasTargetTypeDef,
     VPCTypeDef,
     CidrCollectionChangeTypeDef,
+    ChangeCidrCollectionResponseTypeDef,
     TagTypeDef,
     CidrBlockSummaryTypeDef,
     CidrCollectionTypeDef,
     CidrRoutingConfigTypeDef,
     DimensionTypeDef,
     CollectionSummaryTypeDef,
     CreateCidrCollectionRequestRequestTypeDef,
@@ -436,75 +436,83 @@
     DisableHostedZoneDNSSECRequestRequestTypeDef,
     EnableHostedZoneDNSSECRequestRequestTypeDef,
     GeoLocationDetailsTypeDef,
     GeoLocationTypeDef,
     GetAccountLimitRequestRequestTypeDef,
     GetChangeRequestRequestTypeDef,
     WaiterConfigTypeDef,
+    GetCheckerIpRangesResponseTypeDef,
     GetDNSSECRequestRequestTypeDef,
     GetGeoLocationRequestRequestTypeDef,
+    GetHealthCheckCountResponseTypeDef,
     GetHealthCheckLastFailureReasonRequestRequestTypeDef,
     GetHealthCheckRequestRequestTypeDef,
     GetHealthCheckStatusRequestRequestTypeDef,
+    GetHostedZoneCountResponseTypeDef,
     GetHostedZoneLimitRequestRequestTypeDef,
     HostedZoneLimitTypeDef,
     GetHostedZoneRequestRequestTypeDef,
     GetQueryLoggingConfigRequestRequestTypeDef,
     GetReusableDelegationSetLimitRequestRequestTypeDef,
     ReusableDelegationSetLimitTypeDef,
     GetReusableDelegationSetRequestRequestTypeDef,
+    GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceRequestRequestTypeDef,
     GetTrafficPolicyRequestRequestTypeDef,
     StatusReportTypeDef,
     LinkedServiceTypeDef,
     HostedZoneOwnerTypeDef,
-    PaginatorConfigTypeDef,
+    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
     ListCidrBlocksRequestRequestTypeDef,
+    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
     ListCidrCollectionsRequestRequestTypeDef,
+    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
     ListCidrLocationsRequestRequestTypeDef,
     LocationSummaryTypeDef,
     ListGeoLocationsRequestRequestTypeDef,
+    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
     ListHealthChecksRequestRequestTypeDef,
     ListHostedZonesByNameRequestRequestTypeDef,
     ListHostedZonesByVPCRequestRequestTypeDef,
+    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
     ListHostedZonesRequestRequestTypeDef,
+    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
     ListQueryLoggingConfigsRequestRequestTypeDef,
+    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
     ListResourceRecordSetsRequestRequestTypeDef,
     ListReusableDelegationSetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
     ListTrafficPoliciesRequestRequestTypeDef,
     TrafficPolicySummaryTypeDef,
     ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef,
     ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef,
     ListTrafficPolicyInstancesRequestRequestTypeDef,
     ListTrafficPolicyVersionsRequestRequestTypeDef,
+    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListVPCAssociationAuthorizationsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ResourceRecordTypeDef,
+    ResponseMetadataTypeDef,
     TestDNSAnswerRequestRequestTypeDef,
+    TestDNSAnswerResponseTypeDef,
     UpdateHostedZoneCommentRequestRequestTypeDef,
     UpdateTrafficPolicyCommentRequestRequestTypeDef,
     UpdateTrafficPolicyInstanceRequestRequestTypeDef,
+    GetAccountLimitResponseTypeDef,
     ActivateKeySigningKeyResponseTypeDef,
     AssociateVPCWithHostedZoneResponseTypeDef,
-    ChangeCidrCollectionResponseTypeDef,
     ChangeResourceRecordSetsResponseTypeDef,
     DeactivateKeySigningKeyResponseTypeDef,
     DeleteHostedZoneResponseTypeDef,
     DeleteKeySigningKeyResponseTypeDef,
     DisableHostedZoneDNSSECResponseTypeDef,
     DisassociateVPCFromHostedZoneResponseTypeDef,
     EnableHostedZoneDNSSECResponseTypeDef,
-    GetAccountLimitResponseTypeDef,
     GetChangeResponseTypeDef,
-    GetCheckerIpRangesResponseTypeDef,
-    GetHealthCheckCountResponseTypeDef,
-    GetHostedZoneCountResponseTypeDef,
-    GetTrafficPolicyInstanceCountResponseTypeDef,
-    TestDNSAnswerResponseTypeDef,
     HealthCheckConfigTypeDef,
     UpdateHealthCheckRequestRequestTypeDef,
     AssociateVPCWithHostedZoneRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationResponseTypeDef,
     DeleteVPCAssociationAuthorizationRequestRequestTypeDef,
     DisassociateVPCFromHostedZoneRequestRequestTypeDef,
@@ -540,22 +548,14 @@
     ListGeoLocationsResponseTypeDef,
     GetChangeRequestResourceRecordSetsChangedWaitTypeDef,
     GetHostedZoneLimitResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     HealthCheckObservationTypeDef,
     HostedZoneTypeDef,
     HostedZoneSummaryTypeDef,
-    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
-    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
-    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
-    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
-    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListTrafficPoliciesResponseTypeDef,
     ResourceRecordSetTypeDef,
     CreateHealthCheckRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsForResourcesResponseTypeDef,
     HealthCheckTypeDef,
@@ -585,42 +585,42 @@
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

### Comparing `mypy-boto3-route53-1.26.56/README.md` & `mypy-boto3-route53-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-route53"></a>
 
 # mypy-boto3-route53
 
 [![PyPI - mypy-boto3-route53](https://img.shields.io/pypi/v/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53?color=blue)](https://pypistats.org/packages/mypy-boto3-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53 1.26.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[boto3.Route53 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [mypy-boto3-route53 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,19 +363,19 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53.type_defs import (
     AccountLimitTypeDef,
     ActivateKeySigningKeyRequestRequestTypeDef,
     ChangeInfoTypeDef,
-    ResponseMetadataTypeDef,
     AlarmIdentifierTypeDef,
     AliasTargetTypeDef,
     VPCTypeDef,
     CidrCollectionChangeTypeDef,
+    ChangeCidrCollectionResponseTypeDef,
     TagTypeDef,
     CidrBlockSummaryTypeDef,
     CidrCollectionTypeDef,
     CidrRoutingConfigTypeDef,
     DimensionTypeDef,
     CollectionSummaryTypeDef,
     CreateCidrCollectionRequestRequestTypeDef,
@@ -404,75 +404,83 @@
     DisableHostedZoneDNSSECRequestRequestTypeDef,
     EnableHostedZoneDNSSECRequestRequestTypeDef,
     GeoLocationDetailsTypeDef,
     GeoLocationTypeDef,
     GetAccountLimitRequestRequestTypeDef,
     GetChangeRequestRequestTypeDef,
     WaiterConfigTypeDef,
+    GetCheckerIpRangesResponseTypeDef,
     GetDNSSECRequestRequestTypeDef,
     GetGeoLocationRequestRequestTypeDef,
+    GetHealthCheckCountResponseTypeDef,
     GetHealthCheckLastFailureReasonRequestRequestTypeDef,
     GetHealthCheckRequestRequestTypeDef,
     GetHealthCheckStatusRequestRequestTypeDef,
+    GetHostedZoneCountResponseTypeDef,
     GetHostedZoneLimitRequestRequestTypeDef,
     HostedZoneLimitTypeDef,
     GetHostedZoneRequestRequestTypeDef,
     GetQueryLoggingConfigRequestRequestTypeDef,
     GetReusableDelegationSetLimitRequestRequestTypeDef,
     ReusableDelegationSetLimitTypeDef,
     GetReusableDelegationSetRequestRequestTypeDef,
+    GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceRequestRequestTypeDef,
     GetTrafficPolicyRequestRequestTypeDef,
     StatusReportTypeDef,
     LinkedServiceTypeDef,
     HostedZoneOwnerTypeDef,
-    PaginatorConfigTypeDef,
+    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
     ListCidrBlocksRequestRequestTypeDef,
+    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
     ListCidrCollectionsRequestRequestTypeDef,
+    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
     ListCidrLocationsRequestRequestTypeDef,
     LocationSummaryTypeDef,
     ListGeoLocationsRequestRequestTypeDef,
+    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
     ListHealthChecksRequestRequestTypeDef,
     ListHostedZonesByNameRequestRequestTypeDef,
     ListHostedZonesByVPCRequestRequestTypeDef,
+    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
     ListHostedZonesRequestRequestTypeDef,
+    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
     ListQueryLoggingConfigsRequestRequestTypeDef,
+    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
     ListResourceRecordSetsRequestRequestTypeDef,
     ListReusableDelegationSetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
     ListTrafficPoliciesRequestRequestTypeDef,
     TrafficPolicySummaryTypeDef,
     ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef,
     ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef,
     ListTrafficPolicyInstancesRequestRequestTypeDef,
     ListTrafficPolicyVersionsRequestRequestTypeDef,
+    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListVPCAssociationAuthorizationsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ResourceRecordTypeDef,
+    ResponseMetadataTypeDef,
     TestDNSAnswerRequestRequestTypeDef,
+    TestDNSAnswerResponseTypeDef,
     UpdateHostedZoneCommentRequestRequestTypeDef,
     UpdateTrafficPolicyCommentRequestRequestTypeDef,
     UpdateTrafficPolicyInstanceRequestRequestTypeDef,
+    GetAccountLimitResponseTypeDef,
     ActivateKeySigningKeyResponseTypeDef,
     AssociateVPCWithHostedZoneResponseTypeDef,
-    ChangeCidrCollectionResponseTypeDef,
     ChangeResourceRecordSetsResponseTypeDef,
     DeactivateKeySigningKeyResponseTypeDef,
     DeleteHostedZoneResponseTypeDef,
     DeleteKeySigningKeyResponseTypeDef,
     DisableHostedZoneDNSSECResponseTypeDef,
     DisassociateVPCFromHostedZoneResponseTypeDef,
     EnableHostedZoneDNSSECResponseTypeDef,
-    GetAccountLimitResponseTypeDef,
     GetChangeResponseTypeDef,
-    GetCheckerIpRangesResponseTypeDef,
-    GetHealthCheckCountResponseTypeDef,
-    GetHostedZoneCountResponseTypeDef,
-    GetTrafficPolicyInstanceCountResponseTypeDef,
-    TestDNSAnswerResponseTypeDef,
     HealthCheckConfigTypeDef,
     UpdateHealthCheckRequestRequestTypeDef,
     AssociateVPCWithHostedZoneRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationResponseTypeDef,
     DeleteVPCAssociationAuthorizationRequestRequestTypeDef,
     DisassociateVPCFromHostedZoneRequestRequestTypeDef,
@@ -508,22 +516,14 @@
     ListGeoLocationsResponseTypeDef,
     GetChangeRequestResourceRecordSetsChangedWaitTypeDef,
     GetHostedZoneLimitResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     HealthCheckObservationTypeDef,
     HostedZoneTypeDef,
     HostedZoneSummaryTypeDef,
-    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
-    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
-    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
-    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
-    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListTrafficPoliciesResponseTypeDef,
     ResourceRecordSetTypeDef,
     CreateHealthCheckRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsForResourcesResponseTypeDef,
     HealthCheckTypeDef,
@@ -553,42 +553,42 @@
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

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/__init__.py` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/__init__.pyi` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/__main__.py` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53 1.26.56\nVersion:         1.26.56\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Route53 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.56")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/client.py` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/client.pyi` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/literals.py` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,15 @@
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
@@ -265,21 +266,23 @@
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
@@ -358,14 +361,15 @@
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
@@ -376,14 +380,15 @@
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
@@ -419,14 +424,15 @@
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
@@ -445,16 +451,19 @@
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
@@ -534,18 +543,21 @@
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

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/literals.pyi` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,15 @@
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
@@ -263,21 +264,23 @@
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
@@ -356,14 +359,15 @@
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
@@ -374,14 +378,15 @@
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
@@ -417,14 +422,15 @@
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
@@ -443,16 +449,19 @@
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
@@ -532,18 +541,21 @@
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

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/paginator.py` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,105 +78,105 @@
     """
 
     def paginate(
         self,
         *,
         CollectionId: str,
         LocationName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCidrBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrBlocks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrblockspaginator)
         """
 
 
 class ListCidrCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrcollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCidrCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrcollectionspaginator)
         """
 
 
 class ListCidrLocationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrLocations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrlocationspaginator)
     """
 
     def paginate(
-        self, *, CollectionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CollectionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCidrLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrlocationspaginator)
         """
 
 
 class ListHealthChecksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhealthcheckspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHealthChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhealthcheckspaginator)
         """
 
 
 class ListHostedZonesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhostedzonespaginator)
     """
 
     def paginate(
-        self, *, DelegationSetId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DelegationSetId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHostedZonesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhostedzonespaginator)
         """
 
 
 class ListQueryLoggingConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listqueryloggingconfigspaginator)
     """
 
     def paginate(
-        self, *, HostedZoneId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, HostedZoneId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQueryLoggingConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listqueryloggingconfigspaginator)
         """
 
 
 class ListResourceRecordSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listresourcerecordsetspaginator)
     """
 
     def paginate(
-        self, *, HostedZoneId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, HostedZoneId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceRecordSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listresourcerecordsetspaginator)
         """
 
 
@@ -187,13 +187,13 @@
     """
 
     def paginate(
         self,
         *,
         HostedZoneId: str,
         MaxResults: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVPCAssociationAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListVPCAssociationAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listvpcassociationauthorizationspaginator)
         """
```

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/paginator.pyi` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -75,99 +75,99 @@
     """
 
     def paginate(
         self,
         *,
         CollectionId: str,
         LocationName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCidrBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrBlocks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrblockspaginator)
         """
 
 class ListCidrCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrcollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCidrCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrcollectionspaginator)
         """
 
 class ListCidrLocationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrLocations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrlocationspaginator)
     """
 
     def paginate(
-        self, *, CollectionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CollectionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCidrLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrlocationspaginator)
         """
 
 class ListHealthChecksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhealthcheckspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHealthChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhealthcheckspaginator)
         """
 
 class ListHostedZonesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhostedzonespaginator)
     """
 
     def paginate(
-        self, *, DelegationSetId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DelegationSetId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHostedZonesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhostedzonespaginator)
         """
 
 class ListQueryLoggingConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listqueryloggingconfigspaginator)
     """
 
     def paginate(
-        self, *, HostedZoneId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, HostedZoneId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQueryLoggingConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listqueryloggingconfigspaginator)
         """
 
 class ListResourceRecordSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listresourcerecordsetspaginator)
     """
 
     def paginate(
-        self, *, HostedZoneId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, HostedZoneId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceRecordSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listresourcerecordsetspaginator)
         """
 
 class ListVPCAssociationAuthorizationsPaginator(Paginator):
@@ -177,13 +177,13 @@
     """
 
     def paginate(
         self,
         *,
         HostedZoneId: str,
         MaxResults: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVPCAssociationAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListVPCAssociationAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listvpcassociationauthorizationspaginator)
         """
```

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/type_defs.py` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,19 +45,19 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountLimitTypeDef",
     "ActivateKeySigningKeyRequestRequestTypeDef",
     "ChangeInfoTypeDef",
-    "ResponseMetadataTypeDef",
     "AlarmIdentifierTypeDef",
     "AliasTargetTypeDef",
     "VPCTypeDef",
     "CidrCollectionChangeTypeDef",
+    "ChangeCidrCollectionResponseTypeDef",
     "TagTypeDef",
     "CidrBlockSummaryTypeDef",
     "CidrCollectionTypeDef",
     "CidrRoutingConfigTypeDef",
     "DimensionTypeDef",
     "CollectionSummaryTypeDef",
     "CreateCidrCollectionRequestRequestTypeDef",
@@ -86,75 +86,83 @@
     "DisableHostedZoneDNSSECRequestRequestTypeDef",
     "EnableHostedZoneDNSSECRequestRequestTypeDef",
     "GeoLocationDetailsTypeDef",
     "GeoLocationTypeDef",
     "GetAccountLimitRequestRequestTypeDef",
     "GetChangeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
+    "GetCheckerIpRangesResponseTypeDef",
     "GetDNSSECRequestRequestTypeDef",
     "GetGeoLocationRequestRequestTypeDef",
+    "GetHealthCheckCountResponseTypeDef",
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
     "GetHealthCheckRequestRequestTypeDef",
     "GetHealthCheckStatusRequestRequestTypeDef",
+    "GetHostedZoneCountResponseTypeDef",
     "GetHostedZoneLimitRequestRequestTypeDef",
     "HostedZoneLimitTypeDef",
     "GetHostedZoneRequestRequestTypeDef",
     "GetQueryLoggingConfigRequestRequestTypeDef",
     "GetReusableDelegationSetLimitRequestRequestTypeDef",
     "ReusableDelegationSetLimitTypeDef",
     "GetReusableDelegationSetRequestRequestTypeDef",
+    "GetTrafficPolicyInstanceCountResponseTypeDef",
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     "GetTrafficPolicyRequestRequestTypeDef",
     "StatusReportTypeDef",
     "LinkedServiceTypeDef",
     "HostedZoneOwnerTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
     "ListCidrBlocksRequestRequestTypeDef",
+    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
     "ListCidrCollectionsRequestRequestTypeDef",
+    "ListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
     "ListCidrLocationsRequestRequestTypeDef",
     "LocationSummaryTypeDef",
     "ListGeoLocationsRequestRequestTypeDef",
+    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
     "ListHealthChecksRequestRequestTypeDef",
     "ListHostedZonesByNameRequestRequestTypeDef",
     "ListHostedZonesByVPCRequestRequestTypeDef",
+    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
     "ListHostedZonesRequestRequestTypeDef",
+    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
     "ListQueryLoggingConfigsRequestRequestTypeDef",
+    "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
     "ListResourceRecordSetsRequestRequestTypeDef",
     "ListReusableDelegationSetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourcesRequestRequestTypeDef",
     "ListTrafficPoliciesRequestRequestTypeDef",
     "TrafficPolicySummaryTypeDef",
     "ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef",
     "ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef",
     "ListTrafficPolicyInstancesRequestRequestTypeDef",
     "ListTrafficPolicyVersionsRequestRequestTypeDef",
+    "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListVPCAssociationAuthorizationsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceRecordTypeDef",
+    "ResponseMetadataTypeDef",
     "TestDNSAnswerRequestRequestTypeDef",
+    "TestDNSAnswerResponseTypeDef",
     "UpdateHostedZoneCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyInstanceRequestRequestTypeDef",
+    "GetAccountLimitResponseTypeDef",
     "ActivateKeySigningKeyResponseTypeDef",
     "AssociateVPCWithHostedZoneResponseTypeDef",
-    "ChangeCidrCollectionResponseTypeDef",
     "ChangeResourceRecordSetsResponseTypeDef",
     "DeactivateKeySigningKeyResponseTypeDef",
     "DeleteHostedZoneResponseTypeDef",
     "DeleteKeySigningKeyResponseTypeDef",
     "DisableHostedZoneDNSSECResponseTypeDef",
     "DisassociateVPCFromHostedZoneResponseTypeDef",
     "EnableHostedZoneDNSSECResponseTypeDef",
-    "GetAccountLimitResponseTypeDef",
     "GetChangeResponseTypeDef",
-    "GetCheckerIpRangesResponseTypeDef",
-    "GetHealthCheckCountResponseTypeDef",
-    "GetHostedZoneCountResponseTypeDef",
-    "GetTrafficPolicyInstanceCountResponseTypeDef",
-    "TestDNSAnswerResponseTypeDef",
     "HealthCheckConfigTypeDef",
     "UpdateHealthCheckRequestRequestTypeDef",
     "AssociateVPCWithHostedZoneRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationResponseTypeDef",
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     "DisassociateVPCFromHostedZoneRequestRequestTypeDef",
@@ -190,22 +198,14 @@
     "ListGeoLocationsResponseTypeDef",
     "GetChangeRequestResourceRecordSetsChangedWaitTypeDef",
     "GetHostedZoneLimitResponseTypeDef",
     "GetReusableDelegationSetLimitResponseTypeDef",
     "HealthCheckObservationTypeDef",
     "HostedZoneTypeDef",
     "HostedZoneSummaryTypeDef",
-    "ListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
-    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
-    "ListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
-    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
-    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
-    "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListCidrLocationsResponseTypeDef",
     "ListTrafficPoliciesResponseTypeDef",
     "ResourceRecordSetTypeDef",
     "CreateHealthCheckRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListTagsForResourcesResponseTypeDef",
     "HealthCheckTypeDef",
@@ -260,25 +260,14 @@
 )
 
 
 class ChangeInfoTypeDef(_RequiredChangeInfoTypeDef, _OptionalChangeInfoTypeDef):
     pass
 
 
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
 AlarmIdentifierTypeDef = TypedDict(
     "AlarmIdentifierTypeDef",
     {
         "Region": CloudWatchRegionType,
         "Name": str,
     },
 )
@@ -306,14 +295,22 @@
     {
         "LocationName": str,
         "Action": CidrCollectionChangeActionType,
         "CidrList": Sequence[str],
     },
 )
 
+ChangeCidrCollectionResponseTypeDef = TypedDict(
+    "ChangeCidrCollectionResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -702,14 +699,22 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
+GetCheckerIpRangesResponseTypeDef = TypedDict(
+    "GetCheckerIpRangesResponseTypeDef",
+    {
+        "CheckerIpRanges": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDNSSECRequestRequestTypeDef = TypedDict(
     "GetDNSSECRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 
@@ -719,14 +724,22 @@
         "ContinentCode": str,
         "CountryCode": str,
         "SubdivisionCode": str,
     },
     total=False,
 )
 
+GetHealthCheckCountResponseTypeDef = TypedDict(
+    "GetHealthCheckCountResponseTypeDef",
+    {
+        "HealthCheckCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetHealthCheckLastFailureReasonRequestRequestTypeDef = TypedDict(
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
     {
         "HealthCheckId": str,
     },
 )
 
@@ -740,14 +753,22 @@
 GetHealthCheckStatusRequestRequestTypeDef = TypedDict(
     "GetHealthCheckStatusRequestRequestTypeDef",
     {
         "HealthCheckId": str,
     },
 )
 
+GetHostedZoneCountResponseTypeDef = TypedDict(
+    "GetHostedZoneCountResponseTypeDef",
+    {
+        "HostedZoneCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetHostedZoneLimitRequestRequestTypeDef = TypedDict(
     "GetHostedZoneLimitRequestRequestTypeDef",
     {
         "Type": HostedZoneLimitTypeType,
         "HostedZoneId": str,
     },
 )
@@ -793,14 +814,22 @@
 GetReusableDelegationSetRequestRequestTypeDef = TypedDict(
     "GetReusableDelegationSetRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+GetTrafficPolicyInstanceCountResponseTypeDef = TypedDict(
+    "GetTrafficPolicyInstanceCountResponseTypeDef",
+    {
+        "TrafficPolicyInstanceCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTrafficPolicyInstanceRequestRequestTypeDef = TypedDict(
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -835,24 +864,37 @@
     {
         "OwningAccount": str,
         "OwningService": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
+    "_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "CollectionId": str,
+    },
+)
+_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
+    "_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    {
+        "LocationName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(
+    _RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    _OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListCidrBlocksRequestRequestTypeDef = TypedDict(
     "_RequiredListCidrBlocksRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListCidrBlocksRequestRequestTypeDef = TypedDict(
@@ -868,23 +910,53 @@
 
 class ListCidrBlocksRequestRequestTypeDef(
     _RequiredListCidrBlocksRequestRequestTypeDef, _OptionalListCidrBlocksRequestRequestTypeDef
 ):
     pass
 
 
+ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef = TypedDict(
+    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCidrCollectionsRequestRequestTypeDef = TypedDict(
     "ListCidrCollectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": str,
     },
     total=False,
 )
 
+_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
+    "_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
+    "_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(
+    _RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+    _OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListCidrLocationsRequestRequestTypeDef = TypedDict(
     "_RequiredListCidrLocationsRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListCidrLocationsRequestRequestTypeDef = TypedDict(
@@ -918,14 +990,22 @@
         "StartCountryCode": str,
         "StartSubdivisionCode": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+ListHealthChecksRequestListHealthChecksPaginateTypeDef = TypedDict(
+    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListHealthChecksRequestRequestTypeDef = TypedDict(
     "ListHealthChecksRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -961,34 +1041,74 @@
 class ListHostedZonesByVPCRequestRequestTypeDef(
     _RequiredListHostedZonesByVPCRequestRequestTypeDef,
     _OptionalListHostedZonesByVPCRequestRequestTypeDef,
 ):
     pass
 
 
+ListHostedZonesRequestListHostedZonesPaginateTypeDef = TypedDict(
+    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
+    {
+        "DelegationSetId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListHostedZonesRequestRequestTypeDef = TypedDict(
     "ListHostedZonesRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
         "DelegationSetId": str,
     },
     total=False,
 )
 
+ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = TypedDict(
+    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListQueryLoggingConfigsRequestRequestTypeDef = TypedDict(
     "ListQueryLoggingConfigsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "NextToken": str,
         "MaxResults": str,
     },
     total=False,
 )
 
+_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+    },
+)
+_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(
+    _RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+    _OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListResourceRecordSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceRecordSetsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 _OptionalListResourceRecordSetsRequestRequestTypeDef = TypedDict(
@@ -1135,14 +1255,37 @@
 class ListTrafficPolicyVersionsRequestRequestTypeDef(
     _RequiredListTrafficPolicyVersionsRequestRequestTypeDef,
     _OptionalListTrafficPolicyVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
+    "_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+    },
+)
+_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
+    "_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
+    {
+        "MaxResults": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(
+    _RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
+    _OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef = TypedDict(
     "_RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef = TypedDict(
@@ -1158,21 +1301,42 @@
 class ListVPCAssociationAuthorizationsRequestRequestTypeDef(
     _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef,
     _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef,
 ):
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
 ResourceRecordTypeDef = TypedDict(
     "ResourceRecordTypeDef",
     {
         "Value": str,
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
 _RequiredTestDNSAnswerRequestRequestTypeDef = TypedDict(
     "_RequiredTestDNSAnswerRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "RecordName": str,
         "RecordType": RRTypeType,
     },
@@ -1190,14 +1354,27 @@
 
 class TestDNSAnswerRequestRequestTypeDef(
     _RequiredTestDNSAnswerRequestRequestTypeDef, _OptionalTestDNSAnswerRequestRequestTypeDef
 ):
     pass
 
 
+TestDNSAnswerResponseTypeDef = TypedDict(
+    "TestDNSAnswerResponseTypeDef",
+    {
+        "Nameserver": str,
+        "RecordName": str,
+        "RecordType": RRTypeType,
+        "RecordData": List[str],
+        "ResponseCode": str,
+        "Protocol": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateHostedZoneCommentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHostedZoneCommentRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateHostedZoneCommentRequestRequestTypeDef = TypedDict(
@@ -1231,153 +1408,100 @@
         "Id": str,
         "TTL": int,
         "TrafficPolicyId": str,
         "TrafficPolicyVersion": int,
     },
 )
 
+GetAccountLimitResponseTypeDef = TypedDict(
+    "GetAccountLimitResponseTypeDef",
+    {
+        "Limit": AccountLimitTypeDef,
+        "Count": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ActivateKeySigningKeyResponseTypeDef = TypedDict(
     "ActivateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateVPCWithHostedZoneResponseTypeDef = TypedDict(
     "AssociateVPCWithHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ChangeCidrCollectionResponseTypeDef = TypedDict(
-    "ChangeCidrCollectionResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeResourceRecordSetsResponseTypeDef = TypedDict(
     "ChangeResourceRecordSetsResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeactivateKeySigningKeyResponseTypeDef = TypedDict(
     "DeactivateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteHostedZoneResponseTypeDef = TypedDict(
     "DeleteHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteKeySigningKeyResponseTypeDef = TypedDict(
     "DeleteKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisableHostedZoneDNSSECResponseTypeDef = TypedDict(
     "DisableHostedZoneDNSSECResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateVPCFromHostedZoneResponseTypeDef = TypedDict(
     "DisassociateVPCFromHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnableHostedZoneDNSSECResponseTypeDef = TypedDict(
     "EnableHostedZoneDNSSECResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccountLimitResponseTypeDef = TypedDict(
-    "GetAccountLimitResponseTypeDef",
-    {
-        "Limit": AccountLimitTypeDef,
-        "Count": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChangeResponseTypeDef = TypedDict(
     "GetChangeResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCheckerIpRangesResponseTypeDef = TypedDict(
-    "GetCheckerIpRangesResponseTypeDef",
-    {
-        "CheckerIpRanges": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetHealthCheckCountResponseTypeDef = TypedDict(
-    "GetHealthCheckCountResponseTypeDef",
-    {
-        "HealthCheckCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetHostedZoneCountResponseTypeDef = TypedDict(
-    "GetHostedZoneCountResponseTypeDef",
-    {
-        "HostedZoneCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTrafficPolicyInstanceCountResponseTypeDef = TypedDict(
-    "GetTrafficPolicyInstanceCountResponseTypeDef",
-    {
-        "TrafficPolicyInstanceCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestDNSAnswerResponseTypeDef = TypedDict(
-    "TestDNSAnswerResponseTypeDef",
-    {
-        "Nameserver": str,
-        "RecordName": str,
-        "RecordType": RRTypeType,
-        "RecordData": List[str],
-        "ResponseCode": str,
-        "Protocol": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
@@ -1482,15 +1606,15 @@
 )
 
 CreateVPCAssociationAuthorizationResponseTypeDef = TypedDict(
     "CreateVPCAssociationAuthorizationResponseTypeDef",
     {
         "HostedZoneId": str,
         "VPC": VPCTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVPCAssociationAuthorizationRequestRequestTypeDef = TypedDict(
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     {
         "HostedZoneId": str,
@@ -1523,15 +1647,15 @@
 
 ListVPCAssociationAuthorizationsResponseTypeDef = TypedDict(
     "ListVPCAssociationAuthorizationsResponseTypeDef",
     {
         "HostedZoneId": str,
         "NextToken": str,
         "VPCs": List[VPCTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredChangeCidrCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredChangeCidrCollectionRequestRequestTypeDef",
     {
         "Id": str,
@@ -1589,24 +1713,24 @@
 )
 
 ListCidrBlocksResponseTypeDef = TypedDict(
     "ListCidrBlocksResponseTypeDef",
     {
         "NextToken": str,
         "CidrBlocks": List[CidrBlockSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCidrCollectionResponseTypeDef = TypedDict(
     "CreateCidrCollectionResponseTypeDef",
     {
         "Collection": CidrCollectionTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCloudWatchAlarmConfigurationTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmConfigurationTypeDef",
     {
         "EvaluationPeriods": int,
@@ -1634,15 +1758,15 @@
 
 
 ListCidrCollectionsResponseTypeDef = TypedDict(
     "ListCidrCollectionsResponseTypeDef",
     {
         "NextToken": str,
         "CidrCollections": List[CollectionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateHostedZoneRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHostedZoneRequestRequestTypeDef",
     {
         "Name": str,
@@ -1667,209 +1791,209 @@
 
 
 CreateReusableDelegationSetResponseTypeDef = TypedDict(
     "CreateReusableDelegationSetResponseTypeDef",
     {
         "DelegationSet": DelegationSetTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReusableDelegationSetResponseTypeDef = TypedDict(
     "GetReusableDelegationSetResponseTypeDef",
     {
         "DelegationSet": DelegationSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReusableDelegationSetsResponseTypeDef = TypedDict(
     "ListReusableDelegationSetsResponseTypeDef",
     {
         "DelegationSets": List[DelegationSetTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateKeySigningKeyResponseTypeDef = TypedDict(
     "CreateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
         "KeySigningKey": KeySigningKeyTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateQueryLoggingConfigResponseTypeDef = TypedDict(
     "CreateQueryLoggingConfigResponseTypeDef",
     {
         "QueryLoggingConfig": QueryLoggingConfigTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryLoggingConfigResponseTypeDef = TypedDict(
     "GetQueryLoggingConfigResponseTypeDef",
     {
         "QueryLoggingConfig": QueryLoggingConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListQueryLoggingConfigsResponseTypeDef = TypedDict(
     "ListQueryLoggingConfigsResponseTypeDef",
     {
         "QueryLoggingConfigs": List[QueryLoggingConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "CreateTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "GetTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficPolicyInstancesByHostedZoneResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesByHostedZoneResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficPolicyInstancesByPolicyResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesByPolicyResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "HostedZoneIdMarker": str,
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficPolicyInstancesResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "HostedZoneIdMarker": str,
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "UpdateTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTrafficPolicyResponseTypeDef = TypedDict(
     "CreateTrafficPolicyResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTrafficPolicyVersionResponseTypeDef = TypedDict(
     "CreateTrafficPolicyVersionResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTrafficPolicyResponseTypeDef = TypedDict(
     "GetTrafficPolicyResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficPolicyVersionsResponseTypeDef = TypedDict(
     "ListTrafficPolicyVersionsResponseTypeDef",
     {
         "TrafficPolicies": List[TrafficPolicyTypeDef],
         "IsTruncated": bool,
         "TrafficPolicyVersionMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTrafficPolicyCommentResponseTypeDef = TypedDict(
     "UpdateTrafficPolicyCommentResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDNSSECResponseTypeDef = TypedDict(
     "GetDNSSECResponseTypeDef",
     {
         "Status": DNSSECStatusTypeDef,
         "KeySigningKeys": List[KeySigningKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGeoLocationResponseTypeDef = TypedDict(
     "GetGeoLocationResponseTypeDef",
     {
         "GeoLocationDetails": GeoLocationDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGeoLocationsResponseTypeDef = TypedDict(
     "ListGeoLocationsResponseTypeDef",
     {
         "GeoLocationDetailsList": List[GeoLocationDetailsTypeDef],
         "IsTruncated": bool,
         "NextContinentCode": str,
         "NextCountryCode": str,
         "NextSubdivisionCode": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetChangeRequestResourceRecordSetsChangedWaitTypeDef = TypedDict(
     "_RequiredGetChangeRequestResourceRecordSetsChangedWaitTypeDef",
     {
         "Id": str,
@@ -1892,24 +2016,24 @@
 
 
 GetHostedZoneLimitResponseTypeDef = TypedDict(
     "GetHostedZoneLimitResponseTypeDef",
     {
         "Limit": HostedZoneLimitTypeDef,
         "Count": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReusableDelegationSetLimitResponseTypeDef = TypedDict(
     "GetReusableDelegationSetLimitResponseTypeDef",
     {
         "Limit": ReusableDelegationSetLimitTypeDef,
         "Count": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HealthCheckObservationTypeDef = TypedDict(
     "HealthCheckObservationTypeDef",
     {
         "Region": HealthCheckRegionType,
@@ -1947,155 +2071,31 @@
     {
         "HostedZoneId": str,
         "Name": str,
         "Owner": HostedZoneOwnerTypeDef,
     },
 )
 
-_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
-    "_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
-    "_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
-    {
-        "LocationName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(
-    _RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-    _OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-):
-    pass
-
-
-ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef = TypedDict(
-    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
-    "_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
-    "_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(
-    _RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-    _OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-):
-    pass
-
-
-ListHealthChecksRequestListHealthChecksPaginateTypeDef = TypedDict(
-    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListHostedZonesRequestListHostedZonesPaginateTypeDef = TypedDict(
-    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
-    {
-        "DelegationSetId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = TypedDict(
-    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-    },
-)
-_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(
-    _RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-    _OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
-    "_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-    },
-)
-_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
-    "_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
-    {
-        "MaxResults": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(
-    _RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
-    _OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
-):
-    pass
-
-
 ListCidrLocationsResponseTypeDef = TypedDict(
     "ListCidrLocationsResponseTypeDef",
     {
         "NextToken": str,
         "CidrLocations": List[LocationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficPoliciesResponseTypeDef = TypedDict(
     "ListTrafficPoliciesResponseTypeDef",
     {
         "TrafficPolicySummaries": List[TrafficPolicySummaryTypeDef],
         "IsTruncated": bool,
         "TrafficPolicyIdMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredResourceRecordSetTypeDef = TypedDict(
     "_RequiredResourceRecordSetTypeDef",
     {
         "Name": str,
@@ -2136,23 +2136,23 @@
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTagSet": ResourceTagSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourcesResponseTypeDef = TypedDict(
     "ListTagsForResourcesResponseTypeDef",
     {
         "ResourceTagSets": List[ResourceTagSetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "Id": str,
@@ -2175,89 +2175,89 @@
     pass
 
 
 GetHealthCheckLastFailureReasonResponseTypeDef = TypedDict(
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     {
         "HealthCheckObservations": List[HealthCheckObservationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetHealthCheckStatusResponseTypeDef = TypedDict(
     "GetHealthCheckStatusResponseTypeDef",
     {
         "HealthCheckObservations": List[HealthCheckObservationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHostedZoneResponseTypeDef = TypedDict(
     "CreateHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "ChangeInfo": ChangeInfoTypeDef,
         "DelegationSet": DelegationSetTypeDef,
         "VPC": VPCTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetHostedZoneResponseTypeDef = TypedDict(
     "GetHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "DelegationSet": DelegationSetTypeDef,
         "VPCs": List[VPCTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListHostedZonesByNameResponseTypeDef = TypedDict(
     "ListHostedZonesByNameResponseTypeDef",
     {
         "HostedZones": List[HostedZoneTypeDef],
         "DNSName": str,
         "HostedZoneId": str,
         "IsTruncated": bool,
         "NextDNSName": str,
         "NextHostedZoneId": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListHostedZonesResponseTypeDef = TypedDict(
     "ListHostedZonesResponseTypeDef",
     {
         "HostedZones": List[HostedZoneTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateHostedZoneCommentResponseTypeDef = TypedDict(
     "UpdateHostedZoneCommentResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListHostedZonesByVPCResponseTypeDef = TypedDict(
     "ListHostedZonesByVPCResponseTypeDef",
     {
         "HostedZoneSummaries": List[HostedZoneSummaryTypeDef],
         "MaxItems": str,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeTypeDef = TypedDict(
     "ChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -2270,52 +2270,52 @@
     {
         "ResourceRecordSets": List[ResourceRecordSetTypeDef],
         "IsTruncated": bool,
         "NextRecordName": str,
         "NextRecordType": RRTypeType,
         "NextRecordIdentifier": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHealthCheckResponseTypeDef = TypedDict(
     "CreateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetHealthCheckResponseTypeDef = TypedDict(
     "GetHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListHealthChecksResponseTypeDef = TypedDict(
     "ListHealthChecksResponseTypeDef",
     {
         "HealthChecks": List[HealthCheckTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateHealthCheckResponseTypeDef = TypedDict(
     "UpdateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredChangeBatchTypeDef = TypedDict(
     "_RequiredChangeBatchTypeDef",
     {
         "Changes": Sequence[ChangeTypeDef],
```

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/type_defs.pyi` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,19 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountLimitTypeDef",
     "ActivateKeySigningKeyRequestRequestTypeDef",
     "ChangeInfoTypeDef",
-    "ResponseMetadataTypeDef",
     "AlarmIdentifierTypeDef",
     "AliasTargetTypeDef",
     "VPCTypeDef",
     "CidrCollectionChangeTypeDef",
+    "ChangeCidrCollectionResponseTypeDef",
     "TagTypeDef",
     "CidrBlockSummaryTypeDef",
     "CidrCollectionTypeDef",
     "CidrRoutingConfigTypeDef",
     "DimensionTypeDef",
     "CollectionSummaryTypeDef",
     "CreateCidrCollectionRequestRequestTypeDef",
@@ -85,75 +85,83 @@
     "DisableHostedZoneDNSSECRequestRequestTypeDef",
     "EnableHostedZoneDNSSECRequestRequestTypeDef",
     "GeoLocationDetailsTypeDef",
     "GeoLocationTypeDef",
     "GetAccountLimitRequestRequestTypeDef",
     "GetChangeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
+    "GetCheckerIpRangesResponseTypeDef",
     "GetDNSSECRequestRequestTypeDef",
     "GetGeoLocationRequestRequestTypeDef",
+    "GetHealthCheckCountResponseTypeDef",
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
     "GetHealthCheckRequestRequestTypeDef",
     "GetHealthCheckStatusRequestRequestTypeDef",
+    "GetHostedZoneCountResponseTypeDef",
     "GetHostedZoneLimitRequestRequestTypeDef",
     "HostedZoneLimitTypeDef",
     "GetHostedZoneRequestRequestTypeDef",
     "GetQueryLoggingConfigRequestRequestTypeDef",
     "GetReusableDelegationSetLimitRequestRequestTypeDef",
     "ReusableDelegationSetLimitTypeDef",
     "GetReusableDelegationSetRequestRequestTypeDef",
+    "GetTrafficPolicyInstanceCountResponseTypeDef",
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     "GetTrafficPolicyRequestRequestTypeDef",
     "StatusReportTypeDef",
     "LinkedServiceTypeDef",
     "HostedZoneOwnerTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
     "ListCidrBlocksRequestRequestTypeDef",
+    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
     "ListCidrCollectionsRequestRequestTypeDef",
+    "ListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
     "ListCidrLocationsRequestRequestTypeDef",
     "LocationSummaryTypeDef",
     "ListGeoLocationsRequestRequestTypeDef",
+    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
     "ListHealthChecksRequestRequestTypeDef",
     "ListHostedZonesByNameRequestRequestTypeDef",
     "ListHostedZonesByVPCRequestRequestTypeDef",
+    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
     "ListHostedZonesRequestRequestTypeDef",
+    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
     "ListQueryLoggingConfigsRequestRequestTypeDef",
+    "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
     "ListResourceRecordSetsRequestRequestTypeDef",
     "ListReusableDelegationSetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourcesRequestRequestTypeDef",
     "ListTrafficPoliciesRequestRequestTypeDef",
     "TrafficPolicySummaryTypeDef",
     "ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef",
     "ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef",
     "ListTrafficPolicyInstancesRequestRequestTypeDef",
     "ListTrafficPolicyVersionsRequestRequestTypeDef",
+    "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListVPCAssociationAuthorizationsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceRecordTypeDef",
+    "ResponseMetadataTypeDef",
     "TestDNSAnswerRequestRequestTypeDef",
+    "TestDNSAnswerResponseTypeDef",
     "UpdateHostedZoneCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyInstanceRequestRequestTypeDef",
+    "GetAccountLimitResponseTypeDef",
     "ActivateKeySigningKeyResponseTypeDef",
     "AssociateVPCWithHostedZoneResponseTypeDef",
-    "ChangeCidrCollectionResponseTypeDef",
     "ChangeResourceRecordSetsResponseTypeDef",
     "DeactivateKeySigningKeyResponseTypeDef",
     "DeleteHostedZoneResponseTypeDef",
     "DeleteKeySigningKeyResponseTypeDef",
     "DisableHostedZoneDNSSECResponseTypeDef",
     "DisassociateVPCFromHostedZoneResponseTypeDef",
     "EnableHostedZoneDNSSECResponseTypeDef",
-    "GetAccountLimitResponseTypeDef",
     "GetChangeResponseTypeDef",
-    "GetCheckerIpRangesResponseTypeDef",
-    "GetHealthCheckCountResponseTypeDef",
-    "GetHostedZoneCountResponseTypeDef",
-    "GetTrafficPolicyInstanceCountResponseTypeDef",
-    "TestDNSAnswerResponseTypeDef",
     "HealthCheckConfigTypeDef",
     "UpdateHealthCheckRequestRequestTypeDef",
     "AssociateVPCWithHostedZoneRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationResponseTypeDef",
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     "DisassociateVPCFromHostedZoneRequestRequestTypeDef",
@@ -189,22 +197,14 @@
     "ListGeoLocationsResponseTypeDef",
     "GetChangeRequestResourceRecordSetsChangedWaitTypeDef",
     "GetHostedZoneLimitResponseTypeDef",
     "GetReusableDelegationSetLimitResponseTypeDef",
     "HealthCheckObservationTypeDef",
     "HostedZoneTypeDef",
     "HostedZoneSummaryTypeDef",
-    "ListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
-    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
-    "ListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
-    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
-    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
-    "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListCidrLocationsResponseTypeDef",
     "ListTrafficPoliciesResponseTypeDef",
     "ResourceRecordSetTypeDef",
     "CreateHealthCheckRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListTagsForResourcesResponseTypeDef",
     "HealthCheckTypeDef",
@@ -257,25 +257,14 @@
     },
     total=False,
 )
 
 class ChangeInfoTypeDef(_RequiredChangeInfoTypeDef, _OptionalChangeInfoTypeDef):
     pass
 
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
 AlarmIdentifierTypeDef = TypedDict(
     "AlarmIdentifierTypeDef",
     {
         "Region": CloudWatchRegionType,
         "Name": str,
     },
 )
@@ -303,14 +292,22 @@
     {
         "LocationName": str,
         "Action": CidrCollectionChangeActionType,
         "CidrList": Sequence[str],
     },
 )
 
+ChangeCidrCollectionResponseTypeDef = TypedDict(
+    "ChangeCidrCollectionResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -689,14 +686,22 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
+GetCheckerIpRangesResponseTypeDef = TypedDict(
+    "GetCheckerIpRangesResponseTypeDef",
+    {
+        "CheckerIpRanges": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDNSSECRequestRequestTypeDef = TypedDict(
     "GetDNSSECRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 
@@ -706,14 +711,22 @@
         "ContinentCode": str,
         "CountryCode": str,
         "SubdivisionCode": str,
     },
     total=False,
 )
 
+GetHealthCheckCountResponseTypeDef = TypedDict(
+    "GetHealthCheckCountResponseTypeDef",
+    {
+        "HealthCheckCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetHealthCheckLastFailureReasonRequestRequestTypeDef = TypedDict(
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
     {
         "HealthCheckId": str,
     },
 )
 
@@ -727,14 +740,22 @@
 GetHealthCheckStatusRequestRequestTypeDef = TypedDict(
     "GetHealthCheckStatusRequestRequestTypeDef",
     {
         "HealthCheckId": str,
     },
 )
 
+GetHostedZoneCountResponseTypeDef = TypedDict(
+    "GetHostedZoneCountResponseTypeDef",
+    {
+        "HostedZoneCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetHostedZoneLimitRequestRequestTypeDef = TypedDict(
     "GetHostedZoneLimitRequestRequestTypeDef",
     {
         "Type": HostedZoneLimitTypeType,
         "HostedZoneId": str,
     },
 )
@@ -780,14 +801,22 @@
 GetReusableDelegationSetRequestRequestTypeDef = TypedDict(
     "GetReusableDelegationSetRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+GetTrafficPolicyInstanceCountResponseTypeDef = TypedDict(
+    "GetTrafficPolicyInstanceCountResponseTypeDef",
+    {
+        "TrafficPolicyInstanceCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTrafficPolicyInstanceRequestRequestTypeDef = TypedDict(
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -822,24 +851,35 @@
     {
         "OwningAccount": str,
         "OwningService": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
+    "_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "CollectionId": str,
+    },
+)
+_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
+    "_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    {
+        "LocationName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(
+    _RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    _OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+):
+    pass
+
 _RequiredListCidrBlocksRequestRequestTypeDef = TypedDict(
     "_RequiredListCidrBlocksRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListCidrBlocksRequestRequestTypeDef = TypedDict(
@@ -853,23 +893,51 @@
 )
 
 class ListCidrBlocksRequestRequestTypeDef(
     _RequiredListCidrBlocksRequestRequestTypeDef, _OptionalListCidrBlocksRequestRequestTypeDef
 ):
     pass
 
+ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef = TypedDict(
+    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCidrCollectionsRequestRequestTypeDef = TypedDict(
     "ListCidrCollectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": str,
     },
     total=False,
 )
 
+_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
+    "_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
+    "_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(
+    _RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+    _OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListCidrLocationsRequestRequestTypeDef = TypedDict(
     "_RequiredListCidrLocationsRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListCidrLocationsRequestRequestTypeDef = TypedDict(
@@ -901,14 +969,22 @@
         "StartCountryCode": str,
         "StartSubdivisionCode": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+ListHealthChecksRequestListHealthChecksPaginateTypeDef = TypedDict(
+    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListHealthChecksRequestRequestTypeDef = TypedDict(
     "ListHealthChecksRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -942,34 +1018,72 @@
 
 class ListHostedZonesByVPCRequestRequestTypeDef(
     _RequiredListHostedZonesByVPCRequestRequestTypeDef,
     _OptionalListHostedZonesByVPCRequestRequestTypeDef,
 ):
     pass
 
+ListHostedZonesRequestListHostedZonesPaginateTypeDef = TypedDict(
+    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
+    {
+        "DelegationSetId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListHostedZonesRequestRequestTypeDef = TypedDict(
     "ListHostedZonesRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
         "DelegationSetId": str,
     },
     total=False,
 )
 
+ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = TypedDict(
+    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListQueryLoggingConfigsRequestRequestTypeDef = TypedDict(
     "ListQueryLoggingConfigsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "NextToken": str,
         "MaxResults": str,
     },
     total=False,
 )
 
+_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+    },
+)
+_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(
+    _RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+    _OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListResourceRecordSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceRecordSetsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 _OptionalListResourceRecordSetsRequestRequestTypeDef = TypedDict(
@@ -1108,14 +1222,35 @@
 
 class ListTrafficPolicyVersionsRequestRequestTypeDef(
     _RequiredListTrafficPolicyVersionsRequestRequestTypeDef,
     _OptionalListTrafficPolicyVersionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
+    "_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+    },
+)
+_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
+    "_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
+    {
+        "MaxResults": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(
+    _RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
+    _OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef = TypedDict(
     "_RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef = TypedDict(
@@ -1129,21 +1264,42 @@
 
 class ListVPCAssociationAuthorizationsRequestRequestTypeDef(
     _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef,
     _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef,
 ):
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
 ResourceRecordTypeDef = TypedDict(
     "ResourceRecordTypeDef",
     {
         "Value": str,
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
 _RequiredTestDNSAnswerRequestRequestTypeDef = TypedDict(
     "_RequiredTestDNSAnswerRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "RecordName": str,
         "RecordType": RRTypeType,
     },
@@ -1159,14 +1315,27 @@
 )
 
 class TestDNSAnswerRequestRequestTypeDef(
     _RequiredTestDNSAnswerRequestRequestTypeDef, _OptionalTestDNSAnswerRequestRequestTypeDef
 ):
     pass
 
+TestDNSAnswerResponseTypeDef = TypedDict(
+    "TestDNSAnswerResponseTypeDef",
+    {
+        "Nameserver": str,
+        "RecordName": str,
+        "RecordType": RRTypeType,
+        "RecordData": List[str],
+        "ResponseCode": str,
+        "Protocol": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateHostedZoneCommentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHostedZoneCommentRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateHostedZoneCommentRequestRequestTypeDef = TypedDict(
@@ -1198,153 +1367,100 @@
         "Id": str,
         "TTL": int,
         "TrafficPolicyId": str,
         "TrafficPolicyVersion": int,
     },
 )
 
+GetAccountLimitResponseTypeDef = TypedDict(
+    "GetAccountLimitResponseTypeDef",
+    {
+        "Limit": AccountLimitTypeDef,
+        "Count": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ActivateKeySigningKeyResponseTypeDef = TypedDict(
     "ActivateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateVPCWithHostedZoneResponseTypeDef = TypedDict(
     "AssociateVPCWithHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ChangeCidrCollectionResponseTypeDef = TypedDict(
-    "ChangeCidrCollectionResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeResourceRecordSetsResponseTypeDef = TypedDict(
     "ChangeResourceRecordSetsResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeactivateKeySigningKeyResponseTypeDef = TypedDict(
     "DeactivateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteHostedZoneResponseTypeDef = TypedDict(
     "DeleteHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteKeySigningKeyResponseTypeDef = TypedDict(
     "DeleteKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisableHostedZoneDNSSECResponseTypeDef = TypedDict(
     "DisableHostedZoneDNSSECResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateVPCFromHostedZoneResponseTypeDef = TypedDict(
     "DisassociateVPCFromHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnableHostedZoneDNSSECResponseTypeDef = TypedDict(
     "EnableHostedZoneDNSSECResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccountLimitResponseTypeDef = TypedDict(
-    "GetAccountLimitResponseTypeDef",
-    {
-        "Limit": AccountLimitTypeDef,
-        "Count": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChangeResponseTypeDef = TypedDict(
     "GetChangeResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCheckerIpRangesResponseTypeDef = TypedDict(
-    "GetCheckerIpRangesResponseTypeDef",
-    {
-        "CheckerIpRanges": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetHealthCheckCountResponseTypeDef = TypedDict(
-    "GetHealthCheckCountResponseTypeDef",
-    {
-        "HealthCheckCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetHostedZoneCountResponseTypeDef = TypedDict(
-    "GetHostedZoneCountResponseTypeDef",
-    {
-        "HostedZoneCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTrafficPolicyInstanceCountResponseTypeDef = TypedDict(
-    "GetTrafficPolicyInstanceCountResponseTypeDef",
-    {
-        "TrafficPolicyInstanceCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestDNSAnswerResponseTypeDef = TypedDict(
-    "TestDNSAnswerResponseTypeDef",
-    {
-        "Nameserver": str,
-        "RecordName": str,
-        "RecordType": RRTypeType,
-        "RecordData": List[str],
-        "ResponseCode": str,
-        "Protocol": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
@@ -1443,15 +1559,15 @@
 )
 
 CreateVPCAssociationAuthorizationResponseTypeDef = TypedDict(
     "CreateVPCAssociationAuthorizationResponseTypeDef",
     {
         "HostedZoneId": str,
         "VPC": VPCTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVPCAssociationAuthorizationRequestRequestTypeDef = TypedDict(
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     {
         "HostedZoneId": str,
@@ -1482,15 +1598,15 @@
 
 ListVPCAssociationAuthorizationsResponseTypeDef = TypedDict(
     "ListVPCAssociationAuthorizationsResponseTypeDef",
     {
         "HostedZoneId": str,
         "NextToken": str,
         "VPCs": List[VPCTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredChangeCidrCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredChangeCidrCollectionRequestRequestTypeDef",
     {
         "Id": str,
@@ -1544,24 +1660,24 @@
 )
 
 ListCidrBlocksResponseTypeDef = TypedDict(
     "ListCidrBlocksResponseTypeDef",
     {
         "NextToken": str,
         "CidrBlocks": List[CidrBlockSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCidrCollectionResponseTypeDef = TypedDict(
     "CreateCidrCollectionResponseTypeDef",
     {
         "Collection": CidrCollectionTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCloudWatchAlarmConfigurationTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmConfigurationTypeDef",
     {
         "EvaluationPeriods": int,
@@ -1587,15 +1703,15 @@
     pass
 
 ListCidrCollectionsResponseTypeDef = TypedDict(
     "ListCidrCollectionsResponseTypeDef",
     {
         "NextToken": str,
         "CidrCollections": List[CollectionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateHostedZoneRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHostedZoneRequestRequestTypeDef",
     {
         "Name": str,
@@ -1618,209 +1734,209 @@
     pass
 
 CreateReusableDelegationSetResponseTypeDef = TypedDict(
     "CreateReusableDelegationSetResponseTypeDef",
     {
         "DelegationSet": DelegationSetTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReusableDelegationSetResponseTypeDef = TypedDict(
     "GetReusableDelegationSetResponseTypeDef",
     {
         "DelegationSet": DelegationSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReusableDelegationSetsResponseTypeDef = TypedDict(
     "ListReusableDelegationSetsResponseTypeDef",
     {
         "DelegationSets": List[DelegationSetTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateKeySigningKeyResponseTypeDef = TypedDict(
     "CreateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
         "KeySigningKey": KeySigningKeyTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateQueryLoggingConfigResponseTypeDef = TypedDict(
     "CreateQueryLoggingConfigResponseTypeDef",
     {
         "QueryLoggingConfig": QueryLoggingConfigTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryLoggingConfigResponseTypeDef = TypedDict(
     "GetQueryLoggingConfigResponseTypeDef",
     {
         "QueryLoggingConfig": QueryLoggingConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListQueryLoggingConfigsResponseTypeDef = TypedDict(
     "ListQueryLoggingConfigsResponseTypeDef",
     {
         "QueryLoggingConfigs": List[QueryLoggingConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "CreateTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "GetTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficPolicyInstancesByHostedZoneResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesByHostedZoneResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficPolicyInstancesByPolicyResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesByPolicyResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "HostedZoneIdMarker": str,
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficPolicyInstancesResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "HostedZoneIdMarker": str,
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "UpdateTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTrafficPolicyResponseTypeDef = TypedDict(
     "CreateTrafficPolicyResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTrafficPolicyVersionResponseTypeDef = TypedDict(
     "CreateTrafficPolicyVersionResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTrafficPolicyResponseTypeDef = TypedDict(
     "GetTrafficPolicyResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficPolicyVersionsResponseTypeDef = TypedDict(
     "ListTrafficPolicyVersionsResponseTypeDef",
     {
         "TrafficPolicies": List[TrafficPolicyTypeDef],
         "IsTruncated": bool,
         "TrafficPolicyVersionMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTrafficPolicyCommentResponseTypeDef = TypedDict(
     "UpdateTrafficPolicyCommentResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDNSSECResponseTypeDef = TypedDict(
     "GetDNSSECResponseTypeDef",
     {
         "Status": DNSSECStatusTypeDef,
         "KeySigningKeys": List[KeySigningKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGeoLocationResponseTypeDef = TypedDict(
     "GetGeoLocationResponseTypeDef",
     {
         "GeoLocationDetails": GeoLocationDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGeoLocationsResponseTypeDef = TypedDict(
     "ListGeoLocationsResponseTypeDef",
     {
         "GeoLocationDetailsList": List[GeoLocationDetailsTypeDef],
         "IsTruncated": bool,
         "NextContinentCode": str,
         "NextCountryCode": str,
         "NextSubdivisionCode": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetChangeRequestResourceRecordSetsChangedWaitTypeDef = TypedDict(
     "_RequiredGetChangeRequestResourceRecordSetsChangedWaitTypeDef",
     {
         "Id": str,
@@ -1841,24 +1957,24 @@
     pass
 
 GetHostedZoneLimitResponseTypeDef = TypedDict(
     "GetHostedZoneLimitResponseTypeDef",
     {
         "Limit": HostedZoneLimitTypeDef,
         "Count": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReusableDelegationSetLimitResponseTypeDef = TypedDict(
     "GetReusableDelegationSetLimitResponseTypeDef",
     {
         "Limit": ReusableDelegationSetLimitTypeDef,
         "Count": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HealthCheckObservationTypeDef = TypedDict(
     "HealthCheckObservationTypeDef",
     {
         "Region": HealthCheckRegionType,
@@ -1894,147 +2010,31 @@
     {
         "HostedZoneId": str,
         "Name": str,
         "Owner": HostedZoneOwnerTypeDef,
     },
 )
 
-_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
-    "_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
-    "_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
-    {
-        "LocationName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(
-    _RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-    _OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-):
-    pass
-
-ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef = TypedDict(
-    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
-    "_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
-    "_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(
-    _RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-    _OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-):
-    pass
-
-ListHealthChecksRequestListHealthChecksPaginateTypeDef = TypedDict(
-    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListHostedZonesRequestListHostedZonesPaginateTypeDef = TypedDict(
-    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
-    {
-        "DelegationSetId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = TypedDict(
-    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-    },
-)
-_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(
-    _RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-    _OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-):
-    pass
-
-_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
-    "_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-    },
-)
-_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
-    "_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
-    {
-        "MaxResults": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(
-    _RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
-    _OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
-):
-    pass
-
 ListCidrLocationsResponseTypeDef = TypedDict(
     "ListCidrLocationsResponseTypeDef",
     {
         "NextToken": str,
         "CidrLocations": List[LocationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficPoliciesResponseTypeDef = TypedDict(
     "ListTrafficPoliciesResponseTypeDef",
     {
         "TrafficPolicySummaries": List[TrafficPolicySummaryTypeDef],
         "IsTruncated": bool,
         "TrafficPolicyIdMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredResourceRecordSetTypeDef = TypedDict(
     "_RequiredResourceRecordSetTypeDef",
     {
         "Name": str,
@@ -2073,23 +2073,23 @@
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTagSet": ResourceTagSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourcesResponseTypeDef = TypedDict(
     "ListTagsForResourcesResponseTypeDef",
     {
         "ResourceTagSets": List[ResourceTagSetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "Id": str,
@@ -2110,89 +2110,89 @@
 class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
     pass
 
 GetHealthCheckLastFailureReasonResponseTypeDef = TypedDict(
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     {
         "HealthCheckObservations": List[HealthCheckObservationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetHealthCheckStatusResponseTypeDef = TypedDict(
     "GetHealthCheckStatusResponseTypeDef",
     {
         "HealthCheckObservations": List[HealthCheckObservationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHostedZoneResponseTypeDef = TypedDict(
     "CreateHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "ChangeInfo": ChangeInfoTypeDef,
         "DelegationSet": DelegationSetTypeDef,
         "VPC": VPCTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetHostedZoneResponseTypeDef = TypedDict(
     "GetHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "DelegationSet": DelegationSetTypeDef,
         "VPCs": List[VPCTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListHostedZonesByNameResponseTypeDef = TypedDict(
     "ListHostedZonesByNameResponseTypeDef",
     {
         "HostedZones": List[HostedZoneTypeDef],
         "DNSName": str,
         "HostedZoneId": str,
         "IsTruncated": bool,
         "NextDNSName": str,
         "NextHostedZoneId": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListHostedZonesResponseTypeDef = TypedDict(
     "ListHostedZonesResponseTypeDef",
     {
         "HostedZones": List[HostedZoneTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateHostedZoneCommentResponseTypeDef = TypedDict(
     "UpdateHostedZoneCommentResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListHostedZonesByVPCResponseTypeDef = TypedDict(
     "ListHostedZonesByVPCResponseTypeDef",
     {
         "HostedZoneSummaries": List[HostedZoneSummaryTypeDef],
         "MaxItems": str,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeTypeDef = TypedDict(
     "ChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -2205,52 +2205,52 @@
     {
         "ResourceRecordSets": List[ResourceRecordSetTypeDef],
         "IsTruncated": bool,
         "NextRecordName": str,
         "NextRecordType": RRTypeType,
         "NextRecordIdentifier": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHealthCheckResponseTypeDef = TypedDict(
     "CreateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
         "Location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetHealthCheckResponseTypeDef = TypedDict(
     "GetHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListHealthChecksResponseTypeDef = TypedDict(
     "ListHealthChecksResponseTypeDef",
     {
         "HealthChecks": List[HealthCheckTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateHealthCheckResponseTypeDef = TypedDict(
     "UpdateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredChangeBatchTypeDef = TypedDict(
     "_RequiredChangeBatchTypeDef",
     {
         "Changes": Sequence[ChangeTypeDef],
```

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/waiter.py` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53/waiter.pyi` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53.egg-info/PKG-INFO` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53
-Version: 1.26.56
-Summary: Type annotations for boto3.Route53 1.26.56 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Route53 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-route53"></a>
 
 # mypy-boto3-route53
 
 [![PyPI - mypy-boto3-route53](https://img.shields.io/pypi/v/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53?color=blue)](https://pypistats.org/packages/mypy-boto3-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53 1.26.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[boto3.Route53 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [mypy-boto3-route53 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/).
 
 See how it helps to find and fix potential bugs:
 
@@ -395,19 +395,19 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53.type_defs import (
     AccountLimitTypeDef,
     ActivateKeySigningKeyRequestRequestTypeDef,
     ChangeInfoTypeDef,
-    ResponseMetadataTypeDef,
     AlarmIdentifierTypeDef,
     AliasTargetTypeDef,
     VPCTypeDef,
     CidrCollectionChangeTypeDef,
+    ChangeCidrCollectionResponseTypeDef,
     TagTypeDef,
     CidrBlockSummaryTypeDef,
     CidrCollectionTypeDef,
     CidrRoutingConfigTypeDef,
     DimensionTypeDef,
     CollectionSummaryTypeDef,
     CreateCidrCollectionRequestRequestTypeDef,
@@ -436,75 +436,83 @@
     DisableHostedZoneDNSSECRequestRequestTypeDef,
     EnableHostedZoneDNSSECRequestRequestTypeDef,
     GeoLocationDetailsTypeDef,
     GeoLocationTypeDef,
     GetAccountLimitRequestRequestTypeDef,
     GetChangeRequestRequestTypeDef,
     WaiterConfigTypeDef,
+    GetCheckerIpRangesResponseTypeDef,
     GetDNSSECRequestRequestTypeDef,
     GetGeoLocationRequestRequestTypeDef,
+    GetHealthCheckCountResponseTypeDef,
     GetHealthCheckLastFailureReasonRequestRequestTypeDef,
     GetHealthCheckRequestRequestTypeDef,
     GetHealthCheckStatusRequestRequestTypeDef,
+    GetHostedZoneCountResponseTypeDef,
     GetHostedZoneLimitRequestRequestTypeDef,
     HostedZoneLimitTypeDef,
     GetHostedZoneRequestRequestTypeDef,
     GetQueryLoggingConfigRequestRequestTypeDef,
     GetReusableDelegationSetLimitRequestRequestTypeDef,
     ReusableDelegationSetLimitTypeDef,
     GetReusableDelegationSetRequestRequestTypeDef,
+    GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceRequestRequestTypeDef,
     GetTrafficPolicyRequestRequestTypeDef,
     StatusReportTypeDef,
     LinkedServiceTypeDef,
     HostedZoneOwnerTypeDef,
-    PaginatorConfigTypeDef,
+    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
     ListCidrBlocksRequestRequestTypeDef,
+    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
     ListCidrCollectionsRequestRequestTypeDef,
+    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
     ListCidrLocationsRequestRequestTypeDef,
     LocationSummaryTypeDef,
     ListGeoLocationsRequestRequestTypeDef,
+    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
     ListHealthChecksRequestRequestTypeDef,
     ListHostedZonesByNameRequestRequestTypeDef,
     ListHostedZonesByVPCRequestRequestTypeDef,
+    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
     ListHostedZonesRequestRequestTypeDef,
+    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
     ListQueryLoggingConfigsRequestRequestTypeDef,
+    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
     ListResourceRecordSetsRequestRequestTypeDef,
     ListReusableDelegationSetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
     ListTrafficPoliciesRequestRequestTypeDef,
     TrafficPolicySummaryTypeDef,
     ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef,
     ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef,
     ListTrafficPolicyInstancesRequestRequestTypeDef,
     ListTrafficPolicyVersionsRequestRequestTypeDef,
+    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListVPCAssociationAuthorizationsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ResourceRecordTypeDef,
+    ResponseMetadataTypeDef,
     TestDNSAnswerRequestRequestTypeDef,
+    TestDNSAnswerResponseTypeDef,
     UpdateHostedZoneCommentRequestRequestTypeDef,
     UpdateTrafficPolicyCommentRequestRequestTypeDef,
     UpdateTrafficPolicyInstanceRequestRequestTypeDef,
+    GetAccountLimitResponseTypeDef,
     ActivateKeySigningKeyResponseTypeDef,
     AssociateVPCWithHostedZoneResponseTypeDef,
-    ChangeCidrCollectionResponseTypeDef,
     ChangeResourceRecordSetsResponseTypeDef,
     DeactivateKeySigningKeyResponseTypeDef,
     DeleteHostedZoneResponseTypeDef,
     DeleteKeySigningKeyResponseTypeDef,
     DisableHostedZoneDNSSECResponseTypeDef,
     DisassociateVPCFromHostedZoneResponseTypeDef,
     EnableHostedZoneDNSSECResponseTypeDef,
-    GetAccountLimitResponseTypeDef,
     GetChangeResponseTypeDef,
-    GetCheckerIpRangesResponseTypeDef,
-    GetHealthCheckCountResponseTypeDef,
-    GetHostedZoneCountResponseTypeDef,
-    GetTrafficPolicyInstanceCountResponseTypeDef,
-    TestDNSAnswerResponseTypeDef,
     HealthCheckConfigTypeDef,
     UpdateHealthCheckRequestRequestTypeDef,
     AssociateVPCWithHostedZoneRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationResponseTypeDef,
     DeleteVPCAssociationAuthorizationRequestRequestTypeDef,
     DisassociateVPCFromHostedZoneRequestRequestTypeDef,
@@ -540,22 +548,14 @@
     ListGeoLocationsResponseTypeDef,
     GetChangeRequestResourceRecordSetsChangedWaitTypeDef,
     GetHostedZoneLimitResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     HealthCheckObservationTypeDef,
     HostedZoneTypeDef,
     HostedZoneSummaryTypeDef,
-    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
-    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
-    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
-    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
-    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListTrafficPoliciesResponseTypeDef,
     ResourceRecordSetTypeDef,
     CreateHealthCheckRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsForResourcesResponseTypeDef,
     HealthCheckTypeDef,
@@ -585,42 +585,42 @@
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

### Comparing `mypy-boto3-route53-1.26.56/mypy_boto3_route53.egg-info/SOURCES.txt` & `mypy-boto3-route53-1.27.0/mypy_boto3_route53.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.26.56/setup.py` & `mypy-boto3-route53-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Setup script for mypy-boto3-route53.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53",
-    version="1.26.56",
+    version="1.27.0",
     packages=["mypy_boto3_route53"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53 1.26.56 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Route53 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/",
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


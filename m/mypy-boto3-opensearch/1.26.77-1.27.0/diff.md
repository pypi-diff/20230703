# Comparing `tmp/mypy-boto3-opensearch-1.26.77.tar.gz` & `tmp/mypy-boto3-opensearch-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opensearch-1.26.77.tar", last modified: Wed Feb 22 20:34:22 2023, max compression
+gzip compressed data, was "mypy-boto3-opensearch-1.27.0.tar", last modified: Mon Jul  3 19:51:12 2023, max compression
```

## Comparing `mypy-boto3-opensearch-1.26.77.tar` & `mypy-boto3-opensearch-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.534112 mypy-boto3-opensearch-1.26.77/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20285 2023-02-22 20:34:22.534112 mypy-boto3-opensearch-1.26.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18779 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.530112 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39359 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39300 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-02-22 20:34:00.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64964 2023-02-22 20:34:01.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64907 2023-02-22 20:34:01.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.534112 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20285 2023-02-22 20:34:22.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-02-22 20:34:22.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-22 20:34:22.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 20:34:22.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 20:34:22.534112 mypy-boto3-opensearch-1.26.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:12.167753 mypy-boto3-opensearch-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:00.000000 mypy-boto3-opensearch-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20738 2023-07-03 19:51:12.167753 mypy-boto3-opensearch-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-07-03 19:43:00.000000 mypy-boto3-opensearch-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:12.163753 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-03 19:43:00.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 19:43:00.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:43:00.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41084 2023-07-03 19:43:00.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41023 2023-07-03 19:43:00.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-07-03 19:43:00.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-07-03 19:43:00.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:00.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68125 2023-07-03 19:43:02.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68068 2023-07-03 19:43:01.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:00.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:12.167753 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20738 2023-07-03 19:51:12.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 19:51:12.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:12.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:12.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:12.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:51:12.000000 mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:12.167753 mypy-boto3-opensearch-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-03 19:43:00.000000 mypy-boto3-opensearch-1.27.0/setup.py
```

### Comparing `mypy-boto3-opensearch-1.26.77/LICENSE` & `mypy-boto3-opensearch-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-opensearch-1.26.77/PKG-INFO` & `mypy-boto3-opensearch-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.26.77
-Summary: Type annotations for boto3.OpenSearchService 1.26.77 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.OpenSearchService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-opensearch"></a>
 
 # mypy-boto3-opensearch
 
 [![PyPI - mypy-boto3-opensearch](https://img.shields.io/pypi/v/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearch?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -285,40 +285,47 @@
     ActionTypeType,
     AutoTuneDesiredStateType,
     AutoTuneStateType,
     AutoTuneTypeType,
     ConnectionModeType,
     DeploymentStatusType,
     DescribePackagesFilterNameType,
+    DomainHealthType,
     DomainPackageStatusType,
+    DomainStateType,
     DryRunModeType,
     EngineTypeType,
     InboundConnectionStatusCodeType,
     LogTypeType,
+    MasterNodeStatusType,
+    NodeStatusType,
+    NodeTypeType,
     OpenSearchPartitionInstanceTypeType,
     OpenSearchWarmPartitionInstanceTypeType,
     OptionStateType,
     OutboundConnectionStatusCodeType,
     OverallChangeStatusType,
     PackageStatusType,
     PackageTypeType,
     PrincipalTypeType,
     ReservedInstancePaymentOptionType,
     RollbackOnDisableType,
     ScheduleAtType,
     ScheduledAutoTuneActionTypeType,
     ScheduledAutoTuneSeverityTypeType,
     ScheduledByType,
+    SkipUnavailableStatusType,
     TLSSecurityPolicyType,
     TimeUnitType,
     UpgradeStatusType,
     UpgradeStepType,
     VolumeTypeType,
     VpcEndpointErrorCodeType,
     VpcEndpointStatusType,
+    ZoneStatusType,
     OpenSearchServiceServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
@@ -333,35 +340,35 @@
 `mypy_boto3_opensearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearch.type_defs import (
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
     DurationTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
+    AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
     ColdStorageOptionsTypeDef,
     ZoneAwarenessConfigTypeDef,
     CognitoOptionsTypeDef,
     CompatibleVersionsMapTypeDef,
-    ConnectionPropertiesTypeDef,
+    CrossClusterSearchConnectionPropertiesTypeDef,
     DomainEndpointOptionsTypeDef,
     EBSOptionsTypeDef,
     EncryptionAtRestOptionsTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
     SnapshotOptionsTypeDef,
     SoftwareUpdateOptionsTypeDef,
@@ -373,14 +380,17 @@
     DeleteOutboundConnectionRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeleteVpcEndpointRequestRequestTypeDef,
     VpcEndpointSummaryTypeDef,
     DescribeDomainAutoTunesRequestRequestTypeDef,
     DescribeDomainChangeProgressRequestRequestTypeDef,
     DescribeDomainConfigRequestRequestTypeDef,
+    DescribeDomainHealthRequestRequestTypeDef,
+    DescribeDomainNodesRequestRequestTypeDef,
+    DomainNodesStatusTypeDef,
     DescribeDomainRequestRequestTypeDef,
     DescribeDomainsRequestRequestTypeDef,
     DescribeDryRunProgressRequestRequestTypeDef,
     DryRunResultsTypeDef,
     FilterTypeDef,
     DescribeInstanceTypeLimitsRequestRequestTypeDef,
     DescribePackagesFilterTypeDef,
@@ -389,80 +399,84 @@
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
     VPCDerivedInfoTypeDef,
     ValidationFailureTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCompatibleVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
+    GetUpgradeStatusResponseTypeDef,
     InboundConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     InstanceTypeDetailsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListScheduledActionsRequestRequestTypeDef,
     ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVersionsRequestRequestTypeDef,
+    ListVersionsResponseTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
     WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
+    PurchaseReservedInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
     DomainInformationContainerTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetUpgradeStatusResponseTypeDef,
-    ListVersionsResponseTypeDef,
-    PurchaseReservedInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     VersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
+    EnvironmentInfoTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsStatusTypeDef,
     GetCompatibleVersionsResponseTypeDef,
+    ConnectionPropertiesTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     EBSOptionsStatusTypeDef,
     EncryptionAtRestOptionsStatusTypeDef,
     LogPublishingOptionsStatusTypeDef,
     NodeToNodeEncryptionOptionsStatusTypeDef,
     SnapshotOptionsStatusTypeDef,
     SoftwareUpdateOptionsStatusTypeDef,
     CreateVpcEndpointRequestRequestTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     CreatePackageRequestRequestTypeDef,
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
+    DescribeDomainNodesResponseTypeDef,
     DescribeInboundConnectionsRequestRequestTypeDef,
     DescribeOutboundConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
     VPCDerivedInfoStatusTypeDef,
@@ -476,23 +490,24 @@
     OffPeakWindowTypeDef,
     ReservedInstanceOfferingTypeDef,
     ReservedInstanceTypeDef,
     SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
-    CreateOutboundConnectionRequestRequestTypeDef,
-    CreateOutboundConnectionResponseTypeDef,
     InboundConnectionTypeDef,
-    OutboundConnectionTypeDef,
     AutoTuneTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
+    DescribeDomainHealthResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     ClusterConfigStatusTypeDef,
+    CreateOutboundConnectionRequestRequestTypeDef,
+    CreateOutboundConnectionResponseTypeDef,
+    OutboundConnectionTypeDef,
     AssociatePackageResponseTypeDef,
     DissociatePackageResponseTypeDef,
     ListDomainsForPackageResponseTypeDef,
     ListPackagesForDomainResponseTypeDef,
     CreatePackageResponseTypeDef,
     DeletePackageResponseTypeDef,
     DescribePackagesResponseTypeDef,
@@ -507,18 +522,18 @@
     AdvancedSecurityOptionsTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
-    DeleteOutboundConnectionResponseTypeDef,
-    DescribeOutboundConnectionsResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    DeleteOutboundConnectionResponseTypeDef,
+    DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DomainConfigTypeDef,
@@ -539,42 +554,42 @@
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

### Comparing `mypy-boto3-opensearch-1.26.77/README.md` & `mypy-boto3-opensearch-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-opensearch"></a>
 
 # mypy-boto3-opensearch
 
 [![PyPI - mypy-boto3-opensearch](https://img.shields.io/pypi/v/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearch?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -253,40 +253,47 @@
     ActionTypeType,
     AutoTuneDesiredStateType,
     AutoTuneStateType,
     AutoTuneTypeType,
     ConnectionModeType,
     DeploymentStatusType,
     DescribePackagesFilterNameType,
+    DomainHealthType,
     DomainPackageStatusType,
+    DomainStateType,
     DryRunModeType,
     EngineTypeType,
     InboundConnectionStatusCodeType,
     LogTypeType,
+    MasterNodeStatusType,
+    NodeStatusType,
+    NodeTypeType,
     OpenSearchPartitionInstanceTypeType,
     OpenSearchWarmPartitionInstanceTypeType,
     OptionStateType,
     OutboundConnectionStatusCodeType,
     OverallChangeStatusType,
     PackageStatusType,
     PackageTypeType,
     PrincipalTypeType,
     ReservedInstancePaymentOptionType,
     RollbackOnDisableType,
     ScheduleAtType,
     ScheduledAutoTuneActionTypeType,
     ScheduledAutoTuneSeverityTypeType,
     ScheduledByType,
+    SkipUnavailableStatusType,
     TLSSecurityPolicyType,
     TimeUnitType,
     UpgradeStatusType,
     UpgradeStepType,
     VolumeTypeType,
     VpcEndpointErrorCodeType,
     VpcEndpointStatusType,
+    ZoneStatusType,
     OpenSearchServiceServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
@@ -301,35 +308,35 @@
 `mypy_boto3_opensearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearch.type_defs import (
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
     DurationTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
+    AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
     ColdStorageOptionsTypeDef,
     ZoneAwarenessConfigTypeDef,
     CognitoOptionsTypeDef,
     CompatibleVersionsMapTypeDef,
-    ConnectionPropertiesTypeDef,
+    CrossClusterSearchConnectionPropertiesTypeDef,
     DomainEndpointOptionsTypeDef,
     EBSOptionsTypeDef,
     EncryptionAtRestOptionsTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
     SnapshotOptionsTypeDef,
     SoftwareUpdateOptionsTypeDef,
@@ -341,14 +348,17 @@
     DeleteOutboundConnectionRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeleteVpcEndpointRequestRequestTypeDef,
     VpcEndpointSummaryTypeDef,
     DescribeDomainAutoTunesRequestRequestTypeDef,
     DescribeDomainChangeProgressRequestRequestTypeDef,
     DescribeDomainConfigRequestRequestTypeDef,
+    DescribeDomainHealthRequestRequestTypeDef,
+    DescribeDomainNodesRequestRequestTypeDef,
+    DomainNodesStatusTypeDef,
     DescribeDomainRequestRequestTypeDef,
     DescribeDomainsRequestRequestTypeDef,
     DescribeDryRunProgressRequestRequestTypeDef,
     DryRunResultsTypeDef,
     FilterTypeDef,
     DescribeInstanceTypeLimitsRequestRequestTypeDef,
     DescribePackagesFilterTypeDef,
@@ -357,80 +367,84 @@
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
     VPCDerivedInfoTypeDef,
     ValidationFailureTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCompatibleVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
+    GetUpgradeStatusResponseTypeDef,
     InboundConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     InstanceTypeDetailsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListScheduledActionsRequestRequestTypeDef,
     ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVersionsRequestRequestTypeDef,
+    ListVersionsResponseTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
     WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
+    PurchaseReservedInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
     DomainInformationContainerTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetUpgradeStatusResponseTypeDef,
-    ListVersionsResponseTypeDef,
-    PurchaseReservedInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     VersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
+    EnvironmentInfoTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsStatusTypeDef,
     GetCompatibleVersionsResponseTypeDef,
+    ConnectionPropertiesTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     EBSOptionsStatusTypeDef,
     EncryptionAtRestOptionsStatusTypeDef,
     LogPublishingOptionsStatusTypeDef,
     NodeToNodeEncryptionOptionsStatusTypeDef,
     SnapshotOptionsStatusTypeDef,
     SoftwareUpdateOptionsStatusTypeDef,
     CreateVpcEndpointRequestRequestTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     CreatePackageRequestRequestTypeDef,
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
+    DescribeDomainNodesResponseTypeDef,
     DescribeInboundConnectionsRequestRequestTypeDef,
     DescribeOutboundConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
     VPCDerivedInfoStatusTypeDef,
@@ -444,23 +458,24 @@
     OffPeakWindowTypeDef,
     ReservedInstanceOfferingTypeDef,
     ReservedInstanceTypeDef,
     SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
-    CreateOutboundConnectionRequestRequestTypeDef,
-    CreateOutboundConnectionResponseTypeDef,
     InboundConnectionTypeDef,
-    OutboundConnectionTypeDef,
     AutoTuneTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
+    DescribeDomainHealthResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     ClusterConfigStatusTypeDef,
+    CreateOutboundConnectionRequestRequestTypeDef,
+    CreateOutboundConnectionResponseTypeDef,
+    OutboundConnectionTypeDef,
     AssociatePackageResponseTypeDef,
     DissociatePackageResponseTypeDef,
     ListDomainsForPackageResponseTypeDef,
     ListPackagesForDomainResponseTypeDef,
     CreatePackageResponseTypeDef,
     DeletePackageResponseTypeDef,
     DescribePackagesResponseTypeDef,
@@ -475,18 +490,18 @@
     AdvancedSecurityOptionsTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
-    DeleteOutboundConnectionResponseTypeDef,
-    DescribeOutboundConnectionsResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    DeleteOutboundConnectionResponseTypeDef,
+    DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DomainConfigTypeDef,
@@ -507,42 +522,42 @@
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

### Comparing `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/__main__.py` & `mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchService 1.26.77\nVersion:         1.26.77\nBuilder"
-        " version: 7.12.4\nDocs:           "
+        "Type annotations for boto3.OpenSearchService 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.77")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/client.py` & `mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,26 +33,29 @@
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsTypeDef,
+    ConnectionPropertiesTypeDef,
     CreateDomainResponseTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     CreatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DeletePackageResponseTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
+    DescribeDomainHealthResponseTypeDef,
+    DescribeDomainNodesResponseTypeDef,
     DescribeDomainResponseTypeDef,
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     DescribePackagesFilterTypeDef,
@@ -117,14 +120,15 @@
 
 
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BaseException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
+    DependencyFailureException: Type[BotocoreClientError]
     DisabledOperationException: Type[BotocoreClientError]
     InternalException: Type[BotocoreClientError]
     InvalidPaginationTokenException: Type[BotocoreClientError]
     InvalidTypeException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
@@ -247,15 +251,16 @@
 
     def create_outbound_connection(
         self,
         *,
         LocalDomainInfo: DomainInformationContainerTypeDef,
         RemoteDomainInfo: DomainInformationContainerTypeDef,
         ConnectionAlias: str,
-        ConnectionMode: ConnectionModeType = ...
+        ConnectionMode: ConnectionModeType = ...,
+        ConnectionProperties: ConnectionPropertiesTypeDef = ...
     ) -> CreateOutboundConnectionResponseTypeDef:
         """
         Creates a new cross-cluster search connection from a source Amazon OpenSearch
         Service domain to a destination domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_outbound_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#create_outbound_connection)
@@ -367,14 +372,33 @@
         """
         Returns the configuration of an Amazon OpenSearch Service domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domain_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#describe_domain_config)
         """
 
+    def describe_domain_health(self, *, DomainName: str) -> DescribeDomainHealthResponseTypeDef:
+        """
+        Returns information about domain and node health, the standby Availability Zone,
+        number of nodes per Availability Zone, and shard count per node.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domain_health)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#describe_domain_health)
+        """
+
+    def describe_domain_nodes(self, *, DomainName: str) -> DescribeDomainNodesResponseTypeDef:
+        """
+        Returns information about domain and nodes, including data nodes, master nodes,
+        ultrawarm nodes, Availability Zone(s), standby nodes, node configurations, and
+        node states.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domain_nodes)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#describe_domain_nodes)
+        """
+
     def describe_domains(self, *, DomainNames: Sequence[str]) -> DescribeDomainsResponseTypeDef:
         """
         Returns domain configuration information about the specified Amazon OpenSearch
         Service domains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#describe_domains)
@@ -510,15 +534,16 @@
         """
 
     def get_package_version_history(
         self, *, PackageID: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetPackageVersionHistoryResponseTypeDef:
         """
         Returns a list of Amazon OpenSearch Service package versions, along with their
-        creation time and commit message.
+        creation time, commit message, and plugin properties (if the package is a zip
+        plugin package).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.get_package_version_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#get_package_version_history)
         """
 
     def get_upgrade_history(
         self, *, DomainName: str, MaxResults: int = ..., NextToken: str = ...
@@ -563,15 +588,17 @@
 
     def list_instance_type_details(
         self,
         *,
         EngineVersion: str,
         DomainName: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
+        RetrieveAZs: bool = ...,
+        InstanceType: str = ...
     ) -> ListInstanceTypeDetailsResponseTypeDef:
         """
         Lists all instance types and available features for a given OpenSearch or
         Elasticsearch version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_instance_type_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#list_instance_type_details)
@@ -716,15 +743,16 @@
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
         SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
-        domain.
+        domain.sl See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/opensearch-2021-01-01/UpdateDomainConfig).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_domain_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#update_domain_config)
         """
 
     def update_package(
         self,
```

### Comparing `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/client.pyi` & `mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,26 +33,29 @@
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsTypeDef,
+    ConnectionPropertiesTypeDef,
     CreateDomainResponseTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     CreatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DeletePackageResponseTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
+    DescribeDomainHealthResponseTypeDef,
+    DescribeDomainNodesResponseTypeDef,
     DescribeDomainResponseTypeDef,
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     DescribePackagesFilterTypeDef,
@@ -114,14 +117,15 @@
         self.operation_name: str
 
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BaseException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
+    DependencyFailureException: Type[BotocoreClientError]
     DisabledOperationException: Type[BotocoreClientError]
     InternalException: Type[BotocoreClientError]
     InvalidPaginationTokenException: Type[BotocoreClientError]
     InvalidTypeException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
@@ -234,15 +238,16 @@
         """
     def create_outbound_connection(
         self,
         *,
         LocalDomainInfo: DomainInformationContainerTypeDef,
         RemoteDomainInfo: DomainInformationContainerTypeDef,
         ConnectionAlias: str,
-        ConnectionMode: ConnectionModeType = ...
+        ConnectionMode: ConnectionModeType = ...,
+        ConnectionProperties: ConnectionPropertiesTypeDef = ...
     ) -> CreateOutboundConnectionResponseTypeDef:
         """
         Creates a new cross-cluster search connection from a source Amazon OpenSearch
         Service domain to a destination domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_outbound_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#create_outbound_connection)
@@ -342,14 +347,31 @@
     def describe_domain_config(self, *, DomainName: str) -> DescribeDomainConfigResponseTypeDef:
         """
         Returns the configuration of an Amazon OpenSearch Service domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domain_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#describe_domain_config)
         """
+    def describe_domain_health(self, *, DomainName: str) -> DescribeDomainHealthResponseTypeDef:
+        """
+        Returns information about domain and node health, the standby Availability Zone,
+        number of nodes per Availability Zone, and shard count per node.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domain_health)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#describe_domain_health)
+        """
+    def describe_domain_nodes(self, *, DomainName: str) -> DescribeDomainNodesResponseTypeDef:
+        """
+        Returns information about domain and nodes, including data nodes, master nodes,
+        ultrawarm nodes, Availability Zone(s), standby nodes, node configurations, and
+        node states.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domain_nodes)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#describe_domain_nodes)
+        """
     def describe_domains(self, *, DomainNames: Sequence[str]) -> DescribeDomainsResponseTypeDef:
         """
         Returns domain configuration information about the specified Amazon OpenSearch
         Service domains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#describe_domains)
@@ -473,15 +495,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#get_compatible_versions)
         """
     def get_package_version_history(
         self, *, PackageID: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetPackageVersionHistoryResponseTypeDef:
         """
         Returns a list of Amazon OpenSearch Service package versions, along with their
-        creation time and commit message.
+        creation time, commit message, and plugin properties (if the package is a zip
+        plugin package).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.get_package_version_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#get_package_version_history)
         """
     def get_upgrade_history(
         self, *, DomainName: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetUpgradeHistoryResponseTypeDef:
@@ -521,15 +544,17 @@
         """
     def list_instance_type_details(
         self,
         *,
         EngineVersion: str,
         DomainName: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
+        RetrieveAZs: bool = ...,
+        InstanceType: str = ...
     ) -> ListInstanceTypeDetailsResponseTypeDef:
         """
         Lists all instance types and available features for a given OpenSearch or
         Elasticsearch version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_instance_type_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#list_instance_type_details)
@@ -661,15 +686,16 @@
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
         SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
-        domain.
+        domain.sl See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/opensearch-2021-01-01/UpdateDomainConfig).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_domain_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#update_domain_config)
         """
     def update_package(
         self,
         *,
```

### Comparing `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/literals.py` & `mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,58 +14,63 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActionSeverityType",
     "ActionStatusType",
     "ActionTypeType",
     "AutoTuneDesiredStateType",
     "AutoTuneStateType",
     "AutoTuneTypeType",
     "ConnectionModeType",
     "DeploymentStatusType",
     "DescribePackagesFilterNameType",
+    "DomainHealthType",
     "DomainPackageStatusType",
+    "DomainStateType",
     "DryRunModeType",
     "EngineTypeType",
     "InboundConnectionStatusCodeType",
     "LogTypeType",
+    "MasterNodeStatusType",
+    "NodeStatusType",
+    "NodeTypeType",
     "OpenSearchPartitionInstanceTypeType",
     "OpenSearchWarmPartitionInstanceTypeType",
     "OptionStateType",
     "OutboundConnectionStatusCodeType",
     "OverallChangeStatusType",
     "PackageStatusType",
     "PackageTypeType",
     "PrincipalTypeType",
     "ReservedInstancePaymentOptionType",
     "RollbackOnDisableType",
     "ScheduleAtType",
     "ScheduledAutoTuneActionTypeType",
     "ScheduledAutoTuneSeverityTypeType",
     "ScheduledByType",
+    "SkipUnavailableStatusType",
     "TLSSecurityPolicyType",
     "TimeUnitType",
     "UpgradeStatusType",
     "UpgradeStepType",
     "VolumeTypeType",
     "VpcEndpointErrorCodeType",
     "VpcEndpointStatusType",
+    "ZoneStatusType",
     "OpenSearchServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ActionSeverityType = Literal["HIGH", "LOW", "MEDIUM"]
 ActionStatusType = Literal[
     "COMPLETED", "ELIGIBLE", "FAILED", "IN_PROGRESS", "NOT_ELIGIBLE", "PENDING_UPDATE"
 ]
 ActionTypeType = Literal["JVM_HEAP_SIZE_TUNING", "JVM_YOUNG_GEN_TUNING", "SERVICE_SOFTWARE_UPDATE"]
 AutoTuneDesiredStateType = Literal["DISABLED", "ENABLED"]
 AutoTuneStateType = Literal[
@@ -81,30 +86,35 @@
 ]
 AutoTuneTypeType = Literal["SCHEDULED_ACTION"]
 ConnectionModeType = Literal["DIRECT", "VPC_ENDPOINT"]
 DeploymentStatusType = Literal[
     "COMPLETED", "ELIGIBLE", "IN_PROGRESS", "NOT_ELIGIBLE", "PENDING_UPDATE"
 ]
 DescribePackagesFilterNameType = Literal["PackageID", "PackageName", "PackageStatus"]
+DomainHealthType = Literal["Green", "NotAvailable", "Red", "Yellow"]
 DomainPackageStatusType = Literal[
     "ACTIVE", "ASSOCIATING", "ASSOCIATION_FAILED", "DISSOCIATING", "DISSOCIATION_FAILED"
 ]
+DomainStateType = Literal["Active", "NotAvailable", "Processing"]
 DryRunModeType = Literal["Basic", "Verbose"]
 EngineTypeType = Literal["Elasticsearch", "OpenSearch"]
 InboundConnectionStatusCodeType = Literal[
     "ACTIVE",
     "APPROVED",
     "DELETED",
     "DELETING",
     "PENDING_ACCEPTANCE",
     "PROVISIONING",
     "REJECTED",
     "REJECTING",
 ]
 LogTypeType = Literal["AUDIT_LOGS", "ES_APPLICATION_LOGS", "INDEX_SLOW_LOGS", "SEARCH_SLOW_LOGS"]
+MasterNodeStatusType = Literal["Available", "UnAvailable"]
+NodeStatusType = Literal["Active", "NotAvailable", "StandBy"]
+NodeTypeType = Literal["Data", "Master", "Ultrawarm"]
 OpenSearchPartitionInstanceTypeType = Literal[
     "c4.2xlarge.search",
     "c4.4xlarge.search",
     "c4.8xlarge.search",
     "c4.large.search",
     "c4.xlarge.search",
     "c5.18xlarge.search",
@@ -229,23 +239,25 @@
 PrincipalTypeType = Literal["AWS_ACCOUNT", "AWS_SERVICE"]
 ReservedInstancePaymentOptionType = Literal["ALL_UPFRONT", "NO_UPFRONT", "PARTIAL_UPFRONT"]
 RollbackOnDisableType = Literal["DEFAULT_ROLLBACK", "NO_ROLLBACK"]
 ScheduleAtType = Literal["NOW", "OFF_PEAK_WINDOW", "TIMESTAMP"]
 ScheduledAutoTuneActionTypeType = Literal["JVM_HEAP_SIZE_TUNING", "JVM_YOUNG_GEN_TUNING"]
 ScheduledAutoTuneSeverityTypeType = Literal["HIGH", "LOW", "MEDIUM"]
 ScheduledByType = Literal["CUSTOMER", "SYSTEM"]
+SkipUnavailableStatusType = Literal["DISABLED", "ENABLED"]
 TLSSecurityPolicyType = Literal["Policy-Min-TLS-1-0-2019-07", "Policy-Min-TLS-1-2-2019-07"]
 TimeUnitType = Literal["HOURS"]
 UpgradeStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED", "SUCCEEDED_WITH_ISSUES"]
 UpgradeStepType = Literal["PRE_UPGRADE_CHECK", "SNAPSHOT", "UPGRADE"]
 VolumeTypeType = Literal["gp2", "gp3", "io1", "standard"]
 VpcEndpointErrorCodeType = Literal["ENDPOINT_NOT_FOUND", "SERVER_ERROR"]
 VpcEndpointStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING", "UPDATE_FAILED", "UPDATING"
 ]
+ZoneStatusType = Literal["Active", "NotAvailable", "StandBy"]
 OpenSearchServiceServiceName = Literal["opensearch"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -254,14 +266,15 @@
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
@@ -301,14 +314,15 @@
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
@@ -387,14 +401,15 @@
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
@@ -405,14 +420,15 @@
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
@@ -448,14 +464,15 @@
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
@@ -474,16 +491,19 @@
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
@@ -567,15 +587,17 @@
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

### Comparing `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/literals.pyi` & `mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,56 +14,65 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActionSeverityType",
     "ActionStatusType",
     "ActionTypeType",
     "AutoTuneDesiredStateType",
     "AutoTuneStateType",
     "AutoTuneTypeType",
     "ConnectionModeType",
     "DeploymentStatusType",
     "DescribePackagesFilterNameType",
+    "DomainHealthType",
     "DomainPackageStatusType",
+    "DomainStateType",
     "DryRunModeType",
     "EngineTypeType",
     "InboundConnectionStatusCodeType",
     "LogTypeType",
+    "MasterNodeStatusType",
+    "NodeStatusType",
+    "NodeTypeType",
     "OpenSearchPartitionInstanceTypeType",
     "OpenSearchWarmPartitionInstanceTypeType",
     "OptionStateType",
     "OutboundConnectionStatusCodeType",
     "OverallChangeStatusType",
     "PackageStatusType",
     "PackageTypeType",
     "PrincipalTypeType",
     "ReservedInstancePaymentOptionType",
     "RollbackOnDisableType",
     "ScheduleAtType",
     "ScheduledAutoTuneActionTypeType",
     "ScheduledAutoTuneSeverityTypeType",
     "ScheduledByType",
+    "SkipUnavailableStatusType",
     "TLSSecurityPolicyType",
     "TimeUnitType",
     "UpgradeStatusType",
     "UpgradeStepType",
     "VolumeTypeType",
     "VpcEndpointErrorCodeType",
     "VpcEndpointStatusType",
+    "ZoneStatusType",
     "OpenSearchServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 ActionSeverityType = Literal["HIGH", "LOW", "MEDIUM"]
 ActionStatusType = Literal[
     "COMPLETED", "ELIGIBLE", "FAILED", "IN_PROGRESS", "NOT_ELIGIBLE", "PENDING_UPDATE"
 ]
 ActionTypeType = Literal["JVM_HEAP_SIZE_TUNING", "JVM_YOUNG_GEN_TUNING", "SERVICE_SOFTWARE_UPDATE"]
 AutoTuneDesiredStateType = Literal["DISABLED", "ENABLED"]
 AutoTuneStateType = Literal[
@@ -79,30 +88,35 @@
 ]
 AutoTuneTypeType = Literal["SCHEDULED_ACTION"]
 ConnectionModeType = Literal["DIRECT", "VPC_ENDPOINT"]
 DeploymentStatusType = Literal[
     "COMPLETED", "ELIGIBLE", "IN_PROGRESS", "NOT_ELIGIBLE", "PENDING_UPDATE"
 ]
 DescribePackagesFilterNameType = Literal["PackageID", "PackageName", "PackageStatus"]
+DomainHealthType = Literal["Green", "NotAvailable", "Red", "Yellow"]
 DomainPackageStatusType = Literal[
     "ACTIVE", "ASSOCIATING", "ASSOCIATION_FAILED", "DISSOCIATING", "DISSOCIATION_FAILED"
 ]
+DomainStateType = Literal["Active", "NotAvailable", "Processing"]
 DryRunModeType = Literal["Basic", "Verbose"]
 EngineTypeType = Literal["Elasticsearch", "OpenSearch"]
 InboundConnectionStatusCodeType = Literal[
     "ACTIVE",
     "APPROVED",
     "DELETED",
     "DELETING",
     "PENDING_ACCEPTANCE",
     "PROVISIONING",
     "REJECTED",
     "REJECTING",
 ]
 LogTypeType = Literal["AUDIT_LOGS", "ES_APPLICATION_LOGS", "INDEX_SLOW_LOGS", "SEARCH_SLOW_LOGS"]
+MasterNodeStatusType = Literal["Available", "UnAvailable"]
+NodeStatusType = Literal["Active", "NotAvailable", "StandBy"]
+NodeTypeType = Literal["Data", "Master", "Ultrawarm"]
 OpenSearchPartitionInstanceTypeType = Literal[
     "c4.2xlarge.search",
     "c4.4xlarge.search",
     "c4.8xlarge.search",
     "c4.large.search",
     "c4.xlarge.search",
     "c5.18xlarge.search",
@@ -227,23 +241,25 @@
 PrincipalTypeType = Literal["AWS_ACCOUNT", "AWS_SERVICE"]
 ReservedInstancePaymentOptionType = Literal["ALL_UPFRONT", "NO_UPFRONT", "PARTIAL_UPFRONT"]
 RollbackOnDisableType = Literal["DEFAULT_ROLLBACK", "NO_ROLLBACK"]
 ScheduleAtType = Literal["NOW", "OFF_PEAK_WINDOW", "TIMESTAMP"]
 ScheduledAutoTuneActionTypeType = Literal["JVM_HEAP_SIZE_TUNING", "JVM_YOUNG_GEN_TUNING"]
 ScheduledAutoTuneSeverityTypeType = Literal["HIGH", "LOW", "MEDIUM"]
 ScheduledByType = Literal["CUSTOMER", "SYSTEM"]
+SkipUnavailableStatusType = Literal["DISABLED", "ENABLED"]
 TLSSecurityPolicyType = Literal["Policy-Min-TLS-1-0-2019-07", "Policy-Min-TLS-1-2-2019-07"]
 TimeUnitType = Literal["HOURS"]
 UpgradeStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED", "SUCCEEDED_WITH_ISSUES"]
 UpgradeStepType = Literal["PRE_UPGRADE_CHECK", "SNAPSHOT", "UPGRADE"]
 VolumeTypeType = Literal["gp2", "gp3", "io1", "standard"]
 VpcEndpointErrorCodeType = Literal["ENDPOINT_NOT_FOUND", "SERVER_ERROR"]
 VpcEndpointStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING", "UPDATE_FAILED", "UPDATING"
 ]
+ZoneStatusType = Literal["Active", "NotAvailable", "StandBy"]
 OpenSearchServiceServiceName = Literal["opensearch"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -252,14 +268,15 @@
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
@@ -299,14 +316,15 @@
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
@@ -385,14 +403,15 @@
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
@@ -403,14 +422,15 @@
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
@@ -446,14 +466,15 @@
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
@@ -472,16 +493,19 @@
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
@@ -565,15 +589,17 @@
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

### Comparing `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/type_defs.py` & `mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,38 +20,45 @@
     ActionStatusType,
     ActionTypeType,
     AutoTuneDesiredStateType,
     AutoTuneStateType,
     ConnectionModeType,
     DeploymentStatusType,
     DescribePackagesFilterNameType,
+    DomainHealthType,
     DomainPackageStatusType,
+    DomainStateType,
     DryRunModeType,
     EngineTypeType,
     InboundConnectionStatusCodeType,
     LogTypeType,
+    MasterNodeStatusType,
+    NodeStatusType,
+    NodeTypeType,
     OpenSearchPartitionInstanceTypeType,
     OpenSearchWarmPartitionInstanceTypeType,
     OptionStateType,
     OutboundConnectionStatusCodeType,
     OverallChangeStatusType,
     PackageStatusType,
     PrincipalTypeType,
     ReservedInstancePaymentOptionType,
     RollbackOnDisableType,
     ScheduleAtType,
     ScheduledAutoTuneActionTypeType,
     ScheduledAutoTuneSeverityTypeType,
     ScheduledByType,
+    SkipUnavailableStatusType,
     TLSSecurityPolicyType,
     UpgradeStatusType,
     UpgradeStepType,
     VolumeTypeType,
     VpcEndpointErrorCodeType,
     VpcEndpointStatusType,
+    ZoneStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -59,35 +66,35 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AWSDomainInformationTypeDef",
     "AcceptInboundConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "OptionStatusTypeDef",
     "TagTypeDef",
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
     "AssociatePackageRequestRequestTypeDef",
     "AuthorizeVpcEndpointAccessRequestRequestTypeDef",
     "AuthorizedPrincipalTypeDef",
     "ScheduledAutoTuneDetailsTypeDef",
     "DurationTypeDef",
     "AutoTuneOptionsOutputTypeDef",
     "AutoTuneStatusTypeDef",
+    "AvailabilityZoneInfoTypeDef",
     "CancelServiceSoftwareUpdateRequestRequestTypeDef",
     "ServiceSoftwareOptionsTypeDef",
     "ChangeProgressDetailsTypeDef",
     "ChangeProgressStageTypeDef",
     "ColdStorageOptionsTypeDef",
     "ZoneAwarenessConfigTypeDef",
     "CognitoOptionsTypeDef",
     "CompatibleVersionsMapTypeDef",
-    "ConnectionPropertiesTypeDef",
+    "CrossClusterSearchConnectionPropertiesTypeDef",
     "DomainEndpointOptionsTypeDef",
     "EBSOptionsTypeDef",
     "EncryptionAtRestOptionsTypeDef",
     "LogPublishingOptionTypeDef",
     "NodeToNodeEncryptionOptionsTypeDef",
     "SnapshotOptionsTypeDef",
     "SoftwareUpdateOptionsTypeDef",
@@ -99,14 +106,17 @@
     "DeleteOutboundConnectionRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeleteVpcEndpointRequestRequestTypeDef",
     "VpcEndpointSummaryTypeDef",
     "DescribeDomainAutoTunesRequestRequestTypeDef",
     "DescribeDomainChangeProgressRequestRequestTypeDef",
     "DescribeDomainConfigRequestRequestTypeDef",
+    "DescribeDomainHealthRequestRequestTypeDef",
+    "DescribeDomainNodesRequestRequestTypeDef",
+    "DomainNodesStatusTypeDef",
     "DescribeDomainRequestRequestTypeDef",
     "DescribeDomainsRequestRequestTypeDef",
     "DescribeDryRunProgressRequestRequestTypeDef",
     "DryRunResultsTypeDef",
     "FilterTypeDef",
     "DescribeInstanceTypeLimitsRequestRequestTypeDef",
     "DescribePackagesFilterTypeDef",
@@ -115,80 +125,84 @@
     "DescribeVpcEndpointsRequestRequestTypeDef",
     "VpcEndpointErrorTypeDef",
     "DissociatePackageRequestRequestTypeDef",
     "DomainInfoTypeDef",
     "ErrorDetailsTypeDef",
     "VPCDerivedInfoTypeDef",
     "ValidationFailureTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetCompatibleVersionsRequestRequestTypeDef",
     "GetPackageVersionHistoryRequestRequestTypeDef",
     "PackageVersionHistoryTypeDef",
     "GetUpgradeHistoryRequestRequestTypeDef",
     "GetUpgradeStatusRequestRequestTypeDef",
+    "GetUpgradeStatusResponseTypeDef",
     "InboundConnectionStatusTypeDef",
     "InstanceCountLimitsTypeDef",
     "InstanceTypeDetailsTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
     "ListInstanceTypeDetailsRequestRequestTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
     "ListScheduledActionsRequestRequestTypeDef",
     "ScheduledActionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListVersionsRequestRequestTypeDef",
+    "ListVersionsResponseTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
     "WindowStartTimeTypeDef",
     "PurchaseReservedInstanceOfferingRequestRequestTypeDef",
+    "PurchaseReservedInstanceOfferingResponseTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     "SAMLIdpTypeDef",
     "StartServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
     "UpdateScheduledActionRequestRequestTypeDef",
     "UpgradeDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
     "DomainInformationContainerTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetUpgradeStatusResponseTypeDef",
-    "ListVersionsResponseTypeDef",
-    "PurchaseReservedInstanceOfferingResponseTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AdvancedOptionsStatusTypeDef",
     "VersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
+    "EnvironmentInfoTypeDef",
     "CancelServiceSoftwareUpdateResponseTypeDef",
     "StartServiceSoftwareUpdateResponseTypeDef",
     "UpgradeDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
     "ClusterConfigTypeDef",
     "CognitoOptionsStatusTypeDef",
     "GetCompatibleVersionsResponseTypeDef",
+    "ConnectionPropertiesTypeDef",
     "DomainEndpointOptionsStatusTypeDef",
     "EBSOptionsStatusTypeDef",
     "EncryptionAtRestOptionsStatusTypeDef",
     "LogPublishingOptionsStatusTypeDef",
     "NodeToNodeEncryptionOptionsStatusTypeDef",
     "SnapshotOptionsStatusTypeDef",
     "SoftwareUpdateOptionsStatusTypeDef",
     "CreateVpcEndpointRequestRequestTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "ListVpcEndpointsForDomainResponseTypeDef",
     "ListVpcEndpointsResponseTypeDef",
+    "DescribeDomainNodesResponseTypeDef",
     "DescribeInboundConnectionsRequestRequestTypeDef",
     "DescribeOutboundConnectionsRequestRequestTypeDef",
     "DescribePackagesRequestRequestTypeDef",
     "ListDomainNamesResponseTypeDef",
     "DomainPackageDetailsTypeDef",
     "PackageDetailsTypeDef",
     "VPCDerivedInfoStatusTypeDef",
@@ -202,23 +216,24 @@
     "OffPeakWindowTypeDef",
     "ReservedInstanceOfferingTypeDef",
     "ReservedInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
-    "CreateOutboundConnectionRequestRequestTypeDef",
-    "CreateOutboundConnectionResponseTypeDef",
     "InboundConnectionTypeDef",
-    "OutboundConnectionTypeDef",
     "AutoTuneTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
+    "DescribeDomainHealthResponseTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "ClusterConfigStatusTypeDef",
+    "CreateOutboundConnectionRequestRequestTypeDef",
+    "CreateOutboundConnectionResponseTypeDef",
+    "OutboundConnectionTypeDef",
     "AssociatePackageResponseTypeDef",
     "DissociatePackageResponseTypeDef",
     "ListDomainsForPackageResponseTypeDef",
     "ListPackagesForDomainResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DeletePackageResponseTypeDef",
     "DescribePackagesResponseTypeDef",
@@ -233,18 +248,18 @@
     "AdvancedSecurityOptionsTypeDef",
     "LimitsTypeDef",
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
-    "DeleteOutboundConnectionResponseTypeDef",
-    "DescribeOutboundConnectionsResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
+    "DeleteOutboundConnectionResponseTypeDef",
+    "DescribeOutboundConnectionsResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "DomainStatusTypeDef",
     "DescribeInstanceTypeLimitsResponseTypeDef",
     "DomainConfigTypeDef",
@@ -282,25 +297,14 @@
 AcceptInboundConnectionRequestRequestTypeDef = TypedDict(
     "AcceptInboundConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
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
 _RequiredOptionStatusTypeDef = TypedDict(
     "_RequiredOptionStatusTypeDef",
     {
         "CreationDate": datetime,
         "UpdateDate": datetime,
         "State": OptionStateType,
     },
@@ -420,14 +424,27 @@
 )
 
 
 class AutoTuneStatusTypeDef(_RequiredAutoTuneStatusTypeDef, _OptionalAutoTuneStatusTypeDef):
     pass
 
 
+AvailabilityZoneInfoTypeDef = TypedDict(
+    "AvailabilityZoneInfoTypeDef",
+    {
+        "AvailabilityZoneName": str,
+        "ZoneStatus": ZoneStatusType,
+        "ConfiguredDataNodeCount": str,
+        "AvailableDataNodeCount": str,
+        "TotalShards": str,
+        "TotalUnAssignedShards": str,
+    },
+    total=False,
+)
+
 CancelServiceSoftwareUpdateRequestRequestTypeDef = TypedDict(
     "CancelServiceSoftwareUpdateRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -497,18 +514,18 @@
     {
         "SourceVersion": str,
         "TargetVersions": List[str],
     },
     total=False,
 )
 
-ConnectionPropertiesTypeDef = TypedDict(
-    "ConnectionPropertiesTypeDef",
+CrossClusterSearchConnectionPropertiesTypeDef = TypedDict(
+    "CrossClusterSearchConnectionPropertiesTypeDef",
     {
-        "Endpoint": str,
+        "SkipUnavailable": SkipUnavailableStatusType,
     },
     total=False,
 )
 
 DomainEndpointOptionsTypeDef = TypedDict(
     "DomainEndpointOptionsTypeDef",
     {
@@ -696,14 +713,43 @@
 DescribeDomainConfigRequestRequestTypeDef = TypedDict(
     "DescribeDomainConfigRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+DescribeDomainHealthRequestRequestTypeDef = TypedDict(
+    "DescribeDomainHealthRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+
+DescribeDomainNodesRequestRequestTypeDef = TypedDict(
+    "DescribeDomainNodesRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+
+DomainNodesStatusTypeDef = TypedDict(
+    "DomainNodesStatusTypeDef",
+    {
+        "NodeId": str,
+        "NodeType": NodeTypeType,
+        "AvailabilityZone": str,
+        "InstanceType": OpenSearchPartitionInstanceTypeType,
+        "NodeStatus": NodeStatusType,
+        "StorageType": str,
+        "StorageVolumeType": VolumeTypeType,
+        "StorageSize": str,
+    },
+    total=False,
+)
+
 DescribeDomainRequestRequestTypeDef = TypedDict(
     "DescribeDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -866,14 +912,21 @@
     {
         "Code": str,
         "Message": str,
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
 GetCompatibleVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleVersionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
     total=False,
 )
@@ -936,14 +989,24 @@
 GetUpgradeStatusRequestRequestTypeDef = TypedDict(
     "GetUpgradeStatusRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+GetUpgradeStatusResponseTypeDef = TypedDict(
+    "GetUpgradeStatusResponseTypeDef",
+    {
+        "UpgradeStep": UpgradeStepType,
+        "StepStatus": UpgradeStatusType,
+        "UpgradeName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InboundConnectionStatusTypeDef = TypedDict(
     "InboundConnectionStatusTypeDef",
     {
         "StatusCode": InboundConnectionStatusCodeType,
         "Message": str,
     },
     total=False,
@@ -964,14 +1027,15 @@
         "InstanceType": OpenSearchPartitionInstanceTypeType,
         "EncryptionEnabled": bool,
         "CognitoEnabled": bool,
         "AppLogsEnabled": bool,
         "AdvancedSecurityEnabled": bool,
         "WarmEnabled": bool,
         "InstanceRole": List[str],
+        "AvailabilityZones": List[str],
     },
     total=False,
 )
 
 ListDomainNamesRequestRequestTypeDef = TypedDict(
     "ListDomainNamesRequestRequestTypeDef",
     {
@@ -1011,14 +1075,16 @@
 )
 _OptionalListInstanceTypeDetailsRequestRequestTypeDef = TypedDict(
     "_OptionalListInstanceTypeDetailsRequestRequestTypeDef",
     {
         "DomainName": str,
         "MaxResults": int,
         "NextToken": str,
+        "RetrieveAZs": bool,
+        "InstanceType": str,
     },
     total=False,
 )
 
 
 class ListInstanceTypeDetailsRequestRequestTypeDef(
     _RequiredListInstanceTypeDetailsRequestRequestTypeDef,
@@ -1111,14 +1177,23 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListVersionsResponseTypeDef = TypedDict(
+    "ListVersionsResponseTypeDef",
+    {
+        "Versions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "_RequiredListVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListVpcEndpointAccessRequestRequestTypeDef = TypedDict(
@@ -1194,14 +1269,23 @@
 class PurchaseReservedInstanceOfferingRequestRequestTypeDef(
     _RequiredPurchaseReservedInstanceOfferingRequestRequestTypeDef,
     _OptionalPurchaseReservedInstanceOfferingRequestRequestTypeDef,
 ):
     pass
 
 
+PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
+    "PurchaseReservedInstanceOfferingResponseTypeDef",
+    {
+        "ReservedInstanceId": str,
+        "ReservationName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "RecurringChargeAmount": float,
         "RecurringChargeFrequency": str,
     },
     total=False,
@@ -1218,14 +1302,25 @@
     "RemoveTagsRequestRequestTypeDef",
     {
         "ARN": str,
         "TagKeys": Sequence[str],
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
 RevokeVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
         "Account": str,
     },
 )
@@ -1333,49 +1428,14 @@
     "DomainInformationContainerTypeDef",
     {
         "AWSDomainInformation": AWSDomainInformationTypeDef,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUpgradeStatusResponseTypeDef = TypedDict(
-    "GetUpgradeStatusResponseTypeDef",
-    {
-        "UpgradeStep": UpgradeStepType,
-        "StepStatus": UpgradeStatusType,
-        "UpgradeName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListVersionsResponseTypeDef = TypedDict(
-    "ListVersionsResponseTypeDef",
-    {
-        "Versions": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
-    "PurchaseReservedInstanceOfferingResponseTypeDef",
-    {
-        "ReservedInstanceId": str,
-        "ReservationName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AccessPoliciesStatusTypeDef = TypedDict(
     "AccessPoliciesStatusTypeDef",
     {
         "Options": str,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -1404,32 +1464,32 @@
     },
 )
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthorizeVpcEndpointAccessResponseTypeDef = TypedDict(
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipal": AuthorizedPrincipalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointAccessResponseTypeDef = TypedDict(
     "ListVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipalList": List[AuthorizedPrincipalTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoTuneDetailsTypeDef = TypedDict(
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": ScheduledAutoTuneDetailsTypeDef,
@@ -1443,40 +1503,48 @@
         "StartAt": Union[datetime, str],
         "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
     total=False,
 )
 
+EnvironmentInfoTypeDef = TypedDict(
+    "EnvironmentInfoTypeDef",
+    {
+        "AvailabilityZoneInformation": List[AvailabilityZoneInfoTypeDef],
+    },
+    total=False,
+)
+
 CancelServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "CancelServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "StartServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpgradeDomainResponseTypeDef = TypedDict(
     "UpgradeDomainResponseTypeDef",
     {
         "UpgradeId": str,
         "DomainName": str,
         "TargetVersion": str,
         "PerformCheckOnly": bool,
         "AdvancedOptions": Dict[str, str],
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeProgressStatusDetailsTypeDef = TypedDict(
     "ChangeProgressStatusDetailsTypeDef",
     {
         "ChangeId": str,
@@ -1500,14 +1568,15 @@
         "ZoneAwarenessConfig": ZoneAwarenessConfigTypeDef,
         "DedicatedMasterType": OpenSearchPartitionInstanceTypeType,
         "DedicatedMasterCount": int,
         "WarmEnabled": bool,
         "WarmType": OpenSearchWarmPartitionInstanceTypeType,
         "WarmCount": int,
         "ColdStorageOptions": ColdStorageOptionsTypeDef,
+        "MultiAZWithStandbyEnabled": bool,
     },
     total=False,
 )
 
 CognitoOptionsStatusTypeDef = TypedDict(
     "CognitoOptionsStatusTypeDef",
     {
@@ -1516,18 +1585,27 @@
     },
 )
 
 GetCompatibleVersionsResponseTypeDef = TypedDict(
     "GetCompatibleVersionsResponseTypeDef",
     {
         "CompatibleVersions": List[CompatibleVersionsMapTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ConnectionPropertiesTypeDef = TypedDict(
+    "ConnectionPropertiesTypeDef",
+    {
+        "Endpoint": str,
+        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesTypeDef,
+    },
+    total=False,
+)
+
 DomainEndpointOptionsStatusTypeDef = TypedDict(
     "DomainEndpointOptionsStatusTypeDef",
     {
         "Options": DomainEndpointOptionsTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -1658,33 +1736,41 @@
     pass
 
 
 DeleteVpcEndpointResponseTypeDef = TypedDict(
     "DeleteVpcEndpointResponseTypeDef",
     {
         "VpcEndpointSummary": VpcEndpointSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointsForDomainResponseTypeDef = TypedDict(
     "ListVpcEndpointsForDomainResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointsResponseTypeDef = TypedDict(
     "ListVpcEndpointsResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeDomainNodesResponseTypeDef = TypedDict(
+    "DescribeDomainNodesResponseTypeDef",
+    {
+        "DomainNodesStatusList": List[DomainNodesStatusTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInboundConnectionsRequestRequestTypeDef = TypedDict(
     "DescribeInboundConnectionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -1714,15 +1800,15 @@
     total=False,
 )
 
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "DomainNames": List[DomainInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainPackageDetailsTypeDef = TypedDict(
     "DomainPackageDetailsTypeDef",
     {
         "PackageID": str,
@@ -1801,15 +1887,15 @@
 
 GetPackageVersionHistoryResponseTypeDef = TypedDict(
     "GetPackageVersionHistoryResponseTypeDef",
     {
         "PackageID": str,
         "PackageVersionHistoryList": List[PackageVersionHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceLimitsTypeDef = TypedDict(
     "InstanceLimitsTypeDef",
     {
         "InstanceCountLimits": InstanceCountLimitsTypeDef,
@@ -1818,32 +1904,32 @@
 )
 
 ListInstanceTypeDetailsResponseTypeDef = TypedDict(
     "ListInstanceTypeDetailsResponseTypeDef",
     {
         "InstanceTypeDetails": List[InstanceTypeDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListScheduledActionsResponseTypeDef = TypedDict(
     "ListScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateScheduledActionResponseTypeDef = TypedDict(
     "UpdateScheduledActionResponseTypeDef",
     {
         "ScheduledAction": ScheduledActionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OffPeakWindowTypeDef = TypedDict(
     "OffPeakWindowTypeDef",
     {
         "WindowStartTime": WindowStartTimeTypeDef,
@@ -1930,78 +2016,26 @@
         "StartTimestamp": datetime,
         "UpgradeStatus": UpgradeStatusType,
         "StepsList": List[UpgradeStepItemTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOutboundConnectionRequestRequestTypeDef",
-    {
-        "LocalDomainInfo": DomainInformationContainerTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerTypeDef,
-        "ConnectionAlias": str,
-    },
-)
-_OptionalCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOutboundConnectionRequestRequestTypeDef",
-    {
-        "ConnectionMode": ConnectionModeType,
-    },
-    total=False,
-)
-
-
-class CreateOutboundConnectionRequestRequestTypeDef(
-    _RequiredCreateOutboundConnectionRequestRequestTypeDef,
-    _OptionalCreateOutboundConnectionRequestRequestTypeDef,
-):
-    pass
-
-
-CreateOutboundConnectionResponseTypeDef = TypedDict(
-    "CreateOutboundConnectionResponseTypeDef",
-    {
-        "LocalDomainInfo": DomainInformationContainerTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerTypeDef,
-        "ConnectionAlias": str,
-        "ConnectionStatus": OutboundConnectionStatusTypeDef,
-        "ConnectionId": str,
-        "ConnectionMode": ConnectionModeType,
-        "ConnectionProperties": ConnectionPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 InboundConnectionTypeDef = TypedDict(
     "InboundConnectionTypeDef",
     {
         "LocalDomainInfo": DomainInformationContainerTypeDef,
         "RemoteDomainInfo": DomainInformationContainerTypeDef,
         "ConnectionId": str,
         "ConnectionStatus": InboundConnectionStatusTypeDef,
         "ConnectionMode": ConnectionModeType,
     },
     total=False,
 )
 
-OutboundConnectionTypeDef = TypedDict(
-    "OutboundConnectionTypeDef",
-    {
-        "LocalDomainInfo": DomainInformationContainerTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerTypeDef,
-        "ConnectionId": str,
-        "ConnectionAlias": str,
-        "ConnectionStatus": OutboundConnectionStatusTypeDef,
-        "ConnectionMode": ConnectionModeType,
-        "ConnectionProperties": ConnectionPropertiesTypeDef,
-    },
-    total=False,
-)
-
 AutoTuneTypeDef = TypedDict(
     "AutoTuneTypeDef",
     {
         "AutoTuneType": Literal["SCHEDULED_ACTION"],
         "AutoTuneDetails": AutoTuneDetailsTypeDef,
     },
     total=False,
@@ -2024,119 +2058,192 @@
         "RollbackOnDisable": RollbackOnDisableType,
         "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
+DescribeDomainHealthResponseTypeDef = TypedDict(
+    "DescribeDomainHealthResponseTypeDef",
+    {
+        "DomainState": DomainStateType,
+        "AvailabilityZoneCount": str,
+        "ActiveAvailabilityZoneCount": str,
+        "StandByAvailabilityZoneCount": str,
+        "DataNodeCount": str,
+        "DedicatedMaster": bool,
+        "MasterEligibleNodeCount": str,
+        "WarmNodeCount": str,
+        "MasterNode": MasterNodeStatusType,
+        "ClusterHealth": DomainHealthType,
+        "TotalShards": str,
+        "TotalUnAssignedShards": str,
+        "EnvironmentInformation": List[EnvironmentInfoTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatus": ChangeProgressStatusDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterConfigStatusTypeDef = TypedDict(
     "ClusterConfigStatusTypeDef",
     {
         "Options": ClusterConfigTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
+_RequiredCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOutboundConnectionRequestRequestTypeDef",
+    {
+        "LocalDomainInfo": DomainInformationContainerTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "ConnectionAlias": str,
+    },
+)
+_OptionalCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOutboundConnectionRequestRequestTypeDef",
+    {
+        "ConnectionMode": ConnectionModeType,
+        "ConnectionProperties": ConnectionPropertiesTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateOutboundConnectionRequestRequestTypeDef(
+    _RequiredCreateOutboundConnectionRequestRequestTypeDef,
+    _OptionalCreateOutboundConnectionRequestRequestTypeDef,
+):
+    pass
+
+
+CreateOutboundConnectionResponseTypeDef = TypedDict(
+    "CreateOutboundConnectionResponseTypeDef",
+    {
+        "LocalDomainInfo": DomainInformationContainerTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "ConnectionAlias": str,
+        "ConnectionStatus": OutboundConnectionStatusTypeDef,
+        "ConnectionId": str,
+        "ConnectionMode": ConnectionModeType,
+        "ConnectionProperties": ConnectionPropertiesTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+OutboundConnectionTypeDef = TypedDict(
+    "OutboundConnectionTypeDef",
+    {
+        "LocalDomainInfo": DomainInformationContainerTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "ConnectionId": str,
+        "ConnectionAlias": str,
+        "ConnectionStatus": OutboundConnectionStatusTypeDef,
+        "ConnectionMode": ConnectionModeType,
+        "ConnectionProperties": ConnectionPropertiesTypeDef,
+    },
+    total=False,
+)
+
 AssociatePackageResponseTypeDef = TypedDict(
     "AssociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DissociatePackageResponseTypeDef = TypedDict(
     "DissociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsForPackageResponseTypeDef = TypedDict(
     "ListDomainsForPackageResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPackagesForDomainResponseTypeDef = TypedDict(
     "ListPackagesForDomainResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePackageResponseTypeDef = TypedDict(
     "DeletePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackagesResponseTypeDef = TypedDict(
     "DescribePackagesResponseTypeDef",
     {
         "PackageDetailsList": List[PackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePackageResponseTypeDef = TypedDict(
     "UpdatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVpcEndpointsResponseTypeDef = TypedDict(
     "DescribeVpcEndpointsResponseTypeDef",
     {
         "VpcEndpoints": List[VpcEndpointTypeDef],
         "VpcEndpointErrors": List[VpcEndpointErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVpcEndpointResponseTypeDef = TypedDict(
     "UpdateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OffPeakWindowOptionsTypeDef = TypedDict(
     "OffPeakWindowOptionsTypeDef",
     {
         "Enabled": bool,
@@ -2146,24 +2253,24 @@
 )
 
 DescribeReservedInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstanceOfferings": List[ReservedInstanceOfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservedInstancesResponseTypeDef = TypedDict(
     "DescribeReservedInstancesResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstances": List[ReservedInstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdvancedSecurityOptionsInputTypeDef = TypedDict(
     "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": bool,
@@ -2198,86 +2305,86 @@
 )
 
 GetUpgradeHistoryResponseTypeDef = TypedDict(
     "GetUpgradeHistoryResponseTypeDef",
     {
         "UpgradeHistories": List[UpgradeHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AcceptInboundConnectionResponseTypeDef = TypedDict(
     "AcceptInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInboundConnectionResponseTypeDef = TypedDict(
     "DeleteInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInboundConnectionsResponseTypeDef = TypedDict(
     "DescribeInboundConnectionsResponseTypeDef",
     {
         "Connections": List[InboundConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RejectInboundConnectionResponseTypeDef = TypedDict(
     "RejectInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteOutboundConnectionResponseTypeDef = TypedDict(
-    "DeleteOutboundConnectionResponseTypeDef",
-    {
-        "Connection": OutboundConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeOutboundConnectionsResponseTypeDef = TypedDict(
-    "DescribeOutboundConnectionsResponseTypeDef",
-    {
-        "Connections": List[OutboundConnectionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainAutoTunesResponseTypeDef = TypedDict(
     "DescribeDomainAutoTunesResponseTypeDef",
     {
         "AutoTunes": List[AutoTuneTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
         "Options": AutoTuneOptionsTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
+DeleteOutboundConnectionResponseTypeDef = TypedDict(
+    "DeleteOutboundConnectionResponseTypeDef",
+    {
+        "Connection": OutboundConnectionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeOutboundConnectionsResponseTypeDef = TypedDict(
+    "DescribeOutboundConnectionsResponseTypeDef",
+    {
+        "Connections": List[OutboundConnectionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OffPeakWindowOptionsStatusTypeDef = TypedDict(
     "OffPeakWindowOptionsStatusTypeDef",
     {
         "Options": OffPeakWindowOptionsTypeDef,
         "Status": OptionStatusTypeDef,
     },
     total=False,
@@ -2410,15 +2517,15 @@
     pass
 
 
 DescribeInstanceTypeLimitsResponseTypeDef = TypedDict(
     "DescribeInstanceTypeLimitsResponseTypeDef",
     {
         "LimitsByRole": Dict[str, LimitsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainConfigTypeDef = TypedDict(
     "DomainConfigTypeDef",
     {
         "EngineVersion": VersionStatusTypeDef,
@@ -2442,62 +2549,62 @@
     total=False,
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDomainResponseTypeDef = TypedDict(
     "DeleteDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainsResponseTypeDef = TypedDict(
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDryRunProgressResponseTypeDef = TypedDict(
     "DescribeDryRunProgressResponseTypeDef",
     {
         "DryRunProgressStatus": DryRunProgressStatusTypeDef,
         "DryRunConfig": DomainStatusTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainConfigResponseTypeDef = TypedDict(
     "DescribeDomainConfigResponseTypeDef",
     {
         "DomainConfig": DomainConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainConfigResponseTypeDef = TypedDict(
     "UpdateDomainConfigResponseTypeDef",
     {
         "DomainConfig": DomainConfigTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
         "DryRunProgressStatus": DryRunProgressStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/type_defs.pyi` & `mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -20,73 +20,80 @@
     ActionStatusType,
     ActionTypeType,
     AutoTuneDesiredStateType,
     AutoTuneStateType,
     ConnectionModeType,
     DeploymentStatusType,
     DescribePackagesFilterNameType,
+    DomainHealthType,
     DomainPackageStatusType,
+    DomainStateType,
     DryRunModeType,
     EngineTypeType,
     InboundConnectionStatusCodeType,
     LogTypeType,
+    MasterNodeStatusType,
+    NodeStatusType,
+    NodeTypeType,
     OpenSearchPartitionInstanceTypeType,
     OpenSearchWarmPartitionInstanceTypeType,
     OptionStateType,
     OutboundConnectionStatusCodeType,
     OverallChangeStatusType,
     PackageStatusType,
     PrincipalTypeType,
     ReservedInstancePaymentOptionType,
     RollbackOnDisableType,
     ScheduleAtType,
     ScheduledAutoTuneActionTypeType,
     ScheduledAutoTuneSeverityTypeType,
     ScheduledByType,
+    SkipUnavailableStatusType,
     TLSSecurityPolicyType,
     UpgradeStatusType,
     UpgradeStepType,
     VolumeTypeType,
     VpcEndpointErrorCodeType,
     VpcEndpointStatusType,
+    ZoneStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AWSDomainInformationTypeDef",
     "AcceptInboundConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "OptionStatusTypeDef",
     "TagTypeDef",
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
     "AssociatePackageRequestRequestTypeDef",
     "AuthorizeVpcEndpointAccessRequestRequestTypeDef",
     "AuthorizedPrincipalTypeDef",
     "ScheduledAutoTuneDetailsTypeDef",
     "DurationTypeDef",
     "AutoTuneOptionsOutputTypeDef",
     "AutoTuneStatusTypeDef",
+    "AvailabilityZoneInfoTypeDef",
     "CancelServiceSoftwareUpdateRequestRequestTypeDef",
     "ServiceSoftwareOptionsTypeDef",
     "ChangeProgressDetailsTypeDef",
     "ChangeProgressStageTypeDef",
     "ColdStorageOptionsTypeDef",
     "ZoneAwarenessConfigTypeDef",
     "CognitoOptionsTypeDef",
     "CompatibleVersionsMapTypeDef",
-    "ConnectionPropertiesTypeDef",
+    "CrossClusterSearchConnectionPropertiesTypeDef",
     "DomainEndpointOptionsTypeDef",
     "EBSOptionsTypeDef",
     "EncryptionAtRestOptionsTypeDef",
     "LogPublishingOptionTypeDef",
     "NodeToNodeEncryptionOptionsTypeDef",
     "SnapshotOptionsTypeDef",
     "SoftwareUpdateOptionsTypeDef",
@@ -98,14 +105,17 @@
     "DeleteOutboundConnectionRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeleteVpcEndpointRequestRequestTypeDef",
     "VpcEndpointSummaryTypeDef",
     "DescribeDomainAutoTunesRequestRequestTypeDef",
     "DescribeDomainChangeProgressRequestRequestTypeDef",
     "DescribeDomainConfigRequestRequestTypeDef",
+    "DescribeDomainHealthRequestRequestTypeDef",
+    "DescribeDomainNodesRequestRequestTypeDef",
+    "DomainNodesStatusTypeDef",
     "DescribeDomainRequestRequestTypeDef",
     "DescribeDomainsRequestRequestTypeDef",
     "DescribeDryRunProgressRequestRequestTypeDef",
     "DryRunResultsTypeDef",
     "FilterTypeDef",
     "DescribeInstanceTypeLimitsRequestRequestTypeDef",
     "DescribePackagesFilterTypeDef",
@@ -114,80 +124,84 @@
     "DescribeVpcEndpointsRequestRequestTypeDef",
     "VpcEndpointErrorTypeDef",
     "DissociatePackageRequestRequestTypeDef",
     "DomainInfoTypeDef",
     "ErrorDetailsTypeDef",
     "VPCDerivedInfoTypeDef",
     "ValidationFailureTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetCompatibleVersionsRequestRequestTypeDef",
     "GetPackageVersionHistoryRequestRequestTypeDef",
     "PackageVersionHistoryTypeDef",
     "GetUpgradeHistoryRequestRequestTypeDef",
     "GetUpgradeStatusRequestRequestTypeDef",
+    "GetUpgradeStatusResponseTypeDef",
     "InboundConnectionStatusTypeDef",
     "InstanceCountLimitsTypeDef",
     "InstanceTypeDetailsTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
     "ListInstanceTypeDetailsRequestRequestTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
     "ListScheduledActionsRequestRequestTypeDef",
     "ScheduledActionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListVersionsRequestRequestTypeDef",
+    "ListVersionsResponseTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
     "WindowStartTimeTypeDef",
     "PurchaseReservedInstanceOfferingRequestRequestTypeDef",
+    "PurchaseReservedInstanceOfferingResponseTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     "SAMLIdpTypeDef",
     "StartServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
     "UpdateScheduledActionRequestRequestTypeDef",
     "UpgradeDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
     "DomainInformationContainerTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetUpgradeStatusResponseTypeDef",
-    "ListVersionsResponseTypeDef",
-    "PurchaseReservedInstanceOfferingResponseTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AdvancedOptionsStatusTypeDef",
     "VersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
+    "EnvironmentInfoTypeDef",
     "CancelServiceSoftwareUpdateResponseTypeDef",
     "StartServiceSoftwareUpdateResponseTypeDef",
     "UpgradeDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
     "ClusterConfigTypeDef",
     "CognitoOptionsStatusTypeDef",
     "GetCompatibleVersionsResponseTypeDef",
+    "ConnectionPropertiesTypeDef",
     "DomainEndpointOptionsStatusTypeDef",
     "EBSOptionsStatusTypeDef",
     "EncryptionAtRestOptionsStatusTypeDef",
     "LogPublishingOptionsStatusTypeDef",
     "NodeToNodeEncryptionOptionsStatusTypeDef",
     "SnapshotOptionsStatusTypeDef",
     "SoftwareUpdateOptionsStatusTypeDef",
     "CreateVpcEndpointRequestRequestTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "ListVpcEndpointsForDomainResponseTypeDef",
     "ListVpcEndpointsResponseTypeDef",
+    "DescribeDomainNodesResponseTypeDef",
     "DescribeInboundConnectionsRequestRequestTypeDef",
     "DescribeOutboundConnectionsRequestRequestTypeDef",
     "DescribePackagesRequestRequestTypeDef",
     "ListDomainNamesResponseTypeDef",
     "DomainPackageDetailsTypeDef",
     "PackageDetailsTypeDef",
     "VPCDerivedInfoStatusTypeDef",
@@ -201,23 +215,24 @@
     "OffPeakWindowTypeDef",
     "ReservedInstanceOfferingTypeDef",
     "ReservedInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
-    "CreateOutboundConnectionRequestRequestTypeDef",
-    "CreateOutboundConnectionResponseTypeDef",
     "InboundConnectionTypeDef",
-    "OutboundConnectionTypeDef",
     "AutoTuneTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
+    "DescribeDomainHealthResponseTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "ClusterConfigStatusTypeDef",
+    "CreateOutboundConnectionRequestRequestTypeDef",
+    "CreateOutboundConnectionResponseTypeDef",
+    "OutboundConnectionTypeDef",
     "AssociatePackageResponseTypeDef",
     "DissociatePackageResponseTypeDef",
     "ListDomainsForPackageResponseTypeDef",
     "ListPackagesForDomainResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DeletePackageResponseTypeDef",
     "DescribePackagesResponseTypeDef",
@@ -232,18 +247,18 @@
     "AdvancedSecurityOptionsTypeDef",
     "LimitsTypeDef",
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
-    "DeleteOutboundConnectionResponseTypeDef",
-    "DescribeOutboundConnectionsResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
+    "DeleteOutboundConnectionResponseTypeDef",
+    "DescribeOutboundConnectionsResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "DomainStatusTypeDef",
     "DescribeInstanceTypeLimitsResponseTypeDef",
     "DomainConfigTypeDef",
@@ -279,25 +294,14 @@
 AcceptInboundConnectionRequestRequestTypeDef = TypedDict(
     "AcceptInboundConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
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
 _RequiredOptionStatusTypeDef = TypedDict(
     "_RequiredOptionStatusTypeDef",
     {
         "CreationDate": datetime,
         "UpdateDate": datetime,
         "State": OptionStateType,
     },
@@ -413,14 +417,27 @@
     },
     total=False,
 )
 
 class AutoTuneStatusTypeDef(_RequiredAutoTuneStatusTypeDef, _OptionalAutoTuneStatusTypeDef):
     pass
 
+AvailabilityZoneInfoTypeDef = TypedDict(
+    "AvailabilityZoneInfoTypeDef",
+    {
+        "AvailabilityZoneName": str,
+        "ZoneStatus": ZoneStatusType,
+        "ConfiguredDataNodeCount": str,
+        "AvailableDataNodeCount": str,
+        "TotalShards": str,
+        "TotalUnAssignedShards": str,
+    },
+    total=False,
+)
+
 CancelServiceSoftwareUpdateRequestRequestTypeDef = TypedDict(
     "CancelServiceSoftwareUpdateRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -490,18 +507,18 @@
     {
         "SourceVersion": str,
         "TargetVersions": List[str],
     },
     total=False,
 )
 
-ConnectionPropertiesTypeDef = TypedDict(
-    "ConnectionPropertiesTypeDef",
+CrossClusterSearchConnectionPropertiesTypeDef = TypedDict(
+    "CrossClusterSearchConnectionPropertiesTypeDef",
     {
-        "Endpoint": str,
+        "SkipUnavailable": SkipUnavailableStatusType,
     },
     total=False,
 )
 
 DomainEndpointOptionsTypeDef = TypedDict(
     "DomainEndpointOptionsTypeDef",
     {
@@ -685,14 +702,43 @@
 DescribeDomainConfigRequestRequestTypeDef = TypedDict(
     "DescribeDomainConfigRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+DescribeDomainHealthRequestRequestTypeDef = TypedDict(
+    "DescribeDomainHealthRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+
+DescribeDomainNodesRequestRequestTypeDef = TypedDict(
+    "DescribeDomainNodesRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+
+DomainNodesStatusTypeDef = TypedDict(
+    "DomainNodesStatusTypeDef",
+    {
+        "NodeId": str,
+        "NodeType": NodeTypeType,
+        "AvailabilityZone": str,
+        "InstanceType": OpenSearchPartitionInstanceTypeType,
+        "NodeStatus": NodeStatusType,
+        "StorageType": str,
+        "StorageVolumeType": VolumeTypeType,
+        "StorageSize": str,
+    },
+    total=False,
+)
+
 DescribeDomainRequestRequestTypeDef = TypedDict(
     "DescribeDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -851,14 +897,21 @@
     {
         "Code": str,
         "Message": str,
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
 GetCompatibleVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleVersionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
     total=False,
 )
@@ -917,14 +970,24 @@
 GetUpgradeStatusRequestRequestTypeDef = TypedDict(
     "GetUpgradeStatusRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+GetUpgradeStatusResponseTypeDef = TypedDict(
+    "GetUpgradeStatusResponseTypeDef",
+    {
+        "UpgradeStep": UpgradeStepType,
+        "StepStatus": UpgradeStatusType,
+        "UpgradeName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InboundConnectionStatusTypeDef = TypedDict(
     "InboundConnectionStatusTypeDef",
     {
         "StatusCode": InboundConnectionStatusCodeType,
         "Message": str,
     },
     total=False,
@@ -945,14 +1008,15 @@
         "InstanceType": OpenSearchPartitionInstanceTypeType,
         "EncryptionEnabled": bool,
         "CognitoEnabled": bool,
         "AppLogsEnabled": bool,
         "AdvancedSecurityEnabled": bool,
         "WarmEnabled": bool,
         "InstanceRole": List[str],
+        "AvailabilityZones": List[str],
     },
     total=False,
 )
 
 ListDomainNamesRequestRequestTypeDef = TypedDict(
     "ListDomainNamesRequestRequestTypeDef",
     {
@@ -990,14 +1054,16 @@
 )
 _OptionalListInstanceTypeDetailsRequestRequestTypeDef = TypedDict(
     "_OptionalListInstanceTypeDetailsRequestRequestTypeDef",
     {
         "DomainName": str,
         "MaxResults": int,
         "NextToken": str,
+        "RetrieveAZs": bool,
+        "InstanceType": str,
     },
     total=False,
 )
 
 class ListInstanceTypeDetailsRequestRequestTypeDef(
     _RequiredListInstanceTypeDetailsRequestRequestTypeDef,
     _OptionalListInstanceTypeDetailsRequestRequestTypeDef,
@@ -1082,14 +1148,23 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListVersionsResponseTypeDef = TypedDict(
+    "ListVersionsResponseTypeDef",
+    {
+        "Versions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "_RequiredListVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListVpcEndpointAccessRequestRequestTypeDef = TypedDict(
@@ -1159,14 +1234,23 @@
 
 class PurchaseReservedInstanceOfferingRequestRequestTypeDef(
     _RequiredPurchaseReservedInstanceOfferingRequestRequestTypeDef,
     _OptionalPurchaseReservedInstanceOfferingRequestRequestTypeDef,
 ):
     pass
 
+PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
+    "PurchaseReservedInstanceOfferingResponseTypeDef",
+    {
+        "ReservedInstanceId": str,
+        "ReservationName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "RecurringChargeAmount": float,
         "RecurringChargeFrequency": str,
     },
     total=False,
@@ -1183,14 +1267,25 @@
     "RemoveTagsRequestRequestTypeDef",
     {
         "ARN": str,
         "TagKeys": Sequence[str],
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
 RevokeVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
         "Account": str,
     },
 )
@@ -1292,49 +1387,14 @@
     "DomainInformationContainerTypeDef",
     {
         "AWSDomainInformation": AWSDomainInformationTypeDef,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUpgradeStatusResponseTypeDef = TypedDict(
-    "GetUpgradeStatusResponseTypeDef",
-    {
-        "UpgradeStep": UpgradeStepType,
-        "StepStatus": UpgradeStatusType,
-        "UpgradeName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListVersionsResponseTypeDef = TypedDict(
-    "ListVersionsResponseTypeDef",
-    {
-        "Versions": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
-    "PurchaseReservedInstanceOfferingResponseTypeDef",
-    {
-        "ReservedInstanceId": str,
-        "ReservationName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AccessPoliciesStatusTypeDef = TypedDict(
     "AccessPoliciesStatusTypeDef",
     {
         "Options": str,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -1363,32 +1423,32 @@
     },
 )
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthorizeVpcEndpointAccessResponseTypeDef = TypedDict(
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipal": AuthorizedPrincipalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointAccessResponseTypeDef = TypedDict(
     "ListVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipalList": List[AuthorizedPrincipalTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoTuneDetailsTypeDef = TypedDict(
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": ScheduledAutoTuneDetailsTypeDef,
@@ -1402,40 +1462,48 @@
         "StartAt": Union[datetime, str],
         "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
     total=False,
 )
 
+EnvironmentInfoTypeDef = TypedDict(
+    "EnvironmentInfoTypeDef",
+    {
+        "AvailabilityZoneInformation": List[AvailabilityZoneInfoTypeDef],
+    },
+    total=False,
+)
+
 CancelServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "CancelServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "StartServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpgradeDomainResponseTypeDef = TypedDict(
     "UpgradeDomainResponseTypeDef",
     {
         "UpgradeId": str,
         "DomainName": str,
         "TargetVersion": str,
         "PerformCheckOnly": bool,
         "AdvancedOptions": Dict[str, str],
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeProgressStatusDetailsTypeDef = TypedDict(
     "ChangeProgressStatusDetailsTypeDef",
     {
         "ChangeId": str,
@@ -1459,14 +1527,15 @@
         "ZoneAwarenessConfig": ZoneAwarenessConfigTypeDef,
         "DedicatedMasterType": OpenSearchPartitionInstanceTypeType,
         "DedicatedMasterCount": int,
         "WarmEnabled": bool,
         "WarmType": OpenSearchWarmPartitionInstanceTypeType,
         "WarmCount": int,
         "ColdStorageOptions": ColdStorageOptionsTypeDef,
+        "MultiAZWithStandbyEnabled": bool,
     },
     total=False,
 )
 
 CognitoOptionsStatusTypeDef = TypedDict(
     "CognitoOptionsStatusTypeDef",
     {
@@ -1475,18 +1544,27 @@
     },
 )
 
 GetCompatibleVersionsResponseTypeDef = TypedDict(
     "GetCompatibleVersionsResponseTypeDef",
     {
         "CompatibleVersions": List[CompatibleVersionsMapTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ConnectionPropertiesTypeDef = TypedDict(
+    "ConnectionPropertiesTypeDef",
+    {
+        "Endpoint": str,
+        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesTypeDef,
+    },
+    total=False,
+)
+
 DomainEndpointOptionsStatusTypeDef = TypedDict(
     "DomainEndpointOptionsStatusTypeDef",
     {
         "Options": DomainEndpointOptionsTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -1611,33 +1689,41 @@
 ):
     pass
 
 DeleteVpcEndpointResponseTypeDef = TypedDict(
     "DeleteVpcEndpointResponseTypeDef",
     {
         "VpcEndpointSummary": VpcEndpointSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointsForDomainResponseTypeDef = TypedDict(
     "ListVpcEndpointsForDomainResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointsResponseTypeDef = TypedDict(
     "ListVpcEndpointsResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeDomainNodesResponseTypeDef = TypedDict(
+    "DescribeDomainNodesResponseTypeDef",
+    {
+        "DomainNodesStatusList": List[DomainNodesStatusTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInboundConnectionsRequestRequestTypeDef = TypedDict(
     "DescribeInboundConnectionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -1667,15 +1753,15 @@
     total=False,
 )
 
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "DomainNames": List[DomainInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainPackageDetailsTypeDef = TypedDict(
     "DomainPackageDetailsTypeDef",
     {
         "PackageID": str,
@@ -1752,15 +1838,15 @@
 
 GetPackageVersionHistoryResponseTypeDef = TypedDict(
     "GetPackageVersionHistoryResponseTypeDef",
     {
         "PackageID": str,
         "PackageVersionHistoryList": List[PackageVersionHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceLimitsTypeDef = TypedDict(
     "InstanceLimitsTypeDef",
     {
         "InstanceCountLimits": InstanceCountLimitsTypeDef,
@@ -1769,32 +1855,32 @@
 )
 
 ListInstanceTypeDetailsResponseTypeDef = TypedDict(
     "ListInstanceTypeDetailsResponseTypeDef",
     {
         "InstanceTypeDetails": List[InstanceTypeDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListScheduledActionsResponseTypeDef = TypedDict(
     "ListScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateScheduledActionResponseTypeDef = TypedDict(
     "UpdateScheduledActionResponseTypeDef",
     {
         "ScheduledAction": ScheduledActionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OffPeakWindowTypeDef = TypedDict(
     "OffPeakWindowTypeDef",
     {
         "WindowStartTime": WindowStartTimeTypeDef,
@@ -1881,76 +1967,26 @@
         "StartTimestamp": datetime,
         "UpgradeStatus": UpgradeStatusType,
         "StepsList": List[UpgradeStepItemTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOutboundConnectionRequestRequestTypeDef",
-    {
-        "LocalDomainInfo": DomainInformationContainerTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerTypeDef,
-        "ConnectionAlias": str,
-    },
-)
-_OptionalCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOutboundConnectionRequestRequestTypeDef",
-    {
-        "ConnectionMode": ConnectionModeType,
-    },
-    total=False,
-)
-
-class CreateOutboundConnectionRequestRequestTypeDef(
-    _RequiredCreateOutboundConnectionRequestRequestTypeDef,
-    _OptionalCreateOutboundConnectionRequestRequestTypeDef,
-):
-    pass
-
-CreateOutboundConnectionResponseTypeDef = TypedDict(
-    "CreateOutboundConnectionResponseTypeDef",
-    {
-        "LocalDomainInfo": DomainInformationContainerTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerTypeDef,
-        "ConnectionAlias": str,
-        "ConnectionStatus": OutboundConnectionStatusTypeDef,
-        "ConnectionId": str,
-        "ConnectionMode": ConnectionModeType,
-        "ConnectionProperties": ConnectionPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 InboundConnectionTypeDef = TypedDict(
     "InboundConnectionTypeDef",
     {
         "LocalDomainInfo": DomainInformationContainerTypeDef,
         "RemoteDomainInfo": DomainInformationContainerTypeDef,
         "ConnectionId": str,
         "ConnectionStatus": InboundConnectionStatusTypeDef,
         "ConnectionMode": ConnectionModeType,
     },
     total=False,
 )
 
-OutboundConnectionTypeDef = TypedDict(
-    "OutboundConnectionTypeDef",
-    {
-        "LocalDomainInfo": DomainInformationContainerTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerTypeDef,
-        "ConnectionId": str,
-        "ConnectionAlias": str,
-        "ConnectionStatus": OutboundConnectionStatusTypeDef,
-        "ConnectionMode": ConnectionModeType,
-        "ConnectionProperties": ConnectionPropertiesTypeDef,
-    },
-    total=False,
-)
-
 AutoTuneTypeDef = TypedDict(
     "AutoTuneTypeDef",
     {
         "AutoTuneType": Literal["SCHEDULED_ACTION"],
         "AutoTuneDetails": AutoTuneDetailsTypeDef,
     },
     total=False,
@@ -1973,119 +2009,190 @@
         "RollbackOnDisable": RollbackOnDisableType,
         "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
+DescribeDomainHealthResponseTypeDef = TypedDict(
+    "DescribeDomainHealthResponseTypeDef",
+    {
+        "DomainState": DomainStateType,
+        "AvailabilityZoneCount": str,
+        "ActiveAvailabilityZoneCount": str,
+        "StandByAvailabilityZoneCount": str,
+        "DataNodeCount": str,
+        "DedicatedMaster": bool,
+        "MasterEligibleNodeCount": str,
+        "WarmNodeCount": str,
+        "MasterNode": MasterNodeStatusType,
+        "ClusterHealth": DomainHealthType,
+        "TotalShards": str,
+        "TotalUnAssignedShards": str,
+        "EnvironmentInformation": List[EnvironmentInfoTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatus": ChangeProgressStatusDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterConfigStatusTypeDef = TypedDict(
     "ClusterConfigStatusTypeDef",
     {
         "Options": ClusterConfigTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
+_RequiredCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOutboundConnectionRequestRequestTypeDef",
+    {
+        "LocalDomainInfo": DomainInformationContainerTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "ConnectionAlias": str,
+    },
+)
+_OptionalCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOutboundConnectionRequestRequestTypeDef",
+    {
+        "ConnectionMode": ConnectionModeType,
+        "ConnectionProperties": ConnectionPropertiesTypeDef,
+    },
+    total=False,
+)
+
+class CreateOutboundConnectionRequestRequestTypeDef(
+    _RequiredCreateOutboundConnectionRequestRequestTypeDef,
+    _OptionalCreateOutboundConnectionRequestRequestTypeDef,
+):
+    pass
+
+CreateOutboundConnectionResponseTypeDef = TypedDict(
+    "CreateOutboundConnectionResponseTypeDef",
+    {
+        "LocalDomainInfo": DomainInformationContainerTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "ConnectionAlias": str,
+        "ConnectionStatus": OutboundConnectionStatusTypeDef,
+        "ConnectionId": str,
+        "ConnectionMode": ConnectionModeType,
+        "ConnectionProperties": ConnectionPropertiesTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+OutboundConnectionTypeDef = TypedDict(
+    "OutboundConnectionTypeDef",
+    {
+        "LocalDomainInfo": DomainInformationContainerTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "ConnectionId": str,
+        "ConnectionAlias": str,
+        "ConnectionStatus": OutboundConnectionStatusTypeDef,
+        "ConnectionMode": ConnectionModeType,
+        "ConnectionProperties": ConnectionPropertiesTypeDef,
+    },
+    total=False,
+)
+
 AssociatePackageResponseTypeDef = TypedDict(
     "AssociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DissociatePackageResponseTypeDef = TypedDict(
     "DissociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsForPackageResponseTypeDef = TypedDict(
     "ListDomainsForPackageResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPackagesForDomainResponseTypeDef = TypedDict(
     "ListPackagesForDomainResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePackageResponseTypeDef = TypedDict(
     "DeletePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackagesResponseTypeDef = TypedDict(
     "DescribePackagesResponseTypeDef",
     {
         "PackageDetailsList": List[PackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePackageResponseTypeDef = TypedDict(
     "UpdatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVpcEndpointsResponseTypeDef = TypedDict(
     "DescribeVpcEndpointsResponseTypeDef",
     {
         "VpcEndpoints": List[VpcEndpointTypeDef],
         "VpcEndpointErrors": List[VpcEndpointErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVpcEndpointResponseTypeDef = TypedDict(
     "UpdateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OffPeakWindowOptionsTypeDef = TypedDict(
     "OffPeakWindowOptionsTypeDef",
     {
         "Enabled": bool,
@@ -2095,24 +2202,24 @@
 )
 
 DescribeReservedInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstanceOfferings": List[ReservedInstanceOfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservedInstancesResponseTypeDef = TypedDict(
     "DescribeReservedInstancesResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstances": List[ReservedInstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdvancedSecurityOptionsInputTypeDef = TypedDict(
     "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": bool,
@@ -2147,86 +2254,86 @@
 )
 
 GetUpgradeHistoryResponseTypeDef = TypedDict(
     "GetUpgradeHistoryResponseTypeDef",
     {
         "UpgradeHistories": List[UpgradeHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AcceptInboundConnectionResponseTypeDef = TypedDict(
     "AcceptInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInboundConnectionResponseTypeDef = TypedDict(
     "DeleteInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInboundConnectionsResponseTypeDef = TypedDict(
     "DescribeInboundConnectionsResponseTypeDef",
     {
         "Connections": List[InboundConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RejectInboundConnectionResponseTypeDef = TypedDict(
     "RejectInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteOutboundConnectionResponseTypeDef = TypedDict(
-    "DeleteOutboundConnectionResponseTypeDef",
-    {
-        "Connection": OutboundConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeOutboundConnectionsResponseTypeDef = TypedDict(
-    "DescribeOutboundConnectionsResponseTypeDef",
-    {
-        "Connections": List[OutboundConnectionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainAutoTunesResponseTypeDef = TypedDict(
     "DescribeDomainAutoTunesResponseTypeDef",
     {
         "AutoTunes": List[AutoTuneTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
         "Options": AutoTuneOptionsTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
+DeleteOutboundConnectionResponseTypeDef = TypedDict(
+    "DeleteOutboundConnectionResponseTypeDef",
+    {
+        "Connection": OutboundConnectionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeOutboundConnectionsResponseTypeDef = TypedDict(
+    "DescribeOutboundConnectionsResponseTypeDef",
+    {
+        "Connections": List[OutboundConnectionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OffPeakWindowOptionsStatusTypeDef = TypedDict(
     "OffPeakWindowOptionsStatusTypeDef",
     {
         "Options": OffPeakWindowOptionsTypeDef,
         "Status": OptionStatusTypeDef,
     },
     total=False,
@@ -2353,15 +2460,15 @@
 class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
     pass
 
 DescribeInstanceTypeLimitsResponseTypeDef = TypedDict(
     "DescribeInstanceTypeLimitsResponseTypeDef",
     {
         "LimitsByRole": Dict[str, LimitsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainConfigTypeDef = TypedDict(
     "DomainConfigTypeDef",
     {
         "EngineVersion": VersionStatusTypeDef,
@@ -2385,62 +2492,62 @@
     total=False,
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDomainResponseTypeDef = TypedDict(
     "DeleteDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainsResponseTypeDef = TypedDict(
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDryRunProgressResponseTypeDef = TypedDict(
     "DescribeDryRunProgressResponseTypeDef",
     {
         "DryRunProgressStatus": DryRunProgressStatusTypeDef,
         "DryRunConfig": DomainStatusTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainConfigResponseTypeDef = TypedDict(
     "DescribeDomainConfigResponseTypeDef",
     {
         "DomainConfig": DomainConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainConfigResponseTypeDef = TypedDict(
     "UpdateDomainConfigResponseTypeDef",
     {
         "DomainConfig": DomainConfigTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
         "DryRunProgressStatus": DryRunProgressStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/PKG-INFO` & `mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.26.77
-Summary: Type annotations for boto3.OpenSearchService 1.26.77 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.OpenSearchService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-opensearch"></a>
 
 # mypy-boto3-opensearch
 
 [![PyPI - mypy-boto3-opensearch](https://img.shields.io/pypi/v/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearch?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -285,40 +285,47 @@
     ActionTypeType,
     AutoTuneDesiredStateType,
     AutoTuneStateType,
     AutoTuneTypeType,
     ConnectionModeType,
     DeploymentStatusType,
     DescribePackagesFilterNameType,
+    DomainHealthType,
     DomainPackageStatusType,
+    DomainStateType,
     DryRunModeType,
     EngineTypeType,
     InboundConnectionStatusCodeType,
     LogTypeType,
+    MasterNodeStatusType,
+    NodeStatusType,
+    NodeTypeType,
     OpenSearchPartitionInstanceTypeType,
     OpenSearchWarmPartitionInstanceTypeType,
     OptionStateType,
     OutboundConnectionStatusCodeType,
     OverallChangeStatusType,
     PackageStatusType,
     PackageTypeType,
     PrincipalTypeType,
     ReservedInstancePaymentOptionType,
     RollbackOnDisableType,
     ScheduleAtType,
     ScheduledAutoTuneActionTypeType,
     ScheduledAutoTuneSeverityTypeType,
     ScheduledByType,
+    SkipUnavailableStatusType,
     TLSSecurityPolicyType,
     TimeUnitType,
     UpgradeStatusType,
     UpgradeStepType,
     VolumeTypeType,
     VpcEndpointErrorCodeType,
     VpcEndpointStatusType,
+    ZoneStatusType,
     OpenSearchServiceServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
@@ -333,35 +340,35 @@
 `mypy_boto3_opensearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearch.type_defs import (
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
     DurationTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
+    AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
     ColdStorageOptionsTypeDef,
     ZoneAwarenessConfigTypeDef,
     CognitoOptionsTypeDef,
     CompatibleVersionsMapTypeDef,
-    ConnectionPropertiesTypeDef,
+    CrossClusterSearchConnectionPropertiesTypeDef,
     DomainEndpointOptionsTypeDef,
     EBSOptionsTypeDef,
     EncryptionAtRestOptionsTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
     SnapshotOptionsTypeDef,
     SoftwareUpdateOptionsTypeDef,
@@ -373,14 +380,17 @@
     DeleteOutboundConnectionRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeleteVpcEndpointRequestRequestTypeDef,
     VpcEndpointSummaryTypeDef,
     DescribeDomainAutoTunesRequestRequestTypeDef,
     DescribeDomainChangeProgressRequestRequestTypeDef,
     DescribeDomainConfigRequestRequestTypeDef,
+    DescribeDomainHealthRequestRequestTypeDef,
+    DescribeDomainNodesRequestRequestTypeDef,
+    DomainNodesStatusTypeDef,
     DescribeDomainRequestRequestTypeDef,
     DescribeDomainsRequestRequestTypeDef,
     DescribeDryRunProgressRequestRequestTypeDef,
     DryRunResultsTypeDef,
     FilterTypeDef,
     DescribeInstanceTypeLimitsRequestRequestTypeDef,
     DescribePackagesFilterTypeDef,
@@ -389,80 +399,84 @@
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
     VPCDerivedInfoTypeDef,
     ValidationFailureTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCompatibleVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
+    GetUpgradeStatusResponseTypeDef,
     InboundConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     InstanceTypeDetailsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListScheduledActionsRequestRequestTypeDef,
     ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVersionsRequestRequestTypeDef,
+    ListVersionsResponseTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
     WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
+    PurchaseReservedInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
     DomainInformationContainerTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetUpgradeStatusResponseTypeDef,
-    ListVersionsResponseTypeDef,
-    PurchaseReservedInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     VersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
+    EnvironmentInfoTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsStatusTypeDef,
     GetCompatibleVersionsResponseTypeDef,
+    ConnectionPropertiesTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     EBSOptionsStatusTypeDef,
     EncryptionAtRestOptionsStatusTypeDef,
     LogPublishingOptionsStatusTypeDef,
     NodeToNodeEncryptionOptionsStatusTypeDef,
     SnapshotOptionsStatusTypeDef,
     SoftwareUpdateOptionsStatusTypeDef,
     CreateVpcEndpointRequestRequestTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     CreatePackageRequestRequestTypeDef,
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
+    DescribeDomainNodesResponseTypeDef,
     DescribeInboundConnectionsRequestRequestTypeDef,
     DescribeOutboundConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
     VPCDerivedInfoStatusTypeDef,
@@ -476,23 +490,24 @@
     OffPeakWindowTypeDef,
     ReservedInstanceOfferingTypeDef,
     ReservedInstanceTypeDef,
     SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
-    CreateOutboundConnectionRequestRequestTypeDef,
-    CreateOutboundConnectionResponseTypeDef,
     InboundConnectionTypeDef,
-    OutboundConnectionTypeDef,
     AutoTuneTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
+    DescribeDomainHealthResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     ClusterConfigStatusTypeDef,
+    CreateOutboundConnectionRequestRequestTypeDef,
+    CreateOutboundConnectionResponseTypeDef,
+    OutboundConnectionTypeDef,
     AssociatePackageResponseTypeDef,
     DissociatePackageResponseTypeDef,
     ListDomainsForPackageResponseTypeDef,
     ListPackagesForDomainResponseTypeDef,
     CreatePackageResponseTypeDef,
     DeletePackageResponseTypeDef,
     DescribePackagesResponseTypeDef,
@@ -507,18 +522,18 @@
     AdvancedSecurityOptionsTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
-    DeleteOutboundConnectionResponseTypeDef,
-    DescribeOutboundConnectionsResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    DeleteOutboundConnectionResponseTypeDef,
+    DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DomainConfigTypeDef,
@@ -539,42 +554,42 @@
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

### Comparing `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/SOURCES.txt` & `mypy-boto3-opensearch-1.27.0/mypy_boto3_opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.26.77/setup.py` & `mypy-boto3-opensearch-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-opensearch.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opensearch",
-    version="1.26.77",
+    version="1.27.0",
     packages=["mypy_boto3_opensearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchService 1.26.77 service generated with"
-        " mypy-boto3-builder 7.12.4"
+        "Type annotations for boto3.OpenSearchService 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/",
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


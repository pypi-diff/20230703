# Comparing `tmp/mypy-boto3-lightsail-1.26.81.tar.gz` & `tmp/mypy-boto3-lightsail-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lightsail-1.26.81.tar", last modified: Tue Feb 28 20:28:07 2023, max compression
+gzip compressed data, was "mypy-boto3-lightsail-1.27.0.tar", last modified: Mon Jul  3 19:51:03 2023, max compression
```

## Comparing `mypy-boto3-lightsail-1.26.81.tar` & `mypy-boto3-lightsail-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.522319 mypy-boto3-lightsail-1.26.81/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-02-28 20:28:07.522319 mypy-boto3-lightsail-1.26.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35040 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.518319 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113914 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   113728 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25034 2023-02-28 20:27:49.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25032 2023-02-28 20:27:49.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   146228 2023-02-28 20:27:52.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   146129 2023-02-28 20:27:51.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.522319 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-02-28 20:28:07.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-02-28 20:28:07.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:28:07.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:28:07.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-28 20:28:07.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-28 20:28:07.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 20:28:07.522319 mypy-boto3-lightsail-1.26.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-28 20:27:47.000000 mypy-boto3-lightsail-1.26.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:02.999585 mypy-boto3-lightsail-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:06.000000 mypy-boto3-lightsail-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36513 2023-07-03 19:51:02.991585 mypy-boto3-lightsail-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35020 2023-07-03 19:41:06.000000 mypy-boto3-lightsail-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:02.991585 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-03 19:41:06.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-03 19:41:06.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:41:06.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113940 2023-07-03 19:41:07.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113754 2023-07-03 19:41:06.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25237 2023-07-03 19:41:07.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25235 2023-07-03 19:41:07.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-07-03 19:41:07.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22978 2023-07-03 19:41:07.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:06.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   146638 2023-07-03 19:41:12.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146539 2023-07-03 19:41:10.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:06.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:02.991585 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36513 2023-07-03 19:51:02.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:51:02.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:02.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:02.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:02.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:51:02.000000 mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:02.999585 mypy-boto3-lightsail-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:41:06.000000 mypy-boto3-lightsail-1.27.0/setup.py
```

### Comparing `mypy-boto3-lightsail-1.26.81/LICENSE` & `mypy-boto3-lightsail-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-lightsail-1.26.81/PKG-INFO` & `mypy-boto3-lightsail-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.26.81
-Summary: Type annotations for boto3.Lightsail 1.26.81 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.Lightsail 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-lightsail"></a>
 
 # mypy-boto3-lightsail
 
 [![PyPI - mypy-boto3-lightsail](https://img.shields.io/pypi/v/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lightsail?color=blue)](https://pypistats.org/packages/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -482,15 +482,14 @@
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
     StopInstanceOnIdleRequestTypeDef,
     AddOnTypeDef,
     MonitoredResourceInfoTypeDef,
     ResourceLocationTypeDef,
     AllocateStaticIpRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AttachCertificateToDistributionRequestRequestTypeDef,
     AttachDiskRequestRequestTypeDef,
     AttachInstancesToLoadBalancerRequestRequestTypeDef,
     AttachLoadBalancerTlsCertificateRequestRequestTypeDef,
     AttachStaticIpRequestRequestTypeDef,
     AttachedDiskTypeDef,
     AvailabilityZoneTypeDef,
@@ -553,110 +552,138 @@
     DetachStaticIpRequestRequestTypeDef,
     DisableAddOnRequestRequestTypeDef,
     DiskInfoTypeDef,
     DiskSnapshotInfoTypeDef,
     DistributionBundleTypeDef,
     DnsRecordCreationStateTypeDef,
     ResourceRecordTypeDef,
+    DownloadDefaultKeyPairResultTypeDef,
     TimePeriodTypeDef,
     ExportSnapshotRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
     GetActiveNamesRequestRequestTypeDef,
+    GetActiveNamesResultTypeDef,
     GetAlarmsRequestRequestTypeDef,
     GetAutoSnapshotsRequestRequestTypeDef,
+    GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
     GetBlueprintsRequestRequestTypeDef,
     GetBucketAccessKeysRequestRequestTypeDef,
     GetBucketBundlesRequestRequestTypeDef,
     GetBucketMetricDataRequestRequestTypeDef,
     MetricDatapointTypeDef,
     GetBucketsRequestRequestTypeDef,
+    GetBundlesRequestGetBundlesPaginateTypeDef,
     GetBundlesRequestRequestTypeDef,
     GetCertificatesRequestRequestTypeDef,
+    GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
     GetCloudFormationStackRecordsRequestRequestTypeDef,
     GetContactMethodsRequestRequestTypeDef,
+    GetContainerAPIMetadataResultTypeDef,
     GetContainerImagesRequestRequestTypeDef,
     GetContainerLogRequestRequestTypeDef,
     GetContainerServiceDeploymentsRequestRequestTypeDef,
     GetContainerServiceMetricDataRequestRequestTypeDef,
     GetContainerServicesRequestRequestTypeDef,
     GetCostEstimateRequestRequestTypeDef,
     GetDiskRequestRequestTypeDef,
     GetDiskSnapshotRequestRequestTypeDef,
+    GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
     GetDiskSnapshotsRequestRequestTypeDef,
+    GetDisksRequestGetDisksPaginateTypeDef,
     GetDisksRequestRequestTypeDef,
     GetDistributionLatestCacheResetRequestRequestTypeDef,
+    GetDistributionLatestCacheResetResultTypeDef,
     GetDistributionMetricDataRequestRequestTypeDef,
     GetDistributionsRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
+    GetDomainsRequestGetDomainsPaginateTypeDef,
     GetDomainsRequestRequestTypeDef,
+    GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef,
     GetExportSnapshotRecordsRequestRequestTypeDef,
     GetInstanceAccessDetailsRequestRequestTypeDef,
     GetInstanceMetricDataRequestRequestTypeDef,
     GetInstancePortStatesRequestRequestTypeDef,
     InstancePortStateTypeDef,
     GetInstanceRequestRequestTypeDef,
     GetInstanceSnapshotRequestRequestTypeDef,
+    GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef,
     GetInstanceSnapshotsRequestRequestTypeDef,
     GetInstanceStateRequestRequestTypeDef,
     InstanceStateTypeDef,
+    GetInstancesRequestGetInstancesPaginateTypeDef,
     GetInstancesRequestRequestTypeDef,
     GetKeyPairRequestRequestTypeDef,
+    GetKeyPairsRequestGetKeyPairsPaginateTypeDef,
     GetKeyPairsRequestRequestTypeDef,
     GetLoadBalancerMetricDataRequestRequestTypeDef,
     GetLoadBalancerRequestRequestTypeDef,
     GetLoadBalancerTlsCertificatesRequestRequestTypeDef,
     GetLoadBalancerTlsPoliciesRequestRequestTypeDef,
     LoadBalancerTlsPolicyTypeDef,
+    GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef,
     GetLoadBalancersRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     GetOperationsForResourceRequestRequestTypeDef,
+    GetOperationsRequestGetOperationsPaginateTypeDef,
     GetOperationsRequestRequestTypeDef,
     GetRegionsRequestRequestTypeDef,
+    GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef,
     GetRelationalDatabaseBlueprintsRequestRequestTypeDef,
     RelationalDatabaseBlueprintTypeDef,
+    GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef,
     GetRelationalDatabaseBundlesRequestRequestTypeDef,
     RelationalDatabaseBundleTypeDef,
+    GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
     GetRelationalDatabaseEventsRequestRequestTypeDef,
     RelationalDatabaseEventTypeDef,
     GetRelationalDatabaseLogEventsRequestRequestTypeDef,
     LogEventTypeDef,
     GetRelationalDatabaseLogStreamsRequestRequestTypeDef,
+    GetRelationalDatabaseLogStreamsResultTypeDef,
     GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
+    GetRelationalDatabaseMasterUserPasswordResultTypeDef,
     GetRelationalDatabaseMetricDataRequestRequestTypeDef,
+    GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
     GetRelationalDatabaseParametersRequestRequestTypeDef,
     RelationalDatabaseParameterTypeDef,
     GetRelationalDatabaseRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotRequestRequestTypeDef,
+    GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
     GetRelationalDatabaseSnapshotsRequestRequestTypeDef,
+    GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
     GetRelationalDatabasesRequestRequestTypeDef,
     GetStaticIpRequestRequestTypeDef,
+    GetStaticIpsRequestGetStaticIpsPaginateTypeDef,
     GetStaticIpsRequestRequestTypeDef,
     HostKeyAttributesTypeDef,
     ImportKeyPairRequestRequestTypeDef,
     PasswordDataTypeDef,
     InstanceHealthSummaryTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstancePortInfoTypeDef,
     MonthlyTransferTypeDef,
+    IsVpcPeeredResultTypeDef,
     OriginTypeDef,
     LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef,
     LoadBalancerTlsCertificateDomainValidationOptionTypeDef,
     LoadBalancerTlsCertificateSummaryTypeDef,
     NameServersUpdateStateTypeDef,
+    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PendingModifiedRelationalDatabaseValuesTypeDef,
     PutAlarmRequestRequestTypeDef,
     R53HostedZoneDeletionStateTypeDef,
     RebootInstanceRequestRequestTypeDef,
     RebootRelationalDatabaseRequestRequestTypeDef,
     RegisterContainerImageRequestRequestTypeDef,
     RelationalDatabaseEndpointTypeDef,
     RelationalDatabaseHardwareTypeDef,
     ReleaseStaticIpRequestRequestTypeDef,
     ResetDistributionCacheRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SendContactMethodVerificationRequestRequestTypeDef,
     SetIpAddressTypeRequestRequestTypeDef,
     SetResourceAccessForBucketRequestRequestTypeDef,
     StartGUISessionRequestRequestTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartRelationalDatabaseRequestRequestTypeDef,
     StopGUISessionRequestRequestTypeDef,
@@ -671,21 +698,14 @@
     UpdateRelationalDatabaseRequestRequestTypeDef,
     AccessKeyTypeDef,
     AddOnRequestTypeDef,
     AlarmTypeDef,
     ContactMethodTypeDef,
     OperationTypeDef,
     StaticIpTypeDef,
-    DownloadDefaultKeyPairResultTypeDef,
-    GetActiveNamesResultTypeDef,
-    GetContainerAPIMetadataResultTypeDef,
-    GetDistributionLatestCacheResetResultTypeDef,
-    GetRelationalDatabaseLogStreamsResultTypeDef,
-    GetRelationalDatabaseMasterUserPasswordResultTypeDef,
-    IsVpcPeeredResultTypeDef,
     AutoSnapshotDetailsTypeDef,
     RegionTypeDef,
     GetBlueprintsResultTypeDef,
     UpdateBucketRequestRequestTypeDef,
     GetBucketBundlesResultTypeDef,
     BucketTypeDef,
     CreateBucketRequestRequestTypeDef,
@@ -724,34 +744,14 @@
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
     CreateGUISessionAccessDetailsResultTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
     DomainValidationRecordTypeDef,
     EstimateByTimeTypeDef,
-    GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
-    GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
-    GetBundlesRequestGetBundlesPaginateTypeDef,
-    GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
-    GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
-    GetDisksRequestGetDisksPaginateTypeDef,
-    GetDomainsRequestGetDomainsPaginateTypeDef,
-    GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef,
-    GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef,
-    GetInstancesRequestGetInstancesPaginateTypeDef,
-    GetKeyPairsRequestGetKeyPairsPaginateTypeDef,
-    GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef,
-    GetOperationsRequestGetOperationsPaginateTypeDef,
-    GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef,
-    GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef,
-    GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
-    GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
-    GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
-    GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
-    GetStaticIpsRequestGetStaticIpsPaginateTypeDef,
     GetBucketMetricDataResultTypeDef,
     GetContainerServiceMetricDataResultTypeDef,
     GetDistributionMetricDataResultTypeDef,
     GetInstanceMetricDataResultTypeDef,
     GetLoadBalancerMetricDataResultTypeDef,
     GetRelationalDatabaseMetricDataResultTypeDef,
     GetInstancePortStatesResultTypeDef,
@@ -932,42 +932,42 @@
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

### Comparing `mypy-boto3-lightsail-1.26.81/README.md` & `mypy-boto3-lightsail-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lightsail"></a>
 
 # mypy-boto3-lightsail
 
 [![PyPI - mypy-boto3-lightsail](https://img.shields.io/pypi/v/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lightsail?color=blue)](https://pypistats.org/packages/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -450,15 +450,14 @@
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
     StopInstanceOnIdleRequestTypeDef,
     AddOnTypeDef,
     MonitoredResourceInfoTypeDef,
     ResourceLocationTypeDef,
     AllocateStaticIpRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AttachCertificateToDistributionRequestRequestTypeDef,
     AttachDiskRequestRequestTypeDef,
     AttachInstancesToLoadBalancerRequestRequestTypeDef,
     AttachLoadBalancerTlsCertificateRequestRequestTypeDef,
     AttachStaticIpRequestRequestTypeDef,
     AttachedDiskTypeDef,
     AvailabilityZoneTypeDef,
@@ -521,110 +520,138 @@
     DetachStaticIpRequestRequestTypeDef,
     DisableAddOnRequestRequestTypeDef,
     DiskInfoTypeDef,
     DiskSnapshotInfoTypeDef,
     DistributionBundleTypeDef,
     DnsRecordCreationStateTypeDef,
     ResourceRecordTypeDef,
+    DownloadDefaultKeyPairResultTypeDef,
     TimePeriodTypeDef,
     ExportSnapshotRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
     GetActiveNamesRequestRequestTypeDef,
+    GetActiveNamesResultTypeDef,
     GetAlarmsRequestRequestTypeDef,
     GetAutoSnapshotsRequestRequestTypeDef,
+    GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
     GetBlueprintsRequestRequestTypeDef,
     GetBucketAccessKeysRequestRequestTypeDef,
     GetBucketBundlesRequestRequestTypeDef,
     GetBucketMetricDataRequestRequestTypeDef,
     MetricDatapointTypeDef,
     GetBucketsRequestRequestTypeDef,
+    GetBundlesRequestGetBundlesPaginateTypeDef,
     GetBundlesRequestRequestTypeDef,
     GetCertificatesRequestRequestTypeDef,
+    GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
     GetCloudFormationStackRecordsRequestRequestTypeDef,
     GetContactMethodsRequestRequestTypeDef,
+    GetContainerAPIMetadataResultTypeDef,
     GetContainerImagesRequestRequestTypeDef,
     GetContainerLogRequestRequestTypeDef,
     GetContainerServiceDeploymentsRequestRequestTypeDef,
     GetContainerServiceMetricDataRequestRequestTypeDef,
     GetContainerServicesRequestRequestTypeDef,
     GetCostEstimateRequestRequestTypeDef,
     GetDiskRequestRequestTypeDef,
     GetDiskSnapshotRequestRequestTypeDef,
+    GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
     GetDiskSnapshotsRequestRequestTypeDef,
+    GetDisksRequestGetDisksPaginateTypeDef,
     GetDisksRequestRequestTypeDef,
     GetDistributionLatestCacheResetRequestRequestTypeDef,
+    GetDistributionLatestCacheResetResultTypeDef,
     GetDistributionMetricDataRequestRequestTypeDef,
     GetDistributionsRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
+    GetDomainsRequestGetDomainsPaginateTypeDef,
     GetDomainsRequestRequestTypeDef,
+    GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef,
     GetExportSnapshotRecordsRequestRequestTypeDef,
     GetInstanceAccessDetailsRequestRequestTypeDef,
     GetInstanceMetricDataRequestRequestTypeDef,
     GetInstancePortStatesRequestRequestTypeDef,
     InstancePortStateTypeDef,
     GetInstanceRequestRequestTypeDef,
     GetInstanceSnapshotRequestRequestTypeDef,
+    GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef,
     GetInstanceSnapshotsRequestRequestTypeDef,
     GetInstanceStateRequestRequestTypeDef,
     InstanceStateTypeDef,
+    GetInstancesRequestGetInstancesPaginateTypeDef,
     GetInstancesRequestRequestTypeDef,
     GetKeyPairRequestRequestTypeDef,
+    GetKeyPairsRequestGetKeyPairsPaginateTypeDef,
     GetKeyPairsRequestRequestTypeDef,
     GetLoadBalancerMetricDataRequestRequestTypeDef,
     GetLoadBalancerRequestRequestTypeDef,
     GetLoadBalancerTlsCertificatesRequestRequestTypeDef,
     GetLoadBalancerTlsPoliciesRequestRequestTypeDef,
     LoadBalancerTlsPolicyTypeDef,
+    GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef,
     GetLoadBalancersRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     GetOperationsForResourceRequestRequestTypeDef,
+    GetOperationsRequestGetOperationsPaginateTypeDef,
     GetOperationsRequestRequestTypeDef,
     GetRegionsRequestRequestTypeDef,
+    GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef,
     GetRelationalDatabaseBlueprintsRequestRequestTypeDef,
     RelationalDatabaseBlueprintTypeDef,
+    GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef,
     GetRelationalDatabaseBundlesRequestRequestTypeDef,
     RelationalDatabaseBundleTypeDef,
+    GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
     GetRelationalDatabaseEventsRequestRequestTypeDef,
     RelationalDatabaseEventTypeDef,
     GetRelationalDatabaseLogEventsRequestRequestTypeDef,
     LogEventTypeDef,
     GetRelationalDatabaseLogStreamsRequestRequestTypeDef,
+    GetRelationalDatabaseLogStreamsResultTypeDef,
     GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
+    GetRelationalDatabaseMasterUserPasswordResultTypeDef,
     GetRelationalDatabaseMetricDataRequestRequestTypeDef,
+    GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
     GetRelationalDatabaseParametersRequestRequestTypeDef,
     RelationalDatabaseParameterTypeDef,
     GetRelationalDatabaseRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotRequestRequestTypeDef,
+    GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
     GetRelationalDatabaseSnapshotsRequestRequestTypeDef,
+    GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
     GetRelationalDatabasesRequestRequestTypeDef,
     GetStaticIpRequestRequestTypeDef,
+    GetStaticIpsRequestGetStaticIpsPaginateTypeDef,
     GetStaticIpsRequestRequestTypeDef,
     HostKeyAttributesTypeDef,
     ImportKeyPairRequestRequestTypeDef,
     PasswordDataTypeDef,
     InstanceHealthSummaryTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstancePortInfoTypeDef,
     MonthlyTransferTypeDef,
+    IsVpcPeeredResultTypeDef,
     OriginTypeDef,
     LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef,
     LoadBalancerTlsCertificateDomainValidationOptionTypeDef,
     LoadBalancerTlsCertificateSummaryTypeDef,
     NameServersUpdateStateTypeDef,
+    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PendingModifiedRelationalDatabaseValuesTypeDef,
     PutAlarmRequestRequestTypeDef,
     R53HostedZoneDeletionStateTypeDef,
     RebootInstanceRequestRequestTypeDef,
     RebootRelationalDatabaseRequestRequestTypeDef,
     RegisterContainerImageRequestRequestTypeDef,
     RelationalDatabaseEndpointTypeDef,
     RelationalDatabaseHardwareTypeDef,
     ReleaseStaticIpRequestRequestTypeDef,
     ResetDistributionCacheRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SendContactMethodVerificationRequestRequestTypeDef,
     SetIpAddressTypeRequestRequestTypeDef,
     SetResourceAccessForBucketRequestRequestTypeDef,
     StartGUISessionRequestRequestTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartRelationalDatabaseRequestRequestTypeDef,
     StopGUISessionRequestRequestTypeDef,
@@ -639,21 +666,14 @@
     UpdateRelationalDatabaseRequestRequestTypeDef,
     AccessKeyTypeDef,
     AddOnRequestTypeDef,
     AlarmTypeDef,
     ContactMethodTypeDef,
     OperationTypeDef,
     StaticIpTypeDef,
-    DownloadDefaultKeyPairResultTypeDef,
-    GetActiveNamesResultTypeDef,
-    GetContainerAPIMetadataResultTypeDef,
-    GetDistributionLatestCacheResetResultTypeDef,
-    GetRelationalDatabaseLogStreamsResultTypeDef,
-    GetRelationalDatabaseMasterUserPasswordResultTypeDef,
-    IsVpcPeeredResultTypeDef,
     AutoSnapshotDetailsTypeDef,
     RegionTypeDef,
     GetBlueprintsResultTypeDef,
     UpdateBucketRequestRequestTypeDef,
     GetBucketBundlesResultTypeDef,
     BucketTypeDef,
     CreateBucketRequestRequestTypeDef,
@@ -692,34 +712,14 @@
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
     CreateGUISessionAccessDetailsResultTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
     DomainValidationRecordTypeDef,
     EstimateByTimeTypeDef,
-    GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
-    GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
-    GetBundlesRequestGetBundlesPaginateTypeDef,
-    GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
-    GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
-    GetDisksRequestGetDisksPaginateTypeDef,
-    GetDomainsRequestGetDomainsPaginateTypeDef,
-    GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef,
-    GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef,
-    GetInstancesRequestGetInstancesPaginateTypeDef,
-    GetKeyPairsRequestGetKeyPairsPaginateTypeDef,
-    GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef,
-    GetOperationsRequestGetOperationsPaginateTypeDef,
-    GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef,
-    GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef,
-    GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
-    GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
-    GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
-    GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
-    GetStaticIpsRequestGetStaticIpsPaginateTypeDef,
     GetBucketMetricDataResultTypeDef,
     GetContainerServiceMetricDataResultTypeDef,
     GetDistributionMetricDataResultTypeDef,
     GetInstanceMetricDataResultTypeDef,
     GetLoadBalancerMetricDataResultTypeDef,
     GetRelationalDatabaseMetricDataResultTypeDef,
     GetInstancePortStatesResultTypeDef,
@@ -900,42 +900,42 @@
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

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/__init__.py` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/__init__.pyi` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/__main__.py` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lightsail 1.26.81\nVersion:         1.26.81\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.Lightsail 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.81")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/client.py` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
         availabilityZone: str,
         sizeInGb: int,
         tags: Sequence[TagTypeDef] = ...,
         addOns: Sequence[AddOnRequestTypeDef] = ...
     ) -> CreateDiskResultTypeDef:
         """
         Creates a block storage disk that can be attached to an Amazon Lightsail
-        instance in the same Availability Zone (e.g., `us-east-2a` ).
+        instance in the same Availability Zone (e.g., `us-east-2a`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_disk)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_disk)
         """
 
     def create_disk_from_snapshot(
         self,
@@ -891,15 +891,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#delete_instance)
         """
 
     def delete_instance_snapshot(
         self, *, instanceSnapshotName: str
     ) -> DeleteInstanceSnapshotResultTypeDef:
         """
-        Deletes a specific snapshot of a virtual private server (or *instance* ).
+        Deletes a specific snapshot of a virtual private server (or *instance*).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_instance_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#delete_instance_snapshot)
         """
 
     def delete_key_pair(
         self, *, keyPairName: str, expectedFingerprint: str = ...
@@ -1150,15 +1150,16 @@
         """
 
     def get_certificates(
         self,
         *,
         certificateStatuses: Sequence[CertificateStatusType] = ...,
         includeCertificateDetails: bool = ...,
-        certificateName: str = ...
+        certificateName: str = ...,
+        pageToken: str = ...
     ) -> GetCertificatesResultTypeDef:
         """
         Returns information about one or more Amazon Lightsail SSL/TLS certificates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_certificates)
         """
@@ -1401,15 +1402,15 @@
         """
 
     def get_instance_access_details(
         self, *, instanceName: str, protocol: InstanceAccessProtocolType = ...
     ) -> GetInstanceAccessDetailsResultTypeDef:
         """
         Returns temporary SSH keys you can use to connect to a specific virtual private
-        server, or *instance* .
+        server, or *instance*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_instance_access_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_instance_access_details)
         """
 
     def get_instance_metric_data(
         self,
@@ -1465,15 +1466,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_instance_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_instance_state)
         """
 
     def get_instances(self, *, pageToken: str = ...) -> GetInstancesResultTypeDef:
         """
         Returns information about all Amazon Lightsail virtual private servers, or
-        *instances* .
+        *instances*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_instances)
         """
 
     def get_key_pair(self, *, keyPairName: str) -> GetKeyPairResultTypeDef:
         """
```

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/client.pyi` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -482,15 +482,15 @@
         availabilityZone: str,
         sizeInGb: int,
         tags: Sequence[TagTypeDef] = ...,
         addOns: Sequence[AddOnRequestTypeDef] = ...
     ) -> CreateDiskResultTypeDef:
         """
         Creates a block storage disk that can be attached to an Amazon Lightsail
-        instance in the same Availability Zone (e.g., `us-east-2a` ).
+        instance in the same Availability Zone (e.g., `us-east-2a`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_disk)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_disk)
         """
     def create_disk_from_snapshot(
         self,
         *,
@@ -838,15 +838,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#delete_instance)
         """
     def delete_instance_snapshot(
         self, *, instanceSnapshotName: str
     ) -> DeleteInstanceSnapshotResultTypeDef:
         """
-        Deletes a specific snapshot of a virtual private server (or *instance* ).
+        Deletes a specific snapshot of a virtual private server (or *instance*).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_instance_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#delete_instance_snapshot)
         """
     def delete_key_pair(
         self, *, keyPairName: str, expectedFingerprint: str = ...
     ) -> DeleteKeyPairResultTypeDef:
@@ -1072,15 +1072,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_bundles)
         """
     def get_certificates(
         self,
         *,
         certificateStatuses: Sequence[CertificateStatusType] = ...,
         includeCertificateDetails: bool = ...,
-        certificateName: str = ...
+        certificateName: str = ...,
+        pageToken: str = ...
     ) -> GetCertificatesResultTypeDef:
         """
         Returns information about one or more Amazon Lightsail SSL/TLS certificates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_certificates)
         """
@@ -1300,15 +1301,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_instance)
         """
     def get_instance_access_details(
         self, *, instanceName: str, protocol: InstanceAccessProtocolType = ...
     ) -> GetInstanceAccessDetailsResultTypeDef:
         """
         Returns temporary SSH keys you can use to connect to a specific virtual private
-        server, or *instance* .
+        server, or *instance*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_instance_access_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_instance_access_details)
         """
     def get_instance_metric_data(
         self,
         *,
@@ -1358,15 +1359,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_instance_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_instance_state)
         """
     def get_instances(self, *, pageToken: str = ...) -> GetInstancesResultTypeDef:
         """
         Returns information about all Amazon Lightsail virtual private servers, or
-        *instances* .
+        *instances*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_instances)
         """
     def get_key_pair(self, *, keyPairName: str) -> GetKeyPairResultTypeDef:
         """
         Returns information about a specific key pair.
```

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/literals.py` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,14 +549,15 @@
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
@@ -596,14 +597,15 @@
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
@@ -701,14 +703,15 @@
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
@@ -744,14 +747,15 @@
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
@@ -770,16 +774,19 @@
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
@@ -863,15 +870,17 @@
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

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/literals.pyi` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -547,14 +547,15 @@
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
@@ -594,14 +595,15 @@
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
@@ -699,14 +701,15 @@
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
@@ -742,14 +745,15 @@
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
@@ -768,16 +772,19 @@
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
@@ -861,15 +868,17 @@
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

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/paginator.py` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 class GetActiveNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetActiveNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getactivenamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetActiveNamesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetActiveNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getactivenamespaginator)
         """
 
 
@@ -148,15 +148,15 @@
     """
 
     def paginate(
         self,
         *,
         includeInactive: bool = ...,
         appCategory: Literal["LfR"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBlueprintsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBlueprints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getblueprintspaginator)
         """
 
 
@@ -167,195 +167,195 @@
     """
 
     def paginate(
         self,
         *,
         includeInactive: bool = ...,
         appCategory: Literal["LfR"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getbundlespaginator)
         """
 
 
 class GetCloudFormationStackRecordsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetCloudFormationStackRecords)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getcloudformationstackrecordspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCloudFormationStackRecordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetCloudFormationStackRecords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getcloudformationstackrecordspaginator)
         """
 
 
 class GetDiskSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDiskSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdisksnapshotspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDiskSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDiskSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdisksnapshotspaginator)
         """
 
 
 class GetDisksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDisks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdiskspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDisksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDisks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdiskspaginator)
         """
 
 
 class GetDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdomainspaginator)
         """
 
 
 class GetExportSnapshotRecordsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetExportSnapshotRecords)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getexportsnapshotrecordspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetExportSnapshotRecordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetExportSnapshotRecords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getexportsnapshotrecordspaginator)
         """
 
 
 class GetInstanceSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstanceSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancesnapshotspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetInstanceSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstanceSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancesnapshotspaginator)
         """
 
 
 class GetInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetInstancesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancespaginator)
         """
 
 
 class GetKeyPairsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetKeyPairs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getkeypairspaginator)
     """
 
     def paginate(
-        self, *, includeDefaultKeyPair: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, includeDefaultKeyPair: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetKeyPairsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetKeyPairs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getkeypairspaginator)
         """
 
 
 class GetLoadBalancersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetLoadBalancers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getloadbalancerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetLoadBalancersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getloadbalancerspaginator)
         """
 
 
 class GetOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getoperationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetOperationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getoperationspaginator)
         """
 
 
 class GetRelationalDatabaseBlueprintsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBlueprints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseblueprintspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRelationalDatabaseBlueprintsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBlueprints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseblueprintspaginator)
         """
 
 
 class GetRelationalDatabaseBundlesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBundles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasebundlespaginator)
     """
 
     def paginate(
-        self, *, includeInactive: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, includeInactive: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRelationalDatabaseBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasebundlespaginator)
         """
 
 
@@ -366,73 +366,73 @@
     """
 
     def paginate(
         self,
         *,
         relationalDatabaseName: str,
         durationInMinutes: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRelationalDatabaseEventsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseeventspaginator)
         """
 
 
 class GetRelationalDatabaseParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseparameterspaginator)
     """
 
     def paginate(
-        self, *, relationalDatabaseName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, relationalDatabaseName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRelationalDatabaseParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseparameterspaginator)
         """
 
 
 class GetRelationalDatabaseSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasesnapshotspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRelationalDatabaseSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasesnapshotspaginator)
         """
 
 
 class GetRelationalDatabasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRelationalDatabasesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasespaginator)
         """
 
 
 class GetStaticIpsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetStaticIps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getstaticipspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetStaticIpsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetStaticIps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getstaticipspaginator)
         """
```

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/paginator.pyi` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 class GetActiveNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetActiveNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getactivenamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetActiveNamesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetActiveNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getactivenamespaginator)
         """
 
 class GetBlueprintsPaginator(Paginator):
@@ -143,15 +143,15 @@
     """
 
     def paginate(
         self,
         *,
         includeInactive: bool = ...,
         appCategory: Literal["LfR"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBlueprintsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBlueprints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getblueprintspaginator)
         """
 
 class GetBundlesPaginator(Paginator):
@@ -161,183 +161,183 @@
     """
 
     def paginate(
         self,
         *,
         includeInactive: bool = ...,
         appCategory: Literal["LfR"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getbundlespaginator)
         """
 
 class GetCloudFormationStackRecordsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetCloudFormationStackRecords)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getcloudformationstackrecordspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCloudFormationStackRecordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetCloudFormationStackRecords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getcloudformationstackrecordspaginator)
         """
 
 class GetDiskSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDiskSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdisksnapshotspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDiskSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDiskSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdisksnapshotspaginator)
         """
 
 class GetDisksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDisks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdiskspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDisksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDisks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdiskspaginator)
         """
 
 class GetDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdomainspaginator)
         """
 
 class GetExportSnapshotRecordsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetExportSnapshotRecords)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getexportsnapshotrecordspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetExportSnapshotRecordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetExportSnapshotRecords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getexportsnapshotrecordspaginator)
         """
 
 class GetInstanceSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstanceSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancesnapshotspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetInstanceSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstanceSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancesnapshotspaginator)
         """
 
 class GetInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetInstancesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancespaginator)
         """
 
 class GetKeyPairsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetKeyPairs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getkeypairspaginator)
     """
 
     def paginate(
-        self, *, includeDefaultKeyPair: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, includeDefaultKeyPair: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetKeyPairsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetKeyPairs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getkeypairspaginator)
         """
 
 class GetLoadBalancersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetLoadBalancers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getloadbalancerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetLoadBalancersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getloadbalancerspaginator)
         """
 
 class GetOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getoperationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetOperationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getoperationspaginator)
         """
 
 class GetRelationalDatabaseBlueprintsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBlueprints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseblueprintspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRelationalDatabaseBlueprintsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBlueprints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseblueprintspaginator)
         """
 
 class GetRelationalDatabaseBundlesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBundles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasebundlespaginator)
     """
 
     def paginate(
-        self, *, includeInactive: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, includeInactive: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRelationalDatabaseBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasebundlespaginator)
         """
 
 class GetRelationalDatabaseEventsPaginator(Paginator):
@@ -347,69 +347,69 @@
     """
 
     def paginate(
         self,
         *,
         relationalDatabaseName: str,
         durationInMinutes: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRelationalDatabaseEventsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseeventspaginator)
         """
 
 class GetRelationalDatabaseParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseparameterspaginator)
     """
 
     def paginate(
-        self, *, relationalDatabaseName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, relationalDatabaseName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRelationalDatabaseParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseparameterspaginator)
         """
 
 class GetRelationalDatabaseSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasesnapshotspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRelationalDatabaseSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasesnapshotspaginator)
         """
 
 class GetRelationalDatabasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetRelationalDatabasesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasespaginator)
         """
 
 class GetStaticIpsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetStaticIps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getstaticipspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetStaticIpsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetStaticIps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getstaticipspaginator)
         """
```

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/type_defs.py` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -96,26 +96,24 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessKeyLastUsedTypeDef",
     "AccessRulesTypeDef",
     "AccountLevelBpaSyncTypeDef",
     "AutoSnapshotAddOnRequestTypeDef",
     "StopInstanceOnIdleRequestTypeDef",
     "AddOnTypeDef",
     "MonitoredResourceInfoTypeDef",
     "ResourceLocationTypeDef",
     "AllocateStaticIpRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AttachCertificateToDistributionRequestRequestTypeDef",
     "AttachDiskRequestRequestTypeDef",
     "AttachInstancesToLoadBalancerRequestRequestTypeDef",
     "AttachLoadBalancerTlsCertificateRequestRequestTypeDef",
     "AttachStaticIpRequestRequestTypeDef",
     "AttachedDiskTypeDef",
     "AvailabilityZoneTypeDef",
@@ -178,110 +176,138 @@
     "DetachStaticIpRequestRequestTypeDef",
     "DisableAddOnRequestRequestTypeDef",
     "DiskInfoTypeDef",
     "DiskSnapshotInfoTypeDef",
     "DistributionBundleTypeDef",
     "DnsRecordCreationStateTypeDef",
     "ResourceRecordTypeDef",
+    "DownloadDefaultKeyPairResultTypeDef",
     "TimePeriodTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     "GetActiveNamesRequestRequestTypeDef",
+    "GetActiveNamesResultTypeDef",
     "GetAlarmsRequestRequestTypeDef",
     "GetAutoSnapshotsRequestRequestTypeDef",
+    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     "GetBlueprintsRequestRequestTypeDef",
     "GetBucketAccessKeysRequestRequestTypeDef",
     "GetBucketBundlesRequestRequestTypeDef",
     "GetBucketMetricDataRequestRequestTypeDef",
     "MetricDatapointTypeDef",
     "GetBucketsRequestRequestTypeDef",
+    "GetBundlesRequestGetBundlesPaginateTypeDef",
     "GetBundlesRequestRequestTypeDef",
     "GetCertificatesRequestRequestTypeDef",
+    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
     "GetCloudFormationStackRecordsRequestRequestTypeDef",
     "GetContactMethodsRequestRequestTypeDef",
+    "GetContainerAPIMetadataResultTypeDef",
     "GetContainerImagesRequestRequestTypeDef",
     "GetContainerLogRequestRequestTypeDef",
     "GetContainerServiceDeploymentsRequestRequestTypeDef",
     "GetContainerServiceMetricDataRequestRequestTypeDef",
     "GetContainerServicesRequestRequestTypeDef",
     "GetCostEstimateRequestRequestTypeDef",
     "GetDiskRequestRequestTypeDef",
     "GetDiskSnapshotRequestRequestTypeDef",
+    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
     "GetDiskSnapshotsRequestRequestTypeDef",
+    "GetDisksRequestGetDisksPaginateTypeDef",
     "GetDisksRequestRequestTypeDef",
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
+    "GetDistributionLatestCacheResetResultTypeDef",
     "GetDistributionMetricDataRequestRequestTypeDef",
     "GetDistributionsRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
+    "GetDomainsRequestGetDomainsPaginateTypeDef",
     "GetDomainsRequestRequestTypeDef",
+    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
     "GetExportSnapshotRecordsRequestRequestTypeDef",
     "GetInstanceAccessDetailsRequestRequestTypeDef",
     "GetInstanceMetricDataRequestRequestTypeDef",
     "GetInstancePortStatesRequestRequestTypeDef",
     "InstancePortStateTypeDef",
     "GetInstanceRequestRequestTypeDef",
     "GetInstanceSnapshotRequestRequestTypeDef",
+    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
     "GetInstanceSnapshotsRequestRequestTypeDef",
     "GetInstanceStateRequestRequestTypeDef",
     "InstanceStateTypeDef",
+    "GetInstancesRequestGetInstancesPaginateTypeDef",
     "GetInstancesRequestRequestTypeDef",
     "GetKeyPairRequestRequestTypeDef",
+    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
     "GetKeyPairsRequestRequestTypeDef",
     "GetLoadBalancerMetricDataRequestRequestTypeDef",
     "GetLoadBalancerRequestRequestTypeDef",
     "GetLoadBalancerTlsCertificatesRequestRequestTypeDef",
     "GetLoadBalancerTlsPoliciesRequestRequestTypeDef",
     "LoadBalancerTlsPolicyTypeDef",
+    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
     "GetLoadBalancersRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "GetOperationsForResourceRequestRequestTypeDef",
+    "GetOperationsRequestGetOperationsPaginateTypeDef",
     "GetOperationsRequestRequestTypeDef",
     "GetRegionsRequestRequestTypeDef",
+    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
     "GetRelationalDatabaseBlueprintsRequestRequestTypeDef",
     "RelationalDatabaseBlueprintTypeDef",
+    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
     "GetRelationalDatabaseBundlesRequestRequestTypeDef",
     "RelationalDatabaseBundleTypeDef",
+    "GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
     "GetRelationalDatabaseEventsRequestRequestTypeDef",
     "RelationalDatabaseEventTypeDef",
     "GetRelationalDatabaseLogEventsRequestRequestTypeDef",
     "LogEventTypeDef",
     "GetRelationalDatabaseLogStreamsRequestRequestTypeDef",
+    "GetRelationalDatabaseLogStreamsResultTypeDef",
     "GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
+    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
     "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
+    "GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
     "GetRelationalDatabaseParametersRequestRequestTypeDef",
     "RelationalDatabaseParameterTypeDef",
     "GetRelationalDatabaseRequestRequestTypeDef",
     "GetRelationalDatabaseSnapshotRequestRequestTypeDef",
+    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
     "GetRelationalDatabaseSnapshotsRequestRequestTypeDef",
+    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
     "GetRelationalDatabasesRequestRequestTypeDef",
     "GetStaticIpRequestRequestTypeDef",
+    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
     "GetStaticIpsRequestRequestTypeDef",
     "HostKeyAttributesTypeDef",
     "ImportKeyPairRequestRequestTypeDef",
     "PasswordDataTypeDef",
     "InstanceHealthSummaryTypeDef",
     "InstanceMetadataOptionsTypeDef",
     "InstancePortInfoTypeDef",
     "MonthlyTransferTypeDef",
+    "IsVpcPeeredResultTypeDef",
     "OriginTypeDef",
     "LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef",
     "LoadBalancerTlsCertificateDomainValidationOptionTypeDef",
     "LoadBalancerTlsCertificateSummaryTypeDef",
     "NameServersUpdateStateTypeDef",
+    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PendingModifiedRelationalDatabaseValuesTypeDef",
     "PutAlarmRequestRequestTypeDef",
     "R53HostedZoneDeletionStateTypeDef",
     "RebootInstanceRequestRequestTypeDef",
     "RebootRelationalDatabaseRequestRequestTypeDef",
     "RegisterContainerImageRequestRequestTypeDef",
     "RelationalDatabaseEndpointTypeDef",
     "RelationalDatabaseHardwareTypeDef",
     "ReleaseStaticIpRequestRequestTypeDef",
     "ResetDistributionCacheRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SendContactMethodVerificationRequestRequestTypeDef",
     "SetIpAddressTypeRequestRequestTypeDef",
     "SetResourceAccessForBucketRequestRequestTypeDef",
     "StartGUISessionRequestRequestTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartRelationalDatabaseRequestRequestTypeDef",
     "StopGUISessionRequestRequestTypeDef",
@@ -296,21 +322,14 @@
     "UpdateRelationalDatabaseRequestRequestTypeDef",
     "AccessKeyTypeDef",
     "AddOnRequestTypeDef",
     "AlarmTypeDef",
     "ContactMethodTypeDef",
     "OperationTypeDef",
     "StaticIpTypeDef",
-    "DownloadDefaultKeyPairResultTypeDef",
-    "GetActiveNamesResultTypeDef",
-    "GetContainerAPIMetadataResultTypeDef",
-    "GetDistributionLatestCacheResetResultTypeDef",
-    "GetRelationalDatabaseLogStreamsResultTypeDef",
-    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
-    "IsVpcPeeredResultTypeDef",
     "AutoSnapshotDetailsTypeDef",
     "RegionTypeDef",
     "GetBlueprintsResultTypeDef",
     "UpdateBucketRequestRequestTypeDef",
     "GetBucketBundlesResultTypeDef",
     "BucketTypeDef",
     "CreateBucketRequestRequestTypeDef",
@@ -349,34 +368,14 @@
     "DeleteDomainEntryRequestRequestTypeDef",
     "UpdateDomainEntryRequestRequestTypeDef",
     "CreateGUISessionAccessDetailsResultTypeDef",
     "InstanceSnapshotInfoTypeDef",
     "GetDistributionBundlesResultTypeDef",
     "DomainValidationRecordTypeDef",
     "EstimateByTimeTypeDef",
-    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
-    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
-    "GetBundlesRequestGetBundlesPaginateTypeDef",
-    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
-    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
-    "GetDisksRequestGetDisksPaginateTypeDef",
-    "GetDomainsRequestGetDomainsPaginateTypeDef",
-    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
-    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
-    "GetInstancesRequestGetInstancesPaginateTypeDef",
-    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
-    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
-    "GetOperationsRequestGetOperationsPaginateTypeDef",
-    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
-    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
-    "GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
-    "GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
-    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
-    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
-    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
     "GetBucketMetricDataResultTypeDef",
     "GetContainerServiceMetricDataResultTypeDef",
     "GetDistributionMetricDataResultTypeDef",
     "GetInstanceMetricDataResultTypeDef",
     "GetLoadBalancerMetricDataResultTypeDef",
     "GetRelationalDatabaseMetricDataResultTypeDef",
     "GetInstancePortStatesResultTypeDef",
@@ -631,25 +630,14 @@
 AllocateStaticIpRequestRequestTypeDef = TypedDict(
     "AllocateStaticIpRequestRequestTypeDef",
     {
         "staticIpName": str,
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
 AttachCertificateToDistributionRequestRequestTypeDef = TypedDict(
     "AttachCertificateToDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "certificateName": str,
     },
 )
@@ -666,21 +654,19 @@
     "_OptionalAttachDiskRequestRequestTypeDef",
     {
         "autoMounting": bool,
     },
     total=False,
 )
 
-
 class AttachDiskRequestRequestTypeDef(
     _RequiredAttachDiskRequestRequestTypeDef, _OptionalAttachDiskRequestRequestTypeDef
 ):
     pass
 
-
 AttachInstancesToLoadBalancerRequestRequestTypeDef = TypedDict(
     "AttachInstancesToLoadBalancerRequestRequestTypeDef",
     {
         "loadBalancerName": str,
         "instanceNames": Sequence[str],
     },
 )
@@ -750,21 +736,19 @@
     {
         "destination": str,
         "prefix": str,
     },
     total=False,
 )
 
-
 class BucketAccessLogConfigTypeDef(
     _RequiredBucketAccessLogConfigTypeDef, _OptionalBucketAccessLogConfigTypeDef
 ):
     pass
 
-
 BucketBundleTypeDef = TypedDict(
     "BucketBundleTypeDef",
     {
         "bundleId": str,
         "name": str,
         "price": float,
         "storagePerMonthInGb": int,
@@ -1003,21 +987,19 @@
         "sourceResourceName": str,
         "restoreDate": str,
         "useLatestRestorableAutoSnapshot": bool,
     },
     total=False,
 )
 
-
 class CopySnapshotRequestRequestTypeDef(
     _RequiredCopySnapshotRequestRequestTypeDef, _OptionalCopySnapshotRequestRequestTypeDef
 ):
     pass
 
-
 CreateBucketAccessKeyRequestRequestTypeDef = TypedDict(
     "CreateBucketAccessKeyRequestRequestTypeDef",
     {
         "bucketName": str,
     },
 )
 
@@ -1034,19 +1016,17 @@
     "_OptionalInstanceEntryTypeDef",
     {
         "userData": str,
     },
     total=False,
 )
 
-
 class InstanceEntryTypeDef(_RequiredInstanceEntryTypeDef, _OptionalInstanceEntryTypeDef):
     pass
 
-
 CreateContactMethodRequestRequestTypeDef = TypedDict(
     "CreateContactMethodRequestRequestTypeDef",
     {
         "protocol": ContactProtocolType,
         "contactEndpoint": str,
     },
 )
@@ -1133,21 +1113,19 @@
     "_OptionalDeleteBucketRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
-
 class DeleteBucketRequestRequestTypeDef(
     _RequiredDeleteBucketRequestRequestTypeDef, _OptionalDeleteBucketRequestRequestTypeDef
 ):
     pass
 
-
 DeleteCertificateRequestRequestTypeDef = TypedDict(
     "DeleteCertificateRequestRequestTypeDef",
     {
         "certificateName": str,
     },
 )
 
@@ -1183,21 +1161,19 @@
     "_OptionalDeleteDiskRequestRequestTypeDef",
     {
         "forceDeleteAddOns": bool,
     },
     total=False,
 )
 
-
 class DeleteDiskRequestRequestTypeDef(
     _RequiredDeleteDiskRequestRequestTypeDef, _OptionalDeleteDiskRequestRequestTypeDef
 ):
     pass
 
-
 DeleteDiskSnapshotRequestRequestTypeDef = TypedDict(
     "DeleteDiskSnapshotRequestRequestTypeDef",
     {
         "diskSnapshotName": str,
     },
 )
 
@@ -1226,21 +1202,19 @@
     "_OptionalDeleteInstanceRequestRequestTypeDef",
     {
         "forceDeleteAddOns": bool,
     },
     total=False,
 )
 
-
 class DeleteInstanceRequestRequestTypeDef(
     _RequiredDeleteInstanceRequestRequestTypeDef, _OptionalDeleteInstanceRequestRequestTypeDef
 ):
     pass
 
-
 DeleteInstanceSnapshotRequestRequestTypeDef = TypedDict(
     "DeleteInstanceSnapshotRequestRequestTypeDef",
     {
         "instanceSnapshotName": str,
     },
 )
 
@@ -1254,21 +1228,19 @@
     "_OptionalDeleteKeyPairRequestRequestTypeDef",
     {
         "expectedFingerprint": str,
     },
     total=False,
 )
 
-
 class DeleteKeyPairRequestRequestTypeDef(
     _RequiredDeleteKeyPairRequestRequestTypeDef, _OptionalDeleteKeyPairRequestRequestTypeDef
 ):
     pass
 
-
 DeleteKnownHostKeysRequestRequestTypeDef = TypedDict(
     "DeleteKnownHostKeysRequestRequestTypeDef",
     {
         "instanceName": str,
     },
 )
 
@@ -1290,22 +1262,20 @@
     "_OptionalDeleteLoadBalancerTlsCertificateRequestRequestTypeDef",
     {
         "force": bool,
     },
     total=False,
 )
 
-
 class DeleteLoadBalancerTlsCertificateRequestRequestTypeDef(
     _RequiredDeleteLoadBalancerTlsCertificateRequestRequestTypeDef,
     _OptionalDeleteLoadBalancerTlsCertificateRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteRelationalDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRelationalDatabaseRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalDeleteRelationalDatabaseRequestRequestTypeDef = TypedDict(
@@ -1313,22 +1283,20 @@
     {
         "skipFinalSnapshot": bool,
         "finalRelationalDatabaseSnapshotName": str,
     },
     total=False,
 )
 
-
 class DeleteRelationalDatabaseRequestRequestTypeDef(
     _RequiredDeleteRelationalDatabaseRequestRequestTypeDef,
     _OptionalDeleteRelationalDatabaseRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteRelationalDatabaseSnapshotRequestRequestTypeDef = TypedDict(
     "DeleteRelationalDatabaseSnapshotRequestRequestTypeDef",
     {
         "relationalDatabaseSnapshotName": str,
     },
 )
 
@@ -1415,14 +1383,24 @@
         "name": str,
         "type": str,
         "value": str,
     },
     total=False,
 )
 
+DownloadDefaultKeyPairResultTypeDef = TypedDict(
+    "DownloadDefaultKeyPairResultTypeDef",
+    {
+        "publicKeyBase64": str,
+        "privateKeyBase64": str,
+        "createdAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimePeriodTypeDef = TypedDict(
     "TimePeriodTypeDef",
     {
         "start": datetime,
         "end": datetime,
     },
     total=False,
@@ -1431,32 +1409,39 @@
 ExportSnapshotRequestRequestTypeDef = TypedDict(
     "ExportSnapshotRequestRequestTypeDef",
     {
         "sourceSnapshotName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetActiveNamesRequestGetActiveNamesPaginateTypeDef = TypedDict(
+    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetActiveNamesRequestRequestTypeDef = TypedDict(
     "GetActiveNamesRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
+GetActiveNamesResultTypeDef = TypedDict(
+    "GetActiveNamesResultTypeDef",
+    {
+        "activeNames": List[str],
+        "nextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAlarmsRequestRequestTypeDef = TypedDict(
     "GetAlarmsRequestRequestTypeDef",
     {
         "alarmName": str,
         "pageToken": str,
         "monitoredResourceName": str,
     },
@@ -1466,14 +1451,24 @@
 GetAutoSnapshotsRequestRequestTypeDef = TypedDict(
     "GetAutoSnapshotsRequestRequestTypeDef",
     {
         "resourceName": str,
     },
 )
 
+GetBlueprintsRequestGetBlueprintsPaginateTypeDef = TypedDict(
+    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
+    {
+        "includeInactive": bool,
+        "appCategory": Literal["LfR"],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetBlueprintsRequestRequestTypeDef = TypedDict(
     "GetBlueprintsRequestRequestTypeDef",
     {
         "includeInactive": bool,
         "pageToken": str,
         "appCategory": Literal["LfR"],
     },
@@ -1528,14 +1523,24 @@
         "bucketName": str,
         "pageToken": str,
         "includeConnectedResources": bool,
     },
     total=False,
 )
 
+GetBundlesRequestGetBundlesPaginateTypeDef = TypedDict(
+    "GetBundlesRequestGetBundlesPaginateTypeDef",
+    {
+        "includeInactive": bool,
+        "appCategory": Literal["LfR"],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetBundlesRequestRequestTypeDef = TypedDict(
     "GetBundlesRequestRequestTypeDef",
     {
         "includeInactive": bool,
         "pageToken": str,
         "appCategory": Literal["LfR"],
     },
@@ -1544,14 +1549,23 @@
 
 GetCertificatesRequestRequestTypeDef = TypedDict(
     "GetCertificatesRequestRequestTypeDef",
     {
         "certificateStatuses": Sequence[CertificateStatusType],
         "includeCertificateDetails": bool,
         "certificateName": str,
+        "pageToken": str,
+    },
+    total=False,
+)
+
+GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef = TypedDict(
+    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetCloudFormationStackRecordsRequestRequestTypeDef = TypedDict(
     "GetCloudFormationStackRecordsRequestRequestTypeDef",
     {
@@ -1564,14 +1578,22 @@
     "GetContactMethodsRequestRequestTypeDef",
     {
         "protocols": Sequence[ContactProtocolType],
     },
     total=False,
 )
 
+GetContainerAPIMetadataResultTypeDef = TypedDict(
+    "GetContainerAPIMetadataResultTypeDef",
+    {
+        "metadata": List[Dict[str, str]],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetContainerImagesRequestRequestTypeDef = TypedDict(
     "GetContainerImagesRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
@@ -1589,21 +1611,19 @@
         "endTime": Union[datetime, str],
         "filterPattern": str,
         "pageToken": str,
     },
     total=False,
 )
 
-
 class GetContainerLogRequestRequestTypeDef(
     _RequiredGetContainerLogRequestRequestTypeDef, _OptionalGetContainerLogRequestRequestTypeDef
 ):
     pass
 
-
 GetContainerServiceDeploymentsRequestRequestTypeDef = TypedDict(
     "GetContainerServiceDeploymentsRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
@@ -1646,22 +1666,38 @@
 GetDiskSnapshotRequestRequestTypeDef = TypedDict(
     "GetDiskSnapshotRequestRequestTypeDef",
     {
         "diskSnapshotName": str,
     },
 )
 
+GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef = TypedDict(
+    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetDiskSnapshotsRequestRequestTypeDef = TypedDict(
     "GetDiskSnapshotsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
+GetDisksRequestGetDisksPaginateTypeDef = TypedDict(
+    "GetDisksRequestGetDisksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetDisksRequestRequestTypeDef = TypedDict(
     "GetDisksRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1670,14 +1706,23 @@
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
     {
         "distributionName": str,
     },
     total=False,
 )
 
+GetDistributionLatestCacheResetResultTypeDef = TypedDict(
+    "GetDistributionLatestCacheResetResultTypeDef",
+    {
+        "status": str,
+        "createTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDistributionMetricDataRequestRequestTypeDef = TypedDict(
     "GetDistributionMetricDataRequestRequestTypeDef",
     {
         "distributionName": str,
         "metricName": DistributionMetricNameType,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
@@ -1699,22 +1744,38 @@
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 
+GetDomainsRequestGetDomainsPaginateTypeDef = TypedDict(
+    "GetDomainsRequestGetDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetDomainsRequestRequestTypeDef = TypedDict(
     "GetDomainsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
+GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef = TypedDict(
+    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetExportSnapshotRecordsRequestRequestTypeDef = TypedDict(
     "GetExportSnapshotRecordsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1729,22 +1790,20 @@
     "_OptionalGetInstanceAccessDetailsRequestRequestTypeDef",
     {
         "protocol": InstanceAccessProtocolType,
     },
     total=False,
 )
 
-
 class GetInstanceAccessDetailsRequestRequestTypeDef(
     _RequiredGetInstanceAccessDetailsRequestRequestTypeDef,
     _OptionalGetInstanceAccessDetailsRequestRequestTypeDef,
 ):
     pass
 
-
 GetInstanceMetricDataRequestRequestTypeDef = TypedDict(
     "GetInstanceMetricDataRequestRequestTypeDef",
     {
         "instanceName": str,
         "metricName": InstanceMetricNameType,
         "period": int,
         "startTime": Union[datetime, str],
@@ -1785,14 +1844,22 @@
 GetInstanceSnapshotRequestRequestTypeDef = TypedDict(
     "GetInstanceSnapshotRequestRequestTypeDef",
     {
         "instanceSnapshotName": str,
     },
 )
 
+GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef = TypedDict(
+    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetInstanceSnapshotsRequestRequestTypeDef = TypedDict(
     "GetInstanceSnapshotsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1809,14 +1876,22 @@
     {
         "code": int,
         "name": str,
     },
     total=False,
 )
 
+GetInstancesRequestGetInstancesPaginateTypeDef = TypedDict(
+    "GetInstancesRequestGetInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetInstancesRequestRequestTypeDef = TypedDict(
     "GetInstancesRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1824,14 +1899,23 @@
 GetKeyPairRequestRequestTypeDef = TypedDict(
     "GetKeyPairRequestRequestTypeDef",
     {
         "keyPairName": str,
     },
 )
 
+GetKeyPairsRequestGetKeyPairsPaginateTypeDef = TypedDict(
+    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
+    {
+        "includeDefaultKeyPair": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetKeyPairsRequestRequestTypeDef = TypedDict(
     "GetKeyPairsRequestRequestTypeDef",
     {
         "pageToken": str,
         "includeDefaultKeyPair": bool,
     },
     total=False,
@@ -1880,14 +1964,22 @@
         "description": str,
         "protocols": List[str],
         "ciphers": List[str],
     },
     total=False,
 )
 
+GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef = TypedDict(
+    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetLoadBalancersRequestRequestTypeDef = TypedDict(
     "GetLoadBalancersRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1909,21 +2001,27 @@
     "_OptionalGetOperationsForResourceRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
-
 class GetOperationsForResourceRequestRequestTypeDef(
     _RequiredGetOperationsForResourceRequestRequestTypeDef,
     _OptionalGetOperationsForResourceRequestRequestTypeDef,
 ):
     pass
 
+GetOperationsRequestGetOperationsPaginateTypeDef = TypedDict(
+    "GetOperationsRequestGetOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 GetOperationsRequestRequestTypeDef = TypedDict(
     "GetOperationsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
@@ -1934,14 +2032,22 @@
     {
         "includeAvailabilityZones": bool,
         "includeRelationalDatabaseAvailabilityZones": bool,
     },
     total=False,
 )
 
+GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef = TypedDict(
+    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetRelationalDatabaseBlueprintsRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseBlueprintsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1955,14 +2061,23 @@
         "engineDescription": str,
         "engineVersionDescription": str,
         "isEngineDefault": bool,
     },
     total=False,
 )
 
+GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef = TypedDict(
+    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
+    {
+        "includeInactive": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetRelationalDatabaseBundlesRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseBundlesRequestRequestTypeDef",
     {
         "pageToken": str,
         "includeInactive": bool,
     },
     total=False,
@@ -1980,14 +2095,35 @@
         "cpuCount": int,
         "isEncrypted": bool,
         "isActive": bool,
     },
     total=False,
 )
 
+_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
+    "_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
+    {
+        "relationalDatabaseName": str,
+    },
+)
+_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
+    "_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
+    {
+        "durationInMinutes": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef(
+    _RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
+    _OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetRelationalDatabaseEventsRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseEventsRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseEventsRequestRequestTypeDef = TypedDict(
@@ -1995,22 +2131,20 @@
     {
         "durationInMinutes": int,
         "pageToken": str,
     },
     total=False,
 )
 
-
 class GetRelationalDatabaseEventsRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseEventsRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseEventsRequestRequestTypeDef,
 ):
     pass
 
-
 RelationalDatabaseEventTypeDef = TypedDict(
     "RelationalDatabaseEventTypeDef",
     {
         "resource": str,
         "createdAt": datetime,
         "message": str,
         "eventCategories": List[str],
@@ -2032,22 +2166,20 @@
         "endTime": Union[datetime, str],
         "startFromHead": bool,
         "pageToken": str,
     },
     total=False,
 )
 
-
 class GetRelationalDatabaseLogEventsRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef,
 ):
     pass
 
-
 LogEventTypeDef = TypedDict(
     "LogEventTypeDef",
     {
         "createdAt": datetime,
         "message": str,
     },
     total=False,
@@ -2056,71 +2188,104 @@
 GetRelationalDatabaseLogStreamsRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseLogStreamsRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 
+GetRelationalDatabaseLogStreamsResultTypeDef = TypedDict(
+    "GetRelationalDatabaseLogStreamsResultTypeDef",
+    {
+        "logStreams": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef = TypedDict(
     "_OptionalGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
     {
         "passwordVersion": RelationalDatabasePasswordVersionType,
     },
     total=False,
 )
 
-
 class GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
 ):
     pass
 
+GetRelationalDatabaseMasterUserPasswordResultTypeDef = TypedDict(
+    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
+    {
+        "masterUserPassword": str,
+        "createdAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 GetRelationalDatabaseMetricDataRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
         "metricName": RelationalDatabaseMetricNameType,
         "period": int,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
         "unit": MetricUnitType,
         "statistics": Sequence[MetricStatisticType],
     },
 )
 
+_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
+    "_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
+    {
+        "relationalDatabaseName": str,
+    },
+)
+_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
+    "_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef(
+    _RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
+    _OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
+):
+    pass
+
 _RequiredGetRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseParametersRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
     "_OptionalGetRelationalDatabaseParametersRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
-
 class GetRelationalDatabaseParametersRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseParametersRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseParametersRequestRequestTypeDef,
 ):
     pass
 
-
 RelationalDatabaseParameterTypeDef = TypedDict(
     "RelationalDatabaseParameterTypeDef",
     {
         "allowedValues": str,
         "applyMethod": str,
         "applyType": str,
         "dataType": str,
@@ -2142,22 +2307,38 @@
 GetRelationalDatabaseSnapshotRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotRequestRequestTypeDef",
     {
         "relationalDatabaseSnapshotName": str,
     },
 )
 
+GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef = TypedDict(
+    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetRelationalDatabaseSnapshotsRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
+GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef = TypedDict(
+    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetRelationalDatabasesRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabasesRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2165,14 +2346,22 @@
 GetStaticIpRequestRequestTypeDef = TypedDict(
     "GetStaticIpRequestRequestTypeDef",
     {
         "staticIpName": str,
     },
 )
 
+GetStaticIpsRequestGetStaticIpsPaginateTypeDef = TypedDict(
+    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetStaticIpsRequestRequestTypeDef = TypedDict(
     "GetStaticIpsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2251,14 +2440,22 @@
     "MonthlyTransferTypeDef",
     {
         "gbPerMonthAllocated": int,
     },
     total=False,
 )
 
+IsVpcPeeredResultTypeDef = TypedDict(
+    "IsVpcPeeredResultTypeDef",
+    {
+        "isPeered": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OriginTypeDef = TypedDict(
     "OriginTypeDef",
     {
         "name": str,
         "resourceType": ResourceTypeType,
         "regionName": RegionNameType,
         "protocolPolicy": OriginProtocolPolicyEnumType,
@@ -2298,14 +2495,24 @@
     {
         "code": NameServersUpdateStateCodeType,
         "message": str,
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "action": str,
         "description": str,
         "currentApplyDate": datetime,
     },
@@ -2341,21 +2548,19 @@
         "contactProtocols": Sequence[ContactProtocolType],
         "notificationTriggers": Sequence[AlarmStateType],
         "notificationEnabled": bool,
     },
     total=False,
 )
 
-
 class PutAlarmRequestRequestTypeDef(
     _RequiredPutAlarmRequestRequestTypeDef, _OptionalPutAlarmRequestRequestTypeDef
 ):
     pass
 
-
 R53HostedZoneDeletionStateTypeDef = TypedDict(
     "R53HostedZoneDeletionStateTypeDef",
     {
         "code": R53HostedZoneDeletionStateCodeType,
         "message": str,
     },
     total=False,
@@ -2414,14 +2619,25 @@
     "ResetDistributionCacheRequestRequestTypeDef",
     {
         "distributionName": str,
     },
     total=False,
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
 SendContactMethodVerificationRequestRequestTypeDef = TypedDict(
     "SendContactMethodVerificationRequestRequestTypeDef",
     {
         "protocol": Literal["Email"],
     },
 )
 
@@ -2481,43 +2697,39 @@
     "_OptionalStopInstanceRequestRequestTypeDef",
     {
         "force": bool,
     },
     total=False,
 )
 
-
 class StopInstanceRequestRequestTypeDef(
     _RequiredStopInstanceRequestRequestTypeDef, _OptionalStopInstanceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStopRelationalDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredStopRelationalDatabaseRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalStopRelationalDatabaseRequestRequestTypeDef = TypedDict(
     "_OptionalStopRelationalDatabaseRequestRequestTypeDef",
     {
         "relationalDatabaseSnapshotName": str,
     },
     total=False,
 )
 
-
 class StopRelationalDatabaseRequestRequestTypeDef(
     _RequiredStopRelationalDatabaseRequestRequestTypeDef,
     _OptionalStopRelationalDatabaseRequestRequestTypeDef,
 ):
     pass
 
-
 TestAlarmRequestRequestTypeDef = TypedDict(
     "TestAlarmRequestRequestTypeDef",
     {
         "alarmName": str,
         "state": AlarmStateType,
     },
 )
@@ -2533,21 +2745,19 @@
     "_OptionalUntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
     total=False,
 )
 
-
 class UntagResourceRequestRequestTypeDef(
     _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
 ):
     pass
 
-
 UpdateBucketBundleRequestRequestTypeDef = TypedDict(
     "UpdateBucketBundleRequestRequestTypeDef",
     {
         "bucketName": str,
         "bundleId": str,
     },
 )
@@ -2574,22 +2784,20 @@
         "httpEndpoint": HttpEndpointType,
         "httpPutResponseHopLimit": int,
         "httpProtocolIpv6": HttpProtocolIpv6Type,
     },
     total=False,
 )
 
-
 class UpdateInstanceMetadataOptionsRequestRequestTypeDef(
     _RequiredUpdateInstanceMetadataOptionsRequestRequestTypeDef,
     _OptionalUpdateInstanceMetadataOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateLoadBalancerAttributeRequestRequestTypeDef = TypedDict(
     "UpdateLoadBalancerAttributeRequestRequestTypeDef",
     {
         "loadBalancerName": str,
         "attributeName": LoadBalancerAttributeNameType,
         "attributeValue": str,
     },
@@ -2613,22 +2821,20 @@
         "publiclyAccessible": bool,
         "applyImmediately": bool,
         "caCertificateIdentifier": str,
     },
     total=False,
 )
 
-
 class UpdateRelationalDatabaseRequestRequestTypeDef(
     _RequiredUpdateRelationalDatabaseRequestRequestTypeDef,
     _OptionalUpdateRelationalDatabaseRequestRequestTypeDef,
 ):
     pass
 
-
 AccessKeyTypeDef = TypedDict(
     "AccessKeyTypeDef",
     {
         "accessKeyId": str,
         "secretAccessKey": str,
         "status": StatusTypeType,
         "createdAt": datetime,
@@ -2648,19 +2854,17 @@
     {
         "autoSnapshotAddOnRequest": AutoSnapshotAddOnRequestTypeDef,
         "stopInstanceOnIdleRequest": StopInstanceOnIdleRequestTypeDef,
     },
     total=False,
 )
 
-
 class AddOnRequestTypeDef(_RequiredAddOnRequestTypeDef, _OptionalAddOnRequestTypeDef):
     pass
 
-
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "name": str,
         "arn": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
@@ -2731,75 +2935,14 @@
         "ipAddress": str,
         "attachedTo": str,
         "isAttached": bool,
     },
     total=False,
 )
 
-DownloadDefaultKeyPairResultTypeDef = TypedDict(
-    "DownloadDefaultKeyPairResultTypeDef",
-    {
-        "publicKeyBase64": str,
-        "privateKeyBase64": str,
-        "createdAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetActiveNamesResultTypeDef = TypedDict(
-    "GetActiveNamesResultTypeDef",
-    {
-        "activeNames": List[str],
-        "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetContainerAPIMetadataResultTypeDef = TypedDict(
-    "GetContainerAPIMetadataResultTypeDef",
-    {
-        "metadata": List[Dict[str, str]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDistributionLatestCacheResetResultTypeDef = TypedDict(
-    "GetDistributionLatestCacheResetResultTypeDef",
-    {
-        "status": str,
-        "createTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRelationalDatabaseLogStreamsResultTypeDef = TypedDict(
-    "GetRelationalDatabaseLogStreamsResultTypeDef",
-    {
-        "logStreams": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRelationalDatabaseMasterUserPasswordResultTypeDef = TypedDict(
-    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
-    {
-        "masterUserPassword": str,
-        "createdAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-IsVpcPeeredResultTypeDef = TypedDict(
-    "IsVpcPeeredResultTypeDef",
-    {
-        "isPeered": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AutoSnapshotDetailsTypeDef = TypedDict(
     "AutoSnapshotDetailsTypeDef",
     {
         "date": str,
         "createdAt": datetime,
         "status": AutoSnapshotStatusType,
         "fromAttachedDisks": List[AttachedDiskTypeDef],
@@ -2821,15 +2964,15 @@
 )
 
 GetBlueprintsResultTypeDef = TypedDict(
     "GetBlueprintsResultTypeDef",
     {
         "blueprints": List[BlueprintTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateBucketRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBucketRequestRequestTypeDef",
     {
         "bucketName": str,
@@ -2842,26 +2985,24 @@
         "versioning": str,
         "readonlyAccessAccounts": Sequence[str],
         "accessLogConfig": BucketAccessLogConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateBucketRequestRequestTypeDef(
     _RequiredUpdateBucketRequestRequestTypeDef, _OptionalUpdateBucketRequestRequestTypeDef
 ):
     pass
 
-
 GetBucketBundlesResultTypeDef = TypedDict(
     "GetBucketBundlesResultTypeDef",
     {
         "bundles": List[BucketBundleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "resourceType": str,
@@ -2896,21 +3037,19 @@
     {
         "tags": Sequence[TagTypeDef],
         "enableObjectVersioning": bool,
     },
     total=False,
 )
 
-
 class CreateBucketRequestRequestTypeDef(
     _RequiredCreateBucketRequestRequestTypeDef, _OptionalCreateBucketRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCertificateRequestRequestTypeDef",
     {
         "certificateName": str,
         "domainName": str,
     },
 )
@@ -2919,21 +3058,19 @@
     {
         "subjectAlternativeNames": Sequence[str],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCertificateRequestRequestTypeDef(
     _RequiredCreateCertificateRequestRequestTypeDef, _OptionalCreateCertificateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateDiskSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDiskSnapshotRequestRequestTypeDef",
     {
         "diskSnapshotName": str,
     },
 )
 _OptionalCreateDiskSnapshotRequestRequestTypeDef = TypedDict(
@@ -2942,43 +3079,39 @@
         "diskName": str,
         "instanceName": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDiskSnapshotRequestRequestTypeDef(
     _RequiredCreateDiskSnapshotRequestRequestTypeDef,
     _OptionalCreateDiskSnapshotRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 _OptionalCreateDomainRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDomainRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateInstanceSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstanceSnapshotRequestRequestTypeDef",
     {
         "instanceSnapshotName": str,
         "instanceName": str,
     },
 )
@@ -2986,43 +3119,39 @@
     "_OptionalCreateInstanceSnapshotRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateInstanceSnapshotRequestRequestTypeDef(
     _RequiredCreateInstanceSnapshotRequestRequestTypeDef,
     _OptionalCreateInstanceSnapshotRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateKeyPairRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKeyPairRequestRequestTypeDef",
     {
         "keyPairName": str,
     },
 )
 _OptionalCreateKeyPairRequestRequestTypeDef = TypedDict(
     "_OptionalCreateKeyPairRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateKeyPairRequestRequestTypeDef(
     _RequiredCreateKeyPairRequestRequestTypeDef, _OptionalCreateKeyPairRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateLoadBalancerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoadBalancerRequestRequestTypeDef",
     {
         "loadBalancerName": str,
         "instancePort": int,
     },
 )
@@ -3036,22 +3165,20 @@
         "tags": Sequence[TagTypeDef],
         "ipAddressType": IpAddressTypeType,
         "tlsPolicyName": str,
     },
     total=False,
 )
 
-
 class CreateLoadBalancerRequestRequestTypeDef(
     _RequiredCreateLoadBalancerRequestRequestTypeDef,
     _OptionalCreateLoadBalancerRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef",
     {
         "loadBalancerName": str,
         "certificateName": str,
         "certificateDomainName": str,
     },
@@ -3061,22 +3188,20 @@
     {
         "certificateAlternativeNames": Sequence[str],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateLoadBalancerTlsCertificateRequestRequestTypeDef(
     _RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef,
     _OptionalCreateLoadBalancerTlsCertificateRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
@@ -3090,22 +3215,20 @@
         "restoreTime": Union[datetime, str],
         "useLatestRestorableTime": bool,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef(
     _RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
     _OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateRelationalDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRelationalDatabaseRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
         "relationalDatabaseBlueprintId": str,
         "relationalDatabaseBundleId": str,
         "masterDatabaseName": str,
@@ -3121,22 +3244,20 @@
         "preferredMaintenanceWindow": str,
         "publiclyAccessible": bool,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRelationalDatabaseRequestRequestTypeDef(
     _RequiredCreateRelationalDatabaseRequestRequestTypeDef,
     _OptionalCreateRelationalDatabaseRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
         "relationalDatabaseSnapshotName": str,
     },
 )
@@ -3144,22 +3265,20 @@
     "_OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRelationalDatabaseSnapshotRequestRequestTypeDef(
     _RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     _OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
 ):
     pass
 
-
 DiskSnapshotTypeDef = TypedDict(
     "DiskSnapshotTypeDef",
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
@@ -3251,27 +3370,25 @@
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
     total=False,
 )
 
-
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
-
 GetBundlesResultTypeDef = TypedDict(
     "GetBundlesResultTypeDef",
     {
         "bundles": List[BundleTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheSettingsTypeDef = TypedDict(
     "CacheSettingsTypeDef",
     {
         "defaultTTL": int,
@@ -3325,23 +3442,23 @@
     total=False,
 )
 
 GetContainerImagesResultTypeDef = TypedDict(
     "GetContainerImagesResultTypeDef",
     {
         "containerImages": List[ContainerImageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterContainerImageResultTypeDef = TypedDict(
     "RegisterContainerImageResultTypeDef",
     {
         "containerImage": ContainerImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PrivateRegistryAccessRequestTypeDef = TypedDict(
     "PrivateRegistryAccessRequestTypeDef",
     {
         "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
@@ -3378,41 +3495,39 @@
     "_OptionalEndpointRequestTypeDef",
     {
         "healthCheck": ContainerServiceHealthCheckConfigTypeDef,
     },
     total=False,
 )
 
-
 class EndpointRequestTypeDef(_RequiredEndpointRequestTypeDef, _OptionalEndpointRequestTypeDef):
     pass
 
-
 GetContainerLogResultTypeDef = TypedDict(
     "GetContainerLogResultTypeDef",
     {
         "logEvents": List[ContainerServiceLogEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContainerServicePowersResultTypeDef = TypedDict(
     "GetContainerServicePowersResultTypeDef",
     {
         "powers": List[ContainerServicePowerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateContainerServiceRegistryLoginResultTypeDef = TypedDict(
     "CreateContainerServiceRegistryLoginResultTypeDef",
     {
         "registryLogin": ContainerServiceRegistryLoginTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCloudFormationStackRequestRequestTypeDef = TypedDict(
     "CreateCloudFormationStackRequestRequestTypeDef",
     {
         "instances": Sequence[InstanceEntryTypeDef],
@@ -3447,15 +3562,15 @@
     "CreateGUISessionAccessDetailsResultTypeDef",
     {
         "resourceName": str,
         "status": StatusType,
         "percentageComplete": int,
         "failureReason": str,
         "sessions": List[SessionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceSnapshotInfoTypeDef = TypedDict(
     "InstanceSnapshotInfoTypeDef",
     {
         "fromBundleId": str,
@@ -3465,15 +3580,15 @@
     total=False,
 )
 
 GetDistributionBundlesResultTypeDef = TypedDict(
     "GetDistributionBundlesResultTypeDef",
     {
         "bundles": List[DistributionBundleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainValidationRecordTypeDef = TypedDict(
     "DomainValidationRecordTypeDef",
     {
         "domainName": str,
@@ -3492,331 +3607,136 @@
         "unit": float,
         "currency": Literal["USD"],
         "timePeriod": TimePeriodTypeDef,
     },
     total=False,
 )
 
-GetActiveNamesRequestGetActiveNamesPaginateTypeDef = TypedDict(
-    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetBlueprintsRequestGetBlueprintsPaginateTypeDef = TypedDict(
-    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
-    {
-        "includeInactive": bool,
-        "appCategory": Literal["LfR"],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetBundlesRequestGetBundlesPaginateTypeDef = TypedDict(
-    "GetBundlesRequestGetBundlesPaginateTypeDef",
-    {
-        "includeInactive": bool,
-        "appCategory": Literal["LfR"],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef = TypedDict(
-    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef = TypedDict(
-    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetDisksRequestGetDisksPaginateTypeDef = TypedDict(
-    "GetDisksRequestGetDisksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetDomainsRequestGetDomainsPaginateTypeDef = TypedDict(
-    "GetDomainsRequestGetDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef = TypedDict(
-    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef = TypedDict(
-    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetInstancesRequestGetInstancesPaginateTypeDef = TypedDict(
-    "GetInstancesRequestGetInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetKeyPairsRequestGetKeyPairsPaginateTypeDef = TypedDict(
-    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
-    {
-        "includeDefaultKeyPair": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef = TypedDict(
-    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetOperationsRequestGetOperationsPaginateTypeDef = TypedDict(
-    "GetOperationsRequestGetOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef = TypedDict(
-    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef = TypedDict(
-    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
-    {
-        "includeInactive": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
-    "_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
-    {
-        "relationalDatabaseName": str,
-    },
-)
-_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
-    "_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
-    {
-        "durationInMinutes": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef(
-    _RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
-    _OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
-    "_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
-    {
-        "relationalDatabaseName": str,
-    },
-)
-_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
-    "_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef(
-    _RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
-    _OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
-):
-    pass
-
-
-GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef = TypedDict(
-    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef = TypedDict(
-    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetStaticIpsRequestGetStaticIpsPaginateTypeDef = TypedDict(
-    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetBucketMetricDataResultTypeDef = TypedDict(
     "GetBucketMetricDataResultTypeDef",
     {
         "metricName": BucketMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContainerServiceMetricDataResultTypeDef = TypedDict(
     "GetContainerServiceMetricDataResultTypeDef",
     {
         "metricName": ContainerServiceMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDistributionMetricDataResultTypeDef = TypedDict(
     "GetDistributionMetricDataResultTypeDef",
     {
         "metricName": DistributionMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstanceMetricDataResultTypeDef = TypedDict(
     "GetInstanceMetricDataResultTypeDef",
     {
         "metricName": InstanceMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLoadBalancerMetricDataResultTypeDef = TypedDict(
     "GetLoadBalancerMetricDataResultTypeDef",
     {
         "metricName": LoadBalancerMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseMetricDataResultTypeDef = TypedDict(
     "GetRelationalDatabaseMetricDataResultTypeDef",
     {
         "metricName": RelationalDatabaseMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstancePortStatesResultTypeDef = TypedDict(
     "GetInstancePortStatesResultTypeDef",
     {
         "portStates": List[InstancePortStateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstanceStateResultTypeDef = TypedDict(
     "GetInstanceStateResultTypeDef",
     {
         "state": InstanceStateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLoadBalancerTlsPoliciesResultTypeDef = TypedDict(
     "GetLoadBalancerTlsPoliciesResultTypeDef",
     {
         "tlsPolicies": List[LoadBalancerTlsPolicyTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseBlueprintsResultTypeDef = TypedDict(
     "GetRelationalDatabaseBlueprintsResultTypeDef",
     {
         "blueprints": List[RelationalDatabaseBlueprintTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseBundlesResultTypeDef = TypedDict(
     "GetRelationalDatabaseBundlesResultTypeDef",
     {
         "bundles": List[RelationalDatabaseBundleTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseEventsResultTypeDef = TypedDict(
     "GetRelationalDatabaseEventsResultTypeDef",
     {
         "relationalDatabaseEvents": List[RelationalDatabaseEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseLogEventsResultTypeDef = TypedDict(
     "GetRelationalDatabaseLogEventsResultTypeDef",
     {
         "resourceLogEvents": List[LogEventTypeDef],
         "nextBackwardToken": str,
         "nextForwardToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseParametersResultTypeDef = TypedDict(
     "GetRelationalDatabaseParametersResultTypeDef",
     {
         "parameters": List[RelationalDatabaseParameterTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
     "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
@@ -3940,15 +3860,15 @@
     total=False,
 )
 
 GetBucketAccessKeysResultTypeDef = TypedDict(
     "GetBucketAccessKeysResultTypeDef",
     {
         "accessKeys": List[AccessKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDiskFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDiskFromSnapshotRequestRequestTypeDef",
     {
         "diskName": str,
@@ -3965,22 +3885,20 @@
         "sourceDiskName": str,
         "restoreDate": str,
         "useLatestRestorableAutoSnapshot": bool,
     },
     total=False,
 )
 
-
 class CreateDiskFromSnapshotRequestRequestTypeDef(
     _RequiredCreateDiskFromSnapshotRequestRequestTypeDef,
     _OptionalCreateDiskFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDiskRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDiskRequestRequestTypeDef",
     {
         "diskName": str,
         "availabilityZone": str,
         "sizeInGb": int,
     },
@@ -3990,21 +3908,19 @@
     {
         "tags": Sequence[TagTypeDef],
         "addOns": Sequence[AddOnRequestTypeDef],
     },
     total=False,
 )
 
-
 class CreateDiskRequestRequestTypeDef(
     _RequiredCreateDiskRequestRequestTypeDef, _OptionalCreateDiskRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateInstancesFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstancesFromSnapshotRequestRequestTypeDef",
     {
         "instanceNames": Sequence[str],
         "availabilityZone": str,
         "bundleId": str,
     },
@@ -4022,22 +3938,20 @@
         "sourceInstanceName": str,
         "restoreDate": str,
         "useLatestRestorableAutoSnapshot": bool,
     },
     total=False,
 )
 
-
 class CreateInstancesFromSnapshotRequestRequestTypeDef(
     _RequiredCreateInstancesFromSnapshotRequestRequestTypeDef,
     _OptionalCreateInstancesFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstancesRequestRequestTypeDef",
     {
         "instanceNames": Sequence[str],
         "availabilityZone": str,
         "blueprintId": str,
         "bundleId": str,
@@ -4052,810 +3966,808 @@
         "tags": Sequence[TagTypeDef],
         "addOns": Sequence[AddOnRequestTypeDef],
         "ipAddressType": IpAddressTypeType,
     },
     total=False,
 )
 
-
 class CreateInstancesRequestRequestTypeDef(
     _RequiredCreateInstancesRequestRequestTypeDef, _OptionalCreateInstancesRequestRequestTypeDef
 ):
     pass
 
-
 EnableAddOnRequestRequestTypeDef = TypedDict(
     "EnableAddOnRequestRequestTypeDef",
     {
         "resourceName": str,
         "addOnRequest": AddOnRequestTypeDef,
     },
 )
 
 GetAlarmsResultTypeDef = TypedDict(
     "GetAlarmsResultTypeDef",
     {
         "alarms": List[AlarmTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContactMethodsResultTypeDef = TypedDict(
     "GetContactMethodsResultTypeDef",
     {
         "contactMethods": List[ContactMethodTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AllocateStaticIpResultTypeDef = TypedDict(
     "AllocateStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachCertificateToDistributionResultTypeDef = TypedDict(
     "AttachCertificateToDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachDiskResultTypeDef = TypedDict(
     "AttachDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachInstancesToLoadBalancerResultTypeDef = TypedDict(
     "AttachInstancesToLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachLoadBalancerTlsCertificateResultTypeDef = TypedDict(
     "AttachLoadBalancerTlsCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachStaticIpResultTypeDef = TypedDict(
     "AttachStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CloseInstancePublicPortsResultTypeDef = TypedDict(
     "CloseInstancePublicPortsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CopySnapshotResultTypeDef = TypedDict(
     "CopySnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBucketAccessKeyResultTypeDef = TypedDict(
     "CreateBucketAccessKeyResultTypeDef",
     {
         "accessKey": AccessKeyTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCloudFormationStackResultTypeDef = TypedDict(
     "CreateCloudFormationStackResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateContactMethodResultTypeDef = TypedDict(
     "CreateContactMethodResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDiskFromSnapshotResultTypeDef = TypedDict(
     "CreateDiskFromSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDiskResultTypeDef = TypedDict(
     "CreateDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDiskSnapshotResultTypeDef = TypedDict(
     "CreateDiskSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDomainEntryResultTypeDef = TypedDict(
     "CreateDomainEntryResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDomainResultTypeDef = TypedDict(
     "CreateDomainResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInstanceSnapshotResultTypeDef = TypedDict(
     "CreateInstanceSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInstancesFromSnapshotResultTypeDef = TypedDict(
     "CreateInstancesFromSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInstancesResultTypeDef = TypedDict(
     "CreateInstancesResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateLoadBalancerResultTypeDef = TypedDict(
     "CreateLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateLoadBalancerTlsCertificateResultTypeDef = TypedDict(
     "CreateLoadBalancerTlsCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRelationalDatabaseFromSnapshotResultTypeDef = TypedDict(
     "CreateRelationalDatabaseFromSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRelationalDatabaseResultTypeDef = TypedDict(
     "CreateRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRelationalDatabaseSnapshotResultTypeDef = TypedDict(
     "CreateRelationalDatabaseSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAlarmResultTypeDef = TypedDict(
     "DeleteAlarmResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAutoSnapshotResultTypeDef = TypedDict(
     "DeleteAutoSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteBucketAccessKeyResultTypeDef = TypedDict(
     "DeleteBucketAccessKeyResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteBucketResultTypeDef = TypedDict(
     "DeleteBucketResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCertificateResultTypeDef = TypedDict(
     "DeleteCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteContactMethodResultTypeDef = TypedDict(
     "DeleteContactMethodResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDiskResultTypeDef = TypedDict(
     "DeleteDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDiskSnapshotResultTypeDef = TypedDict(
     "DeleteDiskSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDistributionResultTypeDef = TypedDict(
     "DeleteDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDomainEntryResultTypeDef = TypedDict(
     "DeleteDomainEntryResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDomainResultTypeDef = TypedDict(
     "DeleteDomainResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInstanceResultTypeDef = TypedDict(
     "DeleteInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInstanceSnapshotResultTypeDef = TypedDict(
     "DeleteInstanceSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteKeyPairResultTypeDef = TypedDict(
     "DeleteKeyPairResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteKnownHostKeysResultTypeDef = TypedDict(
     "DeleteKnownHostKeysResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteLoadBalancerResultTypeDef = TypedDict(
     "DeleteLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteLoadBalancerTlsCertificateResultTypeDef = TypedDict(
     "DeleteLoadBalancerTlsCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRelationalDatabaseResultTypeDef = TypedDict(
     "DeleteRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRelationalDatabaseSnapshotResultTypeDef = TypedDict(
     "DeleteRelationalDatabaseSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetachCertificateFromDistributionResultTypeDef = TypedDict(
     "DetachCertificateFromDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetachDiskResultTypeDef = TypedDict(
     "DetachDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetachInstancesFromLoadBalancerResultTypeDef = TypedDict(
     "DetachInstancesFromLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetachStaticIpResultTypeDef = TypedDict(
     "DetachStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisableAddOnResultTypeDef = TypedDict(
     "DisableAddOnResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnableAddOnResultTypeDef = TypedDict(
     "EnableAddOnResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportSnapshotResultTypeDef = TypedDict(
     "ExportSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOperationResultTypeDef = TypedDict(
     "GetOperationResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOperationsForResourceResultTypeDef = TypedDict(
     "GetOperationsForResourceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "nextPageCount": str,
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOperationsResultTypeDef = TypedDict(
     "GetOperationsResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportKeyPairResultTypeDef = TypedDict(
     "ImportKeyPairResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OpenInstancePublicPortsResultTypeDef = TypedDict(
     "OpenInstancePublicPortsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PeerVpcResultTypeDef = TypedDict(
     "PeerVpcResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAlarmResultTypeDef = TypedDict(
     "PutAlarmResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutInstancePublicPortsResultTypeDef = TypedDict(
     "PutInstancePublicPortsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootInstanceResultTypeDef = TypedDict(
     "RebootInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootRelationalDatabaseResultTypeDef = TypedDict(
     "RebootRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReleaseStaticIpResultTypeDef = TypedDict(
     "ReleaseStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetDistributionCacheResultTypeDef = TypedDict(
     "ResetDistributionCacheResultTypeDef",
     {
         "status": str,
         "createTime": datetime,
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendContactMethodVerificationResultTypeDef = TypedDict(
     "SendContactMethodVerificationResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetIpAddressTypeResultTypeDef = TypedDict(
     "SetIpAddressTypeResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetResourceAccessForBucketResultTypeDef = TypedDict(
     "SetResourceAccessForBucketResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartGUISessionResultTypeDef = TypedDict(
     "StartGUISessionResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartInstanceResultTypeDef = TypedDict(
     "StartInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartRelationalDatabaseResultTypeDef = TypedDict(
     "StartRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopGUISessionResultTypeDef = TypedDict(
     "StopGUISessionResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopInstanceResultTypeDef = TypedDict(
     "StopInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopRelationalDatabaseResultTypeDef = TypedDict(
     "StopRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceResultTypeDef = TypedDict(
     "TagResourceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestAlarmResultTypeDef = TypedDict(
     "TestAlarmResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UnpeerVpcResultTypeDef = TypedDict(
     "UnpeerVpcResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UntagResourceResultTypeDef = TypedDict(
     "UntagResourceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBucketBundleResultTypeDef = TypedDict(
     "UpdateBucketBundleResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDistributionBundleResultTypeDef = TypedDict(
     "UpdateDistributionBundleResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDistributionResultTypeDef = TypedDict(
     "UpdateDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainEntryResultTypeDef = TypedDict(
     "UpdateDomainEntryResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInstanceMetadataOptionsResultTypeDef = TypedDict(
     "UpdateInstanceMetadataOptionsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLoadBalancerAttributeResultTypeDef = TypedDict(
     "UpdateLoadBalancerAttributeResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRelationalDatabaseParametersResultTypeDef = TypedDict(
     "UpdateRelationalDatabaseParametersResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRelationalDatabaseResultTypeDef = TypedDict(
     "UpdateRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStaticIpResultTypeDef = TypedDict(
     "GetStaticIpResultTypeDef",
     {
         "staticIp": StaticIpTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStaticIpsResultTypeDef = TypedDict(
     "GetStaticIpsResultTypeDef",
     {
         "staticIps": List[StaticIpTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAutoSnapshotsResultTypeDef = TypedDict(
     "GetAutoSnapshotsResultTypeDef",
     {
         "resourceName": str,
         "resourceType": ResourceTypeType,
         "autoSnapshots": List[AutoSnapshotDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRegionsResultTypeDef = TypedDict(
     "GetRegionsResultTypeDef",
     {
         "regions": List[RegionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBucketResultTypeDef = TypedDict(
     "CreateBucketResultTypeDef",
     {
         "bucket": BucketTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBucketsResultTypeDef = TypedDict(
     "GetBucketsResultTypeDef",
     {
         "buckets": List[BucketTypeDef],
         "nextPageToken": str,
         "accountLevelBpaSync": AccountLevelBpaSyncTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBucketResultTypeDef = TypedDict(
     "UpdateBucketResultTypeDef",
     {
         "bucket": BucketTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDiskSnapshotResultTypeDef = TypedDict(
     "GetDiskSnapshotResultTypeDef",
     {
         "diskSnapshot": DiskSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDiskSnapshotsResultTypeDef = TypedDict(
     "GetDiskSnapshotsResultTypeDef",
     {
         "diskSnapshots": List[DiskSnapshotTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDiskResultTypeDef = TypedDict(
     "GetDiskResultTypeDef",
     {
         "disk": DiskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDisksResultTypeDef = TypedDict(
     "GetDisksResultTypeDef",
     {
         "disks": List[DiskTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceHardwareTypeDef = TypedDict(
     "InstanceHardwareTypeDef",
     {
         "cpuCount": int,
@@ -4891,49 +4803,49 @@
 CreateKeyPairResultTypeDef = TypedDict(
     "CreateKeyPairResultTypeDef",
     {
         "keyPair": KeyPairTypeDef,
         "publicKeyBase64": str,
         "privateKeyBase64": str,
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKeyPairResultTypeDef = TypedDict(
     "GetKeyPairResultTypeDef",
     {
         "keyPair": KeyPairTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKeyPairsResultTypeDef = TypedDict(
     "GetKeyPairsResultTypeDef",
     {
         "keyPairs": List[KeyPairTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseSnapshotResultTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotResultTypeDef",
     {
         "relationalDatabaseSnapshot": RelationalDatabaseSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseSnapshotsResultTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotsResultTypeDef",
     {
         "relationalDatabaseSnapshots": List[RelationalDatabaseSnapshotTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
@@ -4949,22 +4861,20 @@
         "cacheBehaviors": Sequence[CacheBehaviorPerPathTypeDef],
         "ipAddressType": IpAddressTypeType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDistributionRequestRequestTypeDef(
     _RequiredCreateDistributionRequestRequestTypeDef,
     _OptionalCreateDistributionRequestRequestTypeDef,
 ):
     pass
 
-
 LightsailDistributionTypeDef = TypedDict(
     "LightsailDistributionTypeDef",
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
@@ -5002,28 +4912,26 @@
         "cacheBehaviorSettings": CacheSettingsTypeDef,
         "cacheBehaviors": Sequence[CacheBehaviorPerPathTypeDef],
         "isEnabled": bool,
     },
     total=False,
 )
 
-
 class UpdateDistributionRequestRequestTypeDef(
     _RequiredUpdateDistributionRequestRequestTypeDef,
     _OptionalUpdateDistributionRequestRequestTypeDef,
 ):
     pass
 
-
 GetCloudFormationStackRecordsResultTypeDef = TypedDict(
     "GetCloudFormationStackRecordsResultTypeDef",
     {
         "cloudFormationStackRecords": List[CloudFormationStackRecordTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateContainerServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContainerServiceRequestRequestTypeDef",
     {
         "serviceName": str,
@@ -5037,22 +4945,20 @@
         "isDisabled": bool,
         "publicDomainNames": Mapping[str, Sequence[str]],
         "privateRegistryAccess": PrivateRegistryAccessRequestTypeDef,
     },
     total=False,
 )
 
-
 class UpdateContainerServiceRequestRequestTypeDef(
     _RequiredUpdateContainerServiceRequestRequestTypeDef,
     _OptionalUpdateContainerServiceRequestRequestTypeDef,
 ):
     pass
 
-
 ContainerServiceDeploymentTypeDef = TypedDict(
     "ContainerServiceDeploymentTypeDef",
     {
         "version": int,
         "state": ContainerServiceDeploymentStateType,
         "containers": Dict[str, ContainerTypeDef],
         "publicEndpoint": ContainerServiceEndpointTypeDef,
@@ -5081,22 +4987,20 @@
     {
         "containers": Mapping[str, ContainerTypeDef],
         "publicEndpoint": EndpointRequestTypeDef,
     },
     total=False,
 )
 
-
 class CreateContainerServiceDeploymentRequestRequestTypeDef(
     _RequiredCreateContainerServiceDeploymentRequestRequestTypeDef,
     _OptionalCreateContainerServiceDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 ExportSnapshotRecordSourceInfoTypeDef = TypedDict(
     "ExportSnapshotRecordSourceInfoTypeDef",
     {
         "resourceType": ExportSnapshotRecordSourceTypeType,
         "createdAt": datetime,
         "name": str,
         "arn": str,
@@ -5128,15 +5032,15 @@
     total=False,
 )
 
 GetInstanceAccessDetailsResultTypeDef = TypedDict(
     "GetInstanceAccessDetailsResultTypeDef",
     {
         "accessDetails": InstanceAccessDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoadBalancerTlsCertificateTypeDef = TypedDict(
     "LoadBalancerTlsCertificateTypeDef",
     {
         "name": str,
@@ -5168,24 +5072,24 @@
     total=False,
 )
 
 GetLoadBalancerResultTypeDef = TypedDict(
     "GetLoadBalancerResultTypeDef",
     {
         "loadBalancer": LoadBalancerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLoadBalancersResultTypeDef = TypedDict(
     "GetLoadBalancersResultTypeDef",
     {
         "loadBalancers": List[LoadBalancerTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainTypeDef = TypedDict(
     "DomainTypeDef",
     {
         "name": str,
@@ -5201,24 +5105,24 @@
     total=False,
 )
 
 GetRelationalDatabaseResultTypeDef = TypedDict(
     "GetRelationalDatabaseResultTypeDef",
     {
         "relationalDatabase": RelationalDatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabasesResultTypeDef = TypedDict(
     "GetRelationalDatabasesResultTypeDef",
     {
         "relationalDatabases": List[RelationalDatabaseTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "name": str,
@@ -5247,42 +5151,42 @@
     total=False,
 )
 
 GetInstanceSnapshotResultTypeDef = TypedDict(
     "GetInstanceSnapshotResultTypeDef",
     {
         "instanceSnapshot": InstanceSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstanceSnapshotsResultTypeDef = TypedDict(
     "GetInstanceSnapshotsResultTypeDef",
     {
         "instanceSnapshots": List[InstanceSnapshotTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDistributionResultTypeDef = TypedDict(
     "CreateDistributionResultTypeDef",
     {
         "distribution": LightsailDistributionTypeDef,
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDistributionsResultTypeDef = TypedDict(
     "GetDistributionsResultTypeDef",
     {
         "distributions": List[LightsailDistributionTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ContainerServiceTypeDef = TypedDict(
     "ContainerServiceTypeDef",
     {
         "containerServiceName": str,
@@ -5308,15 +5212,15 @@
     total=False,
 )
 
 GetContainerServiceDeploymentsResultTypeDef = TypedDict(
     "GetContainerServiceDeploymentsResultTypeDef",
     {
         "deployments": List[ContainerServiceDeploymentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateContainerServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerServiceRequestRequestTypeDef",
     {
         "serviceName": str,
@@ -5331,22 +5235,20 @@
         "publicDomainNames": Mapping[str, Sequence[str]],
         "deployment": ContainerServiceDeploymentRequestTypeDef,
         "privateRegistryAccess": PrivateRegistryAccessRequestTypeDef,
     },
     total=False,
 )
 
-
 class CreateContainerServiceRequestRequestTypeDef(
     _RequiredCreateContainerServiceRequestRequestTypeDef,
     _OptionalCreateContainerServiceRequestRequestTypeDef,
 ):
     pass
 
-
 ExportSnapshotRecordTypeDef = TypedDict(
     "ExportSnapshotRecordTypeDef",
     {
         "name": str,
         "arn": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
@@ -5398,90 +5300,90 @@
     total=False,
 )
 
 GetLoadBalancerTlsCertificatesResultTypeDef = TypedDict(
     "GetLoadBalancerTlsCertificatesResultTypeDef",
     {
         "tlsCertificates": List[LoadBalancerTlsCertificateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainResultTypeDef = TypedDict(
     "GetDomainResultTypeDef",
     {
         "domain": DomainTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainsResultTypeDef = TypedDict(
     "GetDomainsResultTypeDef",
     {
         "domains": List[DomainTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstanceResultTypeDef = TypedDict(
     "GetInstanceResultTypeDef",
     {
         "instance": InstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstancesResultTypeDef = TypedDict(
     "GetInstancesResultTypeDef",
     {
         "instances": List[InstanceTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ContainerServicesListResultTypeDef = TypedDict(
     "ContainerServicesListResultTypeDef",
     {
         "containerServices": List[ContainerServiceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateContainerServiceDeploymentResultTypeDef = TypedDict(
     "CreateContainerServiceDeploymentResultTypeDef",
     {
         "containerService": ContainerServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateContainerServiceResultTypeDef = TypedDict(
     "CreateContainerServiceResultTypeDef",
     {
         "containerService": ContainerServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContainerServiceResultTypeDef = TypedDict(
     "UpdateContainerServiceResultTypeDef",
     {
         "containerService": ContainerServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExportSnapshotRecordsResultTypeDef = TypedDict(
     "GetExportSnapshotRecordsResultTypeDef",
     {
         "exportSnapshotRecords": List[ExportSnapshotRecordTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "certificateArn": str,
@@ -5493,27 +5395,28 @@
     total=False,
 )
 
 GetCostEstimateResultTypeDef = TypedDict(
     "GetCostEstimateResultTypeDef",
     {
         "resourcesBudgetEstimate": List[ResourceBudgetEstimateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCertificateResultTypeDef = TypedDict(
     "CreateCertificateResultTypeDef",
     {
         "certificate": CertificateSummaryTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCertificatesResultTypeDef = TypedDict(
     "GetCertificatesResultTypeDef",
     {
         "certificates": List[CertificateSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "nextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/type_defs.pyi` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,25 +96,25 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccessKeyLastUsedTypeDef",
     "AccessRulesTypeDef",
     "AccountLevelBpaSyncTypeDef",
     "AutoSnapshotAddOnRequestTypeDef",
     "StopInstanceOnIdleRequestTypeDef",
     "AddOnTypeDef",
     "MonitoredResourceInfoTypeDef",
     "ResourceLocationTypeDef",
     "AllocateStaticIpRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AttachCertificateToDistributionRequestRequestTypeDef",
     "AttachDiskRequestRequestTypeDef",
     "AttachInstancesToLoadBalancerRequestRequestTypeDef",
     "AttachLoadBalancerTlsCertificateRequestRequestTypeDef",
     "AttachStaticIpRequestRequestTypeDef",
     "AttachedDiskTypeDef",
     "AvailabilityZoneTypeDef",
@@ -177,110 +177,138 @@
     "DetachStaticIpRequestRequestTypeDef",
     "DisableAddOnRequestRequestTypeDef",
     "DiskInfoTypeDef",
     "DiskSnapshotInfoTypeDef",
     "DistributionBundleTypeDef",
     "DnsRecordCreationStateTypeDef",
     "ResourceRecordTypeDef",
+    "DownloadDefaultKeyPairResultTypeDef",
     "TimePeriodTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     "GetActiveNamesRequestRequestTypeDef",
+    "GetActiveNamesResultTypeDef",
     "GetAlarmsRequestRequestTypeDef",
     "GetAutoSnapshotsRequestRequestTypeDef",
+    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     "GetBlueprintsRequestRequestTypeDef",
     "GetBucketAccessKeysRequestRequestTypeDef",
     "GetBucketBundlesRequestRequestTypeDef",
     "GetBucketMetricDataRequestRequestTypeDef",
     "MetricDatapointTypeDef",
     "GetBucketsRequestRequestTypeDef",
+    "GetBundlesRequestGetBundlesPaginateTypeDef",
     "GetBundlesRequestRequestTypeDef",
     "GetCertificatesRequestRequestTypeDef",
+    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
     "GetCloudFormationStackRecordsRequestRequestTypeDef",
     "GetContactMethodsRequestRequestTypeDef",
+    "GetContainerAPIMetadataResultTypeDef",
     "GetContainerImagesRequestRequestTypeDef",
     "GetContainerLogRequestRequestTypeDef",
     "GetContainerServiceDeploymentsRequestRequestTypeDef",
     "GetContainerServiceMetricDataRequestRequestTypeDef",
     "GetContainerServicesRequestRequestTypeDef",
     "GetCostEstimateRequestRequestTypeDef",
     "GetDiskRequestRequestTypeDef",
     "GetDiskSnapshotRequestRequestTypeDef",
+    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
     "GetDiskSnapshotsRequestRequestTypeDef",
+    "GetDisksRequestGetDisksPaginateTypeDef",
     "GetDisksRequestRequestTypeDef",
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
+    "GetDistributionLatestCacheResetResultTypeDef",
     "GetDistributionMetricDataRequestRequestTypeDef",
     "GetDistributionsRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
+    "GetDomainsRequestGetDomainsPaginateTypeDef",
     "GetDomainsRequestRequestTypeDef",
+    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
     "GetExportSnapshotRecordsRequestRequestTypeDef",
     "GetInstanceAccessDetailsRequestRequestTypeDef",
     "GetInstanceMetricDataRequestRequestTypeDef",
     "GetInstancePortStatesRequestRequestTypeDef",
     "InstancePortStateTypeDef",
     "GetInstanceRequestRequestTypeDef",
     "GetInstanceSnapshotRequestRequestTypeDef",
+    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
     "GetInstanceSnapshotsRequestRequestTypeDef",
     "GetInstanceStateRequestRequestTypeDef",
     "InstanceStateTypeDef",
+    "GetInstancesRequestGetInstancesPaginateTypeDef",
     "GetInstancesRequestRequestTypeDef",
     "GetKeyPairRequestRequestTypeDef",
+    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
     "GetKeyPairsRequestRequestTypeDef",
     "GetLoadBalancerMetricDataRequestRequestTypeDef",
     "GetLoadBalancerRequestRequestTypeDef",
     "GetLoadBalancerTlsCertificatesRequestRequestTypeDef",
     "GetLoadBalancerTlsPoliciesRequestRequestTypeDef",
     "LoadBalancerTlsPolicyTypeDef",
+    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
     "GetLoadBalancersRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "GetOperationsForResourceRequestRequestTypeDef",
+    "GetOperationsRequestGetOperationsPaginateTypeDef",
     "GetOperationsRequestRequestTypeDef",
     "GetRegionsRequestRequestTypeDef",
+    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
     "GetRelationalDatabaseBlueprintsRequestRequestTypeDef",
     "RelationalDatabaseBlueprintTypeDef",
+    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
     "GetRelationalDatabaseBundlesRequestRequestTypeDef",
     "RelationalDatabaseBundleTypeDef",
+    "GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
     "GetRelationalDatabaseEventsRequestRequestTypeDef",
     "RelationalDatabaseEventTypeDef",
     "GetRelationalDatabaseLogEventsRequestRequestTypeDef",
     "LogEventTypeDef",
     "GetRelationalDatabaseLogStreamsRequestRequestTypeDef",
+    "GetRelationalDatabaseLogStreamsResultTypeDef",
     "GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
+    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
     "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
+    "GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
     "GetRelationalDatabaseParametersRequestRequestTypeDef",
     "RelationalDatabaseParameterTypeDef",
     "GetRelationalDatabaseRequestRequestTypeDef",
     "GetRelationalDatabaseSnapshotRequestRequestTypeDef",
+    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
     "GetRelationalDatabaseSnapshotsRequestRequestTypeDef",
+    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
     "GetRelationalDatabasesRequestRequestTypeDef",
     "GetStaticIpRequestRequestTypeDef",
+    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
     "GetStaticIpsRequestRequestTypeDef",
     "HostKeyAttributesTypeDef",
     "ImportKeyPairRequestRequestTypeDef",
     "PasswordDataTypeDef",
     "InstanceHealthSummaryTypeDef",
     "InstanceMetadataOptionsTypeDef",
     "InstancePortInfoTypeDef",
     "MonthlyTransferTypeDef",
+    "IsVpcPeeredResultTypeDef",
     "OriginTypeDef",
     "LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef",
     "LoadBalancerTlsCertificateDomainValidationOptionTypeDef",
     "LoadBalancerTlsCertificateSummaryTypeDef",
     "NameServersUpdateStateTypeDef",
+    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PendingModifiedRelationalDatabaseValuesTypeDef",
     "PutAlarmRequestRequestTypeDef",
     "R53HostedZoneDeletionStateTypeDef",
     "RebootInstanceRequestRequestTypeDef",
     "RebootRelationalDatabaseRequestRequestTypeDef",
     "RegisterContainerImageRequestRequestTypeDef",
     "RelationalDatabaseEndpointTypeDef",
     "RelationalDatabaseHardwareTypeDef",
     "ReleaseStaticIpRequestRequestTypeDef",
     "ResetDistributionCacheRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SendContactMethodVerificationRequestRequestTypeDef",
     "SetIpAddressTypeRequestRequestTypeDef",
     "SetResourceAccessForBucketRequestRequestTypeDef",
     "StartGUISessionRequestRequestTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartRelationalDatabaseRequestRequestTypeDef",
     "StopGUISessionRequestRequestTypeDef",
@@ -295,21 +323,14 @@
     "UpdateRelationalDatabaseRequestRequestTypeDef",
     "AccessKeyTypeDef",
     "AddOnRequestTypeDef",
     "AlarmTypeDef",
     "ContactMethodTypeDef",
     "OperationTypeDef",
     "StaticIpTypeDef",
-    "DownloadDefaultKeyPairResultTypeDef",
-    "GetActiveNamesResultTypeDef",
-    "GetContainerAPIMetadataResultTypeDef",
-    "GetDistributionLatestCacheResetResultTypeDef",
-    "GetRelationalDatabaseLogStreamsResultTypeDef",
-    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
-    "IsVpcPeeredResultTypeDef",
     "AutoSnapshotDetailsTypeDef",
     "RegionTypeDef",
     "GetBlueprintsResultTypeDef",
     "UpdateBucketRequestRequestTypeDef",
     "GetBucketBundlesResultTypeDef",
     "BucketTypeDef",
     "CreateBucketRequestRequestTypeDef",
@@ -348,34 +369,14 @@
     "DeleteDomainEntryRequestRequestTypeDef",
     "UpdateDomainEntryRequestRequestTypeDef",
     "CreateGUISessionAccessDetailsResultTypeDef",
     "InstanceSnapshotInfoTypeDef",
     "GetDistributionBundlesResultTypeDef",
     "DomainValidationRecordTypeDef",
     "EstimateByTimeTypeDef",
-    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
-    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
-    "GetBundlesRequestGetBundlesPaginateTypeDef",
-    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
-    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
-    "GetDisksRequestGetDisksPaginateTypeDef",
-    "GetDomainsRequestGetDomainsPaginateTypeDef",
-    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
-    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
-    "GetInstancesRequestGetInstancesPaginateTypeDef",
-    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
-    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
-    "GetOperationsRequestGetOperationsPaginateTypeDef",
-    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
-    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
-    "GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
-    "GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
-    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
-    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
-    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
     "GetBucketMetricDataResultTypeDef",
     "GetContainerServiceMetricDataResultTypeDef",
     "GetDistributionMetricDataResultTypeDef",
     "GetInstanceMetricDataResultTypeDef",
     "GetLoadBalancerMetricDataResultTypeDef",
     "GetRelationalDatabaseMetricDataResultTypeDef",
     "GetInstancePortStatesResultTypeDef",
@@ -630,25 +631,14 @@
 AllocateStaticIpRequestRequestTypeDef = TypedDict(
     "AllocateStaticIpRequestRequestTypeDef",
     {
         "staticIpName": str,
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
 AttachCertificateToDistributionRequestRequestTypeDef = TypedDict(
     "AttachCertificateToDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "certificateName": str,
     },
 )
@@ -665,19 +655,21 @@
     "_OptionalAttachDiskRequestRequestTypeDef",
     {
         "autoMounting": bool,
     },
     total=False,
 )
 
+
 class AttachDiskRequestRequestTypeDef(
     _RequiredAttachDiskRequestRequestTypeDef, _OptionalAttachDiskRequestRequestTypeDef
 ):
     pass
 
+
 AttachInstancesToLoadBalancerRequestRequestTypeDef = TypedDict(
     "AttachInstancesToLoadBalancerRequestRequestTypeDef",
     {
         "loadBalancerName": str,
         "instanceNames": Sequence[str],
     },
 )
@@ -747,19 +739,21 @@
     {
         "destination": str,
         "prefix": str,
     },
     total=False,
 )
 
+
 class BucketAccessLogConfigTypeDef(
     _RequiredBucketAccessLogConfigTypeDef, _OptionalBucketAccessLogConfigTypeDef
 ):
     pass
 
+
 BucketBundleTypeDef = TypedDict(
     "BucketBundleTypeDef",
     {
         "bundleId": str,
         "name": str,
         "price": float,
         "storagePerMonthInGb": int,
@@ -998,19 +992,21 @@
         "sourceResourceName": str,
         "restoreDate": str,
         "useLatestRestorableAutoSnapshot": bool,
     },
     total=False,
 )
 
+
 class CopySnapshotRequestRequestTypeDef(
     _RequiredCopySnapshotRequestRequestTypeDef, _OptionalCopySnapshotRequestRequestTypeDef
 ):
     pass
 
+
 CreateBucketAccessKeyRequestRequestTypeDef = TypedDict(
     "CreateBucketAccessKeyRequestRequestTypeDef",
     {
         "bucketName": str,
     },
 )
 
@@ -1027,17 +1023,19 @@
     "_OptionalInstanceEntryTypeDef",
     {
         "userData": str,
     },
     total=False,
 )
 
+
 class InstanceEntryTypeDef(_RequiredInstanceEntryTypeDef, _OptionalInstanceEntryTypeDef):
     pass
 
+
 CreateContactMethodRequestRequestTypeDef = TypedDict(
     "CreateContactMethodRequestRequestTypeDef",
     {
         "protocol": ContactProtocolType,
         "contactEndpoint": str,
     },
 )
@@ -1124,19 +1122,21 @@
     "_OptionalDeleteBucketRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
+
 class DeleteBucketRequestRequestTypeDef(
     _RequiredDeleteBucketRequestRequestTypeDef, _OptionalDeleteBucketRequestRequestTypeDef
 ):
     pass
 
+
 DeleteCertificateRequestRequestTypeDef = TypedDict(
     "DeleteCertificateRequestRequestTypeDef",
     {
         "certificateName": str,
     },
 )
 
@@ -1172,19 +1172,21 @@
     "_OptionalDeleteDiskRequestRequestTypeDef",
     {
         "forceDeleteAddOns": bool,
     },
     total=False,
 )
 
+
 class DeleteDiskRequestRequestTypeDef(
     _RequiredDeleteDiskRequestRequestTypeDef, _OptionalDeleteDiskRequestRequestTypeDef
 ):
     pass
 
+
 DeleteDiskSnapshotRequestRequestTypeDef = TypedDict(
     "DeleteDiskSnapshotRequestRequestTypeDef",
     {
         "diskSnapshotName": str,
     },
 )
 
@@ -1213,19 +1215,21 @@
     "_OptionalDeleteInstanceRequestRequestTypeDef",
     {
         "forceDeleteAddOns": bool,
     },
     total=False,
 )
 
+
 class DeleteInstanceRequestRequestTypeDef(
     _RequiredDeleteInstanceRequestRequestTypeDef, _OptionalDeleteInstanceRequestRequestTypeDef
 ):
     pass
 
+
 DeleteInstanceSnapshotRequestRequestTypeDef = TypedDict(
     "DeleteInstanceSnapshotRequestRequestTypeDef",
     {
         "instanceSnapshotName": str,
     },
 )
 
@@ -1239,19 +1243,21 @@
     "_OptionalDeleteKeyPairRequestRequestTypeDef",
     {
         "expectedFingerprint": str,
     },
     total=False,
 )
 
+
 class DeleteKeyPairRequestRequestTypeDef(
     _RequiredDeleteKeyPairRequestRequestTypeDef, _OptionalDeleteKeyPairRequestRequestTypeDef
 ):
     pass
 
+
 DeleteKnownHostKeysRequestRequestTypeDef = TypedDict(
     "DeleteKnownHostKeysRequestRequestTypeDef",
     {
         "instanceName": str,
     },
 )
 
@@ -1273,20 +1279,22 @@
     "_OptionalDeleteLoadBalancerTlsCertificateRequestRequestTypeDef",
     {
         "force": bool,
     },
     total=False,
 )
 
+
 class DeleteLoadBalancerTlsCertificateRequestRequestTypeDef(
     _RequiredDeleteLoadBalancerTlsCertificateRequestRequestTypeDef,
     _OptionalDeleteLoadBalancerTlsCertificateRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteRelationalDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRelationalDatabaseRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalDeleteRelationalDatabaseRequestRequestTypeDef = TypedDict(
@@ -1294,20 +1302,22 @@
     {
         "skipFinalSnapshot": bool,
         "finalRelationalDatabaseSnapshotName": str,
     },
     total=False,
 )
 
+
 class DeleteRelationalDatabaseRequestRequestTypeDef(
     _RequiredDeleteRelationalDatabaseRequestRequestTypeDef,
     _OptionalDeleteRelationalDatabaseRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteRelationalDatabaseSnapshotRequestRequestTypeDef = TypedDict(
     "DeleteRelationalDatabaseSnapshotRequestRequestTypeDef",
     {
         "relationalDatabaseSnapshotName": str,
     },
 )
 
@@ -1394,14 +1404,24 @@
         "name": str,
         "type": str,
         "value": str,
     },
     total=False,
 )
 
+DownloadDefaultKeyPairResultTypeDef = TypedDict(
+    "DownloadDefaultKeyPairResultTypeDef",
+    {
+        "publicKeyBase64": str,
+        "privateKeyBase64": str,
+        "createdAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimePeriodTypeDef = TypedDict(
     "TimePeriodTypeDef",
     {
         "start": datetime,
         "end": datetime,
     },
     total=False,
@@ -1410,32 +1430,39 @@
 ExportSnapshotRequestRequestTypeDef = TypedDict(
     "ExportSnapshotRequestRequestTypeDef",
     {
         "sourceSnapshotName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetActiveNamesRequestGetActiveNamesPaginateTypeDef = TypedDict(
+    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetActiveNamesRequestRequestTypeDef = TypedDict(
     "GetActiveNamesRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
+GetActiveNamesResultTypeDef = TypedDict(
+    "GetActiveNamesResultTypeDef",
+    {
+        "activeNames": List[str],
+        "nextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAlarmsRequestRequestTypeDef = TypedDict(
     "GetAlarmsRequestRequestTypeDef",
     {
         "alarmName": str,
         "pageToken": str,
         "monitoredResourceName": str,
     },
@@ -1445,14 +1472,24 @@
 GetAutoSnapshotsRequestRequestTypeDef = TypedDict(
     "GetAutoSnapshotsRequestRequestTypeDef",
     {
         "resourceName": str,
     },
 )
 
+GetBlueprintsRequestGetBlueprintsPaginateTypeDef = TypedDict(
+    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
+    {
+        "includeInactive": bool,
+        "appCategory": Literal["LfR"],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetBlueprintsRequestRequestTypeDef = TypedDict(
     "GetBlueprintsRequestRequestTypeDef",
     {
         "includeInactive": bool,
         "pageToken": str,
         "appCategory": Literal["LfR"],
     },
@@ -1507,14 +1544,24 @@
         "bucketName": str,
         "pageToken": str,
         "includeConnectedResources": bool,
     },
     total=False,
 )
 
+GetBundlesRequestGetBundlesPaginateTypeDef = TypedDict(
+    "GetBundlesRequestGetBundlesPaginateTypeDef",
+    {
+        "includeInactive": bool,
+        "appCategory": Literal["LfR"],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetBundlesRequestRequestTypeDef = TypedDict(
     "GetBundlesRequestRequestTypeDef",
     {
         "includeInactive": bool,
         "pageToken": str,
         "appCategory": Literal["LfR"],
     },
@@ -1523,14 +1570,23 @@
 
 GetCertificatesRequestRequestTypeDef = TypedDict(
     "GetCertificatesRequestRequestTypeDef",
     {
         "certificateStatuses": Sequence[CertificateStatusType],
         "includeCertificateDetails": bool,
         "certificateName": str,
+        "pageToken": str,
+    },
+    total=False,
+)
+
+GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef = TypedDict(
+    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetCloudFormationStackRecordsRequestRequestTypeDef = TypedDict(
     "GetCloudFormationStackRecordsRequestRequestTypeDef",
     {
@@ -1543,14 +1599,22 @@
     "GetContactMethodsRequestRequestTypeDef",
     {
         "protocols": Sequence[ContactProtocolType],
     },
     total=False,
 )
 
+GetContainerAPIMetadataResultTypeDef = TypedDict(
+    "GetContainerAPIMetadataResultTypeDef",
+    {
+        "metadata": List[Dict[str, str]],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetContainerImagesRequestRequestTypeDef = TypedDict(
     "GetContainerImagesRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
@@ -1568,19 +1632,21 @@
         "endTime": Union[datetime, str],
         "filterPattern": str,
         "pageToken": str,
     },
     total=False,
 )
 
+
 class GetContainerLogRequestRequestTypeDef(
     _RequiredGetContainerLogRequestRequestTypeDef, _OptionalGetContainerLogRequestRequestTypeDef
 ):
     pass
 
+
 GetContainerServiceDeploymentsRequestRequestTypeDef = TypedDict(
     "GetContainerServiceDeploymentsRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
@@ -1623,22 +1689,38 @@
 GetDiskSnapshotRequestRequestTypeDef = TypedDict(
     "GetDiskSnapshotRequestRequestTypeDef",
     {
         "diskSnapshotName": str,
     },
 )
 
+GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef = TypedDict(
+    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetDiskSnapshotsRequestRequestTypeDef = TypedDict(
     "GetDiskSnapshotsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
+GetDisksRequestGetDisksPaginateTypeDef = TypedDict(
+    "GetDisksRequestGetDisksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetDisksRequestRequestTypeDef = TypedDict(
     "GetDisksRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1647,14 +1729,23 @@
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
     {
         "distributionName": str,
     },
     total=False,
 )
 
+GetDistributionLatestCacheResetResultTypeDef = TypedDict(
+    "GetDistributionLatestCacheResetResultTypeDef",
+    {
+        "status": str,
+        "createTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDistributionMetricDataRequestRequestTypeDef = TypedDict(
     "GetDistributionMetricDataRequestRequestTypeDef",
     {
         "distributionName": str,
         "metricName": DistributionMetricNameType,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
@@ -1676,22 +1767,38 @@
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 
+GetDomainsRequestGetDomainsPaginateTypeDef = TypedDict(
+    "GetDomainsRequestGetDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetDomainsRequestRequestTypeDef = TypedDict(
     "GetDomainsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
+GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef = TypedDict(
+    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetExportSnapshotRecordsRequestRequestTypeDef = TypedDict(
     "GetExportSnapshotRecordsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1706,20 +1813,22 @@
     "_OptionalGetInstanceAccessDetailsRequestRequestTypeDef",
     {
         "protocol": InstanceAccessProtocolType,
     },
     total=False,
 )
 
+
 class GetInstanceAccessDetailsRequestRequestTypeDef(
     _RequiredGetInstanceAccessDetailsRequestRequestTypeDef,
     _OptionalGetInstanceAccessDetailsRequestRequestTypeDef,
 ):
     pass
 
+
 GetInstanceMetricDataRequestRequestTypeDef = TypedDict(
     "GetInstanceMetricDataRequestRequestTypeDef",
     {
         "instanceName": str,
         "metricName": InstanceMetricNameType,
         "period": int,
         "startTime": Union[datetime, str],
@@ -1760,14 +1869,22 @@
 GetInstanceSnapshotRequestRequestTypeDef = TypedDict(
     "GetInstanceSnapshotRequestRequestTypeDef",
     {
         "instanceSnapshotName": str,
     },
 )
 
+GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef = TypedDict(
+    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetInstanceSnapshotsRequestRequestTypeDef = TypedDict(
     "GetInstanceSnapshotsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1784,14 +1901,22 @@
     {
         "code": int,
         "name": str,
     },
     total=False,
 )
 
+GetInstancesRequestGetInstancesPaginateTypeDef = TypedDict(
+    "GetInstancesRequestGetInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetInstancesRequestRequestTypeDef = TypedDict(
     "GetInstancesRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1799,14 +1924,23 @@
 GetKeyPairRequestRequestTypeDef = TypedDict(
     "GetKeyPairRequestRequestTypeDef",
     {
         "keyPairName": str,
     },
 )
 
+GetKeyPairsRequestGetKeyPairsPaginateTypeDef = TypedDict(
+    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
+    {
+        "includeDefaultKeyPair": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetKeyPairsRequestRequestTypeDef = TypedDict(
     "GetKeyPairsRequestRequestTypeDef",
     {
         "pageToken": str,
         "includeDefaultKeyPair": bool,
     },
     total=False,
@@ -1855,14 +1989,22 @@
         "description": str,
         "protocols": List[str],
         "ciphers": List[str],
     },
     total=False,
 )
 
+GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef = TypedDict(
+    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetLoadBalancersRequestRequestTypeDef = TypedDict(
     "GetLoadBalancersRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1884,20 +2026,30 @@
     "_OptionalGetOperationsForResourceRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
+
 class GetOperationsForResourceRequestRequestTypeDef(
     _RequiredGetOperationsForResourceRequestRequestTypeDef,
     _OptionalGetOperationsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
+GetOperationsRequestGetOperationsPaginateTypeDef = TypedDict(
+    "GetOperationsRequestGetOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetOperationsRequestRequestTypeDef = TypedDict(
     "GetOperationsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1907,14 +2059,22 @@
     {
         "includeAvailabilityZones": bool,
         "includeRelationalDatabaseAvailabilityZones": bool,
     },
     total=False,
 )
 
+GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef = TypedDict(
+    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetRelationalDatabaseBlueprintsRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseBlueprintsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1928,14 +2088,23 @@
         "engineDescription": str,
         "engineVersionDescription": str,
         "isEngineDefault": bool,
     },
     total=False,
 )
 
+GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef = TypedDict(
+    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
+    {
+        "includeInactive": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetRelationalDatabaseBundlesRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseBundlesRequestRequestTypeDef",
     {
         "pageToken": str,
         "includeInactive": bool,
     },
     total=False,
@@ -1953,14 +2122,37 @@
         "cpuCount": int,
         "isEncrypted": bool,
         "isActive": bool,
     },
     total=False,
 )
 
+_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
+    "_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
+    {
+        "relationalDatabaseName": str,
+    },
+)
+_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
+    "_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
+    {
+        "durationInMinutes": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef(
+    _RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
+    _OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetRelationalDatabaseEventsRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseEventsRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseEventsRequestRequestTypeDef = TypedDict(
@@ -1968,20 +2160,22 @@
     {
         "durationInMinutes": int,
         "pageToken": str,
     },
     total=False,
 )
 
+
 class GetRelationalDatabaseEventsRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseEventsRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseEventsRequestRequestTypeDef,
 ):
     pass
 
+
 RelationalDatabaseEventTypeDef = TypedDict(
     "RelationalDatabaseEventTypeDef",
     {
         "resource": str,
         "createdAt": datetime,
         "message": str,
         "eventCategories": List[str],
@@ -2003,20 +2197,22 @@
         "endTime": Union[datetime, str],
         "startFromHead": bool,
         "pageToken": str,
     },
     total=False,
 )
 
+
 class GetRelationalDatabaseLogEventsRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef,
 ):
     pass
 
+
 LogEventTypeDef = TypedDict(
     "LogEventTypeDef",
     {
         "createdAt": datetime,
         "message": str,
     },
     total=False,
@@ -2025,67 +2221,110 @@
 GetRelationalDatabaseLogStreamsRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseLogStreamsRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 
+GetRelationalDatabaseLogStreamsResultTypeDef = TypedDict(
+    "GetRelationalDatabaseLogStreamsResultTypeDef",
+    {
+        "logStreams": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef = TypedDict(
     "_OptionalGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
     {
         "passwordVersion": RelationalDatabasePasswordVersionType,
     },
     total=False,
 )
 
+
 class GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
 ):
     pass
 
+
+GetRelationalDatabaseMasterUserPasswordResultTypeDef = TypedDict(
+    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
+    {
+        "masterUserPassword": str,
+        "createdAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRelationalDatabaseMetricDataRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
         "metricName": RelationalDatabaseMetricNameType,
         "period": int,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
         "unit": MetricUnitType,
         "statistics": Sequence[MetricStatisticType],
     },
 )
 
+_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
+    "_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
+    {
+        "relationalDatabaseName": str,
+    },
+)
+_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
+    "_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef(
+    _RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
+    _OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseParametersRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
     "_OptionalGetRelationalDatabaseParametersRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
+
 class GetRelationalDatabaseParametersRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseParametersRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseParametersRequestRequestTypeDef,
 ):
     pass
 
+
 RelationalDatabaseParameterTypeDef = TypedDict(
     "RelationalDatabaseParameterTypeDef",
     {
         "allowedValues": str,
         "applyMethod": str,
         "applyType": str,
         "dataType": str,
@@ -2107,22 +2346,38 @@
 GetRelationalDatabaseSnapshotRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotRequestRequestTypeDef",
     {
         "relationalDatabaseSnapshotName": str,
     },
 )
 
+GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef = TypedDict(
+    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetRelationalDatabaseSnapshotsRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
+GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef = TypedDict(
+    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetRelationalDatabasesRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabasesRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2130,14 +2385,22 @@
 GetStaticIpRequestRequestTypeDef = TypedDict(
     "GetStaticIpRequestRequestTypeDef",
     {
         "staticIpName": str,
     },
 )
 
+GetStaticIpsRequestGetStaticIpsPaginateTypeDef = TypedDict(
+    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetStaticIpsRequestRequestTypeDef = TypedDict(
     "GetStaticIpsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2216,14 +2479,22 @@
     "MonthlyTransferTypeDef",
     {
         "gbPerMonthAllocated": int,
     },
     total=False,
 )
 
+IsVpcPeeredResultTypeDef = TypedDict(
+    "IsVpcPeeredResultTypeDef",
+    {
+        "isPeered": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OriginTypeDef = TypedDict(
     "OriginTypeDef",
     {
         "name": str,
         "resourceType": ResourceTypeType,
         "regionName": RegionNameType,
         "protocolPolicy": OriginProtocolPolicyEnumType,
@@ -2263,14 +2534,24 @@
     {
         "code": NameServersUpdateStateCodeType,
         "message": str,
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "action": str,
         "description": str,
         "currentApplyDate": datetime,
     },
@@ -2306,19 +2587,21 @@
         "contactProtocols": Sequence[ContactProtocolType],
         "notificationTriggers": Sequence[AlarmStateType],
         "notificationEnabled": bool,
     },
     total=False,
 )
 
+
 class PutAlarmRequestRequestTypeDef(
     _RequiredPutAlarmRequestRequestTypeDef, _OptionalPutAlarmRequestRequestTypeDef
 ):
     pass
 
+
 R53HostedZoneDeletionStateTypeDef = TypedDict(
     "R53HostedZoneDeletionStateTypeDef",
     {
         "code": R53HostedZoneDeletionStateCodeType,
         "message": str,
     },
     total=False,
@@ -2377,14 +2660,25 @@
     "ResetDistributionCacheRequestRequestTypeDef",
     {
         "distributionName": str,
     },
     total=False,
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
 SendContactMethodVerificationRequestRequestTypeDef = TypedDict(
     "SendContactMethodVerificationRequestRequestTypeDef",
     {
         "protocol": Literal["Email"],
     },
 )
 
@@ -2444,39 +2738,43 @@
     "_OptionalStopInstanceRequestRequestTypeDef",
     {
         "force": bool,
     },
     total=False,
 )
 
+
 class StopInstanceRequestRequestTypeDef(
     _RequiredStopInstanceRequestRequestTypeDef, _OptionalStopInstanceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStopRelationalDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredStopRelationalDatabaseRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalStopRelationalDatabaseRequestRequestTypeDef = TypedDict(
     "_OptionalStopRelationalDatabaseRequestRequestTypeDef",
     {
         "relationalDatabaseSnapshotName": str,
     },
     total=False,
 )
 
+
 class StopRelationalDatabaseRequestRequestTypeDef(
     _RequiredStopRelationalDatabaseRequestRequestTypeDef,
     _OptionalStopRelationalDatabaseRequestRequestTypeDef,
 ):
     pass
 
+
 TestAlarmRequestRequestTypeDef = TypedDict(
     "TestAlarmRequestRequestTypeDef",
     {
         "alarmName": str,
         "state": AlarmStateType,
     },
 )
@@ -2492,19 +2790,21 @@
     "_OptionalUntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
     total=False,
 )
 
+
 class UntagResourceRequestRequestTypeDef(
     _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
 ):
     pass
 
+
 UpdateBucketBundleRequestRequestTypeDef = TypedDict(
     "UpdateBucketBundleRequestRequestTypeDef",
     {
         "bucketName": str,
         "bundleId": str,
     },
 )
@@ -2531,20 +2831,22 @@
         "httpEndpoint": HttpEndpointType,
         "httpPutResponseHopLimit": int,
         "httpProtocolIpv6": HttpProtocolIpv6Type,
     },
     total=False,
 )
 
+
 class UpdateInstanceMetadataOptionsRequestRequestTypeDef(
     _RequiredUpdateInstanceMetadataOptionsRequestRequestTypeDef,
     _OptionalUpdateInstanceMetadataOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateLoadBalancerAttributeRequestRequestTypeDef = TypedDict(
     "UpdateLoadBalancerAttributeRequestRequestTypeDef",
     {
         "loadBalancerName": str,
         "attributeName": LoadBalancerAttributeNameType,
         "attributeValue": str,
     },
@@ -2568,20 +2870,22 @@
         "publiclyAccessible": bool,
         "applyImmediately": bool,
         "caCertificateIdentifier": str,
     },
     total=False,
 )
 
+
 class UpdateRelationalDatabaseRequestRequestTypeDef(
     _RequiredUpdateRelationalDatabaseRequestRequestTypeDef,
     _OptionalUpdateRelationalDatabaseRequestRequestTypeDef,
 ):
     pass
 
+
 AccessKeyTypeDef = TypedDict(
     "AccessKeyTypeDef",
     {
         "accessKeyId": str,
         "secretAccessKey": str,
         "status": StatusTypeType,
         "createdAt": datetime,
@@ -2601,17 +2905,19 @@
     {
         "autoSnapshotAddOnRequest": AutoSnapshotAddOnRequestTypeDef,
         "stopInstanceOnIdleRequest": StopInstanceOnIdleRequestTypeDef,
     },
     total=False,
 )
 
+
 class AddOnRequestTypeDef(_RequiredAddOnRequestTypeDef, _OptionalAddOnRequestTypeDef):
     pass
 
+
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "name": str,
         "arn": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
@@ -2682,75 +2988,14 @@
         "ipAddress": str,
         "attachedTo": str,
         "isAttached": bool,
     },
     total=False,
 )
 
-DownloadDefaultKeyPairResultTypeDef = TypedDict(
-    "DownloadDefaultKeyPairResultTypeDef",
-    {
-        "publicKeyBase64": str,
-        "privateKeyBase64": str,
-        "createdAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetActiveNamesResultTypeDef = TypedDict(
-    "GetActiveNamesResultTypeDef",
-    {
-        "activeNames": List[str],
-        "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetContainerAPIMetadataResultTypeDef = TypedDict(
-    "GetContainerAPIMetadataResultTypeDef",
-    {
-        "metadata": List[Dict[str, str]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDistributionLatestCacheResetResultTypeDef = TypedDict(
-    "GetDistributionLatestCacheResetResultTypeDef",
-    {
-        "status": str,
-        "createTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRelationalDatabaseLogStreamsResultTypeDef = TypedDict(
-    "GetRelationalDatabaseLogStreamsResultTypeDef",
-    {
-        "logStreams": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRelationalDatabaseMasterUserPasswordResultTypeDef = TypedDict(
-    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
-    {
-        "masterUserPassword": str,
-        "createdAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-IsVpcPeeredResultTypeDef = TypedDict(
-    "IsVpcPeeredResultTypeDef",
-    {
-        "isPeered": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AutoSnapshotDetailsTypeDef = TypedDict(
     "AutoSnapshotDetailsTypeDef",
     {
         "date": str,
         "createdAt": datetime,
         "status": AutoSnapshotStatusType,
         "fromAttachedDisks": List[AttachedDiskTypeDef],
@@ -2772,15 +3017,15 @@
 )
 
 GetBlueprintsResultTypeDef = TypedDict(
     "GetBlueprintsResultTypeDef",
     {
         "blueprints": List[BlueprintTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateBucketRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBucketRequestRequestTypeDef",
     {
         "bucketName": str,
@@ -2793,24 +3038,26 @@
         "versioning": str,
         "readonlyAccessAccounts": Sequence[str],
         "accessLogConfig": BucketAccessLogConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateBucketRequestRequestTypeDef(
     _RequiredUpdateBucketRequestRequestTypeDef, _OptionalUpdateBucketRequestRequestTypeDef
 ):
     pass
 
+
 GetBucketBundlesResultTypeDef = TypedDict(
     "GetBucketBundlesResultTypeDef",
     {
         "bundles": List[BucketBundleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "resourceType": str,
@@ -2845,19 +3092,21 @@
     {
         "tags": Sequence[TagTypeDef],
         "enableObjectVersioning": bool,
     },
     total=False,
 )
 
+
 class CreateBucketRequestRequestTypeDef(
     _RequiredCreateBucketRequestRequestTypeDef, _OptionalCreateBucketRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCertificateRequestRequestTypeDef",
     {
         "certificateName": str,
         "domainName": str,
     },
 )
@@ -2866,19 +3115,21 @@
     {
         "subjectAlternativeNames": Sequence[str],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCertificateRequestRequestTypeDef(
     _RequiredCreateCertificateRequestRequestTypeDef, _OptionalCreateCertificateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateDiskSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDiskSnapshotRequestRequestTypeDef",
     {
         "diskSnapshotName": str,
     },
 )
 _OptionalCreateDiskSnapshotRequestRequestTypeDef = TypedDict(
@@ -2887,39 +3138,43 @@
         "diskName": str,
         "instanceName": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDiskSnapshotRequestRequestTypeDef(
     _RequiredCreateDiskSnapshotRequestRequestTypeDef,
     _OptionalCreateDiskSnapshotRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 _OptionalCreateDomainRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDomainRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateInstanceSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstanceSnapshotRequestRequestTypeDef",
     {
         "instanceSnapshotName": str,
         "instanceName": str,
     },
 )
@@ -2927,39 +3182,43 @@
     "_OptionalCreateInstanceSnapshotRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateInstanceSnapshotRequestRequestTypeDef(
     _RequiredCreateInstanceSnapshotRequestRequestTypeDef,
     _OptionalCreateInstanceSnapshotRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateKeyPairRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKeyPairRequestRequestTypeDef",
     {
         "keyPairName": str,
     },
 )
 _OptionalCreateKeyPairRequestRequestTypeDef = TypedDict(
     "_OptionalCreateKeyPairRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateKeyPairRequestRequestTypeDef(
     _RequiredCreateKeyPairRequestRequestTypeDef, _OptionalCreateKeyPairRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateLoadBalancerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoadBalancerRequestRequestTypeDef",
     {
         "loadBalancerName": str,
         "instancePort": int,
     },
 )
@@ -2973,20 +3232,22 @@
         "tags": Sequence[TagTypeDef],
         "ipAddressType": IpAddressTypeType,
         "tlsPolicyName": str,
     },
     total=False,
 )
 
+
 class CreateLoadBalancerRequestRequestTypeDef(
     _RequiredCreateLoadBalancerRequestRequestTypeDef,
     _OptionalCreateLoadBalancerRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef",
     {
         "loadBalancerName": str,
         "certificateName": str,
         "certificateDomainName": str,
     },
@@ -2996,20 +3257,22 @@
     {
         "certificateAlternativeNames": Sequence[str],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateLoadBalancerTlsCertificateRequestRequestTypeDef(
     _RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef,
     _OptionalCreateLoadBalancerTlsCertificateRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
@@ -3023,20 +3286,22 @@
         "restoreTime": Union[datetime, str],
         "useLatestRestorableTime": bool,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef(
     _RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
     _OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateRelationalDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRelationalDatabaseRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
         "relationalDatabaseBlueprintId": str,
         "relationalDatabaseBundleId": str,
         "masterDatabaseName": str,
@@ -3052,20 +3317,22 @@
         "preferredMaintenanceWindow": str,
         "publiclyAccessible": bool,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRelationalDatabaseRequestRequestTypeDef(
     _RequiredCreateRelationalDatabaseRequestRequestTypeDef,
     _OptionalCreateRelationalDatabaseRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
         "relationalDatabaseSnapshotName": str,
     },
 )
@@ -3073,20 +3340,22 @@
     "_OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRelationalDatabaseSnapshotRequestRequestTypeDef(
     _RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     _OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
 ):
     pass
 
+
 DiskSnapshotTypeDef = TypedDict(
     "DiskSnapshotTypeDef",
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
@@ -3178,25 +3447,27 @@
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
     total=False,
 )
 
+
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
+
 GetBundlesResultTypeDef = TypedDict(
     "GetBundlesResultTypeDef",
     {
         "bundles": List[BundleTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CacheSettingsTypeDef = TypedDict(
     "CacheSettingsTypeDef",
     {
         "defaultTTL": int,
@@ -3250,23 +3521,23 @@
     total=False,
 )
 
 GetContainerImagesResultTypeDef = TypedDict(
     "GetContainerImagesResultTypeDef",
     {
         "containerImages": List[ContainerImageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterContainerImageResultTypeDef = TypedDict(
     "RegisterContainerImageResultTypeDef",
     {
         "containerImage": ContainerImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PrivateRegistryAccessRequestTypeDef = TypedDict(
     "PrivateRegistryAccessRequestTypeDef",
     {
         "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
@@ -3303,39 +3574,41 @@
     "_OptionalEndpointRequestTypeDef",
     {
         "healthCheck": ContainerServiceHealthCheckConfigTypeDef,
     },
     total=False,
 )
 
+
 class EndpointRequestTypeDef(_RequiredEndpointRequestTypeDef, _OptionalEndpointRequestTypeDef):
     pass
 
+
 GetContainerLogResultTypeDef = TypedDict(
     "GetContainerLogResultTypeDef",
     {
         "logEvents": List[ContainerServiceLogEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContainerServicePowersResultTypeDef = TypedDict(
     "GetContainerServicePowersResultTypeDef",
     {
         "powers": List[ContainerServicePowerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateContainerServiceRegistryLoginResultTypeDef = TypedDict(
     "CreateContainerServiceRegistryLoginResultTypeDef",
     {
         "registryLogin": ContainerServiceRegistryLoginTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCloudFormationStackRequestRequestTypeDef = TypedDict(
     "CreateCloudFormationStackRequestRequestTypeDef",
     {
         "instances": Sequence[InstanceEntryTypeDef],
@@ -3370,15 +3643,15 @@
     "CreateGUISessionAccessDetailsResultTypeDef",
     {
         "resourceName": str,
         "status": StatusType,
         "percentageComplete": int,
         "failureReason": str,
         "sessions": List[SessionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceSnapshotInfoTypeDef = TypedDict(
     "InstanceSnapshotInfoTypeDef",
     {
         "fromBundleId": str,
@@ -3388,15 +3661,15 @@
     total=False,
 )
 
 GetDistributionBundlesResultTypeDef = TypedDict(
     "GetDistributionBundlesResultTypeDef",
     {
         "bundles": List[DistributionBundleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainValidationRecordTypeDef = TypedDict(
     "DomainValidationRecordTypeDef",
     {
         "domainName": str,
@@ -3415,327 +3688,136 @@
         "unit": float,
         "currency": Literal["USD"],
         "timePeriod": TimePeriodTypeDef,
     },
     total=False,
 )
 
-GetActiveNamesRequestGetActiveNamesPaginateTypeDef = TypedDict(
-    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetBlueprintsRequestGetBlueprintsPaginateTypeDef = TypedDict(
-    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
-    {
-        "includeInactive": bool,
-        "appCategory": Literal["LfR"],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetBundlesRequestGetBundlesPaginateTypeDef = TypedDict(
-    "GetBundlesRequestGetBundlesPaginateTypeDef",
-    {
-        "includeInactive": bool,
-        "appCategory": Literal["LfR"],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef = TypedDict(
-    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef = TypedDict(
-    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetDisksRequestGetDisksPaginateTypeDef = TypedDict(
-    "GetDisksRequestGetDisksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetDomainsRequestGetDomainsPaginateTypeDef = TypedDict(
-    "GetDomainsRequestGetDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef = TypedDict(
-    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef = TypedDict(
-    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetInstancesRequestGetInstancesPaginateTypeDef = TypedDict(
-    "GetInstancesRequestGetInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetKeyPairsRequestGetKeyPairsPaginateTypeDef = TypedDict(
-    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
-    {
-        "includeDefaultKeyPair": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef = TypedDict(
-    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetOperationsRequestGetOperationsPaginateTypeDef = TypedDict(
-    "GetOperationsRequestGetOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef = TypedDict(
-    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef = TypedDict(
-    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
-    {
-        "includeInactive": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
-    "_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
-    {
-        "relationalDatabaseName": str,
-    },
-)
-_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
-    "_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
-    {
-        "durationInMinutes": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef(
-    _RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
-    _OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
-):
-    pass
-
-_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
-    "_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
-    {
-        "relationalDatabaseName": str,
-    },
-)
-_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
-    "_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef(
-    _RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
-    _OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
-):
-    pass
-
-GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef = TypedDict(
-    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef = TypedDict(
-    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetStaticIpsRequestGetStaticIpsPaginateTypeDef = TypedDict(
-    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetBucketMetricDataResultTypeDef = TypedDict(
     "GetBucketMetricDataResultTypeDef",
     {
         "metricName": BucketMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContainerServiceMetricDataResultTypeDef = TypedDict(
     "GetContainerServiceMetricDataResultTypeDef",
     {
         "metricName": ContainerServiceMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDistributionMetricDataResultTypeDef = TypedDict(
     "GetDistributionMetricDataResultTypeDef",
     {
         "metricName": DistributionMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstanceMetricDataResultTypeDef = TypedDict(
     "GetInstanceMetricDataResultTypeDef",
     {
         "metricName": InstanceMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLoadBalancerMetricDataResultTypeDef = TypedDict(
     "GetLoadBalancerMetricDataResultTypeDef",
     {
         "metricName": LoadBalancerMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseMetricDataResultTypeDef = TypedDict(
     "GetRelationalDatabaseMetricDataResultTypeDef",
     {
         "metricName": RelationalDatabaseMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstancePortStatesResultTypeDef = TypedDict(
     "GetInstancePortStatesResultTypeDef",
     {
         "portStates": List[InstancePortStateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstanceStateResultTypeDef = TypedDict(
     "GetInstanceStateResultTypeDef",
     {
         "state": InstanceStateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLoadBalancerTlsPoliciesResultTypeDef = TypedDict(
     "GetLoadBalancerTlsPoliciesResultTypeDef",
     {
         "tlsPolicies": List[LoadBalancerTlsPolicyTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseBlueprintsResultTypeDef = TypedDict(
     "GetRelationalDatabaseBlueprintsResultTypeDef",
     {
         "blueprints": List[RelationalDatabaseBlueprintTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseBundlesResultTypeDef = TypedDict(
     "GetRelationalDatabaseBundlesResultTypeDef",
     {
         "bundles": List[RelationalDatabaseBundleTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseEventsResultTypeDef = TypedDict(
     "GetRelationalDatabaseEventsResultTypeDef",
     {
         "relationalDatabaseEvents": List[RelationalDatabaseEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseLogEventsResultTypeDef = TypedDict(
     "GetRelationalDatabaseLogEventsResultTypeDef",
     {
         "resourceLogEvents": List[LogEventTypeDef],
         "nextBackwardToken": str,
         "nextForwardToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseParametersResultTypeDef = TypedDict(
     "GetRelationalDatabaseParametersResultTypeDef",
     {
         "parameters": List[RelationalDatabaseParameterTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
     "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
@@ -3859,15 +3941,15 @@
     total=False,
 )
 
 GetBucketAccessKeysResultTypeDef = TypedDict(
     "GetBucketAccessKeysResultTypeDef",
     {
         "accessKeys": List[AccessKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDiskFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDiskFromSnapshotRequestRequestTypeDef",
     {
         "diskName": str,
@@ -3884,20 +3966,22 @@
         "sourceDiskName": str,
         "restoreDate": str,
         "useLatestRestorableAutoSnapshot": bool,
     },
     total=False,
 )
 
+
 class CreateDiskFromSnapshotRequestRequestTypeDef(
     _RequiredCreateDiskFromSnapshotRequestRequestTypeDef,
     _OptionalCreateDiskFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDiskRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDiskRequestRequestTypeDef",
     {
         "diskName": str,
         "availabilityZone": str,
         "sizeInGb": int,
     },
@@ -3907,19 +3991,21 @@
     {
         "tags": Sequence[TagTypeDef],
         "addOns": Sequence[AddOnRequestTypeDef],
     },
     total=False,
 )
 
+
 class CreateDiskRequestRequestTypeDef(
     _RequiredCreateDiskRequestRequestTypeDef, _OptionalCreateDiskRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateInstancesFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstancesFromSnapshotRequestRequestTypeDef",
     {
         "instanceNames": Sequence[str],
         "availabilityZone": str,
         "bundleId": str,
     },
@@ -3937,20 +4023,22 @@
         "sourceInstanceName": str,
         "restoreDate": str,
         "useLatestRestorableAutoSnapshot": bool,
     },
     total=False,
 )
 
+
 class CreateInstancesFromSnapshotRequestRequestTypeDef(
     _RequiredCreateInstancesFromSnapshotRequestRequestTypeDef,
     _OptionalCreateInstancesFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstancesRequestRequestTypeDef",
     {
         "instanceNames": Sequence[str],
         "availabilityZone": str,
         "blueprintId": str,
         "bundleId": str,
@@ -3965,808 +4053,810 @@
         "tags": Sequence[TagTypeDef],
         "addOns": Sequence[AddOnRequestTypeDef],
         "ipAddressType": IpAddressTypeType,
     },
     total=False,
 )
 
+
 class CreateInstancesRequestRequestTypeDef(
     _RequiredCreateInstancesRequestRequestTypeDef, _OptionalCreateInstancesRequestRequestTypeDef
 ):
     pass
 
+
 EnableAddOnRequestRequestTypeDef = TypedDict(
     "EnableAddOnRequestRequestTypeDef",
     {
         "resourceName": str,
         "addOnRequest": AddOnRequestTypeDef,
     },
 )
 
 GetAlarmsResultTypeDef = TypedDict(
     "GetAlarmsResultTypeDef",
     {
         "alarms": List[AlarmTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContactMethodsResultTypeDef = TypedDict(
     "GetContactMethodsResultTypeDef",
     {
         "contactMethods": List[ContactMethodTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AllocateStaticIpResultTypeDef = TypedDict(
     "AllocateStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachCertificateToDistributionResultTypeDef = TypedDict(
     "AttachCertificateToDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachDiskResultTypeDef = TypedDict(
     "AttachDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachInstancesToLoadBalancerResultTypeDef = TypedDict(
     "AttachInstancesToLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachLoadBalancerTlsCertificateResultTypeDef = TypedDict(
     "AttachLoadBalancerTlsCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachStaticIpResultTypeDef = TypedDict(
     "AttachStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CloseInstancePublicPortsResultTypeDef = TypedDict(
     "CloseInstancePublicPortsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CopySnapshotResultTypeDef = TypedDict(
     "CopySnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBucketAccessKeyResultTypeDef = TypedDict(
     "CreateBucketAccessKeyResultTypeDef",
     {
         "accessKey": AccessKeyTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCloudFormationStackResultTypeDef = TypedDict(
     "CreateCloudFormationStackResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateContactMethodResultTypeDef = TypedDict(
     "CreateContactMethodResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDiskFromSnapshotResultTypeDef = TypedDict(
     "CreateDiskFromSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDiskResultTypeDef = TypedDict(
     "CreateDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDiskSnapshotResultTypeDef = TypedDict(
     "CreateDiskSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDomainEntryResultTypeDef = TypedDict(
     "CreateDomainEntryResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDomainResultTypeDef = TypedDict(
     "CreateDomainResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInstanceSnapshotResultTypeDef = TypedDict(
     "CreateInstanceSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInstancesFromSnapshotResultTypeDef = TypedDict(
     "CreateInstancesFromSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInstancesResultTypeDef = TypedDict(
     "CreateInstancesResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateLoadBalancerResultTypeDef = TypedDict(
     "CreateLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateLoadBalancerTlsCertificateResultTypeDef = TypedDict(
     "CreateLoadBalancerTlsCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRelationalDatabaseFromSnapshotResultTypeDef = TypedDict(
     "CreateRelationalDatabaseFromSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRelationalDatabaseResultTypeDef = TypedDict(
     "CreateRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRelationalDatabaseSnapshotResultTypeDef = TypedDict(
     "CreateRelationalDatabaseSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAlarmResultTypeDef = TypedDict(
     "DeleteAlarmResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAutoSnapshotResultTypeDef = TypedDict(
     "DeleteAutoSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteBucketAccessKeyResultTypeDef = TypedDict(
     "DeleteBucketAccessKeyResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteBucketResultTypeDef = TypedDict(
     "DeleteBucketResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCertificateResultTypeDef = TypedDict(
     "DeleteCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteContactMethodResultTypeDef = TypedDict(
     "DeleteContactMethodResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDiskResultTypeDef = TypedDict(
     "DeleteDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDiskSnapshotResultTypeDef = TypedDict(
     "DeleteDiskSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDistributionResultTypeDef = TypedDict(
     "DeleteDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDomainEntryResultTypeDef = TypedDict(
     "DeleteDomainEntryResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDomainResultTypeDef = TypedDict(
     "DeleteDomainResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInstanceResultTypeDef = TypedDict(
     "DeleteInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInstanceSnapshotResultTypeDef = TypedDict(
     "DeleteInstanceSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteKeyPairResultTypeDef = TypedDict(
     "DeleteKeyPairResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteKnownHostKeysResultTypeDef = TypedDict(
     "DeleteKnownHostKeysResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteLoadBalancerResultTypeDef = TypedDict(
     "DeleteLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteLoadBalancerTlsCertificateResultTypeDef = TypedDict(
     "DeleteLoadBalancerTlsCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRelationalDatabaseResultTypeDef = TypedDict(
     "DeleteRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRelationalDatabaseSnapshotResultTypeDef = TypedDict(
     "DeleteRelationalDatabaseSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetachCertificateFromDistributionResultTypeDef = TypedDict(
     "DetachCertificateFromDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetachDiskResultTypeDef = TypedDict(
     "DetachDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetachInstancesFromLoadBalancerResultTypeDef = TypedDict(
     "DetachInstancesFromLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetachStaticIpResultTypeDef = TypedDict(
     "DetachStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisableAddOnResultTypeDef = TypedDict(
     "DisableAddOnResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnableAddOnResultTypeDef = TypedDict(
     "EnableAddOnResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportSnapshotResultTypeDef = TypedDict(
     "ExportSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOperationResultTypeDef = TypedDict(
     "GetOperationResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOperationsForResourceResultTypeDef = TypedDict(
     "GetOperationsForResourceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "nextPageCount": str,
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOperationsResultTypeDef = TypedDict(
     "GetOperationsResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportKeyPairResultTypeDef = TypedDict(
     "ImportKeyPairResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OpenInstancePublicPortsResultTypeDef = TypedDict(
     "OpenInstancePublicPortsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PeerVpcResultTypeDef = TypedDict(
     "PeerVpcResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAlarmResultTypeDef = TypedDict(
     "PutAlarmResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutInstancePublicPortsResultTypeDef = TypedDict(
     "PutInstancePublicPortsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootInstanceResultTypeDef = TypedDict(
     "RebootInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootRelationalDatabaseResultTypeDef = TypedDict(
     "RebootRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReleaseStaticIpResultTypeDef = TypedDict(
     "ReleaseStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetDistributionCacheResultTypeDef = TypedDict(
     "ResetDistributionCacheResultTypeDef",
     {
         "status": str,
         "createTime": datetime,
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendContactMethodVerificationResultTypeDef = TypedDict(
     "SendContactMethodVerificationResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetIpAddressTypeResultTypeDef = TypedDict(
     "SetIpAddressTypeResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetResourceAccessForBucketResultTypeDef = TypedDict(
     "SetResourceAccessForBucketResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartGUISessionResultTypeDef = TypedDict(
     "StartGUISessionResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartInstanceResultTypeDef = TypedDict(
     "StartInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartRelationalDatabaseResultTypeDef = TypedDict(
     "StartRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopGUISessionResultTypeDef = TypedDict(
     "StopGUISessionResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopInstanceResultTypeDef = TypedDict(
     "StopInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopRelationalDatabaseResultTypeDef = TypedDict(
     "StopRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceResultTypeDef = TypedDict(
     "TagResourceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestAlarmResultTypeDef = TypedDict(
     "TestAlarmResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UnpeerVpcResultTypeDef = TypedDict(
     "UnpeerVpcResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UntagResourceResultTypeDef = TypedDict(
     "UntagResourceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBucketBundleResultTypeDef = TypedDict(
     "UpdateBucketBundleResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDistributionBundleResultTypeDef = TypedDict(
     "UpdateDistributionBundleResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDistributionResultTypeDef = TypedDict(
     "UpdateDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainEntryResultTypeDef = TypedDict(
     "UpdateDomainEntryResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInstanceMetadataOptionsResultTypeDef = TypedDict(
     "UpdateInstanceMetadataOptionsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLoadBalancerAttributeResultTypeDef = TypedDict(
     "UpdateLoadBalancerAttributeResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRelationalDatabaseParametersResultTypeDef = TypedDict(
     "UpdateRelationalDatabaseParametersResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRelationalDatabaseResultTypeDef = TypedDict(
     "UpdateRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStaticIpResultTypeDef = TypedDict(
     "GetStaticIpResultTypeDef",
     {
         "staticIp": StaticIpTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStaticIpsResultTypeDef = TypedDict(
     "GetStaticIpsResultTypeDef",
     {
         "staticIps": List[StaticIpTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAutoSnapshotsResultTypeDef = TypedDict(
     "GetAutoSnapshotsResultTypeDef",
     {
         "resourceName": str,
         "resourceType": ResourceTypeType,
         "autoSnapshots": List[AutoSnapshotDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRegionsResultTypeDef = TypedDict(
     "GetRegionsResultTypeDef",
     {
         "regions": List[RegionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBucketResultTypeDef = TypedDict(
     "CreateBucketResultTypeDef",
     {
         "bucket": BucketTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBucketsResultTypeDef = TypedDict(
     "GetBucketsResultTypeDef",
     {
         "buckets": List[BucketTypeDef],
         "nextPageToken": str,
         "accountLevelBpaSync": AccountLevelBpaSyncTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBucketResultTypeDef = TypedDict(
     "UpdateBucketResultTypeDef",
     {
         "bucket": BucketTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDiskSnapshotResultTypeDef = TypedDict(
     "GetDiskSnapshotResultTypeDef",
     {
         "diskSnapshot": DiskSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDiskSnapshotsResultTypeDef = TypedDict(
     "GetDiskSnapshotsResultTypeDef",
     {
         "diskSnapshots": List[DiskSnapshotTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDiskResultTypeDef = TypedDict(
     "GetDiskResultTypeDef",
     {
         "disk": DiskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDisksResultTypeDef = TypedDict(
     "GetDisksResultTypeDef",
     {
         "disks": List[DiskTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceHardwareTypeDef = TypedDict(
     "InstanceHardwareTypeDef",
     {
         "cpuCount": int,
@@ -4802,49 +4892,49 @@
 CreateKeyPairResultTypeDef = TypedDict(
     "CreateKeyPairResultTypeDef",
     {
         "keyPair": KeyPairTypeDef,
         "publicKeyBase64": str,
         "privateKeyBase64": str,
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKeyPairResultTypeDef = TypedDict(
     "GetKeyPairResultTypeDef",
     {
         "keyPair": KeyPairTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKeyPairsResultTypeDef = TypedDict(
     "GetKeyPairsResultTypeDef",
     {
         "keyPairs": List[KeyPairTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseSnapshotResultTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotResultTypeDef",
     {
         "relationalDatabaseSnapshot": RelationalDatabaseSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseSnapshotsResultTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotsResultTypeDef",
     {
         "relationalDatabaseSnapshots": List[RelationalDatabaseSnapshotTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
@@ -4860,20 +4950,22 @@
         "cacheBehaviors": Sequence[CacheBehaviorPerPathTypeDef],
         "ipAddressType": IpAddressTypeType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDistributionRequestRequestTypeDef(
     _RequiredCreateDistributionRequestRequestTypeDef,
     _OptionalCreateDistributionRequestRequestTypeDef,
 ):
     pass
 
+
 LightsailDistributionTypeDef = TypedDict(
     "LightsailDistributionTypeDef",
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
@@ -4911,26 +5003,28 @@
         "cacheBehaviorSettings": CacheSettingsTypeDef,
         "cacheBehaviors": Sequence[CacheBehaviorPerPathTypeDef],
         "isEnabled": bool,
     },
     total=False,
 )
 
+
 class UpdateDistributionRequestRequestTypeDef(
     _RequiredUpdateDistributionRequestRequestTypeDef,
     _OptionalUpdateDistributionRequestRequestTypeDef,
 ):
     pass
 
+
 GetCloudFormationStackRecordsResultTypeDef = TypedDict(
     "GetCloudFormationStackRecordsResultTypeDef",
     {
         "cloudFormationStackRecords": List[CloudFormationStackRecordTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateContainerServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContainerServiceRequestRequestTypeDef",
     {
         "serviceName": str,
@@ -4944,20 +5038,22 @@
         "isDisabled": bool,
         "publicDomainNames": Mapping[str, Sequence[str]],
         "privateRegistryAccess": PrivateRegistryAccessRequestTypeDef,
     },
     total=False,
 )
 
+
 class UpdateContainerServiceRequestRequestTypeDef(
     _RequiredUpdateContainerServiceRequestRequestTypeDef,
     _OptionalUpdateContainerServiceRequestRequestTypeDef,
 ):
     pass
 
+
 ContainerServiceDeploymentTypeDef = TypedDict(
     "ContainerServiceDeploymentTypeDef",
     {
         "version": int,
         "state": ContainerServiceDeploymentStateType,
         "containers": Dict[str, ContainerTypeDef],
         "publicEndpoint": ContainerServiceEndpointTypeDef,
@@ -4986,20 +5082,22 @@
     {
         "containers": Mapping[str, ContainerTypeDef],
         "publicEndpoint": EndpointRequestTypeDef,
     },
     total=False,
 )
 
+
 class CreateContainerServiceDeploymentRequestRequestTypeDef(
     _RequiredCreateContainerServiceDeploymentRequestRequestTypeDef,
     _OptionalCreateContainerServiceDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 ExportSnapshotRecordSourceInfoTypeDef = TypedDict(
     "ExportSnapshotRecordSourceInfoTypeDef",
     {
         "resourceType": ExportSnapshotRecordSourceTypeType,
         "createdAt": datetime,
         "name": str,
         "arn": str,
@@ -5031,15 +5129,15 @@
     total=False,
 )
 
 GetInstanceAccessDetailsResultTypeDef = TypedDict(
     "GetInstanceAccessDetailsResultTypeDef",
     {
         "accessDetails": InstanceAccessDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoadBalancerTlsCertificateTypeDef = TypedDict(
     "LoadBalancerTlsCertificateTypeDef",
     {
         "name": str,
@@ -5071,24 +5169,24 @@
     total=False,
 )
 
 GetLoadBalancerResultTypeDef = TypedDict(
     "GetLoadBalancerResultTypeDef",
     {
         "loadBalancer": LoadBalancerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLoadBalancersResultTypeDef = TypedDict(
     "GetLoadBalancersResultTypeDef",
     {
         "loadBalancers": List[LoadBalancerTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainTypeDef = TypedDict(
     "DomainTypeDef",
     {
         "name": str,
@@ -5104,24 +5202,24 @@
     total=False,
 )
 
 GetRelationalDatabaseResultTypeDef = TypedDict(
     "GetRelationalDatabaseResultTypeDef",
     {
         "relationalDatabase": RelationalDatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabasesResultTypeDef = TypedDict(
     "GetRelationalDatabasesResultTypeDef",
     {
         "relationalDatabases": List[RelationalDatabaseTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "name": str,
@@ -5150,42 +5248,42 @@
     total=False,
 )
 
 GetInstanceSnapshotResultTypeDef = TypedDict(
     "GetInstanceSnapshotResultTypeDef",
     {
         "instanceSnapshot": InstanceSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstanceSnapshotsResultTypeDef = TypedDict(
     "GetInstanceSnapshotsResultTypeDef",
     {
         "instanceSnapshots": List[InstanceSnapshotTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDistributionResultTypeDef = TypedDict(
     "CreateDistributionResultTypeDef",
     {
         "distribution": LightsailDistributionTypeDef,
         "operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDistributionsResultTypeDef = TypedDict(
     "GetDistributionsResultTypeDef",
     {
         "distributions": List[LightsailDistributionTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ContainerServiceTypeDef = TypedDict(
     "ContainerServiceTypeDef",
     {
         "containerServiceName": str,
@@ -5211,15 +5309,15 @@
     total=False,
 )
 
 GetContainerServiceDeploymentsResultTypeDef = TypedDict(
     "GetContainerServiceDeploymentsResultTypeDef",
     {
         "deployments": List[ContainerServiceDeploymentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateContainerServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerServiceRequestRequestTypeDef",
     {
         "serviceName": str,
@@ -5234,20 +5332,22 @@
         "publicDomainNames": Mapping[str, Sequence[str]],
         "deployment": ContainerServiceDeploymentRequestTypeDef,
         "privateRegistryAccess": PrivateRegistryAccessRequestTypeDef,
     },
     total=False,
 )
 
+
 class CreateContainerServiceRequestRequestTypeDef(
     _RequiredCreateContainerServiceRequestRequestTypeDef,
     _OptionalCreateContainerServiceRequestRequestTypeDef,
 ):
     pass
 
+
 ExportSnapshotRecordTypeDef = TypedDict(
     "ExportSnapshotRecordTypeDef",
     {
         "name": str,
         "arn": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
@@ -5299,90 +5399,90 @@
     total=False,
 )
 
 GetLoadBalancerTlsCertificatesResultTypeDef = TypedDict(
     "GetLoadBalancerTlsCertificatesResultTypeDef",
     {
         "tlsCertificates": List[LoadBalancerTlsCertificateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainResultTypeDef = TypedDict(
     "GetDomainResultTypeDef",
     {
         "domain": DomainTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainsResultTypeDef = TypedDict(
     "GetDomainsResultTypeDef",
     {
         "domains": List[DomainTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstanceResultTypeDef = TypedDict(
     "GetInstanceResultTypeDef",
     {
         "instance": InstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInstancesResultTypeDef = TypedDict(
     "GetInstancesResultTypeDef",
     {
         "instances": List[InstanceTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ContainerServicesListResultTypeDef = TypedDict(
     "ContainerServicesListResultTypeDef",
     {
         "containerServices": List[ContainerServiceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateContainerServiceDeploymentResultTypeDef = TypedDict(
     "CreateContainerServiceDeploymentResultTypeDef",
     {
         "containerService": ContainerServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateContainerServiceResultTypeDef = TypedDict(
     "CreateContainerServiceResultTypeDef",
     {
         "containerService": ContainerServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContainerServiceResultTypeDef = TypedDict(
     "UpdateContainerServiceResultTypeDef",
     {
         "containerService": ContainerServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExportSnapshotRecordsResultTypeDef = TypedDict(
     "GetExportSnapshotRecordsResultTypeDef",
     {
         "exportSnapshotRecords": List[ExportSnapshotRecordTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "certificateArn": str,
@@ -5394,27 +5494,28 @@
     total=False,
 )
 
 GetCostEstimateResultTypeDef = TypedDict(
     "GetCostEstimateResultTypeDef",
     {
         "resourcesBudgetEstimate": List[ResourceBudgetEstimateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCertificateResultTypeDef = TypedDict(
     "CreateCertificateResultTypeDef",
     {
         "certificate": CertificateSummaryTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCertificatesResultTypeDef = TypedDict(
     "GetCertificatesResultTypeDef",
     {
         "certificates": List[CertificateSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "nextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/PKG-INFO` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.26.81
-Summary: Type annotations for boto3.Lightsail 1.26.81 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.Lightsail 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-lightsail"></a>
 
 # mypy-boto3-lightsail
 
 [![PyPI - mypy-boto3-lightsail](https://img.shields.io/pypi/v/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lightsail?color=blue)](https://pypistats.org/packages/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -482,15 +482,14 @@
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
     StopInstanceOnIdleRequestTypeDef,
     AddOnTypeDef,
     MonitoredResourceInfoTypeDef,
     ResourceLocationTypeDef,
     AllocateStaticIpRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AttachCertificateToDistributionRequestRequestTypeDef,
     AttachDiskRequestRequestTypeDef,
     AttachInstancesToLoadBalancerRequestRequestTypeDef,
     AttachLoadBalancerTlsCertificateRequestRequestTypeDef,
     AttachStaticIpRequestRequestTypeDef,
     AttachedDiskTypeDef,
     AvailabilityZoneTypeDef,
@@ -553,110 +552,138 @@
     DetachStaticIpRequestRequestTypeDef,
     DisableAddOnRequestRequestTypeDef,
     DiskInfoTypeDef,
     DiskSnapshotInfoTypeDef,
     DistributionBundleTypeDef,
     DnsRecordCreationStateTypeDef,
     ResourceRecordTypeDef,
+    DownloadDefaultKeyPairResultTypeDef,
     TimePeriodTypeDef,
     ExportSnapshotRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
     GetActiveNamesRequestRequestTypeDef,
+    GetActiveNamesResultTypeDef,
     GetAlarmsRequestRequestTypeDef,
     GetAutoSnapshotsRequestRequestTypeDef,
+    GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
     GetBlueprintsRequestRequestTypeDef,
     GetBucketAccessKeysRequestRequestTypeDef,
     GetBucketBundlesRequestRequestTypeDef,
     GetBucketMetricDataRequestRequestTypeDef,
     MetricDatapointTypeDef,
     GetBucketsRequestRequestTypeDef,
+    GetBundlesRequestGetBundlesPaginateTypeDef,
     GetBundlesRequestRequestTypeDef,
     GetCertificatesRequestRequestTypeDef,
+    GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
     GetCloudFormationStackRecordsRequestRequestTypeDef,
     GetContactMethodsRequestRequestTypeDef,
+    GetContainerAPIMetadataResultTypeDef,
     GetContainerImagesRequestRequestTypeDef,
     GetContainerLogRequestRequestTypeDef,
     GetContainerServiceDeploymentsRequestRequestTypeDef,
     GetContainerServiceMetricDataRequestRequestTypeDef,
     GetContainerServicesRequestRequestTypeDef,
     GetCostEstimateRequestRequestTypeDef,
     GetDiskRequestRequestTypeDef,
     GetDiskSnapshotRequestRequestTypeDef,
+    GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
     GetDiskSnapshotsRequestRequestTypeDef,
+    GetDisksRequestGetDisksPaginateTypeDef,
     GetDisksRequestRequestTypeDef,
     GetDistributionLatestCacheResetRequestRequestTypeDef,
+    GetDistributionLatestCacheResetResultTypeDef,
     GetDistributionMetricDataRequestRequestTypeDef,
     GetDistributionsRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
+    GetDomainsRequestGetDomainsPaginateTypeDef,
     GetDomainsRequestRequestTypeDef,
+    GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef,
     GetExportSnapshotRecordsRequestRequestTypeDef,
     GetInstanceAccessDetailsRequestRequestTypeDef,
     GetInstanceMetricDataRequestRequestTypeDef,
     GetInstancePortStatesRequestRequestTypeDef,
     InstancePortStateTypeDef,
     GetInstanceRequestRequestTypeDef,
     GetInstanceSnapshotRequestRequestTypeDef,
+    GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef,
     GetInstanceSnapshotsRequestRequestTypeDef,
     GetInstanceStateRequestRequestTypeDef,
     InstanceStateTypeDef,
+    GetInstancesRequestGetInstancesPaginateTypeDef,
     GetInstancesRequestRequestTypeDef,
     GetKeyPairRequestRequestTypeDef,
+    GetKeyPairsRequestGetKeyPairsPaginateTypeDef,
     GetKeyPairsRequestRequestTypeDef,
     GetLoadBalancerMetricDataRequestRequestTypeDef,
     GetLoadBalancerRequestRequestTypeDef,
     GetLoadBalancerTlsCertificatesRequestRequestTypeDef,
     GetLoadBalancerTlsPoliciesRequestRequestTypeDef,
     LoadBalancerTlsPolicyTypeDef,
+    GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef,
     GetLoadBalancersRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     GetOperationsForResourceRequestRequestTypeDef,
+    GetOperationsRequestGetOperationsPaginateTypeDef,
     GetOperationsRequestRequestTypeDef,
     GetRegionsRequestRequestTypeDef,
+    GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef,
     GetRelationalDatabaseBlueprintsRequestRequestTypeDef,
     RelationalDatabaseBlueprintTypeDef,
+    GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef,
     GetRelationalDatabaseBundlesRequestRequestTypeDef,
     RelationalDatabaseBundleTypeDef,
+    GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
     GetRelationalDatabaseEventsRequestRequestTypeDef,
     RelationalDatabaseEventTypeDef,
     GetRelationalDatabaseLogEventsRequestRequestTypeDef,
     LogEventTypeDef,
     GetRelationalDatabaseLogStreamsRequestRequestTypeDef,
+    GetRelationalDatabaseLogStreamsResultTypeDef,
     GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
+    GetRelationalDatabaseMasterUserPasswordResultTypeDef,
     GetRelationalDatabaseMetricDataRequestRequestTypeDef,
+    GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
     GetRelationalDatabaseParametersRequestRequestTypeDef,
     RelationalDatabaseParameterTypeDef,
     GetRelationalDatabaseRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotRequestRequestTypeDef,
+    GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
     GetRelationalDatabaseSnapshotsRequestRequestTypeDef,
+    GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
     GetRelationalDatabasesRequestRequestTypeDef,
     GetStaticIpRequestRequestTypeDef,
+    GetStaticIpsRequestGetStaticIpsPaginateTypeDef,
     GetStaticIpsRequestRequestTypeDef,
     HostKeyAttributesTypeDef,
     ImportKeyPairRequestRequestTypeDef,
     PasswordDataTypeDef,
     InstanceHealthSummaryTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstancePortInfoTypeDef,
     MonthlyTransferTypeDef,
+    IsVpcPeeredResultTypeDef,
     OriginTypeDef,
     LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef,
     LoadBalancerTlsCertificateDomainValidationOptionTypeDef,
     LoadBalancerTlsCertificateSummaryTypeDef,
     NameServersUpdateStateTypeDef,
+    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PendingModifiedRelationalDatabaseValuesTypeDef,
     PutAlarmRequestRequestTypeDef,
     R53HostedZoneDeletionStateTypeDef,
     RebootInstanceRequestRequestTypeDef,
     RebootRelationalDatabaseRequestRequestTypeDef,
     RegisterContainerImageRequestRequestTypeDef,
     RelationalDatabaseEndpointTypeDef,
     RelationalDatabaseHardwareTypeDef,
     ReleaseStaticIpRequestRequestTypeDef,
     ResetDistributionCacheRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SendContactMethodVerificationRequestRequestTypeDef,
     SetIpAddressTypeRequestRequestTypeDef,
     SetResourceAccessForBucketRequestRequestTypeDef,
     StartGUISessionRequestRequestTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartRelationalDatabaseRequestRequestTypeDef,
     StopGUISessionRequestRequestTypeDef,
@@ -671,21 +698,14 @@
     UpdateRelationalDatabaseRequestRequestTypeDef,
     AccessKeyTypeDef,
     AddOnRequestTypeDef,
     AlarmTypeDef,
     ContactMethodTypeDef,
     OperationTypeDef,
     StaticIpTypeDef,
-    DownloadDefaultKeyPairResultTypeDef,
-    GetActiveNamesResultTypeDef,
-    GetContainerAPIMetadataResultTypeDef,
-    GetDistributionLatestCacheResetResultTypeDef,
-    GetRelationalDatabaseLogStreamsResultTypeDef,
-    GetRelationalDatabaseMasterUserPasswordResultTypeDef,
-    IsVpcPeeredResultTypeDef,
     AutoSnapshotDetailsTypeDef,
     RegionTypeDef,
     GetBlueprintsResultTypeDef,
     UpdateBucketRequestRequestTypeDef,
     GetBucketBundlesResultTypeDef,
     BucketTypeDef,
     CreateBucketRequestRequestTypeDef,
@@ -724,34 +744,14 @@
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
     CreateGUISessionAccessDetailsResultTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
     DomainValidationRecordTypeDef,
     EstimateByTimeTypeDef,
-    GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
-    GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
-    GetBundlesRequestGetBundlesPaginateTypeDef,
-    GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
-    GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
-    GetDisksRequestGetDisksPaginateTypeDef,
-    GetDomainsRequestGetDomainsPaginateTypeDef,
-    GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef,
-    GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef,
-    GetInstancesRequestGetInstancesPaginateTypeDef,
-    GetKeyPairsRequestGetKeyPairsPaginateTypeDef,
-    GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef,
-    GetOperationsRequestGetOperationsPaginateTypeDef,
-    GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef,
-    GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef,
-    GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
-    GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
-    GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
-    GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
-    GetStaticIpsRequestGetStaticIpsPaginateTypeDef,
     GetBucketMetricDataResultTypeDef,
     GetContainerServiceMetricDataResultTypeDef,
     GetDistributionMetricDataResultTypeDef,
     GetInstanceMetricDataResultTypeDef,
     GetLoadBalancerMetricDataResultTypeDef,
     GetRelationalDatabaseMetricDataResultTypeDef,
     GetInstancePortStatesResultTypeDef,
@@ -932,42 +932,42 @@
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

### Comparing `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/SOURCES.txt` & `mypy-boto3-lightsail-1.27.0/mypy_boto3_lightsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.26.81/setup.py` & `mypy-boto3-lightsail-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-lightsail.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lightsail",
-    version="1.26.81",
+    version="1.27.0",
     packages=["mypy_boto3_lightsail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Lightsail 1.26.81 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.Lightsail 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/",
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


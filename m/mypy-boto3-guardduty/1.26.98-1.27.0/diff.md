# Comparing `tmp/mypy-boto3-guardduty-1.26.98.tar.gz` & `tmp/mypy-boto3-guardduty-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-guardduty-1.26.98.tar", last modified: Thu Mar 23 19:33:04 2023, max compression
+gzip compressed data, was "mypy-boto3-guardduty-1.27.0.tar", last modified: Mon Jul  3 19:50:50 2023, max compression
```

## Comparing `mypy-boto3-guardduty-1.26.98.tar` & `mypy-boto3-guardduty-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.379626 mypy-boto3-guardduty-1.26.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24416 2023-03-23 19:33:04.379626 mypy-boto3-guardduty-1.26.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22921 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.375626 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47388 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47307 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    82726 2023-03-23 19:32:13.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    82645 2023-03-23 19:32:12.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.379626 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24416 2023-03-23 19:33:04.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-23 19:33:04.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:04.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 19:33:04.000000 mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:04.379626 mypy-boto3-guardduty-1.26.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-23 19:32:10.000000 mypy-boto3-guardduty-1.26.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.267354 mypy-boto3-guardduty-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25847 2023-07-03 19:50:50.263354 mypy-boto3-guardduty-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24354 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.263354 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49732 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49647 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-03 19:38:47.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    93093 2023-07-03 19:38:48.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93006 2023-07-03 19:38:47.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.263354 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25847 2023-07-03 19:50:50.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:50:50.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:50.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:50.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:50.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:50:50.000000 mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:50.267354 mypy-boto3-guardduty-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:38:45.000000 mypy-boto3-guardduty-1.27.0/setup.py
```

### Comparing `mypy-boto3-guardduty-1.26.98/LICENSE` & `mypy-boto3-guardduty-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.26.98/PKG-INFO` & `mypy-boto3-guardduty-1.27.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.26.98
-Summary: Type annotations for boto3.GuardDuty 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.GuardDuty 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-guardduty"></a>
 
 # mypy-boto3-guardduty
 
 [![PyPI - mypy-boto3-guardduty](https://img.shields.io/pypi/v/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-guardduty?color=blue)](https://pypistats.org/packages/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,14 +280,15 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_guardduty import GuardDutyClient
 from mypy_boto3_guardduty.paginator import (
     DescribeMalwareScansPaginator,
+    ListCoveragePaginator,
     ListDetectorsPaginator,
     ListFiltersPaginator,
     ListFindingsPaginator,
     ListIPSetsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
@@ -297,14 +298,15 @@
 client: GuardDutyClient = Session().client("guardduty")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_malware_scans_paginator: DescribeMalwareScansPaginator = client.get_paginator(
     "describe_malware_scans"
 )
+list_coverage_paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
 list_detectors_paginator: ListDetectorsPaginator = client.get_paginator("list_detectors")
 list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
 list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
 list_ip_sets_paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")
 list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
 list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
 list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = (
@@ -322,46 +324,55 @@
 `mypy_boto3_guardduty.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_guardduty.literals import (
     AdminStatusType,
     AutoEnableMembersType,
+    CoverageFilterCriterionKeyType,
+    CoverageSortKeyType,
+    CoverageStatisticsTypeType,
+    CoverageStatusType,
     CriterionKeyType,
     DataSourceStatusType,
     DataSourceType,
     DescribeMalwareScansPaginatorName,
     DestinationTypeType,
     DetectorFeatureResultType,
     DetectorFeatureType,
     DetectorStatusType,
     EbsSnapshotPreservationType,
+    FeatureAdditionalConfigurationType,
     FeatureStatusType,
     FeedbackType,
     FilterActionType,
     FindingPublishingFrequencyType,
     FindingStatisticTypeType,
     FreeTrialFeatureResultType,
     IpSetFormatType,
     IpSetStatusType,
+    ListCoveragePaginatorName,
     ListDetectorsPaginatorName,
     ListFiltersPaginatorName,
     ListFindingsPaginatorName,
     ListIPSetsPaginatorName,
     ListInvitationsPaginatorName,
     ListMembersPaginatorName,
     ListOrganizationAdminAccountsPaginatorName,
     ListThreatIntelSetsPaginatorName,
     OrderByType,
+    OrgFeatureAdditionalConfigurationType,
     OrgFeatureStatusType,
     OrgFeatureType,
     PublishingStatusType,
+    ResourceTypeType,
     ScanCriterionKeyType,
     ScanResultType,
     ScanStatusType,
+    ScanTypeType,
     ThreatIntelSetFormatType,
     ThreatIntelSetStatusType,
     UsageFeatureType,
     UsageStatisticTypeType,
     GuardDutyServiceName,
     ServiceName,
     ResourceServiceName,
@@ -387,54 +398,59 @@
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccessKeyDetailsTypeDef,
     AccountDetailTypeDef,
     FreeTrialFeatureConfigurationResultTypeDef,
     BlockPublicAccessTypeDef,
     DnsRequestActionTypeDef,
+    AddonDetailsTypeDef,
     AdminAccountTypeDef,
     AdministratorTypeDef,
     ArchiveFindingsRequestRequestTypeDef,
     DomainDetailsTypeDef,
     RemoteAccountDetailsTypeDef,
     BucketPolicyTypeDef,
     CityTypeDef,
     CloudTrailConfigurationResultTypeDef,
     ConditionTypeDef,
     SecurityContextTypeDef,
     VolumeMountTypeDef,
     CountryTypeDef,
-    DetectorFeatureConfigurationTypeDef,
-    ResponseMetadataTypeDef,
+    CoverageFilterConditionTypeDef,
+    CoverageSortCriteriaTypeDef,
+    CoverageStatisticsTypeDef,
+    CreateFilterResponseTypeDef,
     CreateIPSetRequestRequestTypeDef,
+    CreateIPSetResponseTypeDef,
     UnprocessedAccountTypeDef,
     DestinationPropertiesTypeDef,
+    CreatePublishingDestinationResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
     CreateThreatIntelSetRequestRequestTypeDef,
+    CreateThreatIntelSetResponseTypeDef,
     DNSLogsConfigurationResultTypeDef,
     FlowLogsConfigurationResultTypeDef,
     S3LogsConfigurationResultTypeDef,
     S3LogsConfigurationTypeDef,
     DataSourceFreeTrialTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DefaultServerSideEncryptionTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DeletePublishingDestinationRequestRequestTypeDef,
     DeleteThreatIntelSetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     SortCriteriaTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
-    OrganizationFeatureConfigurationResultTypeDef,
     DescribePublishingDestinationRequestRequestTypeDef,
     DestinationTypeDef,
-    DetectorFeatureConfigurationResultTypeDef,
+    DetectorAdditionalConfigurationResultTypeDef,
+    DetectorAdditionalConfigurationTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateFromAdministratorAccountRequestRequestTypeDef,
     DisassociateFromMasterAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     VolumeDetailTypeDef,
     EbsVolumesResultTypeDef,
     TagTypeDef,
@@ -443,121 +459,128 @@
     FilterConditionTypeDef,
     FindingStatisticsTypeDef,
     GeoLocationTypeDef,
     GetAdministratorAccountRequestRequestTypeDef,
     GetDetectorRequestRequestTypeDef,
     GetFilterRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
+    GetIPSetResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
     GetMalwareScanSettingsRequestRequestTypeDef,
     GetMasterAccountRequestRequestTypeDef,
     MasterTypeDef,
     GetMemberDetectorsRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     GetRemainingFreeTrialDaysRequestRequestTypeDef,
     GetThreatIntelSetRequestRequestTypeDef,
+    GetThreatIntelSetResponseTypeDef,
     UsageCriteriaTypeDef,
     HighestSeverityThreatDetailsTypeDef,
     HostPathTypeDef,
     IamInstanceProfileTypeDef,
     ProductCodeTypeDef,
     InvitationTypeDef,
     InviteMembersRequestRequestTypeDef,
     KubernetesAuditLogsConfigurationResultTypeDef,
     KubernetesAuditLogsConfigurationTypeDef,
     KubernetesUserDetailsTypeDef,
+    LineageObjectTypeDef,
+    ListDetectorsRequestListDetectorsPaginateTypeDef,
     ListDetectorsRequestRequestTypeDef,
+    ListDetectorsResponseTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
+    ListFiltersResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
+    ListIPSetsResponseTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListPublishingDestinationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     ListThreatIntelSetsRequestRequestTypeDef,
+    ListThreatIntelSetsResponseTypeDef,
     LocalIpDetailsTypeDef,
     LocalPortDetailsTypeDef,
     LoginAttributeTypeDef,
     ScanEc2InstanceWithFindingsTypeDef,
-    MemberFeaturesConfigurationResultTypeDef,
-    MemberFeaturesConfigurationTypeDef,
+    MemberAdditionalConfigurationResultTypeDef,
+    MemberAdditionalConfigurationTypeDef,
     RemotePortDetailsTypeDef,
     PrivateIpAddressDetailsTypeDef,
     SecurityGroupTypeDef,
+    OrganizationAdditionalConfigurationResultTypeDef,
+    OrganizationAdditionalConfigurationTypeDef,
     OrganizationS3LogsConfigurationResultTypeDef,
     OrganizationS3LogsConfigurationTypeDef,
     OrganizationEbsVolumesResultTypeDef,
     OrganizationEbsVolumesTypeDef,
-    OrganizationFeatureConfigurationTypeDef,
     OrganizationKubernetesAuditLogsConfigurationResultTypeDef,
     OrganizationKubernetesAuditLogsConfigurationTypeDef,
     OrganizationTypeDef,
     OwnerTypeDef,
+    PaginatorConfigTypeDef,
     RdsDbUserDetailsTypeDef,
     ResourceDetailsTypeDef,
+    ResponseMetadataTypeDef,
     ScanConditionPairTypeDef,
     ScannedItemCountTypeDef,
     ThreatsDetectedItemCountTypeDef,
     ScanFilePathTypeDef,
     ScanResultDetailsTypeDef,
     TriggerDetailsTypeDef,
     ServiceAdditionalInfoTypeDef,
+    StartMalwareScanRequestRequestTypeDef,
+    StartMalwareScanResponseTypeDef,
     StartMonitoringMembersRequestRequestTypeDef,
     StopMonitoringMembersRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TotalTypeDef,
     UnarchiveFindingsRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateFilterResponseTypeDef,
     UpdateFindingsFeedbackRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     UpdateThreatIntelSetRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
+    CoverageEksClusterDetailsTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    GetAdministratorAccountResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     FindingCriteriaTypeDef,
     ContainerTypeDef,
-    CreateFilterResponseTypeDef,
-    CreateIPSetResponseTypeDef,
-    CreatePublishingDestinationResponseTypeDef,
-    CreateThreatIntelSetResponseTypeDef,
-    GetAdministratorAccountResponseTypeDef,
-    GetIPSetResponseTypeDef,
-    GetInvitationsCountResponseTypeDef,
-    GetThreatIntelSetResponseTypeDef,
-    ListDetectorsResponseTypeDef,
-    ListFiltersResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListIPSetsResponseTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListThreatIntelSetsResponseTypeDef,
-    UpdateFilterResponseTypeDef,
+    CoverageFilterCriterionTypeDef,
+    GetCoverageStatisticsResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DisassociateMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     CreatePublishingDestinationRequestRequestTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     UpdatePublishingDestinationRequestRequestTypeDef,
     KubernetesDataSourceFreeTrialTypeDef,
     MalwareProtectionDataSourceFreeTrialTypeDef,
-    ListDetectorsRequestListDetectorsPaginateTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
-    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     ListPublishingDestinationsResponseTypeDef,
+    DetectorFeatureConfigurationResultTypeDef,
+    DetectorFeatureConfigurationTypeDef,
     EbsVolumeDetailsTypeDef,
     ScanEc2InstanceWithFindingsResultTypeDef,
     EksClusterDetailsTypeDef,
     RdsDbInstanceDetailsTypeDef,
     EvidenceTypeDef,
     FilterCriterionTypeDef,
     GetFindingsStatisticsResponseTypeDef,
@@ -565,71 +588,87 @@
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     GetUsageStatisticsRequestRequestTypeDef,
     VolumeTypeDef,
     ListInvitationsResponseTypeDef,
     KubernetesConfigurationResultTypeDef,
     KubernetesConfigurationTypeDef,
+    ProcessDetailsTypeDef,
     MalwareProtectionConfigurationTypeDef,
+    MemberFeaturesConfigurationResultTypeDef,
+    MemberFeaturesConfigurationTypeDef,
     NetworkInterfaceTypeDef,
+    VpcConfigTypeDef,
+    OrganizationFeatureConfigurationResultTypeDef,
+    OrganizationFeatureConfigurationTypeDef,
     OrganizationScanEc2InstanceWithFindingsResultTypeDef,
     OrganizationScanEc2InstanceWithFindingsTypeDef,
     OrganizationKubernetesConfigurationResultTypeDef,
     OrganizationKubernetesConfigurationTypeDef,
     RemoteIpDetailsTypeDef,
     ScanConditionTypeDef,
     ScanThreatNameTypeDef,
     ScanTypeDef,
     UsageAccountResultTypeDef,
     UsageDataSourceResultTypeDef,
     UsageFeatureResultTypeDef,
     UsageResourceResultTypeDef,
+    CoverageResourceDetailsTypeDef,
     PermissionConfigurationTypeDef,
     CreateFilterRequestRequestTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
+    CoverageFilterCriteriaTypeDef,
     DataSourcesFreeTrialTypeDef,
     MalwareProtectionConfigurationResultTypeDef,
     FilterCriteriaTypeDef,
     EcsTaskDetailsTypeDef,
     KubernetesWorkloadDetailsTypeDef,
+    RuntimeContextTypeDef,
     DataSourceConfigurationsTypeDef,
     InstanceDetailsTypeDef,
+    LambdaDetailsTypeDef,
     OrganizationMalwareProtectionConfigurationResultTypeDef,
     OrganizationMalwareProtectionConfigurationTypeDef,
     AwsApiCallActionTypeDef,
     KubernetesApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     RdsLoginAttemptActionTypeDef,
     ScanResourceCriteriaTypeDef,
     ThreatDetectedByNameTypeDef,
     DescribeMalwareScansResponseTypeDef,
     UsageStatisticsTypeDef,
+    CoverageResourceTypeDef,
     PublicAccessTypeDef,
+    GetCoverageStatisticsRequestRequestTypeDef,
+    ListCoverageRequestListCoveragePaginateTypeDef,
+    ListCoverageRequestRequestTypeDef,
     AccountFreeTrialInfoTypeDef,
     DataSourceConfigurationsResultTypeDef,
     UnprocessedDataSourcesResultTypeDef,
     DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
     DescribeMalwareScansRequestRequestTypeDef,
     EcsClusterDetailsTypeDef,
     KubernetesDetailsTypeDef,
+    RuntimeDetailsTypeDef,
     CreateDetectorRequestRequestTypeDef,
     UpdateDetectorRequestRequestTypeDef,
     UpdateMemberDetectorsRequestRequestTypeDef,
     OrganizationDataSourceConfigurationsResultTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     PortProbeActionTypeDef,
     GetMalwareScanSettingsResponseTypeDef,
     UpdateMalwareScanSettingsRequestRequestTypeDef,
     ScanDetectionsTypeDef,
     GetUsageStatisticsResponseTypeDef,
+    ListCoverageResponseTypeDef,
     S3BucketDetailTypeDef,
     GetRemainingFreeTrialDaysResponseTypeDef,
     GetDetectorResponseTypeDef,
     MemberDataSourceConfigurationTypeDef,
     CreateDetectorResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-guardduty-1.26.98/README.md` & `mypy-boto3-guardduty-1.27.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-guardduty"></a>
 
 # mypy-boto3-guardduty
 
 [![PyPI - mypy-boto3-guardduty](https://img.shields.io/pypi/v/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-guardduty?color=blue)](https://pypistats.org/packages/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
 
@@ -248,14 +248,15 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_guardduty import GuardDutyClient
 from mypy_boto3_guardduty.paginator import (
     DescribeMalwareScansPaginator,
+    ListCoveragePaginator,
     ListDetectorsPaginator,
     ListFiltersPaginator,
     ListFindingsPaginator,
     ListIPSetsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
@@ -265,14 +266,15 @@
 client: GuardDutyClient = Session().client("guardduty")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_malware_scans_paginator: DescribeMalwareScansPaginator = client.get_paginator(
     "describe_malware_scans"
 )
+list_coverage_paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
 list_detectors_paginator: ListDetectorsPaginator = client.get_paginator("list_detectors")
 list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
 list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
 list_ip_sets_paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")
 list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
 list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
 list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = (
@@ -290,46 +292,55 @@
 `mypy_boto3_guardduty.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_guardduty.literals import (
     AdminStatusType,
     AutoEnableMembersType,
+    CoverageFilterCriterionKeyType,
+    CoverageSortKeyType,
+    CoverageStatisticsTypeType,
+    CoverageStatusType,
     CriterionKeyType,
     DataSourceStatusType,
     DataSourceType,
     DescribeMalwareScansPaginatorName,
     DestinationTypeType,
     DetectorFeatureResultType,
     DetectorFeatureType,
     DetectorStatusType,
     EbsSnapshotPreservationType,
+    FeatureAdditionalConfigurationType,
     FeatureStatusType,
     FeedbackType,
     FilterActionType,
     FindingPublishingFrequencyType,
     FindingStatisticTypeType,
     FreeTrialFeatureResultType,
     IpSetFormatType,
     IpSetStatusType,
+    ListCoveragePaginatorName,
     ListDetectorsPaginatorName,
     ListFiltersPaginatorName,
     ListFindingsPaginatorName,
     ListIPSetsPaginatorName,
     ListInvitationsPaginatorName,
     ListMembersPaginatorName,
     ListOrganizationAdminAccountsPaginatorName,
     ListThreatIntelSetsPaginatorName,
     OrderByType,
+    OrgFeatureAdditionalConfigurationType,
     OrgFeatureStatusType,
     OrgFeatureType,
     PublishingStatusType,
+    ResourceTypeType,
     ScanCriterionKeyType,
     ScanResultType,
     ScanStatusType,
+    ScanTypeType,
     ThreatIntelSetFormatType,
     ThreatIntelSetStatusType,
     UsageFeatureType,
     UsageStatisticTypeType,
     GuardDutyServiceName,
     ServiceName,
     ResourceServiceName,
@@ -355,54 +366,59 @@
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccessKeyDetailsTypeDef,
     AccountDetailTypeDef,
     FreeTrialFeatureConfigurationResultTypeDef,
     BlockPublicAccessTypeDef,
     DnsRequestActionTypeDef,
+    AddonDetailsTypeDef,
     AdminAccountTypeDef,
     AdministratorTypeDef,
     ArchiveFindingsRequestRequestTypeDef,
     DomainDetailsTypeDef,
     RemoteAccountDetailsTypeDef,
     BucketPolicyTypeDef,
     CityTypeDef,
     CloudTrailConfigurationResultTypeDef,
     ConditionTypeDef,
     SecurityContextTypeDef,
     VolumeMountTypeDef,
     CountryTypeDef,
-    DetectorFeatureConfigurationTypeDef,
-    ResponseMetadataTypeDef,
+    CoverageFilterConditionTypeDef,
+    CoverageSortCriteriaTypeDef,
+    CoverageStatisticsTypeDef,
+    CreateFilterResponseTypeDef,
     CreateIPSetRequestRequestTypeDef,
+    CreateIPSetResponseTypeDef,
     UnprocessedAccountTypeDef,
     DestinationPropertiesTypeDef,
+    CreatePublishingDestinationResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
     CreateThreatIntelSetRequestRequestTypeDef,
+    CreateThreatIntelSetResponseTypeDef,
     DNSLogsConfigurationResultTypeDef,
     FlowLogsConfigurationResultTypeDef,
     S3LogsConfigurationResultTypeDef,
     S3LogsConfigurationTypeDef,
     DataSourceFreeTrialTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DefaultServerSideEncryptionTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DeletePublishingDestinationRequestRequestTypeDef,
     DeleteThreatIntelSetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     SortCriteriaTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
-    OrganizationFeatureConfigurationResultTypeDef,
     DescribePublishingDestinationRequestRequestTypeDef,
     DestinationTypeDef,
-    DetectorFeatureConfigurationResultTypeDef,
+    DetectorAdditionalConfigurationResultTypeDef,
+    DetectorAdditionalConfigurationTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateFromAdministratorAccountRequestRequestTypeDef,
     DisassociateFromMasterAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     VolumeDetailTypeDef,
     EbsVolumesResultTypeDef,
     TagTypeDef,
@@ -411,121 +427,128 @@
     FilterConditionTypeDef,
     FindingStatisticsTypeDef,
     GeoLocationTypeDef,
     GetAdministratorAccountRequestRequestTypeDef,
     GetDetectorRequestRequestTypeDef,
     GetFilterRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
+    GetIPSetResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
     GetMalwareScanSettingsRequestRequestTypeDef,
     GetMasterAccountRequestRequestTypeDef,
     MasterTypeDef,
     GetMemberDetectorsRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     GetRemainingFreeTrialDaysRequestRequestTypeDef,
     GetThreatIntelSetRequestRequestTypeDef,
+    GetThreatIntelSetResponseTypeDef,
     UsageCriteriaTypeDef,
     HighestSeverityThreatDetailsTypeDef,
     HostPathTypeDef,
     IamInstanceProfileTypeDef,
     ProductCodeTypeDef,
     InvitationTypeDef,
     InviteMembersRequestRequestTypeDef,
     KubernetesAuditLogsConfigurationResultTypeDef,
     KubernetesAuditLogsConfigurationTypeDef,
     KubernetesUserDetailsTypeDef,
+    LineageObjectTypeDef,
+    ListDetectorsRequestListDetectorsPaginateTypeDef,
     ListDetectorsRequestRequestTypeDef,
+    ListDetectorsResponseTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
+    ListFiltersResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
+    ListIPSetsResponseTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListPublishingDestinationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     ListThreatIntelSetsRequestRequestTypeDef,
+    ListThreatIntelSetsResponseTypeDef,
     LocalIpDetailsTypeDef,
     LocalPortDetailsTypeDef,
     LoginAttributeTypeDef,
     ScanEc2InstanceWithFindingsTypeDef,
-    MemberFeaturesConfigurationResultTypeDef,
-    MemberFeaturesConfigurationTypeDef,
+    MemberAdditionalConfigurationResultTypeDef,
+    MemberAdditionalConfigurationTypeDef,
     RemotePortDetailsTypeDef,
     PrivateIpAddressDetailsTypeDef,
     SecurityGroupTypeDef,
+    OrganizationAdditionalConfigurationResultTypeDef,
+    OrganizationAdditionalConfigurationTypeDef,
     OrganizationS3LogsConfigurationResultTypeDef,
     OrganizationS3LogsConfigurationTypeDef,
     OrganizationEbsVolumesResultTypeDef,
     OrganizationEbsVolumesTypeDef,
-    OrganizationFeatureConfigurationTypeDef,
     OrganizationKubernetesAuditLogsConfigurationResultTypeDef,
     OrganizationKubernetesAuditLogsConfigurationTypeDef,
     OrganizationTypeDef,
     OwnerTypeDef,
+    PaginatorConfigTypeDef,
     RdsDbUserDetailsTypeDef,
     ResourceDetailsTypeDef,
+    ResponseMetadataTypeDef,
     ScanConditionPairTypeDef,
     ScannedItemCountTypeDef,
     ThreatsDetectedItemCountTypeDef,
     ScanFilePathTypeDef,
     ScanResultDetailsTypeDef,
     TriggerDetailsTypeDef,
     ServiceAdditionalInfoTypeDef,
+    StartMalwareScanRequestRequestTypeDef,
+    StartMalwareScanResponseTypeDef,
     StartMonitoringMembersRequestRequestTypeDef,
     StopMonitoringMembersRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TotalTypeDef,
     UnarchiveFindingsRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateFilterResponseTypeDef,
     UpdateFindingsFeedbackRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     UpdateThreatIntelSetRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
+    CoverageEksClusterDetailsTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    GetAdministratorAccountResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     FindingCriteriaTypeDef,
     ContainerTypeDef,
-    CreateFilterResponseTypeDef,
-    CreateIPSetResponseTypeDef,
-    CreatePublishingDestinationResponseTypeDef,
-    CreateThreatIntelSetResponseTypeDef,
-    GetAdministratorAccountResponseTypeDef,
-    GetIPSetResponseTypeDef,
-    GetInvitationsCountResponseTypeDef,
-    GetThreatIntelSetResponseTypeDef,
-    ListDetectorsResponseTypeDef,
-    ListFiltersResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListIPSetsResponseTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListThreatIntelSetsResponseTypeDef,
-    UpdateFilterResponseTypeDef,
+    CoverageFilterCriterionTypeDef,
+    GetCoverageStatisticsResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DisassociateMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     CreatePublishingDestinationRequestRequestTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     UpdatePublishingDestinationRequestRequestTypeDef,
     KubernetesDataSourceFreeTrialTypeDef,
     MalwareProtectionDataSourceFreeTrialTypeDef,
-    ListDetectorsRequestListDetectorsPaginateTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
-    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     ListPublishingDestinationsResponseTypeDef,
+    DetectorFeatureConfigurationResultTypeDef,
+    DetectorFeatureConfigurationTypeDef,
     EbsVolumeDetailsTypeDef,
     ScanEc2InstanceWithFindingsResultTypeDef,
     EksClusterDetailsTypeDef,
     RdsDbInstanceDetailsTypeDef,
     EvidenceTypeDef,
     FilterCriterionTypeDef,
     GetFindingsStatisticsResponseTypeDef,
@@ -533,71 +556,87 @@
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     GetUsageStatisticsRequestRequestTypeDef,
     VolumeTypeDef,
     ListInvitationsResponseTypeDef,
     KubernetesConfigurationResultTypeDef,
     KubernetesConfigurationTypeDef,
+    ProcessDetailsTypeDef,
     MalwareProtectionConfigurationTypeDef,
+    MemberFeaturesConfigurationResultTypeDef,
+    MemberFeaturesConfigurationTypeDef,
     NetworkInterfaceTypeDef,
+    VpcConfigTypeDef,
+    OrganizationFeatureConfigurationResultTypeDef,
+    OrganizationFeatureConfigurationTypeDef,
     OrganizationScanEc2InstanceWithFindingsResultTypeDef,
     OrganizationScanEc2InstanceWithFindingsTypeDef,
     OrganizationKubernetesConfigurationResultTypeDef,
     OrganizationKubernetesConfigurationTypeDef,
     RemoteIpDetailsTypeDef,
     ScanConditionTypeDef,
     ScanThreatNameTypeDef,
     ScanTypeDef,
     UsageAccountResultTypeDef,
     UsageDataSourceResultTypeDef,
     UsageFeatureResultTypeDef,
     UsageResourceResultTypeDef,
+    CoverageResourceDetailsTypeDef,
     PermissionConfigurationTypeDef,
     CreateFilterRequestRequestTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
+    CoverageFilterCriteriaTypeDef,
     DataSourcesFreeTrialTypeDef,
     MalwareProtectionConfigurationResultTypeDef,
     FilterCriteriaTypeDef,
     EcsTaskDetailsTypeDef,
     KubernetesWorkloadDetailsTypeDef,
+    RuntimeContextTypeDef,
     DataSourceConfigurationsTypeDef,
     InstanceDetailsTypeDef,
+    LambdaDetailsTypeDef,
     OrganizationMalwareProtectionConfigurationResultTypeDef,
     OrganizationMalwareProtectionConfigurationTypeDef,
     AwsApiCallActionTypeDef,
     KubernetesApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     RdsLoginAttemptActionTypeDef,
     ScanResourceCriteriaTypeDef,
     ThreatDetectedByNameTypeDef,
     DescribeMalwareScansResponseTypeDef,
     UsageStatisticsTypeDef,
+    CoverageResourceTypeDef,
     PublicAccessTypeDef,
+    GetCoverageStatisticsRequestRequestTypeDef,
+    ListCoverageRequestListCoveragePaginateTypeDef,
+    ListCoverageRequestRequestTypeDef,
     AccountFreeTrialInfoTypeDef,
     DataSourceConfigurationsResultTypeDef,
     UnprocessedDataSourcesResultTypeDef,
     DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
     DescribeMalwareScansRequestRequestTypeDef,
     EcsClusterDetailsTypeDef,
     KubernetesDetailsTypeDef,
+    RuntimeDetailsTypeDef,
     CreateDetectorRequestRequestTypeDef,
     UpdateDetectorRequestRequestTypeDef,
     UpdateMemberDetectorsRequestRequestTypeDef,
     OrganizationDataSourceConfigurationsResultTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     PortProbeActionTypeDef,
     GetMalwareScanSettingsResponseTypeDef,
     UpdateMalwareScanSettingsRequestRequestTypeDef,
     ScanDetectionsTypeDef,
     GetUsageStatisticsResponseTypeDef,
+    ListCoverageResponseTypeDef,
     S3BucketDetailTypeDef,
     GetRemainingFreeTrialDaysResponseTypeDef,
     GetDetectorResponseTypeDef,
     MemberDataSourceConfigurationTypeDef,
     CreateDetectorResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/__init__.py` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,41 +5,44 @@
 
     ```python
     from boto3.session import Session
     from mypy_boto3_guardduty import (
         Client,
         DescribeMalwareScansPaginator,
         GuardDutyClient,
+        ListCoveragePaginator,
         ListDetectorsPaginator,
         ListFiltersPaginator,
         ListFindingsPaginator,
         ListIPSetsPaginator,
         ListInvitationsPaginator,
         ListMembersPaginator,
         ListOrganizationAdminAccountsPaginator,
         ListThreatIntelSetsPaginator,
     )
 
     session = Session()
     client: GuardDutyClient = session.client("guardduty")
 
     describe_malware_scans_paginator: DescribeMalwareScansPaginator = client.get_paginator("describe_malware_scans")
+    list_coverage_paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
     list_detectors_paginator: ListDetectorsPaginator = client.get_paginator("list_detectors")
     list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_ip_sets_paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
     list_threat_intel_sets_paginator: ListThreatIntelSetsPaginator = client.get_paginator("list_threat_intel_sets")
     ```
 """
 from .client import GuardDutyClient
 from .paginator import (
     DescribeMalwareScansPaginator,
+    ListCoveragePaginator,
     ListDetectorsPaginator,
     ListFiltersPaginator,
     ListFindingsPaginator,
     ListInvitationsPaginator,
     ListIPSetsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
@@ -49,14 +52,15 @@
 Client = GuardDutyClient
 
 
 __all__ = (
     "Client",
     "DescribeMalwareScansPaginator",
     "GuardDutyClient",
+    "ListCoveragePaginator",
     "ListDetectorsPaginator",
     "ListFiltersPaginator",
     "ListFindingsPaginator",
     "ListIPSetsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/__init__.pyi` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/__init__.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -5,41 +5,44 @@
 
     ```python
     from boto3.session import Session
     from mypy_boto3_guardduty import (
         Client,
         DescribeMalwareScansPaginator,
         GuardDutyClient,
+        ListCoveragePaginator,
         ListDetectorsPaginator,
         ListFiltersPaginator,
         ListFindingsPaginator,
         ListIPSetsPaginator,
         ListInvitationsPaginator,
         ListMembersPaginator,
         ListOrganizationAdminAccountsPaginator,
         ListThreatIntelSetsPaginator,
     )
 
     session = Session()
     client: GuardDutyClient = session.client("guardduty")
 
     describe_malware_scans_paginator: DescribeMalwareScansPaginator = client.get_paginator("describe_malware_scans")
+    list_coverage_paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
     list_detectors_paginator: ListDetectorsPaginator = client.get_paginator("list_detectors")
     list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_ip_sets_paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
     list_threat_intel_sets_paginator: ListThreatIntelSetsPaginator = client.get_paginator("list_threat_intel_sets")
     ```
 """
 from .client import GuardDutyClient
 from .paginator import (
     DescribeMalwareScansPaginator,
+    ListCoveragePaginator,
     ListDetectorsPaginator,
     ListFiltersPaginator,
     ListFindingsPaginator,
     ListInvitationsPaginator,
     ListIPSetsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
@@ -48,14 +51,15 @@
 
 Client = GuardDutyClient
 
 __all__ = (
     "Client",
     "DescribeMalwareScansPaginator",
     "GuardDutyClient",
+    "ListCoveragePaginator",
     "ListDetectorsPaginator",
     "ListFiltersPaginator",
     "ListFindingsPaginator",
     "ListIPSetsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/__main__.py` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GuardDuty 1.26.98\nVersion:         1.26.98\nBuilder version:"
-        " 7.14.2\nDocs:           "
+        "Type annotations for boto3.GuardDuty 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.98")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/client.py` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,35 +16,39 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoEnableMembersType,
+    CoverageStatisticsTypeType,
     EbsSnapshotPreservationType,
     FeedbackType,
     FilterActionType,
     FindingPublishingFrequencyType,
     IpSetFormatType,
     ThreatIntelSetFormatType,
     UsageStatisticTypeType,
 )
 from .paginator import (
     DescribeMalwareScansPaginator,
+    ListCoveragePaginator,
     ListDetectorsPaginator,
     ListFiltersPaginator,
     ListFindingsPaginator,
     ListInvitationsPaginator,
     ListIPSetsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
     ListThreatIntelSetsPaginator,
 )
 from .type_defs import (
     AccountDetailTypeDef,
+    CoverageFilterCriteriaTypeDef,
+    CoverageSortCriteriaTypeDef,
     CreateDetectorResponseTypeDef,
     CreateFilterResponseTypeDef,
     CreateIPSetResponseTypeDef,
     CreateMembersResponseTypeDef,
     CreatePublishingDestinationResponseTypeDef,
     CreateThreatIntelSetResponseTypeDef,
     DataSourceConfigurationsTypeDef,
@@ -56,28 +60,30 @@
     DescribePublishingDestinationResponseTypeDef,
     DestinationPropertiesTypeDef,
     DetectorFeatureConfigurationTypeDef,
     DisassociateMembersResponseTypeDef,
     FilterCriteriaTypeDef,
     FindingCriteriaTypeDef,
     GetAdministratorAccountResponseTypeDef,
+    GetCoverageStatisticsResponseTypeDef,
     GetDetectorResponseTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetFindingsStatisticsResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
     GetIPSetResponseTypeDef,
     GetMalwareScanSettingsResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     GetMemberDetectorsResponseTypeDef,
     GetMembersResponseTypeDef,
     GetRemainingFreeTrialDaysResponseTypeDef,
     GetThreatIntelSetResponseTypeDef,
     GetUsageStatisticsResponseTypeDef,
     InviteMembersResponseTypeDef,
+    ListCoverageResponseTypeDef,
     ListDetectorsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListIPSetsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
@@ -85,14 +91,15 @@
     ListTagsForResourceResponseTypeDef,
     ListThreatIntelSetsResponseTypeDef,
     MemberFeaturesConfigurationTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     OrganizationFeatureConfigurationTypeDef,
     ScanResourceCriteriaTypeDef,
     SortCriteriaTypeDef,
+    StartMalwareScanResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     UsageCriteriaTypeDef,
 )
 
@@ -110,16 +117,18 @@
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
 
 class Exceptions:
+    AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
+    ConflictException: Type[BotocoreClientError]
     InternalServerErrorException: Type[BotocoreClientError]
 
 
 class GuardDutyClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/)
@@ -428,15 +437,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#disassociate_from_master_account)
         """
 
     def disassociate_members(
         self, *, DetectorId: str, AccountIds: Sequence[str]
     ) -> DisassociateMembersResponseTypeDef:
         """
-        Disassociates GuardDuty member accounts (to the current administrator account)
+        Disassociates GuardDuty member accounts (from the current administrator account)
         specified by the account IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.disassociate_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#disassociate_members)
         """
 
     def enable_organization_admin_account(self, *, AdminAccountId: str) -> Dict[str, Any]:
@@ -469,14 +478,28 @@
         Provides the details for the GuardDuty administrator account associated with the
         current GuardDuty member account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_administrator_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_administrator_account)
         """
 
+    def get_coverage_statistics(
+        self,
+        *,
+        DetectorId: str,
+        StatisticsType: Sequence[CoverageStatisticsTypeType],
+        FilterCriteria: CoverageFilterCriteriaTypeDef = ...
+    ) -> GetCoverageStatisticsResponseTypeDef:
+        """
+        Retrieves aggregated statistics for your account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_coverage_statistics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_coverage_statistics)
+        """
+
     def get_detector(self, *, DetectorId: str) -> GetDetectorResponseTypeDef:
         """
         Retrieves an Amazon GuardDuty detector specified by the detectorId.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_detector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_detector)
         """
@@ -614,23 +637,37 @@
         *,
         DetectorId: str,
         AccountIds: Sequence[str],
         DisableEmailNotification: bool = ...,
         Message: str = ...
     ) -> InviteMembersResponseTypeDef:
         """
-        Invites other Amazon Web Services accounts (created as members of the current
-        Amazon Web Services account by CreateMembers) to enable GuardDuty, and allow the
-        current Amazon Web Services account to view and manage these accounts' findings
-        on their behalf as the GuardDuty administrator account.
+        Invites Amazon Web Services accounts to become members of an organization
+        administered by the Amazon Web Services account that invokes this API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.invite_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#invite_members)
         """
 
+    def list_coverage(
+        self,
+        *,
+        DetectorId: str,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
+        SortCriteria: CoverageSortCriteriaTypeDef = ...
+    ) -> ListCoverageResponseTypeDef:
+        """
+        Lists coverage details for your GuardDuty account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_coverage)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#list_coverage)
+        """
+
     def list_detectors(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListDetectorsResponseTypeDef:
         """
         Lists detectorIds of all the existing Amazon GuardDuty detector resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_detectors)
@@ -735,14 +772,22 @@
         """
         Lists the ThreatIntelSets of the GuardDuty service specified by the detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_threat_intel_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#list_threat_intel_sets)
         """
 
+    def start_malware_scan(self, *, ResourceArn: str) -> StartMalwareScanResponseTypeDef:
+        """
+        Initiates the malware scan.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.start_malware_scan)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#start_malware_scan)
+        """
+
     def start_monitoring_members(
         self, *, DetectorId: str, AccountIds: Sequence[str]
     ) -> StartMonitoringMembersResponseTypeDef:
         """
         Turns on GuardDuty monitoring of the specified member accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.start_monitoring_members)
@@ -929,14 +974,21 @@
     ) -> DescribeMalwareScansPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(self, operation_name: Literal["list_coverage"]) -> ListCoveragePaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_detectors"]) -> ListDetectorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_paginator)
         """
 
     @overload
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/client.pyi` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -16,35 +16,39 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoEnableMembersType,
+    CoverageStatisticsTypeType,
     EbsSnapshotPreservationType,
     FeedbackType,
     FilterActionType,
     FindingPublishingFrequencyType,
     IpSetFormatType,
     ThreatIntelSetFormatType,
     UsageStatisticTypeType,
 )
 from .paginator import (
     DescribeMalwareScansPaginator,
+    ListCoveragePaginator,
     ListDetectorsPaginator,
     ListFiltersPaginator,
     ListFindingsPaginator,
     ListInvitationsPaginator,
     ListIPSetsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
     ListThreatIntelSetsPaginator,
 )
 from .type_defs import (
     AccountDetailTypeDef,
+    CoverageFilterCriteriaTypeDef,
+    CoverageSortCriteriaTypeDef,
     CreateDetectorResponseTypeDef,
     CreateFilterResponseTypeDef,
     CreateIPSetResponseTypeDef,
     CreateMembersResponseTypeDef,
     CreatePublishingDestinationResponseTypeDef,
     CreateThreatIntelSetResponseTypeDef,
     DataSourceConfigurationsTypeDef,
@@ -56,28 +60,30 @@
     DescribePublishingDestinationResponseTypeDef,
     DestinationPropertiesTypeDef,
     DetectorFeatureConfigurationTypeDef,
     DisassociateMembersResponseTypeDef,
     FilterCriteriaTypeDef,
     FindingCriteriaTypeDef,
     GetAdministratorAccountResponseTypeDef,
+    GetCoverageStatisticsResponseTypeDef,
     GetDetectorResponseTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetFindingsStatisticsResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
     GetIPSetResponseTypeDef,
     GetMalwareScanSettingsResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     GetMemberDetectorsResponseTypeDef,
     GetMembersResponseTypeDef,
     GetRemainingFreeTrialDaysResponseTypeDef,
     GetThreatIntelSetResponseTypeDef,
     GetUsageStatisticsResponseTypeDef,
     InviteMembersResponseTypeDef,
+    ListCoverageResponseTypeDef,
     ListDetectorsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListIPSetsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
@@ -85,14 +91,15 @@
     ListTagsForResourceResponseTypeDef,
     ListThreatIntelSetsResponseTypeDef,
     MemberFeaturesConfigurationTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     OrganizationFeatureConfigurationTypeDef,
     ScanResourceCriteriaTypeDef,
     SortCriteriaTypeDef,
+    StartMalwareScanResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     UsageCriteriaTypeDef,
 )
 
@@ -107,16 +114,18 @@
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
 class Exceptions:
+    AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
+    ConflictException: Type[BotocoreClientError]
     InternalServerErrorException: Type[BotocoreClientError]
 
 class GuardDutyClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/)
     """
@@ -397,15 +406,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.disassociate_from_master_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#disassociate_from_master_account)
         """
     def disassociate_members(
         self, *, DetectorId: str, AccountIds: Sequence[str]
     ) -> DisassociateMembersResponseTypeDef:
         """
-        Disassociates GuardDuty member accounts (to the current administrator account)
+        Disassociates GuardDuty member accounts (from the current administrator account)
         specified by the account IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.disassociate_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#disassociate_members)
         """
     def enable_organization_admin_account(self, *, AdminAccountId: str) -> Dict[str, Any]:
         """
@@ -434,14 +443,27 @@
         """
         Provides the details for the GuardDuty administrator account associated with the
         current GuardDuty member account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_administrator_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_administrator_account)
         """
+    def get_coverage_statistics(
+        self,
+        *,
+        DetectorId: str,
+        StatisticsType: Sequence[CoverageStatisticsTypeType],
+        FilterCriteria: CoverageFilterCriteriaTypeDef = ...
+    ) -> GetCoverageStatisticsResponseTypeDef:
+        """
+        Retrieves aggregated statistics for your account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_coverage_statistics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_coverage_statistics)
+        """
     def get_detector(self, *, DetectorId: str) -> GetDetectorResponseTypeDef:
         """
         Retrieves an Amazon GuardDuty detector specified by the detectorId.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_detector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_detector)
         """
@@ -566,22 +588,35 @@
         *,
         DetectorId: str,
         AccountIds: Sequence[str],
         DisableEmailNotification: bool = ...,
         Message: str = ...
     ) -> InviteMembersResponseTypeDef:
         """
-        Invites other Amazon Web Services accounts (created as members of the current
-        Amazon Web Services account by CreateMembers) to enable GuardDuty, and allow the
-        current Amazon Web Services account to view and manage these accounts' findings
-        on their behalf as the GuardDuty administrator account.
+        Invites Amazon Web Services accounts to become members of an organization
+        administered by the Amazon Web Services account that invokes this API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.invite_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#invite_members)
         """
+    def list_coverage(
+        self,
+        *,
+        DetectorId: str,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
+        SortCriteria: CoverageSortCriteriaTypeDef = ...
+    ) -> ListCoverageResponseTypeDef:
+        """
+        Lists coverage details for your GuardDuty account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_coverage)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#list_coverage)
+        """
     def list_detectors(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListDetectorsResponseTypeDef:
         """
         Lists detectorIds of all the existing Amazon GuardDuty detector resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_detectors)
@@ -676,14 +711,21 @@
     ) -> ListThreatIntelSetsResponseTypeDef:
         """
         Lists the ThreatIntelSets of the GuardDuty service specified by the detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_threat_intel_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#list_threat_intel_sets)
         """
+    def start_malware_scan(self, *, ResourceArn: str) -> StartMalwareScanResponseTypeDef:
+        """
+        Initiates the malware scan.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.start_malware_scan)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#start_malware_scan)
+        """
     def start_monitoring_members(
         self, *, DetectorId: str, AccountIds: Sequence[str]
     ) -> StartMonitoringMembersResponseTypeDef:
         """
         Turns on GuardDuty monitoring of the specified member accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.start_monitoring_members)
@@ -855,14 +897,20 @@
         self, operation_name: Literal["describe_malware_scans"]
     ) -> DescribeMalwareScansPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_paginator)
         """
     @overload
+    def get_paginator(self, operation_name: Literal["list_coverage"]) -> ListCoveragePaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_paginator)
+        """
+    @overload
     def get_paginator(self, operation_name: Literal["list_detectors"]) -> ListDetectorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_paginator)
         """
     @overload
     def get_paginator(self, operation_name: Literal["list_filters"]) -> ListFiltersPaginator:
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/literals.py` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,125 +18,162 @@
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AdminStatusType",
     "AutoEnableMembersType",
+    "CoverageFilterCriterionKeyType",
+    "CoverageSortKeyType",
+    "CoverageStatisticsTypeType",
+    "CoverageStatusType",
     "CriterionKeyType",
     "DataSourceStatusType",
     "DataSourceType",
     "DescribeMalwareScansPaginatorName",
     "DestinationTypeType",
     "DetectorFeatureResultType",
     "DetectorFeatureType",
     "DetectorStatusType",
     "EbsSnapshotPreservationType",
+    "FeatureAdditionalConfigurationType",
     "FeatureStatusType",
     "FeedbackType",
     "FilterActionType",
     "FindingPublishingFrequencyType",
     "FindingStatisticTypeType",
     "FreeTrialFeatureResultType",
     "IpSetFormatType",
     "IpSetStatusType",
+    "ListCoveragePaginatorName",
     "ListDetectorsPaginatorName",
     "ListFiltersPaginatorName",
     "ListFindingsPaginatorName",
     "ListIPSetsPaginatorName",
     "ListInvitationsPaginatorName",
     "ListMembersPaginatorName",
     "ListOrganizationAdminAccountsPaginatorName",
     "ListThreatIntelSetsPaginatorName",
     "OrderByType",
+    "OrgFeatureAdditionalConfigurationType",
     "OrgFeatureStatusType",
     "OrgFeatureType",
     "PublishingStatusType",
+    "ResourceTypeType",
     "ScanCriterionKeyType",
     "ScanResultType",
     "ScanStatusType",
+    "ScanTypeType",
     "ThreatIntelSetFormatType",
     "ThreatIntelSetStatusType",
     "UsageFeatureType",
     "UsageStatisticTypeType",
     "GuardDutyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
 AdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
 AutoEnableMembersType = Literal["ALL", "NEW", "NONE"]
+CoverageFilterCriterionKeyType = Literal[
+    "ACCOUNT_ID", "ADDON_VERSION", "CLUSTER_NAME", "COVERAGE_STATUS", "RESOURCE_TYPE"
+]
+CoverageSortKeyType = Literal[
+    "ACCOUNT_ID", "ADDON_VERSION", "CLUSTER_NAME", "COVERAGE_STATUS", "ISSUE", "UPDATED_AT"
+]
+CoverageStatisticsTypeType = Literal["COUNT_BY_COVERAGE_STATUS", "COUNT_BY_RESOURCE_TYPE"]
+CoverageStatusType = Literal["HEALTHY", "UNHEALTHY"]
 CriterionKeyType = Literal[
     "ACCOUNT_ID",
     "EC2_INSTANCE_ARN",
     "GUARDDUTY_FINDING_ID",
     "SCAN_ID",
     "SCAN_START_TIME",
     "SCAN_STATUS",
+    "SCAN_TYPE",
 ]
 DataSourceStatusType = Literal["DISABLED", "ENABLED"]
 DataSourceType = Literal[
     "CLOUD_TRAIL", "DNS_LOGS", "EC2_MALWARE_SCAN", "FLOW_LOGS", "KUBERNETES_AUDIT_LOGS", "S3_LOGS"
 ]
 DescribeMalwareScansPaginatorName = Literal["describe_malware_scans"]
 DestinationTypeType = Literal["S3"]
 DetectorFeatureResultType = Literal[
     "CLOUD_TRAIL",
     "DNS_LOGS",
     "EBS_MALWARE_PROTECTION",
     "EKS_AUDIT_LOGS",
+    "EKS_RUNTIME_MONITORING",
     "FLOW_LOGS",
+    "LAMBDA_NETWORK_LOGS",
     "RDS_LOGIN_EVENTS",
     "S3_DATA_EVENTS",
 ]
 DetectorFeatureType = Literal[
-    "EBS_MALWARE_PROTECTION", "EKS_AUDIT_LOGS", "RDS_LOGIN_EVENTS", "S3_DATA_EVENTS"
+    "EBS_MALWARE_PROTECTION",
+    "EKS_AUDIT_LOGS",
+    "EKS_RUNTIME_MONITORING",
+    "LAMBDA_NETWORK_LOGS",
+    "RDS_LOGIN_EVENTS",
+    "S3_DATA_EVENTS",
 ]
 DetectorStatusType = Literal["DISABLED", "ENABLED"]
 EbsSnapshotPreservationType = Literal["NO_RETENTION", "RETENTION_WITH_FINDING"]
+FeatureAdditionalConfigurationType = Literal["EKS_ADDON_MANAGEMENT"]
 FeatureStatusType = Literal["DISABLED", "ENABLED"]
 FeedbackType = Literal["NOT_USEFUL", "USEFUL"]
 FilterActionType = Literal["ARCHIVE", "NOOP"]
 FindingPublishingFrequencyType = Literal["FIFTEEN_MINUTES", "ONE_HOUR", "SIX_HOURS"]
 FindingStatisticTypeType = Literal["COUNT_BY_SEVERITY"]
 FreeTrialFeatureResultType = Literal[
     "CLOUD_TRAIL",
     "DNS_LOGS",
     "EBS_MALWARE_PROTECTION",
     "EKS_AUDIT_LOGS",
+    "EKS_RUNTIME_MONITORING",
     "FLOW_LOGS",
+    "LAMBDA_NETWORK_LOGS",
     "RDS_LOGIN_EVENTS",
     "S3_DATA_EVENTS",
 ]
 IpSetFormatType = Literal["ALIEN_VAULT", "FIRE_EYE", "OTX_CSV", "PROOF_POINT", "STIX", "TXT"]
 IpSetStatusType = Literal[
     "ACTIVATING", "ACTIVE", "DEACTIVATING", "DELETED", "DELETE_PENDING", "ERROR", "INACTIVE"
 ]
+ListCoveragePaginatorName = Literal["list_coverage"]
 ListDetectorsPaginatorName = Literal["list_detectors"]
 ListFiltersPaginatorName = Literal["list_filters"]
 ListFindingsPaginatorName = Literal["list_findings"]
 ListIPSetsPaginatorName = Literal["list_ip_sets"]
 ListInvitationsPaginatorName = Literal["list_invitations"]
 ListMembersPaginatorName = Literal["list_members"]
 ListOrganizationAdminAccountsPaginatorName = Literal["list_organization_admin_accounts"]
 ListThreatIntelSetsPaginatorName = Literal["list_threat_intel_sets"]
 OrderByType = Literal["ASC", "DESC"]
+OrgFeatureAdditionalConfigurationType = Literal["EKS_ADDON_MANAGEMENT"]
 OrgFeatureStatusType = Literal["NEW", "NONE"]
 OrgFeatureType = Literal[
-    "EBS_MALWARE_PROTECTION", "EKS_AUDIT_LOGS", "RDS_LOGIN_EVENTS", "S3_DATA_EVENTS"
+    "EBS_MALWARE_PROTECTION",
+    "EKS_AUDIT_LOGS",
+    "EKS_RUNTIME_MONITORING",
+    "LAMBDA_NETWORK_LOGS",
+    "RDS_LOGIN_EVENTS",
+    "S3_DATA_EVENTS",
 ]
 PublishingStatusType = Literal[
     "PENDING_VERIFICATION", "PUBLISHING", "STOPPED", "UNABLE_TO_PUBLISH_FIX_DESTINATION_PROPERTY"
 ]
+ResourceTypeType = Literal["EKS"]
 ScanCriterionKeyType = Literal["EC2_INSTANCE_TAG"]
 ScanResultType = Literal["CLEAN", "INFECTED"]
-ScanStatusType = Literal["COMPLETED", "FAILED", "RUNNING"]
+ScanStatusType = Literal["COMPLETED", "FAILED", "RUNNING", "SKIPPED"]
+ScanTypeType = Literal["GUARDDUTY_INITIATED", "ON_DEMAND"]
 ThreatIntelSetFormatType = Literal[
     "ALIEN_VAULT", "FIRE_EYE", "OTX_CSV", "PROOF_POINT", "STIX", "TXT"
 ]
 ThreatIntelSetStatusType = Literal[
     "ACTIVATING", "ACTIVE", "DEACTIVATING", "DELETED", "DELETE_PENDING", "ERROR", "INACTIVE"
 ]
 UsageFeatureType = Literal[
@@ -165,14 +202,15 @@
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
@@ -212,14 +250,15 @@
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
@@ -361,14 +400,15 @@
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
@@ -387,16 +427,19 @@
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
@@ -480,15 +523,17 @@
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
@@ -508,14 +553,15 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "describe_malware_scans",
+    "list_coverage",
     "list_detectors",
     "list_filters",
     "list_findings",
     "list_invitations",
     "list_ip_sets",
     "list_members",
     "list_organization_admin_accounts",
@@ -528,14 +574,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/literals.pyi` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -17,124 +17,161 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AdminStatusType",
     "AutoEnableMembersType",
+    "CoverageFilterCriterionKeyType",
+    "CoverageSortKeyType",
+    "CoverageStatisticsTypeType",
+    "CoverageStatusType",
     "CriterionKeyType",
     "DataSourceStatusType",
     "DataSourceType",
     "DescribeMalwareScansPaginatorName",
     "DestinationTypeType",
     "DetectorFeatureResultType",
     "DetectorFeatureType",
     "DetectorStatusType",
     "EbsSnapshotPreservationType",
+    "FeatureAdditionalConfigurationType",
     "FeatureStatusType",
     "FeedbackType",
     "FilterActionType",
     "FindingPublishingFrequencyType",
     "FindingStatisticTypeType",
     "FreeTrialFeatureResultType",
     "IpSetFormatType",
     "IpSetStatusType",
+    "ListCoveragePaginatorName",
     "ListDetectorsPaginatorName",
     "ListFiltersPaginatorName",
     "ListFindingsPaginatorName",
     "ListIPSetsPaginatorName",
     "ListInvitationsPaginatorName",
     "ListMembersPaginatorName",
     "ListOrganizationAdminAccountsPaginatorName",
     "ListThreatIntelSetsPaginatorName",
     "OrderByType",
+    "OrgFeatureAdditionalConfigurationType",
     "OrgFeatureStatusType",
     "OrgFeatureType",
     "PublishingStatusType",
+    "ResourceTypeType",
     "ScanCriterionKeyType",
     "ScanResultType",
     "ScanStatusType",
+    "ScanTypeType",
     "ThreatIntelSetFormatType",
     "ThreatIntelSetStatusType",
     "UsageFeatureType",
     "UsageStatisticTypeType",
     "GuardDutyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
 AutoEnableMembersType = Literal["ALL", "NEW", "NONE"]
+CoverageFilterCriterionKeyType = Literal[
+    "ACCOUNT_ID", "ADDON_VERSION", "CLUSTER_NAME", "COVERAGE_STATUS", "RESOURCE_TYPE"
+]
+CoverageSortKeyType = Literal[
+    "ACCOUNT_ID", "ADDON_VERSION", "CLUSTER_NAME", "COVERAGE_STATUS", "ISSUE", "UPDATED_AT"
+]
+CoverageStatisticsTypeType = Literal["COUNT_BY_COVERAGE_STATUS", "COUNT_BY_RESOURCE_TYPE"]
+CoverageStatusType = Literal["HEALTHY", "UNHEALTHY"]
 CriterionKeyType = Literal[
     "ACCOUNT_ID",
     "EC2_INSTANCE_ARN",
     "GUARDDUTY_FINDING_ID",
     "SCAN_ID",
     "SCAN_START_TIME",
     "SCAN_STATUS",
+    "SCAN_TYPE",
 ]
 DataSourceStatusType = Literal["DISABLED", "ENABLED"]
 DataSourceType = Literal[
     "CLOUD_TRAIL", "DNS_LOGS", "EC2_MALWARE_SCAN", "FLOW_LOGS", "KUBERNETES_AUDIT_LOGS", "S3_LOGS"
 ]
 DescribeMalwareScansPaginatorName = Literal["describe_malware_scans"]
 DestinationTypeType = Literal["S3"]
 DetectorFeatureResultType = Literal[
     "CLOUD_TRAIL",
     "DNS_LOGS",
     "EBS_MALWARE_PROTECTION",
     "EKS_AUDIT_LOGS",
+    "EKS_RUNTIME_MONITORING",
     "FLOW_LOGS",
+    "LAMBDA_NETWORK_LOGS",
     "RDS_LOGIN_EVENTS",
     "S3_DATA_EVENTS",
 ]
 DetectorFeatureType = Literal[
-    "EBS_MALWARE_PROTECTION", "EKS_AUDIT_LOGS", "RDS_LOGIN_EVENTS", "S3_DATA_EVENTS"
+    "EBS_MALWARE_PROTECTION",
+    "EKS_AUDIT_LOGS",
+    "EKS_RUNTIME_MONITORING",
+    "LAMBDA_NETWORK_LOGS",
+    "RDS_LOGIN_EVENTS",
+    "S3_DATA_EVENTS",
 ]
 DetectorStatusType = Literal["DISABLED", "ENABLED"]
 EbsSnapshotPreservationType = Literal["NO_RETENTION", "RETENTION_WITH_FINDING"]
+FeatureAdditionalConfigurationType = Literal["EKS_ADDON_MANAGEMENT"]
 FeatureStatusType = Literal["DISABLED", "ENABLED"]
 FeedbackType = Literal["NOT_USEFUL", "USEFUL"]
 FilterActionType = Literal["ARCHIVE", "NOOP"]
 FindingPublishingFrequencyType = Literal["FIFTEEN_MINUTES", "ONE_HOUR", "SIX_HOURS"]
 FindingStatisticTypeType = Literal["COUNT_BY_SEVERITY"]
 FreeTrialFeatureResultType = Literal[
     "CLOUD_TRAIL",
     "DNS_LOGS",
     "EBS_MALWARE_PROTECTION",
     "EKS_AUDIT_LOGS",
+    "EKS_RUNTIME_MONITORING",
     "FLOW_LOGS",
+    "LAMBDA_NETWORK_LOGS",
     "RDS_LOGIN_EVENTS",
     "S3_DATA_EVENTS",
 ]
 IpSetFormatType = Literal["ALIEN_VAULT", "FIRE_EYE", "OTX_CSV", "PROOF_POINT", "STIX", "TXT"]
 IpSetStatusType = Literal[
     "ACTIVATING", "ACTIVE", "DEACTIVATING", "DELETED", "DELETE_PENDING", "ERROR", "INACTIVE"
 ]
+ListCoveragePaginatorName = Literal["list_coverage"]
 ListDetectorsPaginatorName = Literal["list_detectors"]
 ListFiltersPaginatorName = Literal["list_filters"]
 ListFindingsPaginatorName = Literal["list_findings"]
 ListIPSetsPaginatorName = Literal["list_ip_sets"]
 ListInvitationsPaginatorName = Literal["list_invitations"]
 ListMembersPaginatorName = Literal["list_members"]
 ListOrganizationAdminAccountsPaginatorName = Literal["list_organization_admin_accounts"]
 ListThreatIntelSetsPaginatorName = Literal["list_threat_intel_sets"]
 OrderByType = Literal["ASC", "DESC"]
+OrgFeatureAdditionalConfigurationType = Literal["EKS_ADDON_MANAGEMENT"]
 OrgFeatureStatusType = Literal["NEW", "NONE"]
 OrgFeatureType = Literal[
-    "EBS_MALWARE_PROTECTION", "EKS_AUDIT_LOGS", "RDS_LOGIN_EVENTS", "S3_DATA_EVENTS"
+    "EBS_MALWARE_PROTECTION",
+    "EKS_AUDIT_LOGS",
+    "EKS_RUNTIME_MONITORING",
+    "LAMBDA_NETWORK_LOGS",
+    "RDS_LOGIN_EVENTS",
+    "S3_DATA_EVENTS",
 ]
 PublishingStatusType = Literal[
     "PENDING_VERIFICATION", "PUBLISHING", "STOPPED", "UNABLE_TO_PUBLISH_FIX_DESTINATION_PROPERTY"
 ]
+ResourceTypeType = Literal["EKS"]
 ScanCriterionKeyType = Literal["EC2_INSTANCE_TAG"]
 ScanResultType = Literal["CLEAN", "INFECTED"]
-ScanStatusType = Literal["COMPLETED", "FAILED", "RUNNING"]
+ScanStatusType = Literal["COMPLETED", "FAILED", "RUNNING", "SKIPPED"]
+ScanTypeType = Literal["GUARDDUTY_INITIATED", "ON_DEMAND"]
 ThreatIntelSetFormatType = Literal[
     "ALIEN_VAULT", "FIRE_EYE", "OTX_CSV", "PROOF_POINT", "STIX", "TXT"
 ]
 ThreatIntelSetStatusType = Literal[
     "ACTIVATING", "ACTIVE", "DEACTIVATING", "DELETED", "DELETE_PENDING", "ERROR", "INACTIVE"
 ]
 UsageFeatureType = Literal[
@@ -163,14 +200,15 @@
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
@@ -210,14 +248,15 @@
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
@@ -359,14 +398,15 @@
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
@@ -385,16 +425,19 @@
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
@@ -478,15 +521,17 @@
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
@@ -506,14 +551,15 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "describe_malware_scans",
+    "list_coverage",
     "list_detectors",
     "list_filters",
     "list_findings",
     "list_invitations",
     "list_ip_sets",
     "list_members",
     "list_organization_admin_accounts",
@@ -526,14 +572,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/paginator.py` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/paginator.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_guardduty.client import GuardDutyClient
     from mypy_boto3_guardduty.paginator import (
         DescribeMalwareScansPaginator,
+        ListCoveragePaginator,
         ListDetectorsPaginator,
         ListFiltersPaginator,
         ListFindingsPaginator,
         ListIPSetsPaginator,
         ListInvitationsPaginator,
         ListMembersPaginator,
         ListOrganizationAdminAccountsPaginator,
         ListThreatIntelSetsPaginator,
     )
 
     session = Session()
     client: GuardDutyClient = session.client("guardduty")
 
     describe_malware_scans_paginator: DescribeMalwareScansPaginator = client.get_paginator("describe_malware_scans")
+    list_coverage_paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
     list_detectors_paginator: ListDetectorsPaginator = client.get_paginator("list_detectors")
     list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_ip_sets_paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
@@ -36,31 +38,35 @@
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
+    CoverageFilterCriteriaTypeDef,
+    CoverageSortCriteriaTypeDef,
     DescribeMalwareScansResponseTypeDef,
     FilterCriteriaTypeDef,
     FindingCriteriaTypeDef,
+    ListCoverageResponseTypeDef,
     ListDetectorsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListIPSetsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     ListThreatIntelSetsResponseTypeDef,
     PaginatorConfigTypeDef,
     SortCriteriaTypeDef,
 )
 
 __all__ = (
     "DescribeMalwareScansPaginator",
+    "ListCoveragePaginator",
     "ListDetectorsPaginator",
     "ListFiltersPaginator",
     "ListFindingsPaginator",
     "ListIPSetsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
@@ -86,45 +92,65 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: FilterCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMalwareScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.DescribeMalwareScans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#describemalwarescanspaginator)
         """
 
 
+class ListCoveragePaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListCoverage)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listcoveragepaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        DetectorId: str,
+        FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
+        SortCriteria: CoverageSortCriteriaTypeDef = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListCoverageResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListCoverage.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listcoveragepaginator)
+        """
+
+
 class ListDetectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listdetectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDetectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listdetectorspaginator)
         """
 
 
 class ListFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfilterspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfilterspaginator)
         """
 
 
@@ -136,45 +162,45 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FindingCriteria: FindingCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
         """
 
 
 class ListIPSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listipsetspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIPSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listipsetspaginator)
         """
 
 
 class ListInvitationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listinvitationspaginator)
         """
 
 
@@ -185,43 +211,43 @@
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         OnlyAssociated: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listmemberspaginator)
         """
 
 
 class ListOrganizationAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listorganizationadminaccountspaginator)
         """
 
 
 class ListThreatIntelSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listthreatintelsetspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListThreatIntelSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listthreatintelsetspaginator)
         """
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/paginator.pyi` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/paginator.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_guardduty.client import GuardDutyClient
     from mypy_boto3_guardduty.paginator import (
         DescribeMalwareScansPaginator,
+        ListCoveragePaginator,
         ListDetectorsPaginator,
         ListFiltersPaginator,
         ListFindingsPaginator,
         ListIPSetsPaginator,
         ListInvitationsPaginator,
         ListMembersPaginator,
         ListOrganizationAdminAccountsPaginator,
         ListThreatIntelSetsPaginator,
     )
 
     session = Session()
     client: GuardDutyClient = session.client("guardduty")
 
     describe_malware_scans_paginator: DescribeMalwareScansPaginator = client.get_paginator("describe_malware_scans")
+    list_coverage_paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
     list_detectors_paginator: ListDetectorsPaginator = client.get_paginator("list_detectors")
     list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_ip_sets_paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
@@ -36,31 +38,35 @@
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
+    CoverageFilterCriteriaTypeDef,
+    CoverageSortCriteriaTypeDef,
     DescribeMalwareScansResponseTypeDef,
     FilterCriteriaTypeDef,
     FindingCriteriaTypeDef,
+    ListCoverageResponseTypeDef,
     ListDetectorsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListIPSetsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     ListThreatIntelSetsResponseTypeDef,
     PaginatorConfigTypeDef,
     SortCriteriaTypeDef,
 )
 
 __all__ = (
     "DescribeMalwareScansPaginator",
+    "ListCoveragePaginator",
     "ListDetectorsPaginator",
     "ListFiltersPaginator",
     "ListFindingsPaginator",
     "ListIPSetsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
@@ -83,43 +89,62 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: FilterCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMalwareScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.DescribeMalwareScans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#describemalwarescanspaginator)
         """
 
+class ListCoveragePaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListCoverage)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listcoveragepaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        DetectorId: str,
+        FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
+        SortCriteria: CoverageSortCriteriaTypeDef = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListCoverageResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListCoverage.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listcoveragepaginator)
+        """
+
 class ListDetectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listdetectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDetectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listdetectorspaginator)
         """
 
 class ListFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfilterspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfilterspaginator)
         """
 
 class ListFindingsPaginator(Paginator):
@@ -130,43 +155,43 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FindingCriteria: FindingCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
         """
 
 class ListIPSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listipsetspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIPSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listipsetspaginator)
         """
 
 class ListInvitationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listinvitationspaginator)
         """
 
 class ListMembersPaginator(Paginator):
@@ -176,41 +201,41 @@
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         OnlyAssociated: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listmemberspaginator)
         """
 
 class ListOrganizationAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listorganizationadminaccountspaginator)
         """
 
 class ListThreatIntelSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listthreatintelsetspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListThreatIntelSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listthreatintelsetspaginator)
         """
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/type_defs.py` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdminStatusType,
     AutoEnableMembersType,
+    CoverageFilterCriterionKeyType,
+    CoverageSortKeyType,
+    CoverageStatisticsTypeType,
+    CoverageStatusType,
     CriterionKeyType,
     DataSourceStatusType,
     DataSourceType,
     DetectorFeatureResultType,
     DetectorFeatureType,
     DetectorStatusType,
     EbsSnapshotPreservationType,
@@ -34,14 +38,15 @@
     IpSetStatusType,
     OrderByType,
     OrgFeatureStatusType,
     OrgFeatureType,
     PublishingStatusType,
     ScanResultType,
     ScanStatusType,
+    ScanTypeType,
     ThreatIntelSetFormatType,
     ThreatIntelSetStatusType,
     UsageFeatureType,
     UsageStatisticTypeType,
 )
 
 if sys.version_info >= (3, 9):
@@ -49,64 +54,68 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     "AcceptInvitationRequestRequestTypeDef",
     "AccessControlListTypeDef",
     "AccessKeyDetailsTypeDef",
     "AccountDetailTypeDef",
     "FreeTrialFeatureConfigurationResultTypeDef",
     "BlockPublicAccessTypeDef",
     "DnsRequestActionTypeDef",
+    "AddonDetailsTypeDef",
     "AdminAccountTypeDef",
     "AdministratorTypeDef",
     "ArchiveFindingsRequestRequestTypeDef",
     "DomainDetailsTypeDef",
     "RemoteAccountDetailsTypeDef",
     "BucketPolicyTypeDef",
     "CityTypeDef",
     "CloudTrailConfigurationResultTypeDef",
     "ConditionTypeDef",
     "SecurityContextTypeDef",
     "VolumeMountTypeDef",
     "CountryTypeDef",
-    "DetectorFeatureConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
+    "CoverageFilterConditionTypeDef",
+    "CoverageSortCriteriaTypeDef",
+    "CoverageStatisticsTypeDef",
+    "CreateFilterResponseTypeDef",
     "CreateIPSetRequestRequestTypeDef",
+    "CreateIPSetResponseTypeDef",
     "UnprocessedAccountTypeDef",
     "DestinationPropertiesTypeDef",
+    "CreatePublishingDestinationResponseTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
     "CreateThreatIntelSetRequestRequestTypeDef",
+    "CreateThreatIntelSetResponseTypeDef",
     "DNSLogsConfigurationResultTypeDef",
     "FlowLogsConfigurationResultTypeDef",
     "S3LogsConfigurationResultTypeDef",
     "S3LogsConfigurationTypeDef",
     "DataSourceFreeTrialTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DefaultServerSideEncryptionTypeDef",
     "DeleteDetectorRequestRequestTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
     "DeletePublishingDestinationRequestRequestTypeDef",
     "DeleteThreatIntelSetRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "SortCriteriaTypeDef",
     "DescribeOrganizationConfigurationRequestRequestTypeDef",
-    "OrganizationFeatureConfigurationResultTypeDef",
     "DescribePublishingDestinationRequestRequestTypeDef",
     "DestinationTypeDef",
-    "DetectorFeatureConfigurationResultTypeDef",
+    "DetectorAdditionalConfigurationResultTypeDef",
+    "DetectorAdditionalConfigurationTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateFromAdministratorAccountRequestRequestTypeDef",
     "DisassociateFromMasterAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
     "VolumeDetailTypeDef",
     "EbsVolumesResultTypeDef",
     "TagTypeDef",
@@ -115,121 +124,128 @@
     "FilterConditionTypeDef",
     "FindingStatisticsTypeDef",
     "GeoLocationTypeDef",
     "GetAdministratorAccountRequestRequestTypeDef",
     "GetDetectorRequestRequestTypeDef",
     "GetFilterRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
+    "GetIPSetResponseTypeDef",
+    "GetInvitationsCountResponseTypeDef",
     "GetMalwareScanSettingsRequestRequestTypeDef",
     "GetMasterAccountRequestRequestTypeDef",
     "MasterTypeDef",
     "GetMemberDetectorsRequestRequestTypeDef",
     "GetMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "GetRemainingFreeTrialDaysRequestRequestTypeDef",
     "GetThreatIntelSetRequestRequestTypeDef",
+    "GetThreatIntelSetResponseTypeDef",
     "UsageCriteriaTypeDef",
     "HighestSeverityThreatDetailsTypeDef",
     "HostPathTypeDef",
     "IamInstanceProfileTypeDef",
     "ProductCodeTypeDef",
     "InvitationTypeDef",
     "InviteMembersRequestRequestTypeDef",
     "KubernetesAuditLogsConfigurationResultTypeDef",
     "KubernetesAuditLogsConfigurationTypeDef",
     "KubernetesUserDetailsTypeDef",
+    "LineageObjectTypeDef",
+    "ListDetectorsRequestListDetectorsPaginateTypeDef",
     "ListDetectorsRequestRequestTypeDef",
+    "ListDetectorsResponseTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
+    "ListFiltersResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
     "ListIPSetsRequestRequestTypeDef",
+    "ListIPSetsResponseTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     "ListPublishingDestinationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
     "ListThreatIntelSetsRequestRequestTypeDef",
+    "ListThreatIntelSetsResponseTypeDef",
     "LocalIpDetailsTypeDef",
     "LocalPortDetailsTypeDef",
     "LoginAttributeTypeDef",
     "ScanEc2InstanceWithFindingsTypeDef",
-    "MemberFeaturesConfigurationResultTypeDef",
-    "MemberFeaturesConfigurationTypeDef",
+    "MemberAdditionalConfigurationResultTypeDef",
+    "MemberAdditionalConfigurationTypeDef",
     "RemotePortDetailsTypeDef",
     "PrivateIpAddressDetailsTypeDef",
     "SecurityGroupTypeDef",
+    "OrganizationAdditionalConfigurationResultTypeDef",
+    "OrganizationAdditionalConfigurationTypeDef",
     "OrganizationS3LogsConfigurationResultTypeDef",
     "OrganizationS3LogsConfigurationTypeDef",
     "OrganizationEbsVolumesResultTypeDef",
     "OrganizationEbsVolumesTypeDef",
-    "OrganizationFeatureConfigurationTypeDef",
     "OrganizationKubernetesAuditLogsConfigurationResultTypeDef",
     "OrganizationKubernetesAuditLogsConfigurationTypeDef",
     "OrganizationTypeDef",
     "OwnerTypeDef",
+    "PaginatorConfigTypeDef",
     "RdsDbUserDetailsTypeDef",
     "ResourceDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "ScanConditionPairTypeDef",
     "ScannedItemCountTypeDef",
     "ThreatsDetectedItemCountTypeDef",
     "ScanFilePathTypeDef",
     "ScanResultDetailsTypeDef",
     "TriggerDetailsTypeDef",
     "ServiceAdditionalInfoTypeDef",
+    "StartMalwareScanRequestRequestTypeDef",
+    "StartMalwareScanResponseTypeDef",
     "StartMonitoringMembersRequestRequestTypeDef",
     "StopMonitoringMembersRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TotalTypeDef",
     "UnarchiveFindingsRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateFilterResponseTypeDef",
     "UpdateFindingsFeedbackRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "UpdateThreatIntelSetRequestRequestTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
+    "CoverageEksClusterDetailsTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "GetAdministratorAccountResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
     "FindingCriteriaTypeDef",
     "ContainerTypeDef",
-    "CreateFilterResponseTypeDef",
-    "CreateIPSetResponseTypeDef",
-    "CreatePublishingDestinationResponseTypeDef",
-    "CreateThreatIntelSetResponseTypeDef",
-    "GetAdministratorAccountResponseTypeDef",
-    "GetIPSetResponseTypeDef",
-    "GetInvitationsCountResponseTypeDef",
-    "GetThreatIntelSetResponseTypeDef",
-    "ListDetectorsResponseTypeDef",
-    "ListFiltersResponseTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListIPSetsResponseTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListThreatIntelSetsResponseTypeDef",
-    "UpdateFilterResponseTypeDef",
+    "CoverageFilterCriterionTypeDef",
+    "GetCoverageStatisticsResponseTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "DisassociateMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "StartMonitoringMembersResponseTypeDef",
     "StopMonitoringMembersResponseTypeDef",
     "UpdateMemberDetectorsResponseTypeDef",
     "CreatePublishingDestinationRequestRequestTypeDef",
     "DescribePublishingDestinationResponseTypeDef",
     "UpdatePublishingDestinationRequestRequestTypeDef",
     "KubernetesDataSourceFreeTrialTypeDef",
     "MalwareProtectionDataSourceFreeTrialTypeDef",
-    "ListDetectorsRequestListDetectorsPaginateTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    "ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "ListPublishingDestinationsResponseTypeDef",
+    "DetectorFeatureConfigurationResultTypeDef",
+    "DetectorFeatureConfigurationTypeDef",
     "EbsVolumeDetailsTypeDef",
     "ScanEc2InstanceWithFindingsResultTypeDef",
     "EksClusterDetailsTypeDef",
     "RdsDbInstanceDetailsTypeDef",
     "EvidenceTypeDef",
     "FilterCriterionTypeDef",
     "GetFindingsStatisticsResponseTypeDef",
@@ -237,71 +253,87 @@
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "GetUsageStatisticsRequestRequestTypeDef",
     "VolumeTypeDef",
     "ListInvitationsResponseTypeDef",
     "KubernetesConfigurationResultTypeDef",
     "KubernetesConfigurationTypeDef",
+    "ProcessDetailsTypeDef",
     "MalwareProtectionConfigurationTypeDef",
+    "MemberFeaturesConfigurationResultTypeDef",
+    "MemberFeaturesConfigurationTypeDef",
     "NetworkInterfaceTypeDef",
+    "VpcConfigTypeDef",
+    "OrganizationFeatureConfigurationResultTypeDef",
+    "OrganizationFeatureConfigurationTypeDef",
     "OrganizationScanEc2InstanceWithFindingsResultTypeDef",
     "OrganizationScanEc2InstanceWithFindingsTypeDef",
     "OrganizationKubernetesConfigurationResultTypeDef",
     "OrganizationKubernetesConfigurationTypeDef",
     "RemoteIpDetailsTypeDef",
     "ScanConditionTypeDef",
     "ScanThreatNameTypeDef",
     "ScanTypeDef",
     "UsageAccountResultTypeDef",
     "UsageDataSourceResultTypeDef",
     "UsageFeatureResultTypeDef",
     "UsageResourceResultTypeDef",
+    "CoverageResourceDetailsTypeDef",
     "PermissionConfigurationTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "GetFilterResponseTypeDef",
     "GetFindingsStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
+    "CoverageFilterCriteriaTypeDef",
     "DataSourcesFreeTrialTypeDef",
     "MalwareProtectionConfigurationResultTypeDef",
     "FilterCriteriaTypeDef",
     "EcsTaskDetailsTypeDef",
     "KubernetesWorkloadDetailsTypeDef",
+    "RuntimeContextTypeDef",
     "DataSourceConfigurationsTypeDef",
     "InstanceDetailsTypeDef",
+    "LambdaDetailsTypeDef",
     "OrganizationMalwareProtectionConfigurationResultTypeDef",
     "OrganizationMalwareProtectionConfigurationTypeDef",
     "AwsApiCallActionTypeDef",
     "KubernetesApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "RdsLoginAttemptActionTypeDef",
     "ScanResourceCriteriaTypeDef",
     "ThreatDetectedByNameTypeDef",
     "DescribeMalwareScansResponseTypeDef",
     "UsageStatisticsTypeDef",
+    "CoverageResourceTypeDef",
     "PublicAccessTypeDef",
+    "GetCoverageStatisticsRequestRequestTypeDef",
+    "ListCoverageRequestListCoveragePaginateTypeDef",
+    "ListCoverageRequestRequestTypeDef",
     "AccountFreeTrialInfoTypeDef",
     "DataSourceConfigurationsResultTypeDef",
     "UnprocessedDataSourcesResultTypeDef",
     "DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef",
     "DescribeMalwareScansRequestRequestTypeDef",
     "EcsClusterDetailsTypeDef",
     "KubernetesDetailsTypeDef",
+    "RuntimeDetailsTypeDef",
     "CreateDetectorRequestRequestTypeDef",
     "UpdateDetectorRequestRequestTypeDef",
     "UpdateMemberDetectorsRequestRequestTypeDef",
     "OrganizationDataSourceConfigurationsResultTypeDef",
     "OrganizationDataSourceConfigurationsTypeDef",
     "PortProbeActionTypeDef",
     "GetMalwareScanSettingsResponseTypeDef",
     "UpdateMalwareScanSettingsRequestRequestTypeDef",
     "ScanDetectionsTypeDef",
     "GetUsageStatisticsResponseTypeDef",
+    "ListCoverageResponseTypeDef",
     "S3BucketDetailTypeDef",
     "GetRemainingFreeTrialDaysResponseTypeDef",
     "GetDetectorResponseTypeDef",
     "MemberDataSourceConfigurationTypeDef",
     "CreateDetectorResponseTypeDef",
     "DescribeOrganizationConfigurationResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
@@ -386,14 +418,23 @@
         "Domain": str,
         "Protocol": str,
         "Blocked": bool,
     },
     total=False,
 )
 
+AddonDetailsTypeDef = TypedDict(
+    "AddonDetailsTypeDef",
+    {
+        "AddonVersion": str,
+        "AddonStatus": str,
+    },
+    total=False,
+)
+
 AdminAccountTypeDef = TypedDict(
     "AdminAccountTypeDef",
     {
         "AdminAccountId": str,
         "AdminStatus": AdminStatusType,
     },
     total=False,
@@ -500,31 +541,46 @@
     {
         "CountryCode": str,
         "CountryName": str,
     },
     total=False,
 )
 
-DetectorFeatureConfigurationTypeDef = TypedDict(
-    "DetectorFeatureConfigurationTypeDef",
+CoverageFilterConditionTypeDef = TypedDict(
+    "CoverageFilterConditionTypeDef",
     {
-        "Name": DetectorFeatureType,
-        "Status": FeatureStatusType,
+        "Equals": Sequence[str],
+        "NotEquals": Sequence[str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CoverageSortCriteriaTypeDef = TypedDict(
+    "CoverageSortCriteriaTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AttributeName": CoverageSortKeyType,
+        "OrderBy": OrderByType,
+    },
+    total=False,
+)
+
+CoverageStatisticsTypeDef = TypedDict(
+    "CoverageStatisticsTypeDef",
+    {
+        "CountByResourceType": Dict[Literal["EKS"], int],
+        "CountByCoverageStatus": Dict[CoverageStatusType, int],
+    },
+    total=False,
+)
+
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateIPSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -539,20 +595,26 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateIPSetRequestRequestTypeDef(
     _RequiredCreateIPSetRequestRequestTypeDef, _OptionalCreateIPSetRequestRequestTypeDef
 ):
     pass
 
+CreateIPSetResponseTypeDef = TypedDict(
+    "CreateIPSetResponseTypeDef",
+    {
+        "IpSetId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 UnprocessedAccountTypeDef = TypedDict(
     "UnprocessedAccountTypeDef",
     {
         "AccountId": str,
         "Result": str,
     },
@@ -563,36 +625,42 @@
     {
         "DestinationArn": str,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+CreatePublishingDestinationResponseTypeDef = TypedDict(
+    "CreatePublishingDestinationResponseTypeDef",
+    {
+        "DestinationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSampleFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSampleFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalCreateSampleFindingsRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSampleFindingsRequestRequestTypeDef",
     {
         "FindingTypes": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateSampleFindingsRequestRequestTypeDef(
     _RequiredCreateSampleFindingsRequestRequestTypeDef,
     _OptionalCreateSampleFindingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateThreatIntelSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "Name": str,
         "Format": ThreatIntelSetFormatType,
         "Location": str,
@@ -604,21 +672,27 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateThreatIntelSetRequestRequestTypeDef(
     _RequiredCreateThreatIntelSetRequestRequestTypeDef,
     _OptionalCreateThreatIntelSetRequestRequestTypeDef,
 ):
     pass
 
+CreateThreatIntelSetResponseTypeDef = TypedDict(
+    "CreateThreatIntelSetResponseTypeDef",
+    {
+        "ThreatIntelSetId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DNSLogsConfigurationResultTypeDef = TypedDict(
     "DNSLogsConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
@@ -718,24 +792,14 @@
     "DeleteThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 SortCriteriaTypeDef = TypedDict(
     "SortCriteriaTypeDef",
     {
         "AttributeName": str,
         "OrderBy": OrderByType,
     },
     total=False,
@@ -752,31 +816,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeOrganizationConfigurationRequestRequestTypeDef(
     _RequiredDescribeOrganizationConfigurationRequestRequestTypeDef,
     _OptionalDescribeOrganizationConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-OrganizationFeatureConfigurationResultTypeDef = TypedDict(
-    "OrganizationFeatureConfigurationResultTypeDef",
-    {
-        "Name": OrgFeatureType,
-        "AutoEnable": OrgFeatureStatusType,
-    },
-    total=False,
-)
-
 DescribePublishingDestinationRequestRequestTypeDef = TypedDict(
     "DescribePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
         "DestinationId": str,
     },
 )
@@ -786,24 +839,33 @@
     {
         "DestinationId": str,
         "DestinationType": Literal["S3"],
         "Status": PublishingStatusType,
     },
 )
 
-DetectorFeatureConfigurationResultTypeDef = TypedDict(
-    "DetectorFeatureConfigurationResultTypeDef",
+DetectorAdditionalConfigurationResultTypeDef = TypedDict(
+    "DetectorAdditionalConfigurationResultTypeDef",
     {
-        "Name": DetectorFeatureResultType,
+        "Name": Literal["EKS_ADDON_MANAGEMENT"],
         "Status": FeatureStatusType,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
+DetectorAdditionalConfigurationTypeDef = TypedDict(
+    "DetectorAdditionalConfigurationTypeDef",
+    {
+        "Name": Literal["EKS_ADDON_MANAGEMENT"],
+        "Status": FeatureStatusType,
+    },
+    total=False,
+)
+
 DisableOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     {
         "AdminAccountId": str,
     },
 )
 
@@ -930,14 +992,34 @@
     "GetIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "IpSetId": str,
     },
 )
 
+GetIPSetResponseTypeDef = TypedDict(
+    "GetIPSetResponseTypeDef",
+    {
+        "Name": str,
+        "Format": IpSetFormatType,
+        "Location": str,
+        "Status": IpSetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "InvitationsCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "GetMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 
@@ -991,49 +1073,57 @@
         "DetectorId": str,
         "InvitedAt": str,
         "AdministratorId": str,
     },
     total=False,
 )
 
-
 class MemberTypeDef(_RequiredMemberTypeDef, _OptionalMemberTypeDef):
     pass
 
-
 _RequiredGetRemainingFreeTrialDaysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRemainingFreeTrialDaysRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalGetRemainingFreeTrialDaysRequestRequestTypeDef = TypedDict(
     "_OptionalGetRemainingFreeTrialDaysRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
     total=False,
 )
 
-
 class GetRemainingFreeTrialDaysRequestRequestTypeDef(
     _RequiredGetRemainingFreeTrialDaysRequestRequestTypeDef,
     _OptionalGetRemainingFreeTrialDaysRequestRequestTypeDef,
 ):
     pass
 
-
 GetThreatIntelSetRequestRequestTypeDef = TypedDict(
     "GetThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
     },
 )
 
+GetThreatIntelSetResponseTypeDef = TypedDict(
+    "GetThreatIntelSetResponseTypeDef",
+    {
+        "Name": str,
+        "Format": ThreatIntelSetFormatType,
+        "Location": str,
+        "Status": ThreatIntelSetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UsageCriteriaTypeDef = TypedDict(
     "UsageCriteriaTypeDef",
     {
         "AccountIds": Sequence[str],
         "DataSources": Sequence[DataSourceType],
         "Resources": Sequence[str],
         "Features": Sequence[UsageFeatureType],
@@ -1100,21 +1190,19 @@
     {
         "DisableEmailNotification": bool,
         "Message": str,
     },
     total=False,
 )
 
-
 class InviteMembersRequestRequestTypeDef(
     _RequiredInviteMembersRequestRequestTypeDef, _OptionalInviteMembersRequestRequestTypeDef
 ):
     pass
 
-
 KubernetesAuditLogsConfigurationResultTypeDef = TypedDict(
     "KubernetesAuditLogsConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
@@ -1127,27 +1215,81 @@
 
 KubernetesUserDetailsTypeDef = TypedDict(
     "KubernetesUserDetailsTypeDef",
     {
         "Username": str,
         "Uid": str,
         "Groups": List[str],
+        "SessionName": List[str],
+    },
+    total=False,
+)
+
+LineageObjectTypeDef = TypedDict(
+    "LineageObjectTypeDef",
+    {
+        "StartTime": datetime,
+        "NamespacePid": int,
+        "UserId": int,
+        "Name": str,
+        "Pid": int,
+        "Uuid": str,
+        "ExecutablePath": str,
+        "Euid": int,
+        "ParentUuid": str,
+    },
+    total=False,
+)
+
+ListDetectorsRequestListDetectorsPaginateTypeDef = TypedDict(
+    "ListDetectorsRequestListDetectorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDetectorsRequestRequestTypeDef = TypedDict(
     "ListDetectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListDetectorsResponseTypeDef = TypedDict(
+    "ListDetectorsResponseTypeDef",
+    {
+        "DetectorIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "_RequiredListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "_OptionalListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFiltersRequestListFiltersPaginateTypeDef(
+    _RequiredListFiltersRequestListFiltersPaginateTypeDef,
+    _OptionalListFiltersRequestListFiltersPaginateTypeDef,
+):
+    pass
+
 _RequiredListFiltersRequestRequestTypeDef = TypedDict(
     "_RequiredListFiltersRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListFiltersRequestRequestTypeDef = TypedDict(
@@ -1155,20 +1297,56 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListFiltersRequestRequestTypeDef(
     _RequiredListFiltersRequestRequestTypeDef, _OptionalListFiltersRequestRequestTypeDef
 ):
     pass
 
+ListFiltersResponseTypeDef = TypedDict(
+    "ListFiltersResponseTypeDef",
+    {
+        "FilterNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "FindingIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "_RequiredListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "_OptionalListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListIPSetsRequestListIPSetsPaginateTypeDef(
+    _RequiredListIPSetsRequestListIPSetsPaginateTypeDef,
+    _OptionalListIPSetsRequestListIPSetsPaginateTypeDef,
+):
+    pass
 
 _RequiredListIPSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListIPSetsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
@@ -1177,30 +1355,66 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListIPSetsRequestRequestTypeDef(
     _RequiredListIPSetsRequestRequestTypeDef, _OptionalListIPSetsRequestRequestTypeDef
 ):
     pass
 
+ListIPSetsResponseTypeDef = TypedDict(
+    "ListIPSetsResponseTypeDef",
+    {
+        "IpSetIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListInvitationsRequestRequestTypeDef = TypedDict(
     "ListInvitationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "_RequiredListMembersRequestListMembersPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "_OptionalListMembersRequestListMembersPaginateTypeDef",
+    {
+        "OnlyAssociated": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListMembersRequestListMembersPaginateTypeDef(
+    _RequiredListMembersRequestListMembersPaginateTypeDef,
+    _OptionalListMembersRequestListMembersPaginateTypeDef,
+):
+    pass
+
 _RequiredListMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListMembersRequestRequestTypeDef = TypedDict(
@@ -1209,20 +1423,26 @@
         "MaxResults": int,
         "NextToken": str,
         "OnlyAssociated": str,
     },
     total=False,
 )
 
-
 class ListMembersRequestRequestTypeDef(
     _RequiredListMembersRequestRequestTypeDef, _OptionalListMembersRequestRequestTypeDef
 ):
     pass
 
+ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListOrganizationAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1240,29 +1460,55 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListPublishingDestinationsRequestRequestTypeDef(
     _RequiredListPublishingDestinationsRequestRequestTypeDef,
     _OptionalListPublishingDestinationsRequestRequestTypeDef,
 ):
     pass
 
-
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
+_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
+    "_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
+    "_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef(
+    _RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
+    _OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListThreatIntelSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListThreatIntelSetsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListThreatIntelSetsRequestRequestTypeDef = TypedDict(
@@ -1270,21 +1516,28 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListThreatIntelSetsRequestRequestTypeDef(
     _RequiredListThreatIntelSetsRequestRequestTypeDef,
     _OptionalListThreatIntelSetsRequestRequestTypeDef,
 ):
     pass
 
+ListThreatIntelSetsResponseTypeDef = TypedDict(
+    "ListThreatIntelSetsResponseTypeDef",
+    {
+        "ThreatIntelSetIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 LocalIpDetailsTypeDef = TypedDict(
     "LocalIpDetailsTypeDef",
     {
         "IpAddressV4": str,
     },
     total=False,
@@ -1314,28 +1567,28 @@
     "ScanEc2InstanceWithFindingsTypeDef",
     {
         "EbsVolumes": bool,
     },
     total=False,
 )
 
-MemberFeaturesConfigurationResultTypeDef = TypedDict(
-    "MemberFeaturesConfigurationResultTypeDef",
+MemberAdditionalConfigurationResultTypeDef = TypedDict(
+    "MemberAdditionalConfigurationResultTypeDef",
     {
-        "Name": OrgFeatureType,
+        "Name": Literal["EKS_ADDON_MANAGEMENT"],
         "Status": FeatureStatusType,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
-MemberFeaturesConfigurationTypeDef = TypedDict(
-    "MemberFeaturesConfigurationTypeDef",
+MemberAdditionalConfigurationTypeDef = TypedDict(
+    "MemberAdditionalConfigurationTypeDef",
     {
-        "Name": OrgFeatureType,
+        "Name": Literal["EKS_ADDON_MANAGEMENT"],
         "Status": FeatureStatusType,
     },
     total=False,
 )
 
 RemotePortDetailsTypeDef = TypedDict(
     "RemotePortDetailsTypeDef",
@@ -1360,14 +1613,32 @@
     {
         "GroupId": str,
         "GroupName": str,
     },
     total=False,
 )
 
+OrganizationAdditionalConfigurationResultTypeDef = TypedDict(
+    "OrganizationAdditionalConfigurationResultTypeDef",
+    {
+        "Name": Literal["EKS_ADDON_MANAGEMENT"],
+        "AutoEnable": OrgFeatureStatusType,
+    },
+    total=False,
+)
+
+OrganizationAdditionalConfigurationTypeDef = TypedDict(
+    "OrganizationAdditionalConfigurationTypeDef",
+    {
+        "Name": Literal["EKS_ADDON_MANAGEMENT"],
+        "AutoEnable": OrgFeatureStatusType,
+    },
+    total=False,
+)
+
 OrganizationS3LogsConfigurationResultTypeDef = TypedDict(
     "OrganizationS3LogsConfigurationResultTypeDef",
     {
         "AutoEnable": bool,
     },
 )
 
@@ -1390,23 +1661,14 @@
     "OrganizationEbsVolumesTypeDef",
     {
         "AutoEnable": bool,
     },
     total=False,
 )
 
-OrganizationFeatureConfigurationTypeDef = TypedDict(
-    "OrganizationFeatureConfigurationTypeDef",
-    {
-        "Name": OrgFeatureType,
-        "AutoEnable": OrgFeatureStatusType,
-    },
-    total=False,
-)
-
 OrganizationKubernetesAuditLogsConfigurationResultTypeDef = TypedDict(
     "OrganizationKubernetesAuditLogsConfigurationResultTypeDef",
     {
         "AutoEnable": bool,
     },
 )
 
@@ -1432,14 +1694,24 @@
     "OwnerTypeDef",
     {
         "Id": str,
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
 RdsDbUserDetailsTypeDef = TypedDict(
     "RdsDbUserDetailsTypeDef",
     {
         "User": str,
         "Application": str,
         "Database": str,
         "Ssl": str,
@@ -1452,35 +1724,44 @@
     "ResourceDetailsTypeDef",
     {
         "InstanceArn": str,
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
 _RequiredScanConditionPairTypeDef = TypedDict(
     "_RequiredScanConditionPairTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalScanConditionPairTypeDef = TypedDict(
     "_OptionalScanConditionPairTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class ScanConditionPairTypeDef(
     _RequiredScanConditionPairTypeDef, _OptionalScanConditionPairTypeDef
 ):
     pass
 
-
 ScannedItemCountTypeDef = TypedDict(
     "ScannedItemCountTypeDef",
     {
         "TotalGb": int,
         "Files": int,
         "Volumes": int,
     },
@@ -1528,14 +1809,29 @@
     {
         "Value": str,
         "Type": str,
     },
     total=False,
 )
 
+StartMalwareScanRequestRequestTypeDef = TypedDict(
+    "StartMalwareScanRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+
+StartMalwareScanResponseTypeDef = TypedDict(
+    "StartMalwareScanResponseTypeDef",
+    {
+        "ScanId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartMonitoringMembersRequestRequestTypeDef = TypedDict(
     "StartMonitoringMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
         "AccountIds": Sequence[str],
     },
 )
@@ -1577,14 +1873,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateFilterResponseTypeDef = TypedDict(
+    "UpdateFilterResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateFindingsFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFindingsFeedbackRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingIds": Sequence[str],
         "Feedback": FeedbackType,
     },
@@ -1593,22 +1897,20 @@
     "_OptionalUpdateFindingsFeedbackRequestRequestTypeDef",
     {
         "Comments": str,
     },
     total=False,
 )
 
-
 class UpdateFindingsFeedbackRequestRequestTypeDef(
     _RequiredUpdateFindingsFeedbackRequestRequestTypeDef,
     _OptionalUpdateFindingsFeedbackRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateIPSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "IpSetId": str,
     },
 )
@@ -1618,21 +1920,19 @@
         "Name": str,
         "Location": str,
         "Activate": bool,
     },
     total=False,
 )
 
-
 class UpdateIPSetRequestRequestTypeDef(
     _RequiredUpdateIPSetRequestRequestTypeDef, _OptionalUpdateIPSetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateThreatIntelSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
     },
 )
@@ -1642,22 +1942,20 @@
         "Name": str,
         "Location": str,
         "Activate": bool,
     },
     total=False,
 )
 
-
 class UpdateThreatIntelSetRequestRequestTypeDef(
     _RequiredUpdateThreatIntelSetRequestRequestTypeDef,
     _OptionalUpdateThreatIntelSetRequestRequestTypeDef,
 ):
     pass
 
-
 CreateMembersRequestRequestTypeDef = TypedDict(
     "CreateMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
         "AccountDetails": Sequence[AccountDetailTypeDef],
     },
 )
@@ -1666,14 +1964,42 @@
     "AccountLevelPermissionsTypeDef",
     {
         "BlockPublicAccess": BlockPublicAccessTypeDef,
     },
     total=False,
 )
 
+CoverageEksClusterDetailsTypeDef = TypedDict(
+    "CoverageEksClusterDetailsTypeDef",
+    {
+        "ClusterName": str,
+        "CoveredNodes": int,
+        "CompatibleNodes": int,
+        "AddonDetails": AddonDetailsTypeDef,
+    },
+    total=False,
+)
+
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetAdministratorAccountResponseTypeDef = TypedDict(
+    "GetAdministratorAccountResponseTypeDef",
+    {
+        "Administrator": AdministratorTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BucketLevelPermissionsTypeDef = TypedDict(
     "BucketLevelPermissionsTypeDef",
     {
         "AccessControlList": AccessControlListTypeDef,
         "BucketPolicy": BucketPolicyTypeDef,
         "BlockPublicAccess": BlockPublicAccessTypeDef,
     },
@@ -1698,225 +2024,100 @@
         "ImagePrefix": str,
         "VolumeMounts": List[VolumeMountTypeDef],
         "SecurityContext": SecurityContextTypeDef,
     },
     total=False,
 )
 
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIPSetResponseTypeDef = TypedDict(
-    "CreateIPSetResponseTypeDef",
-    {
-        "IpSetId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePublishingDestinationResponseTypeDef = TypedDict(
-    "CreatePublishingDestinationResponseTypeDef",
-    {
-        "DestinationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateThreatIntelSetResponseTypeDef = TypedDict(
-    "CreateThreatIntelSetResponseTypeDef",
-    {
-        "ThreatIntelSetId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAdministratorAccountResponseTypeDef = TypedDict(
-    "GetAdministratorAccountResponseTypeDef",
-    {
-        "Administrator": AdministratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetIPSetResponseTypeDef = TypedDict(
-    "GetIPSetResponseTypeDef",
-    {
-        "Name": str,
-        "Format": IpSetFormatType,
-        "Location": str,
-        "Status": IpSetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
-    {
-        "InvitationsCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetThreatIntelSetResponseTypeDef = TypedDict(
-    "GetThreatIntelSetResponseTypeDef",
-    {
-        "Name": str,
-        "Format": ThreatIntelSetFormatType,
-        "Location": str,
-        "Status": ThreatIntelSetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDetectorsResponseTypeDef = TypedDict(
-    "ListDetectorsResponseTypeDef",
-    {
-        "DetectorIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListFiltersResponseTypeDef = TypedDict(
-    "ListFiltersResponseTypeDef",
-    {
-        "FilterNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "FindingIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListIPSetsResponseTypeDef = TypedDict(
-    "ListIPSetsResponseTypeDef",
-    {
-        "IpSetIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    {
-        "AdminAccounts": List[AdminAccountTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+CoverageFilterCriterionTypeDef = TypedDict(
+    "CoverageFilterCriterionTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListThreatIntelSetsResponseTypeDef = TypedDict(
-    "ListThreatIntelSetsResponseTypeDef",
-    {
-        "ThreatIntelSetIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CriterionKey": CoverageFilterCriterionKeyType,
+        "FilterCondition": CoverageFilterConditionTypeDef,
     },
+    total=False,
 )
 
-UpdateFilterResponseTypeDef = TypedDict(
-    "UpdateFilterResponseTypeDef",
+GetCoverageStatisticsResponseTypeDef = TypedDict(
+    "GetCoverageStatisticsResponseTypeDef",
     {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CoverageStatistics": CoverageStatisticsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMembersResponseTypeDef = TypedDict(
     "CreateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteMembersResponseTypeDef = TypedDict(
     "DeleteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateMembersResponseTypeDef = TypedDict(
     "DisassociateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InviteMembersResponseTypeDef = TypedDict(
     "InviteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartMonitoringMembersResponseTypeDef = TypedDict(
     "StartMonitoringMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopMonitoringMembersResponseTypeDef = TypedDict(
     "StopMonitoringMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMemberDetectorsResponseTypeDef = TypedDict(
     "UpdateMemberDetectorsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -1928,31 +2129,29 @@
     "_OptionalCreatePublishingDestinationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreatePublishingDestinationRequestRequestTypeDef(
     _RequiredCreatePublishingDestinationRequestRequestTypeDef,
     _OptionalCreatePublishingDestinationRequestRequestTypeDef,
 ):
     pass
 
-
 DescribePublishingDestinationResponseTypeDef = TypedDict(
     "DescribePublishingDestinationResponseTypeDef",
     {
         "DestinationId": str,
         "DestinationType": Literal["S3"],
         "Status": PublishingStatusType,
         "PublishingFailureStartTimestamp": int,
         "DestinationProperties": DestinationPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -1963,22 +2162,20 @@
     "_OptionalUpdatePublishingDestinationRequestRequestTypeDef",
     {
         "DestinationProperties": DestinationPropertiesTypeDef,
     },
     total=False,
 )
 
-
 class UpdatePublishingDestinationRequestRequestTypeDef(
     _RequiredUpdatePublishingDestinationRequestRequestTypeDef,
     _OptionalUpdatePublishingDestinationRequestRequestTypeDef,
 ):
     pass
 
-
 KubernetesDataSourceFreeTrialTypeDef = TypedDict(
     "KubernetesDataSourceFreeTrialTypeDef",
     {
         "AuditLogs": DataSourceFreeTrialTypeDef,
     },
     total=False,
 )
@@ -1987,127 +2184,14 @@
     "MalwareProtectionDataSourceFreeTrialTypeDef",
     {
         "ScanEc2InstanceWithFindings": DataSourceFreeTrialTypeDef,
     },
     total=False,
 )
 
-ListDetectorsRequestListDetectorsPaginateTypeDef = TypedDict(
-    "ListDetectorsRequestListDetectorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "_RequiredListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "_OptionalListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFiltersRequestListFiltersPaginateTypeDef(
-    _RequiredListFiltersRequestListFiltersPaginateTypeDef,
-    _OptionalListFiltersRequestListFiltersPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "_RequiredListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "_OptionalListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListIPSetsRequestListIPSetsPaginateTypeDef(
-    _RequiredListIPSetsRequestListIPSetsPaginateTypeDef,
-    _OptionalListIPSetsRequestListIPSetsPaginateTypeDef,
-):
-    pass
-
-
-ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "_RequiredListMembersRequestListMembersPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "_OptionalListMembersRequestListMembersPaginateTypeDef",
-    {
-        "OnlyAssociated": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListMembersRequestListMembersPaginateTypeDef(
-    _RequiredListMembersRequestListMembersPaginateTypeDef,
-    _OptionalListMembersRequestListMembersPaginateTypeDef,
-):
-    pass
-
-
-ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
-    "_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
-    "_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef(
-    _RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
-    _OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingIds": Sequence[str],
     },
 )
@@ -2115,28 +2199,47 @@
     "_OptionalGetFindingsRequestRequestTypeDef",
     {
         "SortCriteria": SortCriteriaTypeDef,
     },
     total=False,
 )
 
-
 class GetFindingsRequestRequestTypeDef(
     _RequiredGetFindingsRequestRequestTypeDef, _OptionalGetFindingsRequestRequestTypeDef
 ):
     pass
 
-
 ListPublishingDestinationsResponseTypeDef = TypedDict(
     "ListPublishingDestinationsResponseTypeDef",
     {
         "Destinations": List[DestinationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DetectorFeatureConfigurationResultTypeDef = TypedDict(
+    "DetectorFeatureConfigurationResultTypeDef",
+    {
+        "Name": DetectorFeatureResultType,
+        "Status": FeatureStatusType,
+        "UpdatedAt": datetime,
+        "AdditionalConfiguration": List[DetectorAdditionalConfigurationResultTypeDef],
+    },
+    total=False,
+)
+
+DetectorFeatureConfigurationTypeDef = TypedDict(
+    "DetectorFeatureConfigurationTypeDef",
+    {
+        "Name": DetectorFeatureType,
+        "Status": FeatureStatusType,
+        "AdditionalConfiguration": Sequence[DetectorAdditionalConfigurationTypeDef],
     },
+    total=False,
 )
 
 EbsVolumeDetailsTypeDef = TypedDict(
     "EbsVolumeDetailsTypeDef",
     {
         "ScannedVolumeDetails": List[VolumeDetailTypeDef],
         "SkippedVolumeDetails": List[VolumeDetailTypeDef],
@@ -2195,41 +2298,41 @@
     total=False,
 )
 
 GetFindingsStatisticsResponseTypeDef = TypedDict(
     "GetFindingsStatisticsResponseTypeDef",
     {
         "FindingStatistics": FindingStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "Master": MasterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetUsageStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsageStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2243,37 +2346,35 @@
         "Unit": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetUsageStatisticsRequestRequestTypeDef(
     _RequiredGetUsageStatisticsRequestRequestTypeDef,
     _OptionalGetUsageStatisticsRequestRequestTypeDef,
 ):
     pass
 
-
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "Name": str,
         "HostPath": HostPathTypeDef,
     },
     total=False,
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 KubernetesConfigurationResultTypeDef = TypedDict(
     "KubernetesConfigurationResultTypeDef",
     {
         "AuditLogs": KubernetesAuditLogsConfigurationResultTypeDef,
@@ -2283,22 +2384,63 @@
 KubernetesConfigurationTypeDef = TypedDict(
     "KubernetesConfigurationTypeDef",
     {
         "AuditLogs": KubernetesAuditLogsConfigurationTypeDef,
     },
 )
 
+ProcessDetailsTypeDef = TypedDict(
+    "ProcessDetailsTypeDef",
+    {
+        "Name": str,
+        "ExecutablePath": str,
+        "ExecutableSha256": str,
+        "NamespacePid": int,
+        "Pwd": str,
+        "Pid": int,
+        "StartTime": datetime,
+        "Uuid": str,
+        "ParentUuid": str,
+        "User": str,
+        "UserId": int,
+        "Euid": int,
+        "Lineage": List[LineageObjectTypeDef],
+    },
+    total=False,
+)
+
 MalwareProtectionConfigurationTypeDef = TypedDict(
     "MalwareProtectionConfigurationTypeDef",
     {
         "ScanEc2InstanceWithFindings": ScanEc2InstanceWithFindingsTypeDef,
     },
     total=False,
 )
 
+MemberFeaturesConfigurationResultTypeDef = TypedDict(
+    "MemberFeaturesConfigurationResultTypeDef",
+    {
+        "Name": OrgFeatureType,
+        "Status": FeatureStatusType,
+        "UpdatedAt": datetime,
+        "AdditionalConfiguration": List[MemberAdditionalConfigurationResultTypeDef],
+    },
+    total=False,
+)
+
+MemberFeaturesConfigurationTypeDef = TypedDict(
+    "MemberFeaturesConfigurationTypeDef",
+    {
+        "Name": OrgFeatureType,
+        "Status": FeatureStatusType,
+        "AdditionalConfiguration": Sequence[MemberAdditionalConfigurationTypeDef],
+    },
+    total=False,
+)
+
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "Ipv6Addresses": List[str],
         "NetworkInterfaceId": str,
         "PrivateDnsName": str,
         "PrivateIpAddress": str,
@@ -2308,14 +2450,44 @@
         "SecurityGroups": List[SecurityGroupTypeDef],
         "SubnetId": str,
         "VpcId": str,
     },
     total=False,
 )
 
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "SubnetIds": List[str],
+        "VpcId": str,
+        "SecurityGroups": List[SecurityGroupTypeDef],
+    },
+    total=False,
+)
+
+OrganizationFeatureConfigurationResultTypeDef = TypedDict(
+    "OrganizationFeatureConfigurationResultTypeDef",
+    {
+        "Name": OrgFeatureType,
+        "AutoEnable": OrgFeatureStatusType,
+        "AdditionalConfiguration": List[OrganizationAdditionalConfigurationResultTypeDef],
+    },
+    total=False,
+)
+
+OrganizationFeatureConfigurationTypeDef = TypedDict(
+    "OrganizationFeatureConfigurationTypeDef",
+    {
+        "Name": OrgFeatureType,
+        "AutoEnable": OrgFeatureStatusType,
+        "AdditionalConfiguration": Sequence[OrganizationAdditionalConfigurationTypeDef],
+    },
+    total=False,
+)
+
 OrganizationScanEc2InstanceWithFindingsResultTypeDef = TypedDict(
     "OrganizationScanEc2InstanceWithFindingsResultTypeDef",
     {
         "EbsVolumes": OrganizationEbsVolumesResultTypeDef,
     },
     total=False,
 )
@@ -2385,14 +2557,15 @@
         "TriggerDetails": TriggerDetailsTypeDef,
         "ResourceDetails": ResourceDetailsTypeDef,
         "ScanResultDetails": ScanResultDetailsTypeDef,
         "AccountId": str,
         "TotalBytes": int,
         "FileCount": int,
         "AttachedVolumes": List[VolumeDetailTypeDef],
+        "ScanType": ScanTypeType,
     },
     total=False,
 )
 
 UsageAccountResultTypeDef = TypedDict(
     "UsageAccountResultTypeDef",
     {
@@ -2425,14 +2598,23 @@
     {
         "Resource": str,
         "Total": TotalTypeDef,
     },
     total=False,
 )
 
+CoverageResourceDetailsTypeDef = TypedDict(
+    "CoverageResourceDetailsTypeDef",
+    {
+        "EksClusterDetails": CoverageEksClusterDetailsTypeDef,
+        "ResourceType": Literal["EKS"],
+    },
+    total=False,
+)
+
 PermissionConfigurationTypeDef = TypedDict(
     "PermissionConfigurationTypeDef",
     {
         "BucketLevelPermissions": BucketLevelPermissionsTypeDef,
         "AccountLevelPermissions": AccountLevelPermissionsTypeDef,
     },
     total=False,
@@ -2454,31 +2636,29 @@
         "Rank": int,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateFilterRequestRequestTypeDef(
     _RequiredCreateFilterRequestRequestTypeDef, _OptionalCreateFilterRequestRequestTypeDef
 ):
     pass
 
-
 GetFilterResponseTypeDef = TypedDict(
     "GetFilterResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "Action": FilterActionType,
         "Rank": int,
         "FindingCriteria": FindingCriteriaTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetFindingsStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2489,46 +2669,42 @@
     "_OptionalGetFindingsStatisticsRequestRequestTypeDef",
     {
         "FindingCriteria": FindingCriteriaTypeDef,
     },
     total=False,
 )
 
-
 class GetFindingsStatisticsRequestRequestTypeDef(
     _RequiredGetFindingsStatisticsRequestRequestTypeDef,
     _OptionalGetFindingsStatisticsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "_RequiredListFindingsRequestListFindingsPaginateTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "_OptionalListFindingsRequestListFindingsPaginateTypeDef",
     {
         "FindingCriteria": FindingCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListFindingsRequestListFindingsPaginateTypeDef(
     _RequiredListFindingsRequestListFindingsPaginateTypeDef,
     _OptionalListFindingsRequestListFindingsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredListFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListFindingsRequestRequestTypeDef = TypedDict(
@@ -2538,21 +2714,19 @@
         "SortCriteria": SortCriteriaTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListFindingsRequestRequestTypeDef(
     _RequiredListFindingsRequestRequestTypeDef, _OptionalListFindingsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFilterRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FilterName": str,
     },
 )
@@ -2563,20 +2737,26 @@
         "Action": FilterActionType,
         "Rank": int,
         "FindingCriteria": FindingCriteriaTypeDef,
     },
     total=False,
 )
 
-
 class UpdateFilterRequestRequestTypeDef(
     _RequiredUpdateFilterRequestRequestTypeDef, _OptionalUpdateFilterRequestRequestTypeDef
 ):
     pass
 
+CoverageFilterCriteriaTypeDef = TypedDict(
+    "CoverageFilterCriteriaTypeDef",
+    {
+        "FilterCriterion": Sequence[CoverageFilterCriterionTypeDef],
+    },
+    total=False,
+)
 
 DataSourcesFreeTrialTypeDef = TypedDict(
     "DataSourcesFreeTrialTypeDef",
     {
         "CloudTrail": DataSourceFreeTrialTypeDef,
         "DnsLogs": DataSourceFreeTrialTypeDef,
         "FlowLogs": DataSourceFreeTrialTypeDef,
@@ -2631,14 +2811,41 @@
         "HostNetwork": bool,
         "Containers": List[ContainerTypeDef],
         "Volumes": List[VolumeTypeDef],
     },
     total=False,
 )
 
+RuntimeContextTypeDef = TypedDict(
+    "RuntimeContextTypeDef",
+    {
+        "ModifyingProcess": ProcessDetailsTypeDef,
+        "ModifiedAt": datetime,
+        "ScriptPath": str,
+        "LibraryPath": str,
+        "LdPreloadValue": str,
+        "SocketPath": str,
+        "RuncBinaryPath": str,
+        "ReleaseAgentPath": str,
+        "MountSource": str,
+        "MountTarget": str,
+        "FileSystemType": str,
+        "Flags": List[str],
+        "ModuleName": str,
+        "ModuleFilePath": str,
+        "ModuleSha256": str,
+        "ShellHistoryFilePath": str,
+        "TargetProcess": ProcessDetailsTypeDef,
+        "AddressFamily": str,
+        "IanaProtocolNumber": int,
+        "MemoryRegions": List[str],
+    },
+    total=False,
+)
+
 DataSourceConfigurationsTypeDef = TypedDict(
     "DataSourceConfigurationsTypeDef",
     {
         "S3Logs": S3LogsConfigurationTypeDef,
         "Kubernetes": KubernetesConfigurationTypeDef,
         "MalwareProtection": MalwareProtectionConfigurationTypeDef,
     },
@@ -2661,14 +2868,30 @@
         "Platform": str,
         "ProductCodes": List[ProductCodeTypeDef],
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+LambdaDetailsTypeDef = TypedDict(
+    "LambdaDetailsTypeDef",
+    {
+        "FunctionArn": str,
+        "FunctionName": str,
+        "Description": str,
+        "LastModifiedAt": datetime,
+        "RevisionId": str,
+        "FunctionVersion": str,
+        "Role": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 OrganizationMalwareProtectionConfigurationResultTypeDef = TypedDict(
     "OrganizationMalwareProtectionConfigurationResultTypeDef",
     {
         "ScanEc2InstanceWithFindings": OrganizationScanEc2InstanceWithFindingsResultTypeDef,
     },
     total=False,
 )
@@ -2765,15 +2988,15 @@
 )
 
 DescribeMalwareScansResponseTypeDef = TypedDict(
     "DescribeMalwareScansResponseTypeDef",
     {
         "Scans": List[ScanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UsageStatisticsTypeDef = TypedDict(
     "UsageStatisticsTypeDef",
     {
         "SumByAccount": List[UsageAccountResultTypeDef],
@@ -2781,23 +3004,102 @@
         "SumByResource": List[UsageResourceResultTypeDef],
         "TopResources": List[UsageResourceResultTypeDef],
         "SumByFeature": List[UsageFeatureResultTypeDef],
     },
     total=False,
 )
 
+CoverageResourceTypeDef = TypedDict(
+    "CoverageResourceTypeDef",
+    {
+        "ResourceId": str,
+        "DetectorId": str,
+        "AccountId": str,
+        "ResourceDetails": CoverageResourceDetailsTypeDef,
+        "CoverageStatus": CoverageStatusType,
+        "Issue": str,
+        "UpdatedAt": datetime,
+    },
+    total=False,
+)
+
 PublicAccessTypeDef = TypedDict(
     "PublicAccessTypeDef",
     {
         "PermissionConfiguration": PermissionConfigurationTypeDef,
         "EffectivePermission": str,
     },
     total=False,
 )
 
+_RequiredGetCoverageStatisticsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetCoverageStatisticsRequestRequestTypeDef",
+    {
+        "DetectorId": str,
+        "StatisticsType": Sequence[CoverageStatisticsTypeType],
+    },
+)
+_OptionalGetCoverageStatisticsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetCoverageStatisticsRequestRequestTypeDef",
+    {
+        "FilterCriteria": CoverageFilterCriteriaTypeDef,
+    },
+    total=False,
+)
+
+class GetCoverageStatisticsRequestRequestTypeDef(
+    _RequiredGetCoverageStatisticsRequestRequestTypeDef,
+    _OptionalGetCoverageStatisticsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
+    "_RequiredListCoverageRequestListCoveragePaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
+    "_OptionalListCoverageRequestListCoveragePaginateTypeDef",
+    {
+        "FilterCriteria": CoverageFilterCriteriaTypeDef,
+        "SortCriteria": CoverageSortCriteriaTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListCoverageRequestListCoveragePaginateTypeDef(
+    _RequiredListCoverageRequestListCoveragePaginateTypeDef,
+    _OptionalListCoverageRequestListCoveragePaginateTypeDef,
+):
+    pass
+
+_RequiredListCoverageRequestRequestTypeDef = TypedDict(
+    "_RequiredListCoverageRequestRequestTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListCoverageRequestRequestTypeDef = TypedDict(
+    "_OptionalListCoverageRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "FilterCriteria": CoverageFilterCriteriaTypeDef,
+        "SortCriteria": CoverageSortCriteriaTypeDef,
+    },
+    total=False,
+)
+
+class ListCoverageRequestRequestTypeDef(
+    _RequiredListCoverageRequestRequestTypeDef, _OptionalListCoverageRequestRequestTypeDef
+):
+    pass
+
 AccountFreeTrialInfoTypeDef = TypedDict(
     "AccountFreeTrialInfoTypeDef",
     {
         "AccountId": str,
         "DataSources": DataSourcesFreeTrialTypeDef,
         "Features": List[FreeTrialFeatureConfigurationResultTypeDef],
     },
@@ -2818,21 +3120,19 @@
     {
         "Kubernetes": KubernetesConfigurationResultTypeDef,
         "MalwareProtection": MalwareProtectionConfigurationResultTypeDef,
     },
     total=False,
 )
 
-
 class DataSourceConfigurationsResultTypeDef(
     _RequiredDataSourceConfigurationsResultTypeDef, _OptionalDataSourceConfigurationsResultTypeDef
 ):
     pass
 
-
 UnprocessedDataSourcesResultTypeDef = TypedDict(
     "UnprocessedDataSourcesResultTypeDef",
     {
         "MalwareProtection": MalwareProtectionConfigurationResultTypeDef,
     },
     total=False,
 )
@@ -2844,27 +3144,25 @@
     },
 )
 _OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef = TypedDict(
     "_OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef",
     {
         "FilterCriteria": FilterCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef(
     _RequiredDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
     _OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMalwareScansRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMalwareScansRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalDescribeMalwareScansRequestRequestTypeDef = TypedDict(
@@ -2874,22 +3172,20 @@
         "MaxResults": int,
         "FilterCriteria": FilterCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMalwareScansRequestRequestTypeDef(
     _RequiredDescribeMalwareScansRequestRequestTypeDef,
     _OptionalDescribeMalwareScansRequestRequestTypeDef,
 ):
     pass
 
-
 EcsClusterDetailsTypeDef = TypedDict(
     "EcsClusterDetailsTypeDef",
     {
         "Name": str,
         "Arn": str,
         "Status": str,
         "ActiveServicesCount": int,
@@ -2906,14 +3202,23 @@
     {
         "KubernetesUserDetails": KubernetesUserDetailsTypeDef,
         "KubernetesWorkloadDetails": KubernetesWorkloadDetailsTypeDef,
     },
     total=False,
 )
 
+RuntimeDetailsTypeDef = TypedDict(
+    "RuntimeDetailsTypeDef",
+    {
+        "Process": ProcessDetailsTypeDef,
+        "Context": RuntimeContextTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDetectorRequestRequestTypeDef",
     {
         "Enable": bool,
     },
 )
 _OptionalCreateDetectorRequestRequestTypeDef = TypedDict(
@@ -2924,21 +3229,19 @@
         "DataSources": DataSourceConfigurationsTypeDef,
         "Tags": Mapping[str, str],
         "Features": Sequence[DetectorFeatureConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class CreateDetectorRequestRequestTypeDef(
     _RequiredCreateDetectorRequestRequestTypeDef, _OptionalCreateDetectorRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDetectorRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalUpdateDetectorRequestRequestTypeDef = TypedDict(
@@ -2948,21 +3251,19 @@
         "FindingPublishingFrequency": FindingPublishingFrequencyType,
         "DataSources": DataSourceConfigurationsTypeDef,
         "Features": Sequence[DetectorFeatureConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateDetectorRequestRequestTypeDef(
     _RequiredUpdateDetectorRequestRequestTypeDef, _OptionalUpdateDetectorRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateMemberDetectorsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMemberDetectorsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "AccountIds": Sequence[str],
     },
 )
@@ -2971,22 +3272,20 @@
     {
         "DataSources": DataSourceConfigurationsTypeDef,
         "Features": Sequence[MemberFeaturesConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateMemberDetectorsRequestRequestTypeDef(
     _RequiredUpdateMemberDetectorsRequestRequestTypeDef,
     _OptionalUpdateMemberDetectorsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredOrganizationDataSourceConfigurationsResultTypeDef = TypedDict(
     "_RequiredOrganizationDataSourceConfigurationsResultTypeDef",
     {
         "S3Logs": OrganizationS3LogsConfigurationResultTypeDef,
     },
 )
 _OptionalOrganizationDataSourceConfigurationsResultTypeDef = TypedDict(
@@ -2994,22 +3293,20 @@
     {
         "Kubernetes": OrganizationKubernetesConfigurationResultTypeDef,
         "MalwareProtection": OrganizationMalwareProtectionConfigurationResultTypeDef,
     },
     total=False,
 )
 
-
 class OrganizationDataSourceConfigurationsResultTypeDef(
     _RequiredOrganizationDataSourceConfigurationsResultTypeDef,
     _OptionalOrganizationDataSourceConfigurationsResultTypeDef,
 ):
     pass
 
-
 OrganizationDataSourceConfigurationsTypeDef = TypedDict(
     "OrganizationDataSourceConfigurationsTypeDef",
     {
         "S3Logs": OrganizationS3LogsConfigurationTypeDef,
         "Kubernetes": OrganizationKubernetesConfigurationTypeDef,
         "MalwareProtection": OrganizationMalwareProtectionConfigurationTypeDef,
     },
@@ -3026,15 +3323,15 @@
 )
 
 GetMalwareScanSettingsResponseTypeDef = TypedDict(
     "GetMalwareScanSettingsResponseTypeDef",
     {
         "ScanResourceCriteria": ScanResourceCriteriaTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -3045,22 +3342,20 @@
     {
         "ScanResourceCriteria": ScanResourceCriteriaTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
     },
     total=False,
 )
 
-
 class UpdateMalwareScanSettingsRequestRequestTypeDef(
     _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef,
     _OptionalUpdateMalwareScanSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 ScanDetectionsTypeDef = TypedDict(
     "ScanDetectionsTypeDef",
     {
         "ScannedItemCount": ScannedItemCountTypeDef,
         "ThreatsDetectedItemCount": ThreatsDetectedItemCountTypeDef,
         "HighestSeverityThreatDetails": HighestSeverityThreatDetailsTypeDef,
         "ThreatDetectedByName": ThreatDetectedByNameTypeDef,
@@ -3069,15 +3364,24 @@
 )
 
 GetUsageStatisticsResponseTypeDef = TypedDict(
     "GetUsageStatisticsResponseTypeDef",
     {
         "UsageStatistics": UsageStatisticsTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListCoverageResponseTypeDef = TypedDict(
+    "ListCoverageResponseTypeDef",
+    {
+        "Resources": List[CoverageResourceTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 S3BucketDetailTypeDef = TypedDict(
     "S3BucketDetailTypeDef",
     {
         "Arn": str,
@@ -3093,30 +3397,30 @@
 )
 
 GetRemainingFreeTrialDaysResponseTypeDef = TypedDict(
     "GetRemainingFreeTrialDaysResponseTypeDef",
     {
         "Accounts": List[AccountFreeTrialInfoTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDetectorResponseTypeDef = TypedDict(
     "GetDetectorResponseTypeDef",
     {
         "CreatedAt": str,
         "FindingPublishingFrequency": FindingPublishingFrequencyType,
         "ServiceRole": str,
         "Status": DetectorStatusType,
         "UpdatedAt": str,
         "DataSources": DataSourceConfigurationsResultTypeDef,
         "Tags": Dict[str, str],
         "Features": List[DetectorFeatureConfigurationResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMemberDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredMemberDataSourceConfigurationTypeDef",
     {
         "AccountId": str,
@@ -3127,40 +3431,38 @@
     {
         "DataSources": DataSourceConfigurationsResultTypeDef,
         "Features": List[MemberFeaturesConfigurationResultTypeDef],
     },
     total=False,
 )
 
-
 class MemberDataSourceConfigurationTypeDef(
     _RequiredMemberDataSourceConfigurationTypeDef, _OptionalMemberDataSourceConfigurationTypeDef
 ):
     pass
 
-
 CreateDetectorResponseTypeDef = TypedDict(
     "CreateDetectorResponseTypeDef",
     {
         "DetectorId": str,
         "UnprocessedDataSources": UnprocessedDataSourcesResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
         "AutoEnable": bool,
         "MemberAccountLimitReached": bool,
         "DataSources": OrganizationDataSourceConfigurationsResultTypeDef,
         "Features": List[OrganizationFeatureConfigurationResultTypeDef],
         "NextToken": str,
         "AutoEnableOrganizationMembers": AutoEnableMembersType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -3173,22 +3475,20 @@
         "DataSources": OrganizationDataSourceConfigurationsTypeDef,
         "Features": Sequence[OrganizationFeatureConfigurationTypeDef],
         "AutoEnableOrganizationMembers": AutoEnableMembersType,
     },
     total=False,
 )
 
-
 class UpdateOrganizationConfigurationRequestRequestTypeDef(
     _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef,
     _OptionalUpdateOrganizationConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionType": str,
         "AwsApiCallAction": AwsApiCallActionTypeDef,
         "DnsRequestAction": DnsRequestActionTypeDef,
         "NetworkConnectionAction": NetworkConnectionActionTypeDef,
@@ -3204,14 +3504,15 @@
     {
         "ScanId": str,
         "ScanStartedAt": datetime,
         "ScanCompletedAt": datetime,
         "TriggerFindingId": str,
         "Sources": List[str],
         "ScanDetections": ScanDetectionsTypeDef,
+        "ScanType": ScanTypeType,
     },
     total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
@@ -3222,24 +3523,25 @@
         "KubernetesDetails": KubernetesDetailsTypeDef,
         "ResourceType": str,
         "EbsVolumeDetails": EbsVolumeDetailsTypeDef,
         "EcsClusterDetails": EcsClusterDetailsTypeDef,
         "ContainerDetails": ContainerTypeDef,
         "RdsDbInstanceDetails": RdsDbInstanceDetailsTypeDef,
         "RdsDbUserDetails": RdsDbUserDetailsTypeDef,
+        "LambdaDetails": LambdaDetailsTypeDef,
     },
     total=False,
 )
 
 GetMemberDetectorsResponseTypeDef = TypedDict(
     "GetMemberDetectorsResponseTypeDef",
     {
         "MemberDataSourceConfigurations": List[MemberDataSourceConfigurationTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "Action": ActionTypeDef,
@@ -3251,14 +3553,15 @@
         "EventLastSeen": str,
         "ResourceRole": str,
         "ServiceName": str,
         "UserFeedback": str,
         "AdditionalInfo": ServiceAdditionalInfoTypeDef,
         "FeatureName": str,
         "EbsVolumeScanDetails": EbsVolumeScanDetailsTypeDef,
+        "RuntimeDetails": RuntimeDetailsTypeDef,
     },
     total=False,
 )
 
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
@@ -3282,19 +3585,17 @@
         "Partition": str,
         "Service": ServiceTypeDef,
         "Title": str,
     },
     total=False,
 )
 
-
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
-
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "Findings": List[FindingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty/type_defs.pyi` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdminStatusType,
     AutoEnableMembersType,
+    CoverageFilterCriterionKeyType,
+    CoverageSortKeyType,
+    CoverageStatisticsTypeType,
+    CoverageStatusType,
     CriterionKeyType,
     DataSourceStatusType,
     DataSourceType,
     DetectorFeatureResultType,
     DetectorFeatureType,
     DetectorStatusType,
     EbsSnapshotPreservationType,
@@ -34,14 +38,15 @@
     IpSetStatusType,
     OrderByType,
     OrgFeatureStatusType,
     OrgFeatureType,
     PublishingStatusType,
     ScanResultType,
     ScanStatusType,
+    ScanTypeType,
     ThreatIntelSetFormatType,
     ThreatIntelSetStatusType,
     UsageFeatureType,
     UsageStatisticTypeType,
 )
 
 if sys.version_info >= (3, 9):
@@ -49,63 +54,69 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     "AcceptInvitationRequestRequestTypeDef",
     "AccessControlListTypeDef",
     "AccessKeyDetailsTypeDef",
     "AccountDetailTypeDef",
     "FreeTrialFeatureConfigurationResultTypeDef",
     "BlockPublicAccessTypeDef",
     "DnsRequestActionTypeDef",
+    "AddonDetailsTypeDef",
     "AdminAccountTypeDef",
     "AdministratorTypeDef",
     "ArchiveFindingsRequestRequestTypeDef",
     "DomainDetailsTypeDef",
     "RemoteAccountDetailsTypeDef",
     "BucketPolicyTypeDef",
     "CityTypeDef",
     "CloudTrailConfigurationResultTypeDef",
     "ConditionTypeDef",
     "SecurityContextTypeDef",
     "VolumeMountTypeDef",
     "CountryTypeDef",
-    "DetectorFeatureConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
+    "CoverageFilterConditionTypeDef",
+    "CoverageSortCriteriaTypeDef",
+    "CoverageStatisticsTypeDef",
+    "CreateFilterResponseTypeDef",
     "CreateIPSetRequestRequestTypeDef",
+    "CreateIPSetResponseTypeDef",
     "UnprocessedAccountTypeDef",
     "DestinationPropertiesTypeDef",
+    "CreatePublishingDestinationResponseTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
     "CreateThreatIntelSetRequestRequestTypeDef",
+    "CreateThreatIntelSetResponseTypeDef",
     "DNSLogsConfigurationResultTypeDef",
     "FlowLogsConfigurationResultTypeDef",
     "S3LogsConfigurationResultTypeDef",
     "S3LogsConfigurationTypeDef",
     "DataSourceFreeTrialTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DefaultServerSideEncryptionTypeDef",
     "DeleteDetectorRequestRequestTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
     "DeletePublishingDestinationRequestRequestTypeDef",
     "DeleteThreatIntelSetRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "SortCriteriaTypeDef",
     "DescribeOrganizationConfigurationRequestRequestTypeDef",
-    "OrganizationFeatureConfigurationResultTypeDef",
     "DescribePublishingDestinationRequestRequestTypeDef",
     "DestinationTypeDef",
-    "DetectorFeatureConfigurationResultTypeDef",
+    "DetectorAdditionalConfigurationResultTypeDef",
+    "DetectorAdditionalConfigurationTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateFromAdministratorAccountRequestRequestTypeDef",
     "DisassociateFromMasterAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
     "VolumeDetailTypeDef",
     "EbsVolumesResultTypeDef",
     "TagTypeDef",
@@ -114,121 +125,128 @@
     "FilterConditionTypeDef",
     "FindingStatisticsTypeDef",
     "GeoLocationTypeDef",
     "GetAdministratorAccountRequestRequestTypeDef",
     "GetDetectorRequestRequestTypeDef",
     "GetFilterRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
+    "GetIPSetResponseTypeDef",
+    "GetInvitationsCountResponseTypeDef",
     "GetMalwareScanSettingsRequestRequestTypeDef",
     "GetMasterAccountRequestRequestTypeDef",
     "MasterTypeDef",
     "GetMemberDetectorsRequestRequestTypeDef",
     "GetMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "GetRemainingFreeTrialDaysRequestRequestTypeDef",
     "GetThreatIntelSetRequestRequestTypeDef",
+    "GetThreatIntelSetResponseTypeDef",
     "UsageCriteriaTypeDef",
     "HighestSeverityThreatDetailsTypeDef",
     "HostPathTypeDef",
     "IamInstanceProfileTypeDef",
     "ProductCodeTypeDef",
     "InvitationTypeDef",
     "InviteMembersRequestRequestTypeDef",
     "KubernetesAuditLogsConfigurationResultTypeDef",
     "KubernetesAuditLogsConfigurationTypeDef",
     "KubernetesUserDetailsTypeDef",
+    "LineageObjectTypeDef",
+    "ListDetectorsRequestListDetectorsPaginateTypeDef",
     "ListDetectorsRequestRequestTypeDef",
+    "ListDetectorsResponseTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
+    "ListFiltersResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
     "ListIPSetsRequestRequestTypeDef",
+    "ListIPSetsResponseTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     "ListPublishingDestinationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
     "ListThreatIntelSetsRequestRequestTypeDef",
+    "ListThreatIntelSetsResponseTypeDef",
     "LocalIpDetailsTypeDef",
     "LocalPortDetailsTypeDef",
     "LoginAttributeTypeDef",
     "ScanEc2InstanceWithFindingsTypeDef",
-    "MemberFeaturesConfigurationResultTypeDef",
-    "MemberFeaturesConfigurationTypeDef",
+    "MemberAdditionalConfigurationResultTypeDef",
+    "MemberAdditionalConfigurationTypeDef",
     "RemotePortDetailsTypeDef",
     "PrivateIpAddressDetailsTypeDef",
     "SecurityGroupTypeDef",
+    "OrganizationAdditionalConfigurationResultTypeDef",
+    "OrganizationAdditionalConfigurationTypeDef",
     "OrganizationS3LogsConfigurationResultTypeDef",
     "OrganizationS3LogsConfigurationTypeDef",
     "OrganizationEbsVolumesResultTypeDef",
     "OrganizationEbsVolumesTypeDef",
-    "OrganizationFeatureConfigurationTypeDef",
     "OrganizationKubernetesAuditLogsConfigurationResultTypeDef",
     "OrganizationKubernetesAuditLogsConfigurationTypeDef",
     "OrganizationTypeDef",
     "OwnerTypeDef",
+    "PaginatorConfigTypeDef",
     "RdsDbUserDetailsTypeDef",
     "ResourceDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "ScanConditionPairTypeDef",
     "ScannedItemCountTypeDef",
     "ThreatsDetectedItemCountTypeDef",
     "ScanFilePathTypeDef",
     "ScanResultDetailsTypeDef",
     "TriggerDetailsTypeDef",
     "ServiceAdditionalInfoTypeDef",
+    "StartMalwareScanRequestRequestTypeDef",
+    "StartMalwareScanResponseTypeDef",
     "StartMonitoringMembersRequestRequestTypeDef",
     "StopMonitoringMembersRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TotalTypeDef",
     "UnarchiveFindingsRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateFilterResponseTypeDef",
     "UpdateFindingsFeedbackRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "UpdateThreatIntelSetRequestRequestTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
+    "CoverageEksClusterDetailsTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "GetAdministratorAccountResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
     "FindingCriteriaTypeDef",
     "ContainerTypeDef",
-    "CreateFilterResponseTypeDef",
-    "CreateIPSetResponseTypeDef",
-    "CreatePublishingDestinationResponseTypeDef",
-    "CreateThreatIntelSetResponseTypeDef",
-    "GetAdministratorAccountResponseTypeDef",
-    "GetIPSetResponseTypeDef",
-    "GetInvitationsCountResponseTypeDef",
-    "GetThreatIntelSetResponseTypeDef",
-    "ListDetectorsResponseTypeDef",
-    "ListFiltersResponseTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListIPSetsResponseTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListThreatIntelSetsResponseTypeDef",
-    "UpdateFilterResponseTypeDef",
+    "CoverageFilterCriterionTypeDef",
+    "GetCoverageStatisticsResponseTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "DisassociateMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "StartMonitoringMembersResponseTypeDef",
     "StopMonitoringMembersResponseTypeDef",
     "UpdateMemberDetectorsResponseTypeDef",
     "CreatePublishingDestinationRequestRequestTypeDef",
     "DescribePublishingDestinationResponseTypeDef",
     "UpdatePublishingDestinationRequestRequestTypeDef",
     "KubernetesDataSourceFreeTrialTypeDef",
     "MalwareProtectionDataSourceFreeTrialTypeDef",
-    "ListDetectorsRequestListDetectorsPaginateTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    "ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "ListPublishingDestinationsResponseTypeDef",
+    "DetectorFeatureConfigurationResultTypeDef",
+    "DetectorFeatureConfigurationTypeDef",
     "EbsVolumeDetailsTypeDef",
     "ScanEc2InstanceWithFindingsResultTypeDef",
     "EksClusterDetailsTypeDef",
     "RdsDbInstanceDetailsTypeDef",
     "EvidenceTypeDef",
     "FilterCriterionTypeDef",
     "GetFindingsStatisticsResponseTypeDef",
@@ -236,71 +254,87 @@
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "GetUsageStatisticsRequestRequestTypeDef",
     "VolumeTypeDef",
     "ListInvitationsResponseTypeDef",
     "KubernetesConfigurationResultTypeDef",
     "KubernetesConfigurationTypeDef",
+    "ProcessDetailsTypeDef",
     "MalwareProtectionConfigurationTypeDef",
+    "MemberFeaturesConfigurationResultTypeDef",
+    "MemberFeaturesConfigurationTypeDef",
     "NetworkInterfaceTypeDef",
+    "VpcConfigTypeDef",
+    "OrganizationFeatureConfigurationResultTypeDef",
+    "OrganizationFeatureConfigurationTypeDef",
     "OrganizationScanEc2InstanceWithFindingsResultTypeDef",
     "OrganizationScanEc2InstanceWithFindingsTypeDef",
     "OrganizationKubernetesConfigurationResultTypeDef",
     "OrganizationKubernetesConfigurationTypeDef",
     "RemoteIpDetailsTypeDef",
     "ScanConditionTypeDef",
     "ScanThreatNameTypeDef",
     "ScanTypeDef",
     "UsageAccountResultTypeDef",
     "UsageDataSourceResultTypeDef",
     "UsageFeatureResultTypeDef",
     "UsageResourceResultTypeDef",
+    "CoverageResourceDetailsTypeDef",
     "PermissionConfigurationTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "GetFilterResponseTypeDef",
     "GetFindingsStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
+    "CoverageFilterCriteriaTypeDef",
     "DataSourcesFreeTrialTypeDef",
     "MalwareProtectionConfigurationResultTypeDef",
     "FilterCriteriaTypeDef",
     "EcsTaskDetailsTypeDef",
     "KubernetesWorkloadDetailsTypeDef",
+    "RuntimeContextTypeDef",
     "DataSourceConfigurationsTypeDef",
     "InstanceDetailsTypeDef",
+    "LambdaDetailsTypeDef",
     "OrganizationMalwareProtectionConfigurationResultTypeDef",
     "OrganizationMalwareProtectionConfigurationTypeDef",
     "AwsApiCallActionTypeDef",
     "KubernetesApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "RdsLoginAttemptActionTypeDef",
     "ScanResourceCriteriaTypeDef",
     "ThreatDetectedByNameTypeDef",
     "DescribeMalwareScansResponseTypeDef",
     "UsageStatisticsTypeDef",
+    "CoverageResourceTypeDef",
     "PublicAccessTypeDef",
+    "GetCoverageStatisticsRequestRequestTypeDef",
+    "ListCoverageRequestListCoveragePaginateTypeDef",
+    "ListCoverageRequestRequestTypeDef",
     "AccountFreeTrialInfoTypeDef",
     "DataSourceConfigurationsResultTypeDef",
     "UnprocessedDataSourcesResultTypeDef",
     "DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef",
     "DescribeMalwareScansRequestRequestTypeDef",
     "EcsClusterDetailsTypeDef",
     "KubernetesDetailsTypeDef",
+    "RuntimeDetailsTypeDef",
     "CreateDetectorRequestRequestTypeDef",
     "UpdateDetectorRequestRequestTypeDef",
     "UpdateMemberDetectorsRequestRequestTypeDef",
     "OrganizationDataSourceConfigurationsResultTypeDef",
     "OrganizationDataSourceConfigurationsTypeDef",
     "PortProbeActionTypeDef",
     "GetMalwareScanSettingsResponseTypeDef",
     "UpdateMalwareScanSettingsRequestRequestTypeDef",
     "ScanDetectionsTypeDef",
     "GetUsageStatisticsResponseTypeDef",
+    "ListCoverageResponseTypeDef",
     "S3BucketDetailTypeDef",
     "GetRemainingFreeTrialDaysResponseTypeDef",
     "GetDetectorResponseTypeDef",
     "MemberDataSourceConfigurationTypeDef",
     "CreateDetectorResponseTypeDef",
     "DescribeOrganizationConfigurationResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
@@ -385,14 +419,23 @@
         "Domain": str,
         "Protocol": str,
         "Blocked": bool,
     },
     total=False,
 )
 
+AddonDetailsTypeDef = TypedDict(
+    "AddonDetailsTypeDef",
+    {
+        "AddonVersion": str,
+        "AddonStatus": str,
+    },
+    total=False,
+)
+
 AdminAccountTypeDef = TypedDict(
     "AdminAccountTypeDef",
     {
         "AdminAccountId": str,
         "AdminStatus": AdminStatusType,
     },
     total=False,
@@ -499,31 +542,46 @@
     {
         "CountryCode": str,
         "CountryName": str,
     },
     total=False,
 )
 
-DetectorFeatureConfigurationTypeDef = TypedDict(
-    "DetectorFeatureConfigurationTypeDef",
+CoverageFilterConditionTypeDef = TypedDict(
+    "CoverageFilterConditionTypeDef",
     {
-        "Name": DetectorFeatureType,
-        "Status": FeatureStatusType,
+        "Equals": Sequence[str],
+        "NotEquals": Sequence[str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CoverageSortCriteriaTypeDef = TypedDict(
+    "CoverageSortCriteriaTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AttributeName": CoverageSortKeyType,
+        "OrderBy": OrderByType,
+    },
+    total=False,
+)
+
+CoverageStatisticsTypeDef = TypedDict(
+    "CoverageStatisticsTypeDef",
+    {
+        "CountByResourceType": Dict[Literal["EKS"], int],
+        "CountByCoverageStatus": Dict[CoverageStatusType, int],
+    },
+    total=False,
+)
+
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateIPSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -538,19 +596,29 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateIPSetRequestRequestTypeDef(
     _RequiredCreateIPSetRequestRequestTypeDef, _OptionalCreateIPSetRequestRequestTypeDef
 ):
     pass
 
+
+CreateIPSetResponseTypeDef = TypedDict(
+    "CreateIPSetResponseTypeDef",
+    {
+        "IpSetId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UnprocessedAccountTypeDef = TypedDict(
     "UnprocessedAccountTypeDef",
     {
         "AccountId": str,
         "Result": str,
     },
 )
@@ -560,34 +628,44 @@
     {
         "DestinationArn": str,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+CreatePublishingDestinationResponseTypeDef = TypedDict(
+    "CreatePublishingDestinationResponseTypeDef",
+    {
+        "DestinationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSampleFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSampleFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalCreateSampleFindingsRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSampleFindingsRequestRequestTypeDef",
     {
         "FindingTypes": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateSampleFindingsRequestRequestTypeDef(
     _RequiredCreateSampleFindingsRequestRequestTypeDef,
     _OptionalCreateSampleFindingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateThreatIntelSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "Name": str,
         "Format": ThreatIntelSetFormatType,
         "Location": str,
@@ -599,20 +677,30 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateThreatIntelSetRequestRequestTypeDef(
     _RequiredCreateThreatIntelSetRequestRequestTypeDef,
     _OptionalCreateThreatIntelSetRequestRequestTypeDef,
 ):
     pass
 
+
+CreateThreatIntelSetResponseTypeDef = TypedDict(
+    "CreateThreatIntelSetResponseTypeDef",
+    {
+        "ThreatIntelSetId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DNSLogsConfigurationResultTypeDef = TypedDict(
     "DNSLogsConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
@@ -711,24 +799,14 @@
     "DeleteThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 SortCriteriaTypeDef = TypedDict(
     "SortCriteriaTypeDef",
     {
         "AttributeName": str,
         "OrderBy": OrderByType,
     },
     total=False,
@@ -745,28 +823,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeOrganizationConfigurationRequestRequestTypeDef(
     _RequiredDescribeOrganizationConfigurationRequestRequestTypeDef,
     _OptionalDescribeOrganizationConfigurationRequestRequestTypeDef,
 ):
     pass
 
-OrganizationFeatureConfigurationResultTypeDef = TypedDict(
-    "OrganizationFeatureConfigurationResultTypeDef",
-    {
-        "Name": OrgFeatureType,
-        "AutoEnable": OrgFeatureStatusType,
-    },
-    total=False,
-)
 
 DescribePublishingDestinationRequestRequestTypeDef = TypedDict(
     "DescribePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
         "DestinationId": str,
     },
@@ -777,24 +848,33 @@
     {
         "DestinationId": str,
         "DestinationType": Literal["S3"],
         "Status": PublishingStatusType,
     },
 )
 
-DetectorFeatureConfigurationResultTypeDef = TypedDict(
-    "DetectorFeatureConfigurationResultTypeDef",
+DetectorAdditionalConfigurationResultTypeDef = TypedDict(
+    "DetectorAdditionalConfigurationResultTypeDef",
     {
-        "Name": DetectorFeatureResultType,
+        "Name": Literal["EKS_ADDON_MANAGEMENT"],
         "Status": FeatureStatusType,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
+DetectorAdditionalConfigurationTypeDef = TypedDict(
+    "DetectorAdditionalConfigurationTypeDef",
+    {
+        "Name": Literal["EKS_ADDON_MANAGEMENT"],
+        "Status": FeatureStatusType,
+    },
+    total=False,
+)
+
 DisableOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     {
         "AdminAccountId": str,
     },
 )
 
@@ -921,14 +1001,34 @@
     "GetIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "IpSetId": str,
     },
 )
 
+GetIPSetResponseTypeDef = TypedDict(
+    "GetIPSetResponseTypeDef",
+    {
+        "Name": str,
+        "Format": IpSetFormatType,
+        "Location": str,
+        "Status": IpSetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "InvitationsCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "GetMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 
@@ -982,45 +1082,61 @@
         "DetectorId": str,
         "InvitedAt": str,
         "AdministratorId": str,
     },
     total=False,
 )
 
+
 class MemberTypeDef(_RequiredMemberTypeDef, _OptionalMemberTypeDef):
     pass
 
+
 _RequiredGetRemainingFreeTrialDaysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRemainingFreeTrialDaysRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalGetRemainingFreeTrialDaysRequestRequestTypeDef = TypedDict(
     "_OptionalGetRemainingFreeTrialDaysRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
     total=False,
 )
 
+
 class GetRemainingFreeTrialDaysRequestRequestTypeDef(
     _RequiredGetRemainingFreeTrialDaysRequestRequestTypeDef,
     _OptionalGetRemainingFreeTrialDaysRequestRequestTypeDef,
 ):
     pass
 
+
 GetThreatIntelSetRequestRequestTypeDef = TypedDict(
     "GetThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
     },
 )
 
+GetThreatIntelSetResponseTypeDef = TypedDict(
+    "GetThreatIntelSetResponseTypeDef",
+    {
+        "Name": str,
+        "Format": ThreatIntelSetFormatType,
+        "Location": str,
+        "Status": ThreatIntelSetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UsageCriteriaTypeDef = TypedDict(
     "UsageCriteriaTypeDef",
     {
         "AccountIds": Sequence[str],
         "DataSources": Sequence[DataSourceType],
         "Resources": Sequence[str],
         "Features": Sequence[UsageFeatureType],
@@ -1087,19 +1203,21 @@
     {
         "DisableEmailNotification": bool,
         "Message": str,
     },
     total=False,
 )
 
+
 class InviteMembersRequestRequestTypeDef(
     _RequiredInviteMembersRequestRequestTypeDef, _OptionalInviteMembersRequestRequestTypeDef
 ):
     pass
 
+
 KubernetesAuditLogsConfigurationResultTypeDef = TypedDict(
     "KubernetesAuditLogsConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
@@ -1112,27 +1230,83 @@
 
 KubernetesUserDetailsTypeDef = TypedDict(
     "KubernetesUserDetailsTypeDef",
     {
         "Username": str,
         "Uid": str,
         "Groups": List[str],
+        "SessionName": List[str],
+    },
+    total=False,
+)
+
+LineageObjectTypeDef = TypedDict(
+    "LineageObjectTypeDef",
+    {
+        "StartTime": datetime,
+        "NamespacePid": int,
+        "UserId": int,
+        "Name": str,
+        "Pid": int,
+        "Uuid": str,
+        "ExecutablePath": str,
+        "Euid": int,
+        "ParentUuid": str,
+    },
+    total=False,
+)
+
+ListDetectorsRequestListDetectorsPaginateTypeDef = TypedDict(
+    "ListDetectorsRequestListDetectorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDetectorsRequestRequestTypeDef = TypedDict(
     "ListDetectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListDetectorsResponseTypeDef = TypedDict(
+    "ListDetectorsResponseTypeDef",
+    {
+        "DetectorIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "_RequiredListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "_OptionalListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFiltersRequestListFiltersPaginateTypeDef(
+    _RequiredListFiltersRequestListFiltersPaginateTypeDef,
+    _OptionalListFiltersRequestListFiltersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFiltersRequestRequestTypeDef = TypedDict(
     "_RequiredListFiltersRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListFiltersRequestRequestTypeDef = TypedDict(
@@ -1140,19 +1314,61 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListFiltersRequestRequestTypeDef(
     _RequiredListFiltersRequestRequestTypeDef, _OptionalListFiltersRequestRequestTypeDef
 ):
     pass
 
+
+ListFiltersResponseTypeDef = TypedDict(
+    "ListFiltersResponseTypeDef",
+    {
+        "FilterNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "FindingIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "_RequiredListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "_OptionalListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListIPSetsRequestListIPSetsPaginateTypeDef(
+    _RequiredListIPSetsRequestListIPSetsPaginateTypeDef,
+    _OptionalListIPSetsRequestListIPSetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListIPSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListIPSetsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListIPSetsRequestRequestTypeDef = TypedDict(
@@ -1160,28 +1376,70 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListIPSetsRequestRequestTypeDef(
     _RequiredListIPSetsRequestRequestTypeDef, _OptionalListIPSetsRequestRequestTypeDef
 ):
     pass
 
+
+ListIPSetsResponseTypeDef = TypedDict(
+    "ListIPSetsResponseTypeDef",
+    {
+        "IpSetIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInvitationsRequestRequestTypeDef = TypedDict(
     "ListInvitationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "_RequiredListMembersRequestListMembersPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "_OptionalListMembersRequestListMembersPaginateTypeDef",
+    {
+        "OnlyAssociated": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListMembersRequestListMembersPaginateTypeDef(
+    _RequiredListMembersRequestListMembersPaginateTypeDef,
+    _OptionalListMembersRequestListMembersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListMembersRequestRequestTypeDef = TypedDict(
@@ -1190,19 +1448,29 @@
         "MaxResults": int,
         "NextToken": str,
         "OnlyAssociated": str,
     },
     total=False,
 )
 
+
 class ListMembersRequestRequestTypeDef(
     _RequiredListMembersRequestRequestTypeDef, _OptionalListMembersRequestRequestTypeDef
 ):
     pass
 
+
+ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOrganizationAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1219,27 +1487,59 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListPublishingDestinationsRequestRequestTypeDef(
     _RequiredListPublishingDestinationsRequestRequestTypeDef,
     _OptionalListPublishingDestinationsRequestRequestTypeDef,
 ):
     pass
 
+
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
+_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
+    "_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
+    "_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef(
+    _RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
+    _OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListThreatIntelSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListThreatIntelSetsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListThreatIntelSetsRequestRequestTypeDef = TypedDict(
@@ -1247,20 +1547,31 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListThreatIntelSetsRequestRequestTypeDef(
     _RequiredListThreatIntelSetsRequestRequestTypeDef,
     _OptionalListThreatIntelSetsRequestRequestTypeDef,
 ):
     pass
 
+
+ListThreatIntelSetsResponseTypeDef = TypedDict(
+    "ListThreatIntelSetsResponseTypeDef",
+    {
+        "ThreatIntelSetIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LocalIpDetailsTypeDef = TypedDict(
     "LocalIpDetailsTypeDef",
     {
         "IpAddressV4": str,
     },
     total=False,
 )
@@ -1289,28 +1600,28 @@
     "ScanEc2InstanceWithFindingsTypeDef",
     {
         "EbsVolumes": bool,
     },
     total=False,
 )
 
-MemberFeaturesConfigurationResultTypeDef = TypedDict(
-    "MemberFeaturesConfigurationResultTypeDef",
+MemberAdditionalConfigurationResultTypeDef = TypedDict(
+    "MemberAdditionalConfigurationResultTypeDef",
     {
-        "Name": OrgFeatureType,
+        "Name": Literal["EKS_ADDON_MANAGEMENT"],
         "Status": FeatureStatusType,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
-MemberFeaturesConfigurationTypeDef = TypedDict(
-    "MemberFeaturesConfigurationTypeDef",
+MemberAdditionalConfigurationTypeDef = TypedDict(
+    "MemberAdditionalConfigurationTypeDef",
     {
-        "Name": OrgFeatureType,
+        "Name": Literal["EKS_ADDON_MANAGEMENT"],
         "Status": FeatureStatusType,
     },
     total=False,
 )
 
 RemotePortDetailsTypeDef = TypedDict(
     "RemotePortDetailsTypeDef",
@@ -1335,14 +1646,32 @@
     {
         "GroupId": str,
         "GroupName": str,
     },
     total=False,
 )
 
+OrganizationAdditionalConfigurationResultTypeDef = TypedDict(
+    "OrganizationAdditionalConfigurationResultTypeDef",
+    {
+        "Name": Literal["EKS_ADDON_MANAGEMENT"],
+        "AutoEnable": OrgFeatureStatusType,
+    },
+    total=False,
+)
+
+OrganizationAdditionalConfigurationTypeDef = TypedDict(
+    "OrganizationAdditionalConfigurationTypeDef",
+    {
+        "Name": Literal["EKS_ADDON_MANAGEMENT"],
+        "AutoEnable": OrgFeatureStatusType,
+    },
+    total=False,
+)
+
 OrganizationS3LogsConfigurationResultTypeDef = TypedDict(
     "OrganizationS3LogsConfigurationResultTypeDef",
     {
         "AutoEnable": bool,
     },
 )
 
@@ -1365,23 +1694,14 @@
     "OrganizationEbsVolumesTypeDef",
     {
         "AutoEnable": bool,
     },
     total=False,
 )
 
-OrganizationFeatureConfigurationTypeDef = TypedDict(
-    "OrganizationFeatureConfigurationTypeDef",
-    {
-        "Name": OrgFeatureType,
-        "AutoEnable": OrgFeatureStatusType,
-    },
-    total=False,
-)
-
 OrganizationKubernetesAuditLogsConfigurationResultTypeDef = TypedDict(
     "OrganizationKubernetesAuditLogsConfigurationResultTypeDef",
     {
         "AutoEnable": bool,
     },
 )
 
@@ -1407,14 +1727,24 @@
     "OwnerTypeDef",
     {
         "Id": str,
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
 RdsDbUserDetailsTypeDef = TypedDict(
     "RdsDbUserDetailsTypeDef",
     {
         "User": str,
         "Application": str,
         "Database": str,
         "Ssl": str,
@@ -1427,33 +1757,46 @@
     "ResourceDetailsTypeDef",
     {
         "InstanceArn": str,
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
 _RequiredScanConditionPairTypeDef = TypedDict(
     "_RequiredScanConditionPairTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalScanConditionPairTypeDef = TypedDict(
     "_OptionalScanConditionPairTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class ScanConditionPairTypeDef(
     _RequiredScanConditionPairTypeDef, _OptionalScanConditionPairTypeDef
 ):
     pass
 
+
 ScannedItemCountTypeDef = TypedDict(
     "ScannedItemCountTypeDef",
     {
         "TotalGb": int,
         "Files": int,
         "Volumes": int,
     },
@@ -1501,14 +1844,29 @@
     {
         "Value": str,
         "Type": str,
     },
     total=False,
 )
 
+StartMalwareScanRequestRequestTypeDef = TypedDict(
+    "StartMalwareScanRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+
+StartMalwareScanResponseTypeDef = TypedDict(
+    "StartMalwareScanResponseTypeDef",
+    {
+        "ScanId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartMonitoringMembersRequestRequestTypeDef = TypedDict(
     "StartMonitoringMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
         "AccountIds": Sequence[str],
     },
 )
@@ -1550,14 +1908,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateFilterResponseTypeDef = TypedDict(
+    "UpdateFilterResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateFindingsFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFindingsFeedbackRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingIds": Sequence[str],
         "Feedback": FeedbackType,
     },
@@ -1566,20 +1932,22 @@
     "_OptionalUpdateFindingsFeedbackRequestRequestTypeDef",
     {
         "Comments": str,
     },
     total=False,
 )
 
+
 class UpdateFindingsFeedbackRequestRequestTypeDef(
     _RequiredUpdateFindingsFeedbackRequestRequestTypeDef,
     _OptionalUpdateFindingsFeedbackRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateIPSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "IpSetId": str,
     },
 )
@@ -1589,19 +1957,21 @@
         "Name": str,
         "Location": str,
         "Activate": bool,
     },
     total=False,
 )
 
+
 class UpdateIPSetRequestRequestTypeDef(
     _RequiredUpdateIPSetRequestRequestTypeDef, _OptionalUpdateIPSetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateThreatIntelSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
     },
 )
@@ -1611,20 +1981,22 @@
         "Name": str,
         "Location": str,
         "Activate": bool,
     },
     total=False,
 )
 
+
 class UpdateThreatIntelSetRequestRequestTypeDef(
     _RequiredUpdateThreatIntelSetRequestRequestTypeDef,
     _OptionalUpdateThreatIntelSetRequestRequestTypeDef,
 ):
     pass
 
+
 CreateMembersRequestRequestTypeDef = TypedDict(
     "CreateMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
         "AccountDetails": Sequence[AccountDetailTypeDef],
     },
 )
@@ -1633,14 +2005,42 @@
     "AccountLevelPermissionsTypeDef",
     {
         "BlockPublicAccess": BlockPublicAccessTypeDef,
     },
     total=False,
 )
 
+CoverageEksClusterDetailsTypeDef = TypedDict(
+    "CoverageEksClusterDetailsTypeDef",
+    {
+        "ClusterName": str,
+        "CoveredNodes": int,
+        "CompatibleNodes": int,
+        "AddonDetails": AddonDetailsTypeDef,
+    },
+    total=False,
+)
+
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetAdministratorAccountResponseTypeDef = TypedDict(
+    "GetAdministratorAccountResponseTypeDef",
+    {
+        "Administrator": AdministratorTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BucketLevelPermissionsTypeDef = TypedDict(
     "BucketLevelPermissionsTypeDef",
     {
         "AccessControlList": AccessControlListTypeDef,
         "BucketPolicy": BucketPolicyTypeDef,
         "BlockPublicAccess": BlockPublicAccessTypeDef,
     },
@@ -1665,225 +2065,100 @@
         "ImagePrefix": str,
         "VolumeMounts": List[VolumeMountTypeDef],
         "SecurityContext": SecurityContextTypeDef,
     },
     total=False,
 )
 
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIPSetResponseTypeDef = TypedDict(
-    "CreateIPSetResponseTypeDef",
-    {
-        "IpSetId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePublishingDestinationResponseTypeDef = TypedDict(
-    "CreatePublishingDestinationResponseTypeDef",
-    {
-        "DestinationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateThreatIntelSetResponseTypeDef = TypedDict(
-    "CreateThreatIntelSetResponseTypeDef",
-    {
-        "ThreatIntelSetId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAdministratorAccountResponseTypeDef = TypedDict(
-    "GetAdministratorAccountResponseTypeDef",
-    {
-        "Administrator": AdministratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetIPSetResponseTypeDef = TypedDict(
-    "GetIPSetResponseTypeDef",
-    {
-        "Name": str,
-        "Format": IpSetFormatType,
-        "Location": str,
-        "Status": IpSetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
-    {
-        "InvitationsCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetThreatIntelSetResponseTypeDef = TypedDict(
-    "GetThreatIntelSetResponseTypeDef",
-    {
-        "Name": str,
-        "Format": ThreatIntelSetFormatType,
-        "Location": str,
-        "Status": ThreatIntelSetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDetectorsResponseTypeDef = TypedDict(
-    "ListDetectorsResponseTypeDef",
-    {
-        "DetectorIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListFiltersResponseTypeDef = TypedDict(
-    "ListFiltersResponseTypeDef",
+CoverageFilterCriterionTypeDef = TypedDict(
+    "CoverageFilterCriterionTypeDef",
     {
-        "FilterNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "FindingIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListIPSetsResponseTypeDef = TypedDict(
-    "ListIPSetsResponseTypeDef",
-    {
-        "IpSetIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    {
-        "AdminAccounts": List[AdminAccountTypeDef],
-        "NextToken": str,
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
-ListThreatIntelSetsResponseTypeDef = TypedDict(
-    "ListThreatIntelSetsResponseTypeDef",
-    {
-        "ThreatIntelSetIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CriterionKey": CoverageFilterCriterionKeyType,
+        "FilterCondition": CoverageFilterConditionTypeDef,
     },
+    total=False,
 )
 
-UpdateFilterResponseTypeDef = TypedDict(
-    "UpdateFilterResponseTypeDef",
+GetCoverageStatisticsResponseTypeDef = TypedDict(
+    "GetCoverageStatisticsResponseTypeDef",
     {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CoverageStatistics": CoverageStatisticsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMembersResponseTypeDef = TypedDict(
     "CreateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteMembersResponseTypeDef = TypedDict(
     "DeleteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateMembersResponseTypeDef = TypedDict(
     "DisassociateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InviteMembersResponseTypeDef = TypedDict(
     "InviteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartMonitoringMembersResponseTypeDef = TypedDict(
     "StartMonitoringMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopMonitoringMembersResponseTypeDef = TypedDict(
     "StopMonitoringMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMemberDetectorsResponseTypeDef = TypedDict(
     "UpdateMemberDetectorsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -1895,29 +2170,31 @@
     "_OptionalCreatePublishingDestinationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreatePublishingDestinationRequestRequestTypeDef(
     _RequiredCreatePublishingDestinationRequestRequestTypeDef,
     _OptionalCreatePublishingDestinationRequestRequestTypeDef,
 ):
     pass
 
+
 DescribePublishingDestinationResponseTypeDef = TypedDict(
     "DescribePublishingDestinationResponseTypeDef",
     {
         "DestinationId": str,
         "DestinationType": Literal["S3"],
         "Status": PublishingStatusType,
         "PublishingFailureStartTimestamp": int,
         "DestinationProperties": DestinationPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -1928,20 +2205,22 @@
     "_OptionalUpdatePublishingDestinationRequestRequestTypeDef",
     {
         "DestinationProperties": DestinationPropertiesTypeDef,
     },
     total=False,
 )
 
+
 class UpdatePublishingDestinationRequestRequestTypeDef(
     _RequiredUpdatePublishingDestinationRequestRequestTypeDef,
     _OptionalUpdatePublishingDestinationRequestRequestTypeDef,
 ):
     pass
 
+
 KubernetesDataSourceFreeTrialTypeDef = TypedDict(
     "KubernetesDataSourceFreeTrialTypeDef",
     {
         "AuditLogs": DataSourceFreeTrialTypeDef,
     },
     total=False,
 )
@@ -1950,119 +2229,14 @@
     "MalwareProtectionDataSourceFreeTrialTypeDef",
     {
         "ScanEc2InstanceWithFindings": DataSourceFreeTrialTypeDef,
     },
     total=False,
 )
 
-ListDetectorsRequestListDetectorsPaginateTypeDef = TypedDict(
-    "ListDetectorsRequestListDetectorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "_RequiredListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "_OptionalListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFiltersRequestListFiltersPaginateTypeDef(
-    _RequiredListFiltersRequestListFiltersPaginateTypeDef,
-    _OptionalListFiltersRequestListFiltersPaginateTypeDef,
-):
-    pass
-
-_RequiredListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "_RequiredListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "_OptionalListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListIPSetsRequestListIPSetsPaginateTypeDef(
-    _RequiredListIPSetsRequestListIPSetsPaginateTypeDef,
-    _OptionalListIPSetsRequestListIPSetsPaginateTypeDef,
-):
-    pass
-
-ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "_RequiredListMembersRequestListMembersPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "_OptionalListMembersRequestListMembersPaginateTypeDef",
-    {
-        "OnlyAssociated": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListMembersRequestListMembersPaginateTypeDef(
-    _RequiredListMembersRequestListMembersPaginateTypeDef,
-    _OptionalListMembersRequestListMembersPaginateTypeDef,
-):
-    pass
-
-ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
-    "_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
-    "_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef(
-    _RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
-    _OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingIds": Sequence[str],
     },
 )
@@ -2070,26 +2244,49 @@
     "_OptionalGetFindingsRequestRequestTypeDef",
     {
         "SortCriteria": SortCriteriaTypeDef,
     },
     total=False,
 )
 
+
 class GetFindingsRequestRequestTypeDef(
     _RequiredGetFindingsRequestRequestTypeDef, _OptionalGetFindingsRequestRequestTypeDef
 ):
     pass
 
+
 ListPublishingDestinationsResponseTypeDef = TypedDict(
     "ListPublishingDestinationsResponseTypeDef",
     {
         "Destinations": List[DestinationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DetectorFeatureConfigurationResultTypeDef = TypedDict(
+    "DetectorFeatureConfigurationResultTypeDef",
+    {
+        "Name": DetectorFeatureResultType,
+        "Status": FeatureStatusType,
+        "UpdatedAt": datetime,
+        "AdditionalConfiguration": List[DetectorAdditionalConfigurationResultTypeDef],
     },
+    total=False,
+)
+
+DetectorFeatureConfigurationTypeDef = TypedDict(
+    "DetectorFeatureConfigurationTypeDef",
+    {
+        "Name": DetectorFeatureType,
+        "Status": FeatureStatusType,
+        "AdditionalConfiguration": Sequence[DetectorAdditionalConfigurationTypeDef],
+    },
+    total=False,
 )
 
 EbsVolumeDetailsTypeDef = TypedDict(
     "EbsVolumeDetailsTypeDef",
     {
         "ScannedVolumeDetails": List[VolumeDetailTypeDef],
         "SkippedVolumeDetails": List[VolumeDetailTypeDef],
@@ -2148,41 +2345,41 @@
     total=False,
 )
 
 GetFindingsStatisticsResponseTypeDef = TypedDict(
     "GetFindingsStatisticsResponseTypeDef",
     {
         "FindingStatistics": FindingStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "Master": MasterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetUsageStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsageStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2196,35 +2393,37 @@
         "Unit": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetUsageStatisticsRequestRequestTypeDef(
     _RequiredGetUsageStatisticsRequestRequestTypeDef,
     _OptionalGetUsageStatisticsRequestRequestTypeDef,
 ):
     pass
 
+
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "Name": str,
         "HostPath": HostPathTypeDef,
     },
     total=False,
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 KubernetesConfigurationResultTypeDef = TypedDict(
     "KubernetesConfigurationResultTypeDef",
     {
         "AuditLogs": KubernetesAuditLogsConfigurationResultTypeDef,
@@ -2234,22 +2433,63 @@
 KubernetesConfigurationTypeDef = TypedDict(
     "KubernetesConfigurationTypeDef",
     {
         "AuditLogs": KubernetesAuditLogsConfigurationTypeDef,
     },
 )
 
+ProcessDetailsTypeDef = TypedDict(
+    "ProcessDetailsTypeDef",
+    {
+        "Name": str,
+        "ExecutablePath": str,
+        "ExecutableSha256": str,
+        "NamespacePid": int,
+        "Pwd": str,
+        "Pid": int,
+        "StartTime": datetime,
+        "Uuid": str,
+        "ParentUuid": str,
+        "User": str,
+        "UserId": int,
+        "Euid": int,
+        "Lineage": List[LineageObjectTypeDef],
+    },
+    total=False,
+)
+
 MalwareProtectionConfigurationTypeDef = TypedDict(
     "MalwareProtectionConfigurationTypeDef",
     {
         "ScanEc2InstanceWithFindings": ScanEc2InstanceWithFindingsTypeDef,
     },
     total=False,
 )
 
+MemberFeaturesConfigurationResultTypeDef = TypedDict(
+    "MemberFeaturesConfigurationResultTypeDef",
+    {
+        "Name": OrgFeatureType,
+        "Status": FeatureStatusType,
+        "UpdatedAt": datetime,
+        "AdditionalConfiguration": List[MemberAdditionalConfigurationResultTypeDef],
+    },
+    total=False,
+)
+
+MemberFeaturesConfigurationTypeDef = TypedDict(
+    "MemberFeaturesConfigurationTypeDef",
+    {
+        "Name": OrgFeatureType,
+        "Status": FeatureStatusType,
+        "AdditionalConfiguration": Sequence[MemberAdditionalConfigurationTypeDef],
+    },
+    total=False,
+)
+
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "Ipv6Addresses": List[str],
         "NetworkInterfaceId": str,
         "PrivateDnsName": str,
         "PrivateIpAddress": str,
@@ -2259,14 +2499,44 @@
         "SecurityGroups": List[SecurityGroupTypeDef],
         "SubnetId": str,
         "VpcId": str,
     },
     total=False,
 )
 
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "SubnetIds": List[str],
+        "VpcId": str,
+        "SecurityGroups": List[SecurityGroupTypeDef],
+    },
+    total=False,
+)
+
+OrganizationFeatureConfigurationResultTypeDef = TypedDict(
+    "OrganizationFeatureConfigurationResultTypeDef",
+    {
+        "Name": OrgFeatureType,
+        "AutoEnable": OrgFeatureStatusType,
+        "AdditionalConfiguration": List[OrganizationAdditionalConfigurationResultTypeDef],
+    },
+    total=False,
+)
+
+OrganizationFeatureConfigurationTypeDef = TypedDict(
+    "OrganizationFeatureConfigurationTypeDef",
+    {
+        "Name": OrgFeatureType,
+        "AutoEnable": OrgFeatureStatusType,
+        "AdditionalConfiguration": Sequence[OrganizationAdditionalConfigurationTypeDef],
+    },
+    total=False,
+)
+
 OrganizationScanEc2InstanceWithFindingsResultTypeDef = TypedDict(
     "OrganizationScanEc2InstanceWithFindingsResultTypeDef",
     {
         "EbsVolumes": OrganizationEbsVolumesResultTypeDef,
     },
     total=False,
 )
@@ -2336,14 +2606,15 @@
         "TriggerDetails": TriggerDetailsTypeDef,
         "ResourceDetails": ResourceDetailsTypeDef,
         "ScanResultDetails": ScanResultDetailsTypeDef,
         "AccountId": str,
         "TotalBytes": int,
         "FileCount": int,
         "AttachedVolumes": List[VolumeDetailTypeDef],
+        "ScanType": ScanTypeType,
     },
     total=False,
 )
 
 UsageAccountResultTypeDef = TypedDict(
     "UsageAccountResultTypeDef",
     {
@@ -2376,14 +2647,23 @@
     {
         "Resource": str,
         "Total": TotalTypeDef,
     },
     total=False,
 )
 
+CoverageResourceDetailsTypeDef = TypedDict(
+    "CoverageResourceDetailsTypeDef",
+    {
+        "EksClusterDetails": CoverageEksClusterDetailsTypeDef,
+        "ResourceType": Literal["EKS"],
+    },
+    total=False,
+)
+
 PermissionConfigurationTypeDef = TypedDict(
     "PermissionConfigurationTypeDef",
     {
         "BucketLevelPermissions": BucketLevelPermissionsTypeDef,
         "AccountLevelPermissions": AccountLevelPermissionsTypeDef,
     },
     total=False,
@@ -2405,29 +2685,31 @@
         "Rank": int,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateFilterRequestRequestTypeDef(
     _RequiredCreateFilterRequestRequestTypeDef, _OptionalCreateFilterRequestRequestTypeDef
 ):
     pass
 
+
 GetFilterResponseTypeDef = TypedDict(
     "GetFilterResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "Action": FilterActionType,
         "Rank": int,
         "FindingCriteria": FindingCriteriaTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetFindingsStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2438,42 +2720,46 @@
     "_OptionalGetFindingsStatisticsRequestRequestTypeDef",
     {
         "FindingCriteria": FindingCriteriaTypeDef,
     },
     total=False,
 )
 
+
 class GetFindingsStatisticsRequestRequestTypeDef(
     _RequiredGetFindingsStatisticsRequestRequestTypeDef,
     _OptionalGetFindingsStatisticsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "_RequiredListFindingsRequestListFindingsPaginateTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "_OptionalListFindingsRequestListFindingsPaginateTypeDef",
     {
         "FindingCriteria": FindingCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListFindingsRequestListFindingsPaginateTypeDef(
     _RequiredListFindingsRequestListFindingsPaginateTypeDef,
     _OptionalListFindingsRequestListFindingsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredListFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListFindingsRequestRequestTypeDef = TypedDict(
@@ -2483,19 +2769,21 @@
         "SortCriteria": SortCriteriaTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListFindingsRequestRequestTypeDef(
     _RequiredListFindingsRequestRequestTypeDef, _OptionalListFindingsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFilterRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FilterName": str,
     },
 )
@@ -2506,19 +2794,29 @@
         "Action": FilterActionType,
         "Rank": int,
         "FindingCriteria": FindingCriteriaTypeDef,
     },
     total=False,
 )
 
+
 class UpdateFilterRequestRequestTypeDef(
     _RequiredUpdateFilterRequestRequestTypeDef, _OptionalUpdateFilterRequestRequestTypeDef
 ):
     pass
 
+
+CoverageFilterCriteriaTypeDef = TypedDict(
+    "CoverageFilterCriteriaTypeDef",
+    {
+        "FilterCriterion": Sequence[CoverageFilterCriterionTypeDef],
+    },
+    total=False,
+)
+
 DataSourcesFreeTrialTypeDef = TypedDict(
     "DataSourcesFreeTrialTypeDef",
     {
         "CloudTrail": DataSourceFreeTrialTypeDef,
         "DnsLogs": DataSourceFreeTrialTypeDef,
         "FlowLogs": DataSourceFreeTrialTypeDef,
         "S3Logs": DataSourceFreeTrialTypeDef,
@@ -2572,14 +2870,41 @@
         "HostNetwork": bool,
         "Containers": List[ContainerTypeDef],
         "Volumes": List[VolumeTypeDef],
     },
     total=False,
 )
 
+RuntimeContextTypeDef = TypedDict(
+    "RuntimeContextTypeDef",
+    {
+        "ModifyingProcess": ProcessDetailsTypeDef,
+        "ModifiedAt": datetime,
+        "ScriptPath": str,
+        "LibraryPath": str,
+        "LdPreloadValue": str,
+        "SocketPath": str,
+        "RuncBinaryPath": str,
+        "ReleaseAgentPath": str,
+        "MountSource": str,
+        "MountTarget": str,
+        "FileSystemType": str,
+        "Flags": List[str],
+        "ModuleName": str,
+        "ModuleFilePath": str,
+        "ModuleSha256": str,
+        "ShellHistoryFilePath": str,
+        "TargetProcess": ProcessDetailsTypeDef,
+        "AddressFamily": str,
+        "IanaProtocolNumber": int,
+        "MemoryRegions": List[str],
+    },
+    total=False,
+)
+
 DataSourceConfigurationsTypeDef = TypedDict(
     "DataSourceConfigurationsTypeDef",
     {
         "S3Logs": S3LogsConfigurationTypeDef,
         "Kubernetes": KubernetesConfigurationTypeDef,
         "MalwareProtection": MalwareProtectionConfigurationTypeDef,
     },
@@ -2602,14 +2927,30 @@
         "Platform": str,
         "ProductCodes": List[ProductCodeTypeDef],
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+LambdaDetailsTypeDef = TypedDict(
+    "LambdaDetailsTypeDef",
+    {
+        "FunctionArn": str,
+        "FunctionName": str,
+        "Description": str,
+        "LastModifiedAt": datetime,
+        "RevisionId": str,
+        "FunctionVersion": str,
+        "Role": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 OrganizationMalwareProtectionConfigurationResultTypeDef = TypedDict(
     "OrganizationMalwareProtectionConfigurationResultTypeDef",
     {
         "ScanEc2InstanceWithFindings": OrganizationScanEc2InstanceWithFindingsResultTypeDef,
     },
     total=False,
 )
@@ -2706,15 +3047,15 @@
 )
 
 DescribeMalwareScansResponseTypeDef = TypedDict(
     "DescribeMalwareScansResponseTypeDef",
     {
         "Scans": List[ScanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UsageStatisticsTypeDef = TypedDict(
     "UsageStatisticsTypeDef",
     {
         "SumByAccount": List[UsageAccountResultTypeDef],
@@ -2722,23 +3063,108 @@
         "SumByResource": List[UsageResourceResultTypeDef],
         "TopResources": List[UsageResourceResultTypeDef],
         "SumByFeature": List[UsageFeatureResultTypeDef],
     },
     total=False,
 )
 
+CoverageResourceTypeDef = TypedDict(
+    "CoverageResourceTypeDef",
+    {
+        "ResourceId": str,
+        "DetectorId": str,
+        "AccountId": str,
+        "ResourceDetails": CoverageResourceDetailsTypeDef,
+        "CoverageStatus": CoverageStatusType,
+        "Issue": str,
+        "UpdatedAt": datetime,
+    },
+    total=False,
+)
+
 PublicAccessTypeDef = TypedDict(
     "PublicAccessTypeDef",
     {
         "PermissionConfiguration": PermissionConfigurationTypeDef,
         "EffectivePermission": str,
     },
     total=False,
 )
 
+_RequiredGetCoverageStatisticsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetCoverageStatisticsRequestRequestTypeDef",
+    {
+        "DetectorId": str,
+        "StatisticsType": Sequence[CoverageStatisticsTypeType],
+    },
+)
+_OptionalGetCoverageStatisticsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetCoverageStatisticsRequestRequestTypeDef",
+    {
+        "FilterCriteria": CoverageFilterCriteriaTypeDef,
+    },
+    total=False,
+)
+
+
+class GetCoverageStatisticsRequestRequestTypeDef(
+    _RequiredGetCoverageStatisticsRequestRequestTypeDef,
+    _OptionalGetCoverageStatisticsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
+    "_RequiredListCoverageRequestListCoveragePaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
+    "_OptionalListCoverageRequestListCoveragePaginateTypeDef",
+    {
+        "FilterCriteria": CoverageFilterCriteriaTypeDef,
+        "SortCriteria": CoverageSortCriteriaTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListCoverageRequestListCoveragePaginateTypeDef(
+    _RequiredListCoverageRequestListCoveragePaginateTypeDef,
+    _OptionalListCoverageRequestListCoveragePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListCoverageRequestRequestTypeDef = TypedDict(
+    "_RequiredListCoverageRequestRequestTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListCoverageRequestRequestTypeDef = TypedDict(
+    "_OptionalListCoverageRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "FilterCriteria": CoverageFilterCriteriaTypeDef,
+        "SortCriteria": CoverageSortCriteriaTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCoverageRequestRequestTypeDef(
+    _RequiredListCoverageRequestRequestTypeDef, _OptionalListCoverageRequestRequestTypeDef
+):
+    pass
+
+
 AccountFreeTrialInfoTypeDef = TypedDict(
     "AccountFreeTrialInfoTypeDef",
     {
         "AccountId": str,
         "DataSources": DataSourcesFreeTrialTypeDef,
         "Features": List[FreeTrialFeatureConfigurationResultTypeDef],
     },
@@ -2759,19 +3185,21 @@
     {
         "Kubernetes": KubernetesConfigurationResultTypeDef,
         "MalwareProtection": MalwareProtectionConfigurationResultTypeDef,
     },
     total=False,
 )
 
+
 class DataSourceConfigurationsResultTypeDef(
     _RequiredDataSourceConfigurationsResultTypeDef, _OptionalDataSourceConfigurationsResultTypeDef
 ):
     pass
 
+
 UnprocessedDataSourcesResultTypeDef = TypedDict(
     "UnprocessedDataSourcesResultTypeDef",
     {
         "MalwareProtection": MalwareProtectionConfigurationResultTypeDef,
     },
     total=False,
 )
@@ -2783,25 +3211,27 @@
     },
 )
 _OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef = TypedDict(
     "_OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef",
     {
         "FilterCriteria": FilterCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef(
     _RequiredDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
     _OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMalwareScansRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMalwareScansRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalDescribeMalwareScansRequestRequestTypeDef = TypedDict(
@@ -2811,20 +3241,22 @@
         "MaxResults": int,
         "FilterCriteria": FilterCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMalwareScansRequestRequestTypeDef(
     _RequiredDescribeMalwareScansRequestRequestTypeDef,
     _OptionalDescribeMalwareScansRequestRequestTypeDef,
 ):
     pass
 
+
 EcsClusterDetailsTypeDef = TypedDict(
     "EcsClusterDetailsTypeDef",
     {
         "Name": str,
         "Arn": str,
         "Status": str,
         "ActiveServicesCount": int,
@@ -2841,14 +3273,23 @@
     {
         "KubernetesUserDetails": KubernetesUserDetailsTypeDef,
         "KubernetesWorkloadDetails": KubernetesWorkloadDetailsTypeDef,
     },
     total=False,
 )
 
+RuntimeDetailsTypeDef = TypedDict(
+    "RuntimeDetailsTypeDef",
+    {
+        "Process": ProcessDetailsTypeDef,
+        "Context": RuntimeContextTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDetectorRequestRequestTypeDef",
     {
         "Enable": bool,
     },
 )
 _OptionalCreateDetectorRequestRequestTypeDef = TypedDict(
@@ -2859,19 +3300,21 @@
         "DataSources": DataSourceConfigurationsTypeDef,
         "Tags": Mapping[str, str],
         "Features": Sequence[DetectorFeatureConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class CreateDetectorRequestRequestTypeDef(
     _RequiredCreateDetectorRequestRequestTypeDef, _OptionalCreateDetectorRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDetectorRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalUpdateDetectorRequestRequestTypeDef = TypedDict(
@@ -2881,19 +3324,21 @@
         "FindingPublishingFrequency": FindingPublishingFrequencyType,
         "DataSources": DataSourceConfigurationsTypeDef,
         "Features": Sequence[DetectorFeatureConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateDetectorRequestRequestTypeDef(
     _RequiredUpdateDetectorRequestRequestTypeDef, _OptionalUpdateDetectorRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateMemberDetectorsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMemberDetectorsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "AccountIds": Sequence[str],
     },
 )
@@ -2902,20 +3347,22 @@
     {
         "DataSources": DataSourceConfigurationsTypeDef,
         "Features": Sequence[MemberFeaturesConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateMemberDetectorsRequestRequestTypeDef(
     _RequiredUpdateMemberDetectorsRequestRequestTypeDef,
     _OptionalUpdateMemberDetectorsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredOrganizationDataSourceConfigurationsResultTypeDef = TypedDict(
     "_RequiredOrganizationDataSourceConfigurationsResultTypeDef",
     {
         "S3Logs": OrganizationS3LogsConfigurationResultTypeDef,
     },
 )
 _OptionalOrganizationDataSourceConfigurationsResultTypeDef = TypedDict(
@@ -2923,20 +3370,22 @@
     {
         "Kubernetes": OrganizationKubernetesConfigurationResultTypeDef,
         "MalwareProtection": OrganizationMalwareProtectionConfigurationResultTypeDef,
     },
     total=False,
 )
 
+
 class OrganizationDataSourceConfigurationsResultTypeDef(
     _RequiredOrganizationDataSourceConfigurationsResultTypeDef,
     _OptionalOrganizationDataSourceConfigurationsResultTypeDef,
 ):
     pass
 
+
 OrganizationDataSourceConfigurationsTypeDef = TypedDict(
     "OrganizationDataSourceConfigurationsTypeDef",
     {
         "S3Logs": OrganizationS3LogsConfigurationTypeDef,
         "Kubernetes": OrganizationKubernetesConfigurationTypeDef,
         "MalwareProtection": OrganizationMalwareProtectionConfigurationTypeDef,
     },
@@ -2953,15 +3402,15 @@
 )
 
 GetMalwareScanSettingsResponseTypeDef = TypedDict(
     "GetMalwareScanSettingsResponseTypeDef",
     {
         "ScanResourceCriteria": ScanResourceCriteriaTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2972,20 +3421,22 @@
     {
         "ScanResourceCriteria": ScanResourceCriteriaTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
     },
     total=False,
 )
 
+
 class UpdateMalwareScanSettingsRequestRequestTypeDef(
     _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef,
     _OptionalUpdateMalwareScanSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 ScanDetectionsTypeDef = TypedDict(
     "ScanDetectionsTypeDef",
     {
         "ScannedItemCount": ScannedItemCountTypeDef,
         "ThreatsDetectedItemCount": ThreatsDetectedItemCountTypeDef,
         "HighestSeverityThreatDetails": HighestSeverityThreatDetailsTypeDef,
         "ThreatDetectedByName": ThreatDetectedByNameTypeDef,
@@ -2994,15 +3445,24 @@
 )
 
 GetUsageStatisticsResponseTypeDef = TypedDict(
     "GetUsageStatisticsResponseTypeDef",
     {
         "UsageStatistics": UsageStatisticsTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListCoverageResponseTypeDef = TypedDict(
+    "ListCoverageResponseTypeDef",
+    {
+        "Resources": List[CoverageResourceTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 S3BucketDetailTypeDef = TypedDict(
     "S3BucketDetailTypeDef",
     {
         "Arn": str,
@@ -3018,30 +3478,30 @@
 )
 
 GetRemainingFreeTrialDaysResponseTypeDef = TypedDict(
     "GetRemainingFreeTrialDaysResponseTypeDef",
     {
         "Accounts": List[AccountFreeTrialInfoTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDetectorResponseTypeDef = TypedDict(
     "GetDetectorResponseTypeDef",
     {
         "CreatedAt": str,
         "FindingPublishingFrequency": FindingPublishingFrequencyType,
         "ServiceRole": str,
         "Status": DetectorStatusType,
         "UpdatedAt": str,
         "DataSources": DataSourceConfigurationsResultTypeDef,
         "Tags": Dict[str, str],
         "Features": List[DetectorFeatureConfigurationResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMemberDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredMemberDataSourceConfigurationTypeDef",
     {
         "AccountId": str,
@@ -3052,38 +3512,40 @@
     {
         "DataSources": DataSourceConfigurationsResultTypeDef,
         "Features": List[MemberFeaturesConfigurationResultTypeDef],
     },
     total=False,
 )
 
+
 class MemberDataSourceConfigurationTypeDef(
     _RequiredMemberDataSourceConfigurationTypeDef, _OptionalMemberDataSourceConfigurationTypeDef
 ):
     pass
 
+
 CreateDetectorResponseTypeDef = TypedDict(
     "CreateDetectorResponseTypeDef",
     {
         "DetectorId": str,
         "UnprocessedDataSources": UnprocessedDataSourcesResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
         "AutoEnable": bool,
         "MemberAccountLimitReached": bool,
         "DataSources": OrganizationDataSourceConfigurationsResultTypeDef,
         "Features": List[OrganizationFeatureConfigurationResultTypeDef],
         "NextToken": str,
         "AutoEnableOrganizationMembers": AutoEnableMembersType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -3096,20 +3558,22 @@
         "DataSources": OrganizationDataSourceConfigurationsTypeDef,
         "Features": Sequence[OrganizationFeatureConfigurationTypeDef],
         "AutoEnableOrganizationMembers": AutoEnableMembersType,
     },
     total=False,
 )
 
+
 class UpdateOrganizationConfigurationRequestRequestTypeDef(
     _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef,
     _OptionalUpdateOrganizationConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionType": str,
         "AwsApiCallAction": AwsApiCallActionTypeDef,
         "DnsRequestAction": DnsRequestActionTypeDef,
         "NetworkConnectionAction": NetworkConnectionActionTypeDef,
@@ -3125,14 +3589,15 @@
     {
         "ScanId": str,
         "ScanStartedAt": datetime,
         "ScanCompletedAt": datetime,
         "TriggerFindingId": str,
         "Sources": List[str],
         "ScanDetections": ScanDetectionsTypeDef,
+        "ScanType": ScanTypeType,
     },
     total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
@@ -3143,24 +3608,25 @@
         "KubernetesDetails": KubernetesDetailsTypeDef,
         "ResourceType": str,
         "EbsVolumeDetails": EbsVolumeDetailsTypeDef,
         "EcsClusterDetails": EcsClusterDetailsTypeDef,
         "ContainerDetails": ContainerTypeDef,
         "RdsDbInstanceDetails": RdsDbInstanceDetailsTypeDef,
         "RdsDbUserDetails": RdsDbUserDetailsTypeDef,
+        "LambdaDetails": LambdaDetailsTypeDef,
     },
     total=False,
 )
 
 GetMemberDetectorsResponseTypeDef = TypedDict(
     "GetMemberDetectorsResponseTypeDef",
     {
         "MemberDataSourceConfigurations": List[MemberDataSourceConfigurationTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "Action": ActionTypeDef,
@@ -3172,14 +3638,15 @@
         "EventLastSeen": str,
         "ResourceRole": str,
         "ServiceName": str,
         "UserFeedback": str,
         "AdditionalInfo": ServiceAdditionalInfoTypeDef,
         "FeatureName": str,
         "EbsVolumeScanDetails": EbsVolumeScanDetailsTypeDef,
+        "RuntimeDetails": RuntimeDetailsTypeDef,
     },
     total=False,
 )
 
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
@@ -3203,17 +3670,19 @@
         "Partition": str,
         "Service": ServiceTypeDef,
         "Title": str,
     },
     total=False,
 )
 
+
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
+
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "Findings": List[FindingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/PKG-INFO` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.26.98
-Summary: Type annotations for boto3.GuardDuty 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.GuardDuty 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-guardduty"></a>
 
 # mypy-boto3-guardduty
 
 [![PyPI - mypy-boto3-guardduty](https://img.shields.io/pypi/v/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-guardduty?color=blue)](https://pypistats.org/packages/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,14 +280,15 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_guardduty import GuardDutyClient
 from mypy_boto3_guardduty.paginator import (
     DescribeMalwareScansPaginator,
+    ListCoveragePaginator,
     ListDetectorsPaginator,
     ListFiltersPaginator,
     ListFindingsPaginator,
     ListIPSetsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
@@ -297,14 +298,15 @@
 client: GuardDutyClient = Session().client("guardduty")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_malware_scans_paginator: DescribeMalwareScansPaginator = client.get_paginator(
     "describe_malware_scans"
 )
+list_coverage_paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
 list_detectors_paginator: ListDetectorsPaginator = client.get_paginator("list_detectors")
 list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
 list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
 list_ip_sets_paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")
 list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
 list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
 list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = (
@@ -322,46 +324,55 @@
 `mypy_boto3_guardduty.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_guardduty.literals import (
     AdminStatusType,
     AutoEnableMembersType,
+    CoverageFilterCriterionKeyType,
+    CoverageSortKeyType,
+    CoverageStatisticsTypeType,
+    CoverageStatusType,
     CriterionKeyType,
     DataSourceStatusType,
     DataSourceType,
     DescribeMalwareScansPaginatorName,
     DestinationTypeType,
     DetectorFeatureResultType,
     DetectorFeatureType,
     DetectorStatusType,
     EbsSnapshotPreservationType,
+    FeatureAdditionalConfigurationType,
     FeatureStatusType,
     FeedbackType,
     FilterActionType,
     FindingPublishingFrequencyType,
     FindingStatisticTypeType,
     FreeTrialFeatureResultType,
     IpSetFormatType,
     IpSetStatusType,
+    ListCoveragePaginatorName,
     ListDetectorsPaginatorName,
     ListFiltersPaginatorName,
     ListFindingsPaginatorName,
     ListIPSetsPaginatorName,
     ListInvitationsPaginatorName,
     ListMembersPaginatorName,
     ListOrganizationAdminAccountsPaginatorName,
     ListThreatIntelSetsPaginatorName,
     OrderByType,
+    OrgFeatureAdditionalConfigurationType,
     OrgFeatureStatusType,
     OrgFeatureType,
     PublishingStatusType,
+    ResourceTypeType,
     ScanCriterionKeyType,
     ScanResultType,
     ScanStatusType,
+    ScanTypeType,
     ThreatIntelSetFormatType,
     ThreatIntelSetStatusType,
     UsageFeatureType,
     UsageStatisticTypeType,
     GuardDutyServiceName,
     ServiceName,
     ResourceServiceName,
@@ -387,54 +398,59 @@
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccessKeyDetailsTypeDef,
     AccountDetailTypeDef,
     FreeTrialFeatureConfigurationResultTypeDef,
     BlockPublicAccessTypeDef,
     DnsRequestActionTypeDef,
+    AddonDetailsTypeDef,
     AdminAccountTypeDef,
     AdministratorTypeDef,
     ArchiveFindingsRequestRequestTypeDef,
     DomainDetailsTypeDef,
     RemoteAccountDetailsTypeDef,
     BucketPolicyTypeDef,
     CityTypeDef,
     CloudTrailConfigurationResultTypeDef,
     ConditionTypeDef,
     SecurityContextTypeDef,
     VolumeMountTypeDef,
     CountryTypeDef,
-    DetectorFeatureConfigurationTypeDef,
-    ResponseMetadataTypeDef,
+    CoverageFilterConditionTypeDef,
+    CoverageSortCriteriaTypeDef,
+    CoverageStatisticsTypeDef,
+    CreateFilterResponseTypeDef,
     CreateIPSetRequestRequestTypeDef,
+    CreateIPSetResponseTypeDef,
     UnprocessedAccountTypeDef,
     DestinationPropertiesTypeDef,
+    CreatePublishingDestinationResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
     CreateThreatIntelSetRequestRequestTypeDef,
+    CreateThreatIntelSetResponseTypeDef,
     DNSLogsConfigurationResultTypeDef,
     FlowLogsConfigurationResultTypeDef,
     S3LogsConfigurationResultTypeDef,
     S3LogsConfigurationTypeDef,
     DataSourceFreeTrialTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DefaultServerSideEncryptionTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DeletePublishingDestinationRequestRequestTypeDef,
     DeleteThreatIntelSetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     SortCriteriaTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
-    OrganizationFeatureConfigurationResultTypeDef,
     DescribePublishingDestinationRequestRequestTypeDef,
     DestinationTypeDef,
-    DetectorFeatureConfigurationResultTypeDef,
+    DetectorAdditionalConfigurationResultTypeDef,
+    DetectorAdditionalConfigurationTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateFromAdministratorAccountRequestRequestTypeDef,
     DisassociateFromMasterAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     VolumeDetailTypeDef,
     EbsVolumesResultTypeDef,
     TagTypeDef,
@@ -443,121 +459,128 @@
     FilterConditionTypeDef,
     FindingStatisticsTypeDef,
     GeoLocationTypeDef,
     GetAdministratorAccountRequestRequestTypeDef,
     GetDetectorRequestRequestTypeDef,
     GetFilterRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
+    GetIPSetResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
     GetMalwareScanSettingsRequestRequestTypeDef,
     GetMasterAccountRequestRequestTypeDef,
     MasterTypeDef,
     GetMemberDetectorsRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     GetRemainingFreeTrialDaysRequestRequestTypeDef,
     GetThreatIntelSetRequestRequestTypeDef,
+    GetThreatIntelSetResponseTypeDef,
     UsageCriteriaTypeDef,
     HighestSeverityThreatDetailsTypeDef,
     HostPathTypeDef,
     IamInstanceProfileTypeDef,
     ProductCodeTypeDef,
     InvitationTypeDef,
     InviteMembersRequestRequestTypeDef,
     KubernetesAuditLogsConfigurationResultTypeDef,
     KubernetesAuditLogsConfigurationTypeDef,
     KubernetesUserDetailsTypeDef,
+    LineageObjectTypeDef,
+    ListDetectorsRequestListDetectorsPaginateTypeDef,
     ListDetectorsRequestRequestTypeDef,
+    ListDetectorsResponseTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
+    ListFiltersResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
+    ListIPSetsResponseTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListPublishingDestinationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     ListThreatIntelSetsRequestRequestTypeDef,
+    ListThreatIntelSetsResponseTypeDef,
     LocalIpDetailsTypeDef,
     LocalPortDetailsTypeDef,
     LoginAttributeTypeDef,
     ScanEc2InstanceWithFindingsTypeDef,
-    MemberFeaturesConfigurationResultTypeDef,
-    MemberFeaturesConfigurationTypeDef,
+    MemberAdditionalConfigurationResultTypeDef,
+    MemberAdditionalConfigurationTypeDef,
     RemotePortDetailsTypeDef,
     PrivateIpAddressDetailsTypeDef,
     SecurityGroupTypeDef,
+    OrganizationAdditionalConfigurationResultTypeDef,
+    OrganizationAdditionalConfigurationTypeDef,
     OrganizationS3LogsConfigurationResultTypeDef,
     OrganizationS3LogsConfigurationTypeDef,
     OrganizationEbsVolumesResultTypeDef,
     OrganizationEbsVolumesTypeDef,
-    OrganizationFeatureConfigurationTypeDef,
     OrganizationKubernetesAuditLogsConfigurationResultTypeDef,
     OrganizationKubernetesAuditLogsConfigurationTypeDef,
     OrganizationTypeDef,
     OwnerTypeDef,
+    PaginatorConfigTypeDef,
     RdsDbUserDetailsTypeDef,
     ResourceDetailsTypeDef,
+    ResponseMetadataTypeDef,
     ScanConditionPairTypeDef,
     ScannedItemCountTypeDef,
     ThreatsDetectedItemCountTypeDef,
     ScanFilePathTypeDef,
     ScanResultDetailsTypeDef,
     TriggerDetailsTypeDef,
     ServiceAdditionalInfoTypeDef,
+    StartMalwareScanRequestRequestTypeDef,
+    StartMalwareScanResponseTypeDef,
     StartMonitoringMembersRequestRequestTypeDef,
     StopMonitoringMembersRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TotalTypeDef,
     UnarchiveFindingsRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateFilterResponseTypeDef,
     UpdateFindingsFeedbackRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     UpdateThreatIntelSetRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
+    CoverageEksClusterDetailsTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    GetAdministratorAccountResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     FindingCriteriaTypeDef,
     ContainerTypeDef,
-    CreateFilterResponseTypeDef,
-    CreateIPSetResponseTypeDef,
-    CreatePublishingDestinationResponseTypeDef,
-    CreateThreatIntelSetResponseTypeDef,
-    GetAdministratorAccountResponseTypeDef,
-    GetIPSetResponseTypeDef,
-    GetInvitationsCountResponseTypeDef,
-    GetThreatIntelSetResponseTypeDef,
-    ListDetectorsResponseTypeDef,
-    ListFiltersResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListIPSetsResponseTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListThreatIntelSetsResponseTypeDef,
-    UpdateFilterResponseTypeDef,
+    CoverageFilterCriterionTypeDef,
+    GetCoverageStatisticsResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DisassociateMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     CreatePublishingDestinationRequestRequestTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     UpdatePublishingDestinationRequestRequestTypeDef,
     KubernetesDataSourceFreeTrialTypeDef,
     MalwareProtectionDataSourceFreeTrialTypeDef,
-    ListDetectorsRequestListDetectorsPaginateTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
-    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     ListPublishingDestinationsResponseTypeDef,
+    DetectorFeatureConfigurationResultTypeDef,
+    DetectorFeatureConfigurationTypeDef,
     EbsVolumeDetailsTypeDef,
     ScanEc2InstanceWithFindingsResultTypeDef,
     EksClusterDetailsTypeDef,
     RdsDbInstanceDetailsTypeDef,
     EvidenceTypeDef,
     FilterCriterionTypeDef,
     GetFindingsStatisticsResponseTypeDef,
@@ -565,71 +588,87 @@
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     GetUsageStatisticsRequestRequestTypeDef,
     VolumeTypeDef,
     ListInvitationsResponseTypeDef,
     KubernetesConfigurationResultTypeDef,
     KubernetesConfigurationTypeDef,
+    ProcessDetailsTypeDef,
     MalwareProtectionConfigurationTypeDef,
+    MemberFeaturesConfigurationResultTypeDef,
+    MemberFeaturesConfigurationTypeDef,
     NetworkInterfaceTypeDef,
+    VpcConfigTypeDef,
+    OrganizationFeatureConfigurationResultTypeDef,
+    OrganizationFeatureConfigurationTypeDef,
     OrganizationScanEc2InstanceWithFindingsResultTypeDef,
     OrganizationScanEc2InstanceWithFindingsTypeDef,
     OrganizationKubernetesConfigurationResultTypeDef,
     OrganizationKubernetesConfigurationTypeDef,
     RemoteIpDetailsTypeDef,
     ScanConditionTypeDef,
     ScanThreatNameTypeDef,
     ScanTypeDef,
     UsageAccountResultTypeDef,
     UsageDataSourceResultTypeDef,
     UsageFeatureResultTypeDef,
     UsageResourceResultTypeDef,
+    CoverageResourceDetailsTypeDef,
     PermissionConfigurationTypeDef,
     CreateFilterRequestRequestTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
+    CoverageFilterCriteriaTypeDef,
     DataSourcesFreeTrialTypeDef,
     MalwareProtectionConfigurationResultTypeDef,
     FilterCriteriaTypeDef,
     EcsTaskDetailsTypeDef,
     KubernetesWorkloadDetailsTypeDef,
+    RuntimeContextTypeDef,
     DataSourceConfigurationsTypeDef,
     InstanceDetailsTypeDef,
+    LambdaDetailsTypeDef,
     OrganizationMalwareProtectionConfigurationResultTypeDef,
     OrganizationMalwareProtectionConfigurationTypeDef,
     AwsApiCallActionTypeDef,
     KubernetesApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     RdsLoginAttemptActionTypeDef,
     ScanResourceCriteriaTypeDef,
     ThreatDetectedByNameTypeDef,
     DescribeMalwareScansResponseTypeDef,
     UsageStatisticsTypeDef,
+    CoverageResourceTypeDef,
     PublicAccessTypeDef,
+    GetCoverageStatisticsRequestRequestTypeDef,
+    ListCoverageRequestListCoveragePaginateTypeDef,
+    ListCoverageRequestRequestTypeDef,
     AccountFreeTrialInfoTypeDef,
     DataSourceConfigurationsResultTypeDef,
     UnprocessedDataSourcesResultTypeDef,
     DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
     DescribeMalwareScansRequestRequestTypeDef,
     EcsClusterDetailsTypeDef,
     KubernetesDetailsTypeDef,
+    RuntimeDetailsTypeDef,
     CreateDetectorRequestRequestTypeDef,
     UpdateDetectorRequestRequestTypeDef,
     UpdateMemberDetectorsRequestRequestTypeDef,
     OrganizationDataSourceConfigurationsResultTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     PortProbeActionTypeDef,
     GetMalwareScanSettingsResponseTypeDef,
     UpdateMalwareScanSettingsRequestRequestTypeDef,
     ScanDetectionsTypeDef,
     GetUsageStatisticsResponseTypeDef,
+    ListCoverageResponseTypeDef,
     S3BucketDetailTypeDef,
     GetRemainingFreeTrialDaysResponseTypeDef,
     GetDetectorResponseTypeDef,
     MemberDataSourceConfigurationTypeDef,
     CreateDetectorResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-guardduty-1.26.98/mypy_boto3_guardduty.egg-info/SOURCES.txt` & `mypy-boto3-guardduty-1.27.0/mypy_boto3_guardduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.26.98/setup.py` & `mypy-boto3-guardduty-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-guardduty",
-    version="1.26.98",
+    version="1.27.0",
     packages=["mypy_boto3_guardduty"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GuardDuty 1.26.98 service generated with mypy-boto3-builder"
-        " 7.14.2"
+        "Type annotations for boto3.GuardDuty 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


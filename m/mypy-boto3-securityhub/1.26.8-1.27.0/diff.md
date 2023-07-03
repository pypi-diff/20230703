# Comparing `tmp/mypy-boto3-securityhub-1.26.8.tar.gz` & `tmp/mypy-boto3-securityhub-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-securityhub-1.26.8.tar", last modified: Fri Nov 11 21:07:54 2022, max compression
+gzip compressed data, was "mypy-boto3-securityhub-1.27.0.tar", last modified: Mon Jul  3 19:51:26 2023, max compression
```

## Comparing `mypy-boto3-securityhub-1.26.8.tar` & `mypy-boto3-securityhub-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.070122 mypy-boto3-securityhub-1.26.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    42413 2022-11-11 21:07:54.066122 mypy-boto3-securityhub-1.26.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    40962 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.066122 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/
--rw-r--r--   0 runner    (1001) docker     (121)     3084 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    41843 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    41768 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12060 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    12058 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    14452 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    14438 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)   219409 2022-11-11 21:07:43.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)   219366 2022-11-11 21:07:41.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.066122 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    42413 2022-11-11 21:07:53.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-11-11 21:07:53.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 21:07:53.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-11 21:07:53.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 21:07:54.070122 mypy-boto3-securityhub-1.26.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-11-11 21:07:38.000000 mypy-boto3-securityhub-1.26.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.175976 mypy-boto3-securityhub-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:42.000000 mypy-boto3-securityhub-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    50956 2023-07-03 19:51:26.175976 mypy-boto3-securityhub-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    49455 2023-07-03 19:47:42.000000 mypy-boto3-securityhub-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.171976 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-03 19:47:42.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-03 19:47:42.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-03 19:47:42.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-07-03 19:47:43.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51783 2023-07-03 19:47:42.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-03 19:47:43.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-07-03 19:47:43.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-07-03 19:47:43.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-07-03 19:47:43.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:42.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   279880 2023-07-03 19:47:51.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   279813 2023-07-03 19:47:46.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:42.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.175976 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50956 2023-07-03 19:51:26.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-03 19:51:26.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:26.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:26.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:26.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 19:51:26.000000 mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:26.175976 mypy-boto3-securityhub-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-03 19:47:42.000000 mypy-boto3-securityhub-1.27.0/setup.py
```

### Comparing `mypy-boto3-securityhub-1.26.8/LICENSE` & `mypy-boto3-securityhub-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-securityhub-1.26.8/PKG-INFO` & `mypy-boto3-securityhub-1.27.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.26.8
-Summary: Type annotations for boto3.SecurityHub 1.26.8 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SecurityHub 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
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
 
 <a id="mypy-boto3-securityhub"></a>
 
 # mypy-boto3-securityhub
 
 [![PyPI - mypy-boto3-securityhub](https://img.shields.io/pypi/v/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securityhub?color=blue)](https://pypistats.org/packages/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,21 +284,24 @@
 from mypy_boto3_securityhub import SecurityHubClient
 from mypy_boto3_securityhub.paginator import (
     DescribeActionTargetsPaginator,
     DescribeProductsPaginator,
     DescribeStandardsPaginator,
     DescribeStandardsControlsPaginator,
     GetEnabledStandardsPaginator,
+    GetFindingHistoryPaginator,
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
+    ListSecurityControlDefinitionsPaginator,
+    ListStandardsControlAssociationsPaginator,
 )
 
 client: SecurityHubClient = Session().client("securityhub")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator(
@@ -309,72 +313,91 @@
 )
 describe_standards_controls_paginator: DescribeStandardsControlsPaginator = client.get_paginator(
     "describe_standards_controls"
 )
 get_enabled_standards_paginator: GetEnabledStandardsPaginator = client.get_paginator(
     "get_enabled_standards"
 )
+get_finding_history_paginator: GetFindingHistoryPaginator = client.get_paginator(
+    "get_finding_history"
+)
 get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
 get_insights_paginator: GetInsightsPaginator = client.get_paginator("get_insights")
 list_enabled_products_for_import_paginator: ListEnabledProductsForImportPaginator = (
     client.get_paginator("list_enabled_products_for_import")
 )
 list_finding_aggregators_paginator: ListFindingAggregatorsPaginator = client.get_paginator(
     "list_finding_aggregators"
 )
 list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
 list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
 list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = (
     client.get_paginator("list_organization_admin_accounts")
 )
+list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = (
+    client.get_paginator("list_security_control_definitions")
+)
+list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = (
+    client.get_paginator("list_standards_control_associations")
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_securityhub.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_securityhub.literals import (
     AdminStatusType,
+    AssociationStatusType,
     AutoEnableStandardsType,
+    AutomationRulesActionTypeType,
     AwsIamAccessKeyStatusType,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
     ComplianceStatusType,
+    ControlFindingGeneratorType,
     ControlStatusType,
     DateRangeUnitType,
     DescribeActionTargetsPaginatorName,
     DescribeProductsPaginatorName,
     DescribeStandardsControlsPaginatorName,
     DescribeStandardsPaginatorName,
+    FindingHistoryUpdateSourceTypeType,
     GetEnabledStandardsPaginatorName,
+    GetFindingHistoryPaginatorName,
     GetFindingsPaginatorName,
     GetInsightsPaginatorName,
     IntegrationTypeType,
     ListEnabledProductsForImportPaginatorName,
     ListFindingAggregatorsPaginatorName,
     ListInvitationsPaginatorName,
     ListMembersPaginatorName,
     ListOrganizationAdminAccountsPaginatorName,
+    ListSecurityControlDefinitionsPaginatorName,
+    ListStandardsControlAssociationsPaginatorName,
     MalwareStateType,
     MalwareTypeType,
     MapFilterComparisonType,
     NetworkDirectionType,
     PartitionType,
     RecordStateType,
+    RegionAvailabilityStatusType,
+    RuleStatusType,
     SeverityLabelType,
     SeverityRatingType,
     SortOrderType,
     StandardsStatusType,
     StatusReasonCodeType,
     StringFilterComparisonType,
     ThreatIntelIndicatorCategoryType,
     ThreatIntelIndicatorTypeType,
+    UnprocessedErrorCodeType,
     VerificationStateType,
     VulnerabilityFixAvailableType,
     WorkflowStateType,
     WorkflowStatusType,
     SecurityHubServiceName,
     ServiceName,
     ResourceServiceName,
@@ -406,22 +429,41 @@
     GeoLocationTypeDef,
     IpOrganizationDetailsTypeDef,
     ActionRemotePortDetailsTypeDef,
     ActionTargetTypeDef,
     DnsRequestActionTypeDef,
     AdjustmentTypeDef,
     AdminAccountTypeDef,
+    AssociatedStandardTypeDef,
+    AssociationStateDetailsTypeDef,
+    NoteUpdateTypeDef,
+    RelatedFindingTypeDef,
+    SeverityUpdateTypeDef,
+    WorkflowUpdateTypeDef,
+    MapFilterTypeDef,
+    NumberFilterTypeDef,
+    StringFilterTypeDef,
+    AutomationRulesMetadataTypeDef,
     AvailabilityZoneTypeDef,
+    AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
+    AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
+    AwsAmazonMqBrokerUsersDetailsTypeDef,
+    AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
     AwsApiCallActionDomainDetailsTypeDef,
     AwsApiGatewayAccessLogSettingsTypeDef,
     AwsApiGatewayCanarySettingsTypeDef,
     AwsApiGatewayEndpointConfigurationTypeDef,
     AwsApiGatewayMethodSettingsTypeDef,
     AwsCorsConfigurationTypeDef,
     AwsApiGatewayV2RouteSettingsTypeDef,
+    AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
+    AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
+    AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
+    AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
@@ -461,22 +503,53 @@
     AwsDynamoDbTableRestoreSummaryTypeDef,
     AwsDynamoDbTableSseDescriptionTypeDef,
     AwsDynamoDbTableStreamSpecificationTypeDef,
     AwsDynamoDbTableProjectionTypeDef,
     AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     AwsEc2EipDetailsTypeDef,
     AwsEc2InstanceMetadataOptionsTypeDef,
+    AwsEc2InstanceMonitoringDetailsTypeDef,
     AwsEc2InstanceNetworkInterfacesDetailsTypeDef,
+    AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
+    AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
+    AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
+    AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
+    AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef,
     AwsEc2NetworkAclAssociationTypeDef,
     IcmpTypeCodeTypeDef,
     PortRangeFromToTypeDef,
     AwsEc2NetworkInterfaceAttachmentTypeDef,
     AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef,
     AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef,
     AwsEc2NetworkInterfaceSecurityGroupTypeDef,
+    PropagatingVgwSetDetailsTypeDef,
+    RouteSetDetailsTypeDef,
     AwsEc2SecurityGroupIpRangeTypeDef,
     AwsEc2SecurityGroupIpv6RangeTypeDef,
     AwsEc2SecurityGroupPrefixListIdTypeDef,
     AwsEc2SecurityGroupUserIdGroupPairTypeDef,
     Ipv6CidrBlockAssociationTypeDef,
     AwsEc2TransitGatewayDetailsTypeDef,
     AwsEc2VolumeAttachmentTypeDef,
@@ -553,14 +626,22 @@
     AwsElbLoadBalancerBackendServerDescriptionTypeDef,
     AwsElbLoadBalancerHealthCheckTypeDef,
     AwsElbLoadBalancerInstanceTypeDef,
     AwsElbLoadBalancerSourceSecurityGroupTypeDef,
     AwsElbLoadBalancerListenerTypeDef,
     AwsElbv2LoadBalancerAttributeTypeDef,
     LoadBalancerStateTypeDef,
+    AwsEventSchemasRegistryDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef,
+    AwsGuardDutyDetectorFeaturesDetailsTypeDef,
     AwsIamAccessKeySessionContextAttributesTypeDef,
     AwsIamAccessKeySessionContextSessionIssuerTypeDef,
     AwsIamAttachedManagedPolicyTypeDef,
     AwsIamGroupPolicyTypeDef,
     AwsIamInstanceProfileRoleTypeDef,
     AwsIamPermissionsBoundaryTypeDef,
     AwsIamPolicyVersionTypeDef,
@@ -620,139 +701,189 @@
     AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef,
     AwsS3BucketBucketVersioningConfigurationTypeDef,
     AwsS3BucketLoggingConfigurationTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef,
+    AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef,
     AwsS3BucketServerSideEncryptionByDefaultTypeDef,
     AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     AwsS3ObjectDetailsTypeDef,
+    AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef,
     AwsSecretsManagerSecretRotationRulesTypeDef,
     BooleanFilterTypeDef,
     IpFilterTypeDef,
     KeywordFilterTypeDef,
-    MapFilterTypeDef,
-    NumberFilterTypeDef,
-    StringFilterTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     MalwareTypeDef,
     NoteTypeDef,
     PatchSummaryTypeDef,
     ProcessDetailsTypeDef,
-    RelatedFindingTypeDef,
     SeverityTypeDef,
     ThreatIntelIndicatorTypeDef,
     WorkflowTypeDef,
     AwsSnsTopicSubscriptionTypeDef,
     AwsSqsQueueDetailsTypeDef,
     AwsSsmComplianceSummaryTypeDef,
+    AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
+    AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
     AwsWafRateBasedRuleMatchPredicateTypeDef,
     AwsWafRegionalRateBasedRuleMatchPredicateTypeDef,
     AwsWafRegionalRulePredicateListDetailsTypeDef,
     AwsWafRegionalRuleGroupRulesActionDetailsTypeDef,
     AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
     AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
     AwsWafRulePredicateListDetailsTypeDef,
     AwsWafRuleGroupRulesActionDetailsTypeDef,
     WafActionTypeDef,
     WafExcludedRuleTypeDef,
     WafOverrideActionTypeDef,
+    AwsWafv2CustomHttpHeaderTypeDef,
+    AwsWafv2VisibilityConfigDetailsTypeDef,
+    AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     AwsXrayEncryptionConfigDetailsTypeDef,
+    BatchDeleteAutomationRulesRequestRequestTypeDef,
+    UnprocessedAutomationRuleTypeDef,
     BatchDisableStandardsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StandardsSubscriptionRequestTypeDef,
+    BatchGetAutomationRulesRequestRequestTypeDef,
+    BatchGetSecurityControlsRequestRequestTypeDef,
+    SecurityControlTypeDef,
+    UnprocessedSecurityControlTypeDef,
+    StandardsControlAssociationIdTypeDef,
+    StandardsControlAssociationDetailTypeDef,
     ImportFindingsErrorTypeDef,
-    NoteUpdateTypeDef,
-    SeverityUpdateTypeDef,
-    WorkflowUpdateTypeDef,
+    StandardsControlAssociationUpdateTypeDef,
     CellTypeDef,
     ClassificationStatusTypeDef,
     StatusReasonTypeDef,
     VolumeMountTypeDef,
     CreateActionTargetRequestRequestTypeDef,
+    CreateActionTargetResponseTypeDef,
+    CreateAutomationRuleResponseTypeDef,
     CreateFindingAggregatorRequestRequestTypeDef,
+    CreateFindingAggregatorResponseTypeDef,
+    CreateInsightResponseTypeDef,
     ResultTypeDef,
     DateRangeTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteActionTargetRequestRequestTypeDef,
+    DeleteActionTargetResponseTypeDef,
     DeleteFindingAggregatorRequestRequestTypeDef,
     DeleteInsightRequestRequestTypeDef,
+    DeleteInsightResponseTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
     DescribeActionTargetsRequestRequestTypeDef,
     DescribeHubRequestRequestTypeDef,
+    DescribeHubResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    DescribeProductsRequestDescribeProductsPaginateTypeDef,
     DescribeProductsRequestRequestTypeDef,
     ProductTypeDef,
+    DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
     DescribeStandardsControlsRequestRequestTypeDef,
     StandardsControlTypeDef,
+    DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
     DescribeStandardsRequestRequestTypeDef,
-    StandardTypeDef,
     DisableImportFindingsForProductRequestRequestTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     EnableImportFindingsForProductRequestRequestTypeDef,
+    EnableImportFindingsForProductResponseTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     EnableSecurityHubRequestRequestTypeDef,
     FilePathsTypeDef,
     FindingAggregatorTypeDef,
+    FindingHistoryUpdateSourceTypeDef,
+    FindingHistoryUpdateTypeDef,
     FindingProviderSeverityTypeDef,
     FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef,
     FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef,
     InvitationTypeDef,
+    GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
     GetEnabledStandardsRequestRequestTypeDef,
     GetFindingAggregatorRequestRequestTypeDef,
+    GetFindingAggregatorResponseTypeDef,
     SortCriterionTypeDef,
     GetInsightResultsRequestRequestTypeDef,
+    GetInsightsRequestGetInsightsPaginateTypeDef,
     GetInsightsRequestRequestTypeDef,
+    GetInvitationsCountResponseTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     InsightResultValueTypeDef,
     InviteMembersRequestRequestTypeDef,
+    ListAutomationRulesRequestRequestTypeDef,
+    ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
     ListEnabledProductsForImportRequestRequestTypeDef,
+    ListEnabledProductsForImportResponseTypeDef,
+    ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
     ListFindingAggregatorsRequestRequestTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
+    ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
+    ListSecurityControlDefinitionsRequestRequestTypeDef,
+    SecurityControlDefinitionTypeDef,
+    ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
+    ListStandardsControlAssociationsRequestRequestTypeDef,
+    StandardsControlAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PortRangeTypeDef,
     RangeTypeDef,
     RecordTypeDef,
+    PaginatorConfigTypeDef,
     RecommendationTypeDef,
+    ResponseMetadataTypeDef,
     RuleGroupSourceListDetailsTypeDef,
     RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
     RuleGroupSourceStatefulRulesOptionsDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef,
     RuleGroupVariablesIpSetsDetailsTypeDef,
     RuleGroupVariablesPortSetsDetailsTypeDef,
     SoftwarePackageTypeDef,
+    StandardsManagedByTypeDef,
     StandardsStatusReasonTypeDef,
     StatelessCustomPublishMetricActionDimensionTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateActionTargetRequestRequestTypeDef,
     UpdateFindingAggregatorRequestRequestTypeDef,
+    UpdateFindingAggregatorResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateSecurityHubConfigurationRequestRequestTypeDef,
     UpdateStandardsControlRequestRequestTypeDef,
     VulnerabilityVendorTypeDef,
     CreateMembersRequestRequestTypeDef,
     ActionRemoteIpDetailsTypeDef,
+    DescribeActionTargetsResponseTypeDef,
     CvssTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    AssociationSetDetailsTypeDef,
+    AutomationRulesFindingFieldsUpdateTypeDef,
+    ListAutomationRulesResponseTypeDef,
+    AwsAmazonMqBrokerLogsDetailsTypeDef,
     AwsApiGatewayRestApiDetailsTypeDef,
     AwsApiGatewayStageDetailsTypeDef,
     AwsApiGatewayV2ApiDetailsTypeDef,
     AwsApiGatewayV2StageDetailsTypeDef,
+    AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef,
     AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef,
     AwsBackupBackupVaultDetailsTypeDef,
     AwsBackupRecoveryPointDetailsTypeDef,
     AwsCertificateManagerCertificateDomainValidationOptionTypeDef,
     AwsCloudFormationStackDetailsTypeDef,
@@ -762,14 +893,19 @@
     AwsCloudWatchAlarmDetailsTypeDef,
     AwsCodeBuildProjectEnvironmentTypeDef,
     AwsCodeBuildProjectLogsConfigDetailsTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexTypeDef,
     AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef,
     AwsEc2InstanceDetailsTypeDef,
+    AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef,
     AwsEc2NetworkAclEntryTypeDef,
     AwsEc2NetworkInterfaceDetailsTypeDef,
     AwsEc2SecurityGroupIpPermissionTypeDef,
     AwsEc2SubnetDetailsTypeDef,
     AwsEc2VolumeDetailsTypeDef,
     AwsEc2VpcDetailsTypeDef,
     AwsEc2VpcEndpointServiceDetailsTypeDef,
@@ -790,14 +926,16 @@
     AwsElasticBeanstalkEnvironmentDetailsTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsTypeDef,
     AwsElbLoadBalancerPoliciesTypeDef,
     AwsElbLoadBalancerAttributesTypeDef,
     AwsElbLoadBalancerListenerDescriptionTypeDef,
     AwsElbv2LoadBalancerDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
     AwsIamAccessKeySessionContextTypeDef,
     AwsIamGroupDetailsTypeDef,
     AwsIamInstanceProfileTypeDef,
     AwsIamPolicyDetailsTypeDef,
     AwsIamUserDetailsTypeDef,
     AwsKinesisStreamDetailsTypeDef,
     AwsLambdaFunctionEnvironmentTypeDef,
@@ -809,148 +947,165 @@
     AwsRdsDbSnapshotDetailsTypeDef,
     AwsRdsDbPendingModifiedValuesTypeDef,
     AwsRdsDbSecurityGroupDetailsTypeDef,
     AwsRdsDbSubnetGroupSubnetTypeDef,
     AwsRedshiftClusterClusterParameterGroupTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
+    AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
     AwsS3BucketServerSideEncryptionRuleTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
+    AwsSageMakerNotebookInstanceDetailsTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
+    BatchUpdateFindingsRequestRequestTypeDef,
     BatchUpdateFindingsUnprocessedFindingTypeDef,
+    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    GetFindingHistoryRequestRequestTypeDef,
     AwsSnsTopicDetailsTypeDef,
     AwsSsmPatchTypeDef,
+    AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRuleDetailsTypeDef,
     AwsWafRegionalRuleGroupRulesDetailsTypeDef,
     AwsWafRegionalWebAclRulesListDetailsTypeDef,
     AwsWafRuleDetailsTypeDef,
     AwsWafRuleGroupRulesDetailsTypeDef,
     AwsWafWebAclRuleTypeDef,
-    CreateActionTargetResponseTypeDef,
-    CreateFindingAggregatorResponseTypeDef,
-    CreateInsightResponseTypeDef,
-    DeleteActionTargetResponseTypeDef,
-    DeleteInsightResponseTypeDef,
-    DescribeActionTargetsResponseTypeDef,
-    DescribeHubResponseTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
-    EnableImportFindingsForProductResponseTypeDef,
-    GetFindingAggregatorResponseTypeDef,
-    GetInvitationsCountResponseTypeDef,
-    ListEnabledProductsForImportResponseTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateFindingAggregatorResponseTypeDef,
+    AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    AwsWafv2CustomResponseDetailsTypeDef,
+    AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
+    BatchDeleteAutomationRulesResponseTypeDef,
+    BatchUpdateAutomationRulesResponseTypeDef,
     BatchEnableStandardsRequestRequestTypeDef,
+    BatchGetSecurityControlsResponseTypeDef,
+    BatchGetStandardsControlAssociationsRequestRequestTypeDef,
+    UnprocessedStandardsControlAssociationTypeDef,
     BatchImportFindingsResponseTypeDef,
-    BatchUpdateFindingsRequestRequestTypeDef,
+    BatchUpdateStandardsControlAssociationsRequestRequestTypeDef,
+    UnprocessedStandardsControlAssociationUpdateTypeDef,
     ComplianceTypeDef,
     ContainerDetailsTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     DateFilterTypeDef,
-    DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
-    DescribeProductsRequestDescribeProductsPaginateTypeDef,
-    DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
-    DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
-    GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
-    GetInsightsRequestGetInsightsPaginateTypeDef,
-    ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
-    ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
-    DescribeStandardsResponseTypeDef,
     ThreatTypeDef,
     ListFindingAggregatorsResponseTypeDef,
+    FindingHistoryRecordTypeDef,
     FindingProviderFieldsTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
+    ListSecurityControlDefinitionsResponseTypeDef,
+    ListStandardsControlAssociationsResponseTypeDef,
     NetworkPathComponentDetailsTypeDef,
     NetworkTypeDef,
     PageTypeDef,
     RemediationTypeDef,
     RuleGroupSourceStatefulRulesDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     RuleGroupVariablesTypeDef,
+    StandardTypeDef,
     StandardsSubscriptionTypeDef,
     StatelessCustomPublishMetricActionTypeDef,
     AwsApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     VulnerabilityTypeDef,
+    AwsEc2RouteTableDetailsTypeDef,
+    AutomationRulesActionTypeDef,
+    AwsAmazonMqBrokerDetailsTypeDef,
+    AwsAppSyncGraphQlApiDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsTypeDef,
     AwsBackupBackupPlanRuleDetailsTypeDef,
     AwsCertificateManagerCertificateRenewalSummaryTypeDef,
     AwsCloudFrontDistributionOriginItemTypeDef,
     AwsCloudFrontDistributionOriginGroupTypeDef,
     AwsCodeBuildProjectDetailsTypeDef,
     AwsDynamoDbTableReplicaTypeDef,
+    AwsEc2LaunchTemplateDataDetailsTypeDef,
     AwsEc2NetworkAclDetailsTypeDef,
     AwsEc2SecurityGroupDetailsTypeDef,
     AwsEc2VpcPeeringConnectionDetailsTypeDef,
     AwsEc2VpnConnectionDetailsTypeDef,
     AwsEcsClusterConfigurationDetailsTypeDef,
     AwsEcsServiceDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesDetailsTypeDef,
     AwsEcsTaskDetailsTypeDef,
     AwsEfsAccessPointDetailsTypeDef,
     AwsEksClusterDetailsTypeDef,
     AwsElasticsearchDomainDetailsTypeDef,
     AwsElbLoadBalancerDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
     AwsIamAccessKeyDetailsTypeDef,
     AwsIamRoleDetailsTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     AwsOpenSearchServiceDomainDetailsTypeDef,
     AwsRdsDbSubnetGroupTypeDef,
     AwsRedshiftClusterDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
     AwsS3BucketNotificationConfigurationFilterTypeDef,
+    AwsS3BucketObjectLockConfigurationTypeDef,
     AwsS3BucketServerSideEncryptionConfigurationTypeDef,
     AwsS3BucketWebsiteConfigurationTypeDef,
     BatchUpdateFindingsResponseTypeDef,
     AwsSsmPatchComplianceDetailsTypeDef,
+    AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
     AwsWafRegionalRuleGroupDetailsTypeDef,
     AwsWafRegionalWebAclDetailsTypeDef,
     AwsWafRuleGroupDetailsTypeDef,
     AwsWafWebAclDetailsTypeDef,
+    AwsWafv2ActionAllowDetailsTypeDef,
+    AwsWafv2RulesActionCaptchaDetailsTypeDef,
+    AwsWafv2RulesActionCountDetailsTypeDef,
+    AwsWafv2ActionBlockDetailsTypeDef,
+    BatchGetStandardsControlAssociationsResponseTypeDef,
+    BatchUpdateStandardsControlAssociationsResponseTypeDef,
+    AutomationRulesFindingFiltersTypeDef,
     AwsSecurityFindingFiltersTypeDef,
+    GetFindingHistoryResponseTypeDef,
     GetInsightResultsResponseTypeDef,
     NetworkHeaderTypeDef,
     OccurrencesTypeDef,
     RuleGroupSourceStatelessRuleDefinitionTypeDef,
+    DescribeStandardsResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     StatelessCustomActionDefinitionTypeDef,
     PortProbeActionTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
     AwsCloudFrontDistributionOriginsTypeDef,
     AwsCloudFrontDistributionOriginGroupsTypeDef,
     AwsDynamoDbTableDetailsTypeDef,
+    AwsEc2LaunchTemplateDetailsTypeDef,
     AwsEcsClusterDetailsTypeDef,
     AwsEcsTaskDefinitionDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
     AwsRdsDbInstanceDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
     AwsS3BucketNotificationConfigurationDetailTypeDef,
+    AwsStepFunctionStateMachineDetailsTypeDef,
+    AwsWafv2RulesActionDetailsTypeDef,
+    AwsWafv2WebAclActionDetailsTypeDef,
+    AutomationRulesConfigTypeDef,
+    CreateAutomationRuleRequestRequestTypeDef,
+    UpdateAutomationRulesRequestItemTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     InsightTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
     NetworkPathComponentTypeDef,
@@ -958,22 +1113,28 @@
     SensitiveDataDetectionsTypeDef,
     RuleGroupSourceStatelessRulesDetailsTypeDef,
     FirewallPolicyStatelessCustomActionsDetailsTypeDef,
     RuleGroupSourceCustomActionsDetailsTypeDef,
     ActionTypeDef,
     AwsBackupBackupPlanDetailsTypeDef,
     AwsCloudFrontDistributionDetailsTypeDef,
+    AwsGuardDutyDetectorDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef,
     AwsS3BucketNotificationConfigurationTypeDef,
+    AwsWafv2RulesDetailsTypeDef,
+    BatchGetAutomationRulesResponseTypeDef,
+    BatchUpdateAutomationRulesRequestRequestTypeDef,
     GetInsightsResponseTypeDef,
     CustomDataIdentifiersResultTypeDef,
     SensitiveDataResultTypeDef,
     FirewallPolicyDetailsTypeDef,
     RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef,
+    AwsWafv2RuleGroupDetailsTypeDef,
+    AwsWafv2WebAclDetailsTypeDef,
     ClassificationResultTypeDef,
     AwsNetworkFirewallFirewallPolicyDetailsTypeDef,
     RuleGroupSourceTypeDef,
     AwsS3BucketDetailsTypeDef,
     DataClassificationDetailsTypeDef,
     RuleGroupDetailsTypeDef,
     AwsNetworkFirewallRuleGroupDetailsTypeDef,
@@ -992,42 +1153,42 @@
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

### Comparing `mypy-boto3-securityhub-1.26.8/README.md` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-securityhub
+Version: 1.27.0
+Summary: Type annotations for boto3.SecurityHub 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 securityhub type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-securityhub"></a>
 
 # mypy-boto3-securityhub
 
 [![PyPI - mypy-boto3-securityhub](https://img.shields.io/pypi/v/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securityhub?color=blue)](https://pypistats.org/packages/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -252,21 +284,24 @@
 from mypy_boto3_securityhub import SecurityHubClient
 from mypy_boto3_securityhub.paginator import (
     DescribeActionTargetsPaginator,
     DescribeProductsPaginator,
     DescribeStandardsPaginator,
     DescribeStandardsControlsPaginator,
     GetEnabledStandardsPaginator,
+    GetFindingHistoryPaginator,
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
+    ListSecurityControlDefinitionsPaginator,
+    ListStandardsControlAssociationsPaginator,
 )
 
 client: SecurityHubClient = Session().client("securityhub")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator(
@@ -278,72 +313,91 @@
 )
 describe_standards_controls_paginator: DescribeStandardsControlsPaginator = client.get_paginator(
     "describe_standards_controls"
 )
 get_enabled_standards_paginator: GetEnabledStandardsPaginator = client.get_paginator(
     "get_enabled_standards"
 )
+get_finding_history_paginator: GetFindingHistoryPaginator = client.get_paginator(
+    "get_finding_history"
+)
 get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
 get_insights_paginator: GetInsightsPaginator = client.get_paginator("get_insights")
 list_enabled_products_for_import_paginator: ListEnabledProductsForImportPaginator = (
     client.get_paginator("list_enabled_products_for_import")
 )
 list_finding_aggregators_paginator: ListFindingAggregatorsPaginator = client.get_paginator(
     "list_finding_aggregators"
 )
 list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
 list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
 list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = (
     client.get_paginator("list_organization_admin_accounts")
 )
+list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = (
+    client.get_paginator("list_security_control_definitions")
+)
+list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = (
+    client.get_paginator("list_standards_control_associations")
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_securityhub.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_securityhub.literals import (
     AdminStatusType,
+    AssociationStatusType,
     AutoEnableStandardsType,
+    AutomationRulesActionTypeType,
     AwsIamAccessKeyStatusType,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
     ComplianceStatusType,
+    ControlFindingGeneratorType,
     ControlStatusType,
     DateRangeUnitType,
     DescribeActionTargetsPaginatorName,
     DescribeProductsPaginatorName,
     DescribeStandardsControlsPaginatorName,
     DescribeStandardsPaginatorName,
+    FindingHistoryUpdateSourceTypeType,
     GetEnabledStandardsPaginatorName,
+    GetFindingHistoryPaginatorName,
     GetFindingsPaginatorName,
     GetInsightsPaginatorName,
     IntegrationTypeType,
     ListEnabledProductsForImportPaginatorName,
     ListFindingAggregatorsPaginatorName,
     ListInvitationsPaginatorName,
     ListMembersPaginatorName,
     ListOrganizationAdminAccountsPaginatorName,
+    ListSecurityControlDefinitionsPaginatorName,
+    ListStandardsControlAssociationsPaginatorName,
     MalwareStateType,
     MalwareTypeType,
     MapFilterComparisonType,
     NetworkDirectionType,
     PartitionType,
     RecordStateType,
+    RegionAvailabilityStatusType,
+    RuleStatusType,
     SeverityLabelType,
     SeverityRatingType,
     SortOrderType,
     StandardsStatusType,
     StatusReasonCodeType,
     StringFilterComparisonType,
     ThreatIntelIndicatorCategoryType,
     ThreatIntelIndicatorTypeType,
+    UnprocessedErrorCodeType,
     VerificationStateType,
     VulnerabilityFixAvailableType,
     WorkflowStateType,
     WorkflowStatusType,
     SecurityHubServiceName,
     ServiceName,
     ResourceServiceName,
@@ -375,22 +429,41 @@
     GeoLocationTypeDef,
     IpOrganizationDetailsTypeDef,
     ActionRemotePortDetailsTypeDef,
     ActionTargetTypeDef,
     DnsRequestActionTypeDef,
     AdjustmentTypeDef,
     AdminAccountTypeDef,
+    AssociatedStandardTypeDef,
+    AssociationStateDetailsTypeDef,
+    NoteUpdateTypeDef,
+    RelatedFindingTypeDef,
+    SeverityUpdateTypeDef,
+    WorkflowUpdateTypeDef,
+    MapFilterTypeDef,
+    NumberFilterTypeDef,
+    StringFilterTypeDef,
+    AutomationRulesMetadataTypeDef,
     AvailabilityZoneTypeDef,
+    AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
+    AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
+    AwsAmazonMqBrokerUsersDetailsTypeDef,
+    AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
     AwsApiCallActionDomainDetailsTypeDef,
     AwsApiGatewayAccessLogSettingsTypeDef,
     AwsApiGatewayCanarySettingsTypeDef,
     AwsApiGatewayEndpointConfigurationTypeDef,
     AwsApiGatewayMethodSettingsTypeDef,
     AwsCorsConfigurationTypeDef,
     AwsApiGatewayV2RouteSettingsTypeDef,
+    AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
+    AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
+    AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
+    AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
@@ -430,22 +503,53 @@
     AwsDynamoDbTableRestoreSummaryTypeDef,
     AwsDynamoDbTableSseDescriptionTypeDef,
     AwsDynamoDbTableStreamSpecificationTypeDef,
     AwsDynamoDbTableProjectionTypeDef,
     AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     AwsEc2EipDetailsTypeDef,
     AwsEc2InstanceMetadataOptionsTypeDef,
+    AwsEc2InstanceMonitoringDetailsTypeDef,
     AwsEc2InstanceNetworkInterfacesDetailsTypeDef,
+    AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
+    AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
+    AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
+    AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
+    AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef,
     AwsEc2NetworkAclAssociationTypeDef,
     IcmpTypeCodeTypeDef,
     PortRangeFromToTypeDef,
     AwsEc2NetworkInterfaceAttachmentTypeDef,
     AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef,
     AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef,
     AwsEc2NetworkInterfaceSecurityGroupTypeDef,
+    PropagatingVgwSetDetailsTypeDef,
+    RouteSetDetailsTypeDef,
     AwsEc2SecurityGroupIpRangeTypeDef,
     AwsEc2SecurityGroupIpv6RangeTypeDef,
     AwsEc2SecurityGroupPrefixListIdTypeDef,
     AwsEc2SecurityGroupUserIdGroupPairTypeDef,
     Ipv6CidrBlockAssociationTypeDef,
     AwsEc2TransitGatewayDetailsTypeDef,
     AwsEc2VolumeAttachmentTypeDef,
@@ -522,14 +626,22 @@
     AwsElbLoadBalancerBackendServerDescriptionTypeDef,
     AwsElbLoadBalancerHealthCheckTypeDef,
     AwsElbLoadBalancerInstanceTypeDef,
     AwsElbLoadBalancerSourceSecurityGroupTypeDef,
     AwsElbLoadBalancerListenerTypeDef,
     AwsElbv2LoadBalancerAttributeTypeDef,
     LoadBalancerStateTypeDef,
+    AwsEventSchemasRegistryDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef,
+    AwsGuardDutyDetectorFeaturesDetailsTypeDef,
     AwsIamAccessKeySessionContextAttributesTypeDef,
     AwsIamAccessKeySessionContextSessionIssuerTypeDef,
     AwsIamAttachedManagedPolicyTypeDef,
     AwsIamGroupPolicyTypeDef,
     AwsIamInstanceProfileRoleTypeDef,
     AwsIamPermissionsBoundaryTypeDef,
     AwsIamPolicyVersionTypeDef,
@@ -589,139 +701,189 @@
     AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef,
     AwsS3BucketBucketVersioningConfigurationTypeDef,
     AwsS3BucketLoggingConfigurationTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef,
+    AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef,
     AwsS3BucketServerSideEncryptionByDefaultTypeDef,
     AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     AwsS3ObjectDetailsTypeDef,
+    AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef,
     AwsSecretsManagerSecretRotationRulesTypeDef,
     BooleanFilterTypeDef,
     IpFilterTypeDef,
     KeywordFilterTypeDef,
-    MapFilterTypeDef,
-    NumberFilterTypeDef,
-    StringFilterTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     MalwareTypeDef,
     NoteTypeDef,
     PatchSummaryTypeDef,
     ProcessDetailsTypeDef,
-    RelatedFindingTypeDef,
     SeverityTypeDef,
     ThreatIntelIndicatorTypeDef,
     WorkflowTypeDef,
     AwsSnsTopicSubscriptionTypeDef,
     AwsSqsQueueDetailsTypeDef,
     AwsSsmComplianceSummaryTypeDef,
+    AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
+    AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
     AwsWafRateBasedRuleMatchPredicateTypeDef,
     AwsWafRegionalRateBasedRuleMatchPredicateTypeDef,
     AwsWafRegionalRulePredicateListDetailsTypeDef,
     AwsWafRegionalRuleGroupRulesActionDetailsTypeDef,
     AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
     AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
     AwsWafRulePredicateListDetailsTypeDef,
     AwsWafRuleGroupRulesActionDetailsTypeDef,
     WafActionTypeDef,
     WafExcludedRuleTypeDef,
     WafOverrideActionTypeDef,
+    AwsWafv2CustomHttpHeaderTypeDef,
+    AwsWafv2VisibilityConfigDetailsTypeDef,
+    AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     AwsXrayEncryptionConfigDetailsTypeDef,
+    BatchDeleteAutomationRulesRequestRequestTypeDef,
+    UnprocessedAutomationRuleTypeDef,
     BatchDisableStandardsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StandardsSubscriptionRequestTypeDef,
+    BatchGetAutomationRulesRequestRequestTypeDef,
+    BatchGetSecurityControlsRequestRequestTypeDef,
+    SecurityControlTypeDef,
+    UnprocessedSecurityControlTypeDef,
+    StandardsControlAssociationIdTypeDef,
+    StandardsControlAssociationDetailTypeDef,
     ImportFindingsErrorTypeDef,
-    NoteUpdateTypeDef,
-    SeverityUpdateTypeDef,
-    WorkflowUpdateTypeDef,
+    StandardsControlAssociationUpdateTypeDef,
     CellTypeDef,
     ClassificationStatusTypeDef,
     StatusReasonTypeDef,
     VolumeMountTypeDef,
     CreateActionTargetRequestRequestTypeDef,
+    CreateActionTargetResponseTypeDef,
+    CreateAutomationRuleResponseTypeDef,
     CreateFindingAggregatorRequestRequestTypeDef,
+    CreateFindingAggregatorResponseTypeDef,
+    CreateInsightResponseTypeDef,
     ResultTypeDef,
     DateRangeTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteActionTargetRequestRequestTypeDef,
+    DeleteActionTargetResponseTypeDef,
     DeleteFindingAggregatorRequestRequestTypeDef,
     DeleteInsightRequestRequestTypeDef,
+    DeleteInsightResponseTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
     DescribeActionTargetsRequestRequestTypeDef,
     DescribeHubRequestRequestTypeDef,
+    DescribeHubResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    DescribeProductsRequestDescribeProductsPaginateTypeDef,
     DescribeProductsRequestRequestTypeDef,
     ProductTypeDef,
+    DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
     DescribeStandardsControlsRequestRequestTypeDef,
     StandardsControlTypeDef,
+    DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
     DescribeStandardsRequestRequestTypeDef,
-    StandardTypeDef,
     DisableImportFindingsForProductRequestRequestTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     EnableImportFindingsForProductRequestRequestTypeDef,
+    EnableImportFindingsForProductResponseTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     EnableSecurityHubRequestRequestTypeDef,
     FilePathsTypeDef,
     FindingAggregatorTypeDef,
+    FindingHistoryUpdateSourceTypeDef,
+    FindingHistoryUpdateTypeDef,
     FindingProviderSeverityTypeDef,
     FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef,
     FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef,
     InvitationTypeDef,
+    GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
     GetEnabledStandardsRequestRequestTypeDef,
     GetFindingAggregatorRequestRequestTypeDef,
+    GetFindingAggregatorResponseTypeDef,
     SortCriterionTypeDef,
     GetInsightResultsRequestRequestTypeDef,
+    GetInsightsRequestGetInsightsPaginateTypeDef,
     GetInsightsRequestRequestTypeDef,
+    GetInvitationsCountResponseTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     InsightResultValueTypeDef,
     InviteMembersRequestRequestTypeDef,
+    ListAutomationRulesRequestRequestTypeDef,
+    ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
     ListEnabledProductsForImportRequestRequestTypeDef,
+    ListEnabledProductsForImportResponseTypeDef,
+    ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
     ListFindingAggregatorsRequestRequestTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
+    ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
+    ListSecurityControlDefinitionsRequestRequestTypeDef,
+    SecurityControlDefinitionTypeDef,
+    ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
+    ListStandardsControlAssociationsRequestRequestTypeDef,
+    StandardsControlAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PortRangeTypeDef,
     RangeTypeDef,
     RecordTypeDef,
+    PaginatorConfigTypeDef,
     RecommendationTypeDef,
+    ResponseMetadataTypeDef,
     RuleGroupSourceListDetailsTypeDef,
     RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
     RuleGroupSourceStatefulRulesOptionsDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef,
     RuleGroupVariablesIpSetsDetailsTypeDef,
     RuleGroupVariablesPortSetsDetailsTypeDef,
     SoftwarePackageTypeDef,
+    StandardsManagedByTypeDef,
     StandardsStatusReasonTypeDef,
     StatelessCustomPublishMetricActionDimensionTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateActionTargetRequestRequestTypeDef,
     UpdateFindingAggregatorRequestRequestTypeDef,
+    UpdateFindingAggregatorResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateSecurityHubConfigurationRequestRequestTypeDef,
     UpdateStandardsControlRequestRequestTypeDef,
     VulnerabilityVendorTypeDef,
     CreateMembersRequestRequestTypeDef,
     ActionRemoteIpDetailsTypeDef,
+    DescribeActionTargetsResponseTypeDef,
     CvssTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    AssociationSetDetailsTypeDef,
+    AutomationRulesFindingFieldsUpdateTypeDef,
+    ListAutomationRulesResponseTypeDef,
+    AwsAmazonMqBrokerLogsDetailsTypeDef,
     AwsApiGatewayRestApiDetailsTypeDef,
     AwsApiGatewayStageDetailsTypeDef,
     AwsApiGatewayV2ApiDetailsTypeDef,
     AwsApiGatewayV2StageDetailsTypeDef,
+    AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef,
     AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef,
     AwsBackupBackupVaultDetailsTypeDef,
     AwsBackupRecoveryPointDetailsTypeDef,
     AwsCertificateManagerCertificateDomainValidationOptionTypeDef,
     AwsCloudFormationStackDetailsTypeDef,
@@ -731,14 +893,19 @@
     AwsCloudWatchAlarmDetailsTypeDef,
     AwsCodeBuildProjectEnvironmentTypeDef,
     AwsCodeBuildProjectLogsConfigDetailsTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexTypeDef,
     AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef,
     AwsEc2InstanceDetailsTypeDef,
+    AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef,
     AwsEc2NetworkAclEntryTypeDef,
     AwsEc2NetworkInterfaceDetailsTypeDef,
     AwsEc2SecurityGroupIpPermissionTypeDef,
     AwsEc2SubnetDetailsTypeDef,
     AwsEc2VolumeDetailsTypeDef,
     AwsEc2VpcDetailsTypeDef,
     AwsEc2VpcEndpointServiceDetailsTypeDef,
@@ -759,14 +926,16 @@
     AwsElasticBeanstalkEnvironmentDetailsTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsTypeDef,
     AwsElbLoadBalancerPoliciesTypeDef,
     AwsElbLoadBalancerAttributesTypeDef,
     AwsElbLoadBalancerListenerDescriptionTypeDef,
     AwsElbv2LoadBalancerDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
     AwsIamAccessKeySessionContextTypeDef,
     AwsIamGroupDetailsTypeDef,
     AwsIamInstanceProfileTypeDef,
     AwsIamPolicyDetailsTypeDef,
     AwsIamUserDetailsTypeDef,
     AwsKinesisStreamDetailsTypeDef,
     AwsLambdaFunctionEnvironmentTypeDef,
@@ -778,148 +947,165 @@
     AwsRdsDbSnapshotDetailsTypeDef,
     AwsRdsDbPendingModifiedValuesTypeDef,
     AwsRdsDbSecurityGroupDetailsTypeDef,
     AwsRdsDbSubnetGroupSubnetTypeDef,
     AwsRedshiftClusterClusterParameterGroupTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
+    AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
     AwsS3BucketServerSideEncryptionRuleTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
+    AwsSageMakerNotebookInstanceDetailsTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
+    BatchUpdateFindingsRequestRequestTypeDef,
     BatchUpdateFindingsUnprocessedFindingTypeDef,
+    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    GetFindingHistoryRequestRequestTypeDef,
     AwsSnsTopicDetailsTypeDef,
     AwsSsmPatchTypeDef,
+    AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRuleDetailsTypeDef,
     AwsWafRegionalRuleGroupRulesDetailsTypeDef,
     AwsWafRegionalWebAclRulesListDetailsTypeDef,
     AwsWafRuleDetailsTypeDef,
     AwsWafRuleGroupRulesDetailsTypeDef,
     AwsWafWebAclRuleTypeDef,
-    CreateActionTargetResponseTypeDef,
-    CreateFindingAggregatorResponseTypeDef,
-    CreateInsightResponseTypeDef,
-    DeleteActionTargetResponseTypeDef,
-    DeleteInsightResponseTypeDef,
-    DescribeActionTargetsResponseTypeDef,
-    DescribeHubResponseTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
-    EnableImportFindingsForProductResponseTypeDef,
-    GetFindingAggregatorResponseTypeDef,
-    GetInvitationsCountResponseTypeDef,
-    ListEnabledProductsForImportResponseTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateFindingAggregatorResponseTypeDef,
+    AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    AwsWafv2CustomResponseDetailsTypeDef,
+    AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
+    BatchDeleteAutomationRulesResponseTypeDef,
+    BatchUpdateAutomationRulesResponseTypeDef,
     BatchEnableStandardsRequestRequestTypeDef,
+    BatchGetSecurityControlsResponseTypeDef,
+    BatchGetStandardsControlAssociationsRequestRequestTypeDef,
+    UnprocessedStandardsControlAssociationTypeDef,
     BatchImportFindingsResponseTypeDef,
-    BatchUpdateFindingsRequestRequestTypeDef,
+    BatchUpdateStandardsControlAssociationsRequestRequestTypeDef,
+    UnprocessedStandardsControlAssociationUpdateTypeDef,
     ComplianceTypeDef,
     ContainerDetailsTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     DateFilterTypeDef,
-    DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
-    DescribeProductsRequestDescribeProductsPaginateTypeDef,
-    DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
-    DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
-    GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
-    GetInsightsRequestGetInsightsPaginateTypeDef,
-    ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
-    ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
-    DescribeStandardsResponseTypeDef,
     ThreatTypeDef,
     ListFindingAggregatorsResponseTypeDef,
+    FindingHistoryRecordTypeDef,
     FindingProviderFieldsTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
+    ListSecurityControlDefinitionsResponseTypeDef,
+    ListStandardsControlAssociationsResponseTypeDef,
     NetworkPathComponentDetailsTypeDef,
     NetworkTypeDef,
     PageTypeDef,
     RemediationTypeDef,
     RuleGroupSourceStatefulRulesDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     RuleGroupVariablesTypeDef,
+    StandardTypeDef,
     StandardsSubscriptionTypeDef,
     StatelessCustomPublishMetricActionTypeDef,
     AwsApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     VulnerabilityTypeDef,
+    AwsEc2RouteTableDetailsTypeDef,
+    AutomationRulesActionTypeDef,
+    AwsAmazonMqBrokerDetailsTypeDef,
+    AwsAppSyncGraphQlApiDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsTypeDef,
     AwsBackupBackupPlanRuleDetailsTypeDef,
     AwsCertificateManagerCertificateRenewalSummaryTypeDef,
     AwsCloudFrontDistributionOriginItemTypeDef,
     AwsCloudFrontDistributionOriginGroupTypeDef,
     AwsCodeBuildProjectDetailsTypeDef,
     AwsDynamoDbTableReplicaTypeDef,
+    AwsEc2LaunchTemplateDataDetailsTypeDef,
     AwsEc2NetworkAclDetailsTypeDef,
     AwsEc2SecurityGroupDetailsTypeDef,
     AwsEc2VpcPeeringConnectionDetailsTypeDef,
     AwsEc2VpnConnectionDetailsTypeDef,
     AwsEcsClusterConfigurationDetailsTypeDef,
     AwsEcsServiceDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesDetailsTypeDef,
     AwsEcsTaskDetailsTypeDef,
     AwsEfsAccessPointDetailsTypeDef,
     AwsEksClusterDetailsTypeDef,
     AwsElasticsearchDomainDetailsTypeDef,
     AwsElbLoadBalancerDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
     AwsIamAccessKeyDetailsTypeDef,
     AwsIamRoleDetailsTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     AwsOpenSearchServiceDomainDetailsTypeDef,
     AwsRdsDbSubnetGroupTypeDef,
     AwsRedshiftClusterDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
     AwsS3BucketNotificationConfigurationFilterTypeDef,
+    AwsS3BucketObjectLockConfigurationTypeDef,
     AwsS3BucketServerSideEncryptionConfigurationTypeDef,
     AwsS3BucketWebsiteConfigurationTypeDef,
     BatchUpdateFindingsResponseTypeDef,
     AwsSsmPatchComplianceDetailsTypeDef,
+    AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
     AwsWafRegionalRuleGroupDetailsTypeDef,
     AwsWafRegionalWebAclDetailsTypeDef,
     AwsWafRuleGroupDetailsTypeDef,
     AwsWafWebAclDetailsTypeDef,
+    AwsWafv2ActionAllowDetailsTypeDef,
+    AwsWafv2RulesActionCaptchaDetailsTypeDef,
+    AwsWafv2RulesActionCountDetailsTypeDef,
+    AwsWafv2ActionBlockDetailsTypeDef,
+    BatchGetStandardsControlAssociationsResponseTypeDef,
+    BatchUpdateStandardsControlAssociationsResponseTypeDef,
+    AutomationRulesFindingFiltersTypeDef,
     AwsSecurityFindingFiltersTypeDef,
+    GetFindingHistoryResponseTypeDef,
     GetInsightResultsResponseTypeDef,
     NetworkHeaderTypeDef,
     OccurrencesTypeDef,
     RuleGroupSourceStatelessRuleDefinitionTypeDef,
+    DescribeStandardsResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     StatelessCustomActionDefinitionTypeDef,
     PortProbeActionTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
     AwsCloudFrontDistributionOriginsTypeDef,
     AwsCloudFrontDistributionOriginGroupsTypeDef,
     AwsDynamoDbTableDetailsTypeDef,
+    AwsEc2LaunchTemplateDetailsTypeDef,
     AwsEcsClusterDetailsTypeDef,
     AwsEcsTaskDefinitionDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
     AwsRdsDbInstanceDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
     AwsS3BucketNotificationConfigurationDetailTypeDef,
+    AwsStepFunctionStateMachineDetailsTypeDef,
+    AwsWafv2RulesActionDetailsTypeDef,
+    AwsWafv2WebAclActionDetailsTypeDef,
+    AutomationRulesConfigTypeDef,
+    CreateAutomationRuleRequestRequestTypeDef,
+    UpdateAutomationRulesRequestItemTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     InsightTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
     NetworkPathComponentTypeDef,
@@ -927,22 +1113,28 @@
     SensitiveDataDetectionsTypeDef,
     RuleGroupSourceStatelessRulesDetailsTypeDef,
     FirewallPolicyStatelessCustomActionsDetailsTypeDef,
     RuleGroupSourceCustomActionsDetailsTypeDef,
     ActionTypeDef,
     AwsBackupBackupPlanDetailsTypeDef,
     AwsCloudFrontDistributionDetailsTypeDef,
+    AwsGuardDutyDetectorDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef,
     AwsS3BucketNotificationConfigurationTypeDef,
+    AwsWafv2RulesDetailsTypeDef,
+    BatchGetAutomationRulesResponseTypeDef,
+    BatchUpdateAutomationRulesRequestRequestTypeDef,
     GetInsightsResponseTypeDef,
     CustomDataIdentifiersResultTypeDef,
     SensitiveDataResultTypeDef,
     FirewallPolicyDetailsTypeDef,
     RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef,
+    AwsWafv2RuleGroupDetailsTypeDef,
+    AwsWafv2WebAclDetailsTypeDef,
     ClassificationResultTypeDef,
     AwsNetworkFirewallFirewallPolicyDetailsTypeDef,
     RuleGroupSourceTypeDef,
     AwsS3BucketDetailsTypeDef,
     DataClassificationDetailsTypeDef,
     RuleGroupDetailsTypeDef,
     AwsNetworkFirewallRuleGroupDetailsTypeDef,
@@ -961,42 +1153,42 @@
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

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/__init__.py` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,69 +8,81 @@
     from mypy_boto3_securityhub import (
         Client,
         DescribeActionTargetsPaginator,
         DescribeProductsPaginator,
         DescribeStandardsControlsPaginator,
         DescribeStandardsPaginator,
         GetEnabledStandardsPaginator,
+        GetFindingHistoryPaginator,
         GetFindingsPaginator,
         GetInsightsPaginator,
         ListEnabledProductsForImportPaginator,
         ListFindingAggregatorsPaginator,
         ListInvitationsPaginator,
         ListMembersPaginator,
         ListOrganizationAdminAccountsPaginator,
+        ListSecurityControlDefinitionsPaginator,
+        ListStandardsControlAssociationsPaginator,
         SecurityHubClient,
     )
 
     session = Session()
     client: SecurityHubClient = session.client("securityhub")
 
     describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator("describe_action_targets")
     describe_products_paginator: DescribeProductsPaginator = client.get_paginator("describe_products")
     describe_standards_paginator: DescribeStandardsPaginator = client.get_paginator("describe_standards")
     describe_standards_controls_paginator: DescribeStandardsControlsPaginator = client.get_paginator("describe_standards_controls")
     get_enabled_standards_paginator: GetEnabledStandardsPaginator = client.get_paginator("get_enabled_standards")
+    get_finding_history_paginator: GetFindingHistoryPaginator = client.get_paginator("get_finding_history")
     get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
     get_insights_paginator: GetInsightsPaginator = client.get_paginator("get_insights")
     list_enabled_products_for_import_paginator: ListEnabledProductsForImportPaginator = client.get_paginator("list_enabled_products_for_import")
     list_finding_aggregators_paginator: ListFindingAggregatorsPaginator = client.get_paginator("list_finding_aggregators")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
+    list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")
+    list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")
     ```
 """
 from .client import SecurityHubClient
 from .paginator import (
     DescribeActionTargetsPaginator,
     DescribeProductsPaginator,
     DescribeStandardsControlsPaginator,
     DescribeStandardsPaginator,
     GetEnabledStandardsPaginator,
+    GetFindingHistoryPaginator,
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
+    ListSecurityControlDefinitionsPaginator,
+    ListStandardsControlAssociationsPaginator,
 )
 
 Client = SecurityHubClient
 
 
 __all__ = (
     "Client",
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
     "DescribeStandardsControlsPaginator",
     "DescribeStandardsPaginator",
     "GetEnabledStandardsPaginator",
+    "GetFindingHistoryPaginator",
     "GetFindingsPaginator",
     "GetInsightsPaginator",
     "ListEnabledProductsForImportPaginator",
     "ListFindingAggregatorsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
+    "ListSecurityControlDefinitionsPaginator",
+    "ListStandardsControlAssociationsPaginator",
     "SecurityHubClient",
 )
```

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/__init__.pyi` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -8,68 +8,80 @@
     from mypy_boto3_securityhub import (
         Client,
         DescribeActionTargetsPaginator,
         DescribeProductsPaginator,
         DescribeStandardsControlsPaginator,
         DescribeStandardsPaginator,
         GetEnabledStandardsPaginator,
+        GetFindingHistoryPaginator,
         GetFindingsPaginator,
         GetInsightsPaginator,
         ListEnabledProductsForImportPaginator,
         ListFindingAggregatorsPaginator,
         ListInvitationsPaginator,
         ListMembersPaginator,
         ListOrganizationAdminAccountsPaginator,
+        ListSecurityControlDefinitionsPaginator,
+        ListStandardsControlAssociationsPaginator,
         SecurityHubClient,
     )
 
     session = Session()
     client: SecurityHubClient = session.client("securityhub")
 
     describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator("describe_action_targets")
     describe_products_paginator: DescribeProductsPaginator = client.get_paginator("describe_products")
     describe_standards_paginator: DescribeStandardsPaginator = client.get_paginator("describe_standards")
     describe_standards_controls_paginator: DescribeStandardsControlsPaginator = client.get_paginator("describe_standards_controls")
     get_enabled_standards_paginator: GetEnabledStandardsPaginator = client.get_paginator("get_enabled_standards")
+    get_finding_history_paginator: GetFindingHistoryPaginator = client.get_paginator("get_finding_history")
     get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
     get_insights_paginator: GetInsightsPaginator = client.get_paginator("get_insights")
     list_enabled_products_for_import_paginator: ListEnabledProductsForImportPaginator = client.get_paginator("list_enabled_products_for_import")
     list_finding_aggregators_paginator: ListFindingAggregatorsPaginator = client.get_paginator("list_finding_aggregators")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
+    list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")
+    list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")
     ```
 """
 from .client import SecurityHubClient
 from .paginator import (
     DescribeActionTargetsPaginator,
     DescribeProductsPaginator,
     DescribeStandardsControlsPaginator,
     DescribeStandardsPaginator,
     GetEnabledStandardsPaginator,
+    GetFindingHistoryPaginator,
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
+    ListSecurityControlDefinitionsPaginator,
+    ListStandardsControlAssociationsPaginator,
 )
 
 Client = SecurityHubClient
 
 __all__ = (
     "Client",
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
     "DescribeStandardsControlsPaginator",
     "DescribeStandardsPaginator",
     "GetEnabledStandardsPaginator",
+    "GetFindingHistoryPaginator",
     "GetFindingsPaginator",
     "GetInsightsPaginator",
     "ListEnabledProductsForImportPaginator",
     "ListFindingAggregatorsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
+    "ListSecurityControlDefinitionsPaginator",
+    "ListStandardsControlAssociationsPaginator",
     "SecurityHubClient",
 )
```

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/__main__.py` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecurityHub 1.26.8\nVersion:         1.26.8\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.SecurityHub 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.8")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/client.py` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,48 +10,63 @@
     from mypy_boto3_securityhub.client import SecurityHubClient
 
     session = Session()
     client: SecurityHubClient = session.client("securityhub")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoEnableStandardsType,
+    ControlFindingGeneratorType,
     ControlStatusType,
     RecordStateType,
+    RuleStatusType,
     VerificationStateType,
 )
 from .paginator import (
     DescribeActionTargetsPaginator,
     DescribeProductsPaginator,
     DescribeStandardsControlsPaginator,
     DescribeStandardsPaginator,
     GetEnabledStandardsPaginator,
+    GetFindingHistoryPaginator,
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
+    ListSecurityControlDefinitionsPaginator,
+    ListStandardsControlAssociationsPaginator,
 )
 from .type_defs import (
     AccountDetailsTypeDef,
+    AutomationRulesActionTypeDef,
+    AutomationRulesFindingFiltersTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     AwsSecurityFindingTypeDef,
+    BatchDeleteAutomationRulesResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
+    BatchGetAutomationRulesResponseTypeDef,
+    BatchGetSecurityControlsResponseTypeDef,
+    BatchGetStandardsControlAssociationsResponseTypeDef,
     BatchImportFindingsResponseTypeDef,
+    BatchUpdateAutomationRulesResponseTypeDef,
     BatchUpdateFindingsResponseTypeDef,
+    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     CreateActionTargetResponseTypeDef,
+    CreateAutomationRuleResponseTypeDef,
     CreateFindingAggregatorResponseTypeDef,
     CreateInsightResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteActionTargetResponseTypeDef,
     DeleteInsightResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
@@ -62,32 +77,39 @@
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
     DescribeStandardsResponseTypeDef,
     EnableImportFindingsForProductResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     GetFindingAggregatorResponseTypeDef,
+    GetFindingHistoryResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetInsightResultsResponseTypeDef,
     GetInsightsResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     GetMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
+    ListAutomationRulesResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
+    ListSecurityControlDefinitionsResponseTypeDef,
+    ListStandardsControlAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     SortCriterionTypeDef,
+    StandardsControlAssociationIdTypeDef,
+    StandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionRequestTypeDef,
+    UpdateAutomationRulesRequestItemTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     WorkflowUpdateTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -148,19 +170,29 @@
         """
         This method is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.accept_invitation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#accept_invitation)
         """
 
+    def batch_delete_automation_rules(
+        self, *, AutomationRulesArns: Sequence[str]
+    ) -> BatchDeleteAutomationRulesResponseTypeDef:
+        """
+        Deletes one or more automation rules.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_delete_automation_rules)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_delete_automation_rules)
+        """
+
     def batch_disable_standards(
         self, *, StandardsSubscriptionArns: Sequence[str]
     ) -> BatchDisableStandardsResponseTypeDef:
         """
-        Disables the standards specified by the provided `StandardsSubscriptionArns` .
+        Disables the standards specified by the provided `StandardsSubscriptionArns`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_disable_standards)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_disable_standards)
         """
 
     def batch_enable_standards(
         self, *, StandardsSubscriptionRequests: Sequence[StandardsSubscriptionRequestTypeDef]
@@ -168,24 +200,70 @@
         """
         Enables the standards specified by the provided `StandardsArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_enable_standards)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_enable_standards)
         """
 
+    def batch_get_automation_rules(
+        self, *, AutomationRulesArns: Sequence[str]
+    ) -> BatchGetAutomationRulesResponseTypeDef:
+        """
+        Retrieves a list of details for automation rules based on rule Amazon Resource
+        Names (ARNs).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_automation_rules)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_automation_rules)
+        """
+
+    def batch_get_security_controls(
+        self, *, SecurityControlIds: Sequence[str]
+    ) -> BatchGetSecurityControlsResponseTypeDef:
+        """
+        Provides details about a batch of security controls for the current Amazon Web
+        Services account and Amazon Web Services Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_security_controls)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_security_controls)
+        """
+
+    def batch_get_standards_control_associations(
+        self, *, StandardsControlAssociationIds: Sequence[StandardsControlAssociationIdTypeDef]
+    ) -> BatchGetStandardsControlAssociationsResponseTypeDef:
+        """
+        For a batch of security controls and standards, identifies whether each control
+        is currently enabled or disabled in a standard.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_standards_control_associations)
+        """
+
     def batch_import_findings(
         self, *, Findings: Sequence[AwsSecurityFindingTypeDef]
     ) -> BatchImportFindingsResponseTypeDef:
         """
-        .
+        Imports security findings generated by a finding provider into Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_import_findings)
         """
 
+    def batch_update_automation_rules(
+        self,
+        *,
+        UpdateAutomationRulesRequestItems: Sequence[UpdateAutomationRulesRequestItemTypeDef]
+    ) -> BatchUpdateAutomationRulesResponseTypeDef:
+        """
+        Updates one or more automation rules based on rule Amazon Resource Names (ARNs)
+        and input parameters.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_automation_rules)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_update_automation_rules)
+        """
+
     def batch_update_findings(
         self,
         *,
         FindingIdentifiers: Sequence[AwsSecurityFindingIdentifierTypeDef],
         Note: NoteUpdateTypeDef = ...,
         Severity: SeverityUpdateTypeDef = ...,
         VerificationState: VerificationStateType = ...,
@@ -193,20 +271,34 @@
         Criticality: int = ...,
         Types: Sequence[str] = ...,
         UserDefinedFields: Mapping[str, str] = ...,
         Workflow: WorkflowUpdateTypeDef = ...,
         RelatedFindings: Sequence[RelatedFindingTypeDef] = ...
     ) -> BatchUpdateFindingsResponseTypeDef:
         """
-        .
+        Used by Security Hub customers to update information about their investigation
+        into a finding.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_update_findings)
         """
 
+    def batch_update_standards_control_associations(
+        self,
+        *,
+        StandardsControlAssociationUpdates: Sequence[StandardsControlAssociationUpdateTypeDef]
+    ) -> BatchUpdateStandardsControlAssociationsResponseTypeDef:
+        """
+        For a batch of security controls and standards, this operation updates the
+        enablement status of a control in a standard.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_standards_control_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_update_standards_control_associations)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#can_paginate)
         """
@@ -225,14 +317,33 @@
         """
         Creates a custom action target in Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_action_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_action_target)
         """
 
+    def create_automation_rule(
+        self,
+        *,
+        RuleOrder: int,
+        RuleName: str,
+        Description: str,
+        Criteria: AutomationRulesFindingFiltersTypeDef,
+        Actions: Sequence[AutomationRulesActionTypeDef],
+        Tags: Mapping[str, str] = ...,
+        RuleStatus: RuleStatusType = ...,
+        IsTerminal: bool = ...
+    ) -> CreateAutomationRuleResponseTypeDef:
+        """
+        Creates an automation rule based on input parameters.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_automation_rule)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_automation_rule)
+        """
+
     def create_finding_aggregator(
         self, *, RegionLinkingMode: str, Regions: Sequence[str] = ...
     ) -> CreateFindingAggregatorResponseTypeDef:
         """
         Used to enable finding aggregation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_finding_aggregator)
@@ -284,15 +395,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.delete_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#delete_finding_aggregator)
         """
 
     def delete_insight(self, *, InsightArn: str) -> DeleteInsightResponseTypeDef:
         """
-        Deletes the insight specified by the `InsightArn` .
+        Deletes the insight specified by the `InsightArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.delete_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#delete_insight)
         """
 
     def delete_invitations(self, *, AccountIds: Sequence[str]) -> DeleteInvitationsResponseTypeDef:
         """
@@ -435,15 +546,19 @@
         Designates the Security Hub administrator account for an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_organization_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#enable_organization_admin_account)
         """
 
     def enable_security_hub(
-        self, *, Tags: Mapping[str, str] = ..., EnableDefaultStandards: bool = ...
+        self,
+        *,
+        Tags: Mapping[str, str] = ...,
+        EnableDefaultStandards: bool = ...,
+        ControlFindingGenerator: ControlFindingGeneratorType = ...
     ) -> Dict[str, Any]:
         """
         Enables Security Hub for your account in the current Region or the Region you
         specify in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_security_hub)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#enable_security_hub)
@@ -492,24 +607,40 @@
         """
         Returns the current finding aggregation configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_finding_aggregator)
         """
 
+    def get_finding_history(
+        self,
+        *,
+        FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
+        StartTime: Union[datetime, str] = ...,
+        EndTime: Union[datetime, str] = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> GetFindingHistoryResponseTypeDef:
+        """
+        Returns history for a Security Hub finding in the last 90 days.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_finding_history)
+        """
+
     def get_findings(
         self,
         *,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingsResponseTypeDef:
         """
-        .
+        Returns a list of findings that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_findings)
         """
 
     def get_insight_results(self, *, InsightArn: str) -> GetInsightResultsResponseTypeDef:
         """
@@ -560,14 +691,24 @@
         Invites other Amazon Web Services accounts to become member accounts for the
         Security Hub administrator account that the invitation is sent from.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.invite_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#invite_members)
         """
 
+    def list_automation_rules(
+        self, *, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListAutomationRulesResponseTypeDef:
+        """
+        A list of automation rules and their metadata for the calling account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_automation_rules)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_automation_rules)
+        """
+
     def list_enabled_products_for_import(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListEnabledProductsForImportResponseTypeDef:
         """
         Lists all findings-generating solutions (products) that you are subscribed to
         receive findings from in Security Hub.
 
@@ -614,14 +755,35 @@
         """
         Lists the Security Hub administrator accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_organization_admin_accounts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_organization_admin_accounts)
         """
 
+    def list_security_control_definitions(
+        self, *, StandardsArn: str = ..., NextToken: str = ..., MaxResults: int = ...
+    ) -> ListSecurityControlDefinitionsResponseTypeDef:
+        """
+        Lists all of the security controls that apply to a specified standard.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_security_control_definitions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_security_control_definitions)
+        """
+
+    def list_standards_control_associations(
+        self, *, SecurityControlId: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListStandardsControlAssociationsResponseTypeDef:
+        """
+        Specifies whether a control is currently enabled or disabled in each enabled
+        standard in the calling account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_standards_control_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_standards_control_associations)
+        """
+
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags associated with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_tags_for_resource)
         """
@@ -698,15 +860,18 @@
         Used to update the configuration related to Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_organization_configuration)
         """
 
     def update_security_hub_configuration(
-        self, *, AutoEnableControls: bool = ...
+        self,
+        *,
+        AutoEnableControls: bool = ...,
+        ControlFindingGenerator: ControlFindingGeneratorType = ...
     ) -> Dict[str, Any]:
         """
         Updates configuration options for Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_security_hub_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_security_hub_configuration)
         """
@@ -768,14 +933,23 @@
     ) -> GetEnabledStandardsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["get_finding_history"]
+    ) -> GetFindingHistoryPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["get_findings"]) -> GetFindingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
         """
 
     @overload
@@ -823,7 +997,25 @@
     def get_paginator(
         self, operation_name: Literal["list_organization_admin_accounts"]
     ) -> ListOrganizationAdminAccountsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
         """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_security_control_definitions"]
+    ) -> ListSecurityControlDefinitionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_standards_control_associations"]
+    ) -> ListStandardsControlAssociationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/client.pyi` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/client.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -10,48 +10,63 @@
     from mypy_boto3_securityhub.client import SecurityHubClient
 
     session = Session()
     client: SecurityHubClient = session.client("securityhub")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoEnableStandardsType,
+    ControlFindingGeneratorType,
     ControlStatusType,
     RecordStateType,
+    RuleStatusType,
     VerificationStateType,
 )
 from .paginator import (
     DescribeActionTargetsPaginator,
     DescribeProductsPaginator,
     DescribeStandardsControlsPaginator,
     DescribeStandardsPaginator,
     GetEnabledStandardsPaginator,
+    GetFindingHistoryPaginator,
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
+    ListSecurityControlDefinitionsPaginator,
+    ListStandardsControlAssociationsPaginator,
 )
 from .type_defs import (
     AccountDetailsTypeDef,
+    AutomationRulesActionTypeDef,
+    AutomationRulesFindingFiltersTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     AwsSecurityFindingTypeDef,
+    BatchDeleteAutomationRulesResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
+    BatchGetAutomationRulesResponseTypeDef,
+    BatchGetSecurityControlsResponseTypeDef,
+    BatchGetStandardsControlAssociationsResponseTypeDef,
     BatchImportFindingsResponseTypeDef,
+    BatchUpdateAutomationRulesResponseTypeDef,
     BatchUpdateFindingsResponseTypeDef,
+    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     CreateActionTargetResponseTypeDef,
+    CreateAutomationRuleResponseTypeDef,
     CreateFindingAggregatorResponseTypeDef,
     CreateInsightResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteActionTargetResponseTypeDef,
     DeleteInsightResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
@@ -62,32 +77,39 @@
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
     DescribeStandardsResponseTypeDef,
     EnableImportFindingsForProductResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     GetFindingAggregatorResponseTypeDef,
+    GetFindingHistoryResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetInsightResultsResponseTypeDef,
     GetInsightsResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     GetMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
+    ListAutomationRulesResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
+    ListSecurityControlDefinitionsResponseTypeDef,
+    ListStandardsControlAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     SortCriterionTypeDef,
+    StandardsControlAssociationIdTypeDef,
+    StandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionRequestTypeDef,
+    UpdateAutomationRulesRequestItemTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     WorkflowUpdateTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -141,41 +163,92 @@
     def accept_invitation(self, *, MasterId: str, InvitationId: str) -> Dict[str, Any]:
         """
         This method is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.accept_invitation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#accept_invitation)
         """
+    def batch_delete_automation_rules(
+        self, *, AutomationRulesArns: Sequence[str]
+    ) -> BatchDeleteAutomationRulesResponseTypeDef:
+        """
+        Deletes one or more automation rules.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_delete_automation_rules)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_delete_automation_rules)
+        """
     def batch_disable_standards(
         self, *, StandardsSubscriptionArns: Sequence[str]
     ) -> BatchDisableStandardsResponseTypeDef:
         """
-        Disables the standards specified by the provided `StandardsSubscriptionArns` .
+        Disables the standards specified by the provided `StandardsSubscriptionArns`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_disable_standards)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_disable_standards)
         """
     def batch_enable_standards(
         self, *, StandardsSubscriptionRequests: Sequence[StandardsSubscriptionRequestTypeDef]
     ) -> BatchEnableStandardsResponseTypeDef:
         """
         Enables the standards specified by the provided `StandardsArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_enable_standards)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_enable_standards)
         """
+    def batch_get_automation_rules(
+        self, *, AutomationRulesArns: Sequence[str]
+    ) -> BatchGetAutomationRulesResponseTypeDef:
+        """
+        Retrieves a list of details for automation rules based on rule Amazon Resource
+        Names (ARNs).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_automation_rules)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_automation_rules)
+        """
+    def batch_get_security_controls(
+        self, *, SecurityControlIds: Sequence[str]
+    ) -> BatchGetSecurityControlsResponseTypeDef:
+        """
+        Provides details about a batch of security controls for the current Amazon Web
+        Services account and Amazon Web Services Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_security_controls)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_security_controls)
+        """
+    def batch_get_standards_control_associations(
+        self, *, StandardsControlAssociationIds: Sequence[StandardsControlAssociationIdTypeDef]
+    ) -> BatchGetStandardsControlAssociationsResponseTypeDef:
+        """
+        For a batch of security controls and standards, identifies whether each control
+        is currently enabled or disabled in a standard.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_standards_control_associations)
+        """
     def batch_import_findings(
         self, *, Findings: Sequence[AwsSecurityFindingTypeDef]
     ) -> BatchImportFindingsResponseTypeDef:
         """
-        .
+        Imports security findings generated by a finding provider into Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_import_findings)
         """
+    def batch_update_automation_rules(
+        self,
+        *,
+        UpdateAutomationRulesRequestItems: Sequence[UpdateAutomationRulesRequestItemTypeDef]
+    ) -> BatchUpdateAutomationRulesResponseTypeDef:
+        """
+        Updates one or more automation rules based on rule Amazon Resource Names (ARNs)
+        and input parameters.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_automation_rules)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_update_automation_rules)
+        """
     def batch_update_findings(
         self,
         *,
         FindingIdentifiers: Sequence[AwsSecurityFindingIdentifierTypeDef],
         Note: NoteUpdateTypeDef = ...,
         Severity: SeverityUpdateTypeDef = ...,
         VerificationState: VerificationStateType = ...,
@@ -183,19 +256,32 @@
         Criticality: int = ...,
         Types: Sequence[str] = ...,
         UserDefinedFields: Mapping[str, str] = ...,
         Workflow: WorkflowUpdateTypeDef = ...,
         RelatedFindings: Sequence[RelatedFindingTypeDef] = ...
     ) -> BatchUpdateFindingsResponseTypeDef:
         """
-        .
+        Used by Security Hub customers to update information about their investigation
+        into a finding.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_update_findings)
         """
+    def batch_update_standards_control_associations(
+        self,
+        *,
+        StandardsControlAssociationUpdates: Sequence[StandardsControlAssociationUpdateTypeDef]
+    ) -> BatchUpdateStandardsControlAssociationsResponseTypeDef:
+        """
+        For a batch of security controls and standards, this operation updates the
+        enablement status of a control in a standard.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_standards_control_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_update_standards_control_associations)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#can_paginate)
         """
@@ -211,14 +297,32 @@
     ) -> CreateActionTargetResponseTypeDef:
         """
         Creates a custom action target in Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_action_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_action_target)
         """
+    def create_automation_rule(
+        self,
+        *,
+        RuleOrder: int,
+        RuleName: str,
+        Description: str,
+        Criteria: AutomationRulesFindingFiltersTypeDef,
+        Actions: Sequence[AutomationRulesActionTypeDef],
+        Tags: Mapping[str, str] = ...,
+        RuleStatus: RuleStatusType = ...,
+        IsTerminal: bool = ...
+    ) -> CreateAutomationRuleResponseTypeDef:
+        """
+        Creates an automation rule based on input parameters.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_automation_rule)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_automation_rule)
+        """
     def create_finding_aggregator(
         self, *, RegionLinkingMode: str, Regions: Sequence[str] = ...
     ) -> CreateFindingAggregatorResponseTypeDef:
         """
         Used to enable finding aggregation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_finding_aggregator)
@@ -264,15 +368,15 @@
         Deletes a finding aggregator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.delete_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#delete_finding_aggregator)
         """
     def delete_insight(self, *, InsightArn: str) -> DeleteInsightResponseTypeDef:
         """
-        Deletes the insight specified by the `InsightArn` .
+        Deletes the insight specified by the `InsightArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.delete_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#delete_insight)
         """
     def delete_invitations(self, *, AccountIds: Sequence[str]) -> DeleteInvitationsResponseTypeDef:
         """
         Deletes invitations received by the Amazon Web Services account to become a
@@ -398,15 +502,19 @@
         """
         Designates the Security Hub administrator account for an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_organization_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#enable_organization_admin_account)
         """
     def enable_security_hub(
-        self, *, Tags: Mapping[str, str] = ..., EnableDefaultStandards: bool = ...
+        self,
+        *,
+        Tags: Mapping[str, str] = ...,
+        EnableDefaultStandards: bool = ...,
+        ControlFindingGenerator: ControlFindingGeneratorType = ...
     ) -> Dict[str, Any]:
         """
         Enables Security Hub for your account in the current Region or the Region you
         specify in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_security_hub)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#enable_security_hub)
@@ -450,24 +558,39 @@
     ) -> GetFindingAggregatorResponseTypeDef:
         """
         Returns the current finding aggregation configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_finding_aggregator)
         """
+    def get_finding_history(
+        self,
+        *,
+        FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
+        StartTime: Union[datetime, str] = ...,
+        EndTime: Union[datetime, str] = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> GetFindingHistoryResponseTypeDef:
+        """
+        Returns history for a Security Hub finding in the last 90 days.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_finding_history)
+        """
     def get_findings(
         self,
         *,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingsResponseTypeDef:
         """
-        .
+        Returns a list of findings that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_findings)
         """
     def get_insight_results(self, *, InsightArn: str) -> GetInsightResultsResponseTypeDef:
         """
         Lists the results of the Security Hub insight specified by the insight ARN.
@@ -511,14 +634,23 @@
         """
         Invites other Amazon Web Services accounts to become member accounts for the
         Security Hub administrator account that the invitation is sent from.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.invite_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#invite_members)
         """
+    def list_automation_rules(
+        self, *, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListAutomationRulesResponseTypeDef:
+        """
+        A list of automation rules and their metadata for the calling account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_automation_rules)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_automation_rules)
+        """
     def list_enabled_products_for_import(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListEnabledProductsForImportResponseTypeDef:
         """
         Lists all findings-generating solutions (products) that you are subscribed to
         receive findings from in Security Hub.
 
@@ -560,14 +692,33 @@
     ) -> ListOrganizationAdminAccountsResponseTypeDef:
         """
         Lists the Security Hub administrator accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_organization_admin_accounts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_organization_admin_accounts)
         """
+    def list_security_control_definitions(
+        self, *, StandardsArn: str = ..., NextToken: str = ..., MaxResults: int = ...
+    ) -> ListSecurityControlDefinitionsResponseTypeDef:
+        """
+        Lists all of the security controls that apply to a specified standard.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_security_control_definitions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_security_control_definitions)
+        """
+    def list_standards_control_associations(
+        self, *, SecurityControlId: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListStandardsControlAssociationsResponseTypeDef:
+        """
+        Specifies whether a control is currently enabled or disabled in each enabled
+        standard in the calling account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_standards_control_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_standards_control_associations)
+        """
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags associated with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_tags_for_resource)
         """
@@ -636,15 +787,18 @@
         """
         Used to update the configuration related to Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_organization_configuration)
         """
     def update_security_hub_configuration(
-        self, *, AutoEnableControls: bool = ...
+        self,
+        *,
+        AutoEnableControls: bool = ...,
+        ControlFindingGenerator: ControlFindingGeneratorType = ...
     ) -> Dict[str, Any]:
         """
         Updates configuration options for Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_security_hub_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_security_hub_configuration)
         """
@@ -699,14 +853,22 @@
         self, operation_name: Literal["get_enabled_standards"]
     ) -> GetEnabledStandardsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
         """
     @overload
+    def get_paginator(
+        self, operation_name: Literal["get_finding_history"]
+    ) -> GetFindingHistoryPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
+        """
+    @overload
     def get_paginator(self, operation_name: Literal["get_findings"]) -> GetFindingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
         """
     @overload
     def get_paginator(self, operation_name: Literal["get_insights"]) -> GetInsightsPaginator:
@@ -748,7 +910,23 @@
     def get_paginator(
         self, operation_name: Literal["list_organization_admin_accounts"]
     ) -> ListOrganizationAdminAccountsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
         """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_security_control_definitions"]
+    ) -> ListSecurityControlDefinitionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_standards_control_associations"]
+    ) -> ListStandardsControlAssociationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/literals.py` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,86 +14,101 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AdminStatusType",
+    "AssociationStatusType",
     "AutoEnableStandardsType",
+    "AutomationRulesActionTypeType",
     "AwsIamAccessKeyStatusType",
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType",
     "ComplianceStatusType",
+    "ControlFindingGeneratorType",
     "ControlStatusType",
     "DateRangeUnitType",
     "DescribeActionTargetsPaginatorName",
     "DescribeProductsPaginatorName",
     "DescribeStandardsControlsPaginatorName",
     "DescribeStandardsPaginatorName",
+    "FindingHistoryUpdateSourceTypeType",
     "GetEnabledStandardsPaginatorName",
+    "GetFindingHistoryPaginatorName",
     "GetFindingsPaginatorName",
     "GetInsightsPaginatorName",
     "IntegrationTypeType",
     "ListEnabledProductsForImportPaginatorName",
     "ListFindingAggregatorsPaginatorName",
     "ListInvitationsPaginatorName",
     "ListMembersPaginatorName",
     "ListOrganizationAdminAccountsPaginatorName",
+    "ListSecurityControlDefinitionsPaginatorName",
+    "ListStandardsControlAssociationsPaginatorName",
     "MalwareStateType",
     "MalwareTypeType",
     "MapFilterComparisonType",
     "NetworkDirectionType",
     "PartitionType",
     "RecordStateType",
+    "RegionAvailabilityStatusType",
+    "RuleStatusType",
     "SeverityLabelType",
     "SeverityRatingType",
     "SortOrderType",
     "StandardsStatusType",
     "StatusReasonCodeType",
     "StringFilterComparisonType",
     "ThreatIntelIndicatorCategoryType",
     "ThreatIntelIndicatorTypeType",
+    "UnprocessedErrorCodeType",
     "VerificationStateType",
     "VulnerabilityFixAvailableType",
     "WorkflowStateType",
     "WorkflowStatusType",
     "SecurityHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
+AssociationStatusType = Literal["DISABLED", "ENABLED"]
 AutoEnableStandardsType = Literal["DEFAULT", "NONE"]
+AutomationRulesActionTypeType = Literal["FINDING_FIELDS_UPDATE"]
 AwsIamAccessKeyStatusType = Literal["Active", "Inactive"]
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType = Literal["Prefix", "Suffix"]
 ComplianceStatusType = Literal["FAILED", "NOT_AVAILABLE", "PASSED", "WARNING"]
+ControlFindingGeneratorType = Literal["SECURITY_CONTROL", "STANDARD_CONTROL"]
 ControlStatusType = Literal["DISABLED", "ENABLED"]
 DateRangeUnitType = Literal["DAYS"]
 DescribeActionTargetsPaginatorName = Literal["describe_action_targets"]
 DescribeProductsPaginatorName = Literal["describe_products"]
 DescribeStandardsControlsPaginatorName = Literal["describe_standards_controls"]
 DescribeStandardsPaginatorName = Literal["describe_standards"]
+FindingHistoryUpdateSourceTypeType = Literal["BATCH_IMPORT_FINDINGS", "BATCH_UPDATE_FINDINGS"]
 GetEnabledStandardsPaginatorName = Literal["get_enabled_standards"]
+GetFindingHistoryPaginatorName = Literal["get_finding_history"]
 GetFindingsPaginatorName = Literal["get_findings"]
 GetInsightsPaginatorName = Literal["get_insights"]
 IntegrationTypeType = Literal[
     "RECEIVE_FINDINGS_FROM_SECURITY_HUB",
     "SEND_FINDINGS_TO_SECURITY_HUB",
     "UPDATE_FINDINGS_IN_SECURITY_HUB",
 ]
 ListEnabledProductsForImportPaginatorName = Literal["list_enabled_products_for_import"]
 ListFindingAggregatorsPaginatorName = Literal["list_finding_aggregators"]
 ListInvitationsPaginatorName = Literal["list_invitations"]
 ListMembersPaginatorName = Literal["list_members"]
 ListOrganizationAdminAccountsPaginatorName = Literal["list_organization_admin_accounts"]
+ListSecurityControlDefinitionsPaginatorName = Literal["list_security_control_definitions"]
+ListStandardsControlAssociationsPaginatorName = Literal["list_standards_control_associations"]
 MalwareStateType = Literal["OBSERVED", "REMOVAL_FAILED", "REMOVED"]
 MalwareTypeType = Literal[
     "ADWARE",
     "BLENDED_THREAT",
     "BOTNET_AGENT",
     "COIN_MINER",
     "EXPLOIT_KIT",
@@ -108,14 +123,16 @@
     "VIRUS",
     "WORM",
 ]
 MapFilterComparisonType = Literal["EQUALS", "NOT_EQUALS"]
 NetworkDirectionType = Literal["IN", "OUT"]
 PartitionType = Literal["aws", "aws-cn", "aws-us-gov"]
 RecordStateType = Literal["ACTIVE", "ARCHIVED"]
+RegionAvailabilityStatusType = Literal["AVAILABLE", "UNAVAILABLE"]
+RuleStatusType = Literal["DISABLED", "ENABLED"]
 SeverityLabelType = Literal["CRITICAL", "HIGH", "INFORMATIONAL", "LOW", "MEDIUM"]
 SeverityRatingType = Literal["CRITICAL", "HIGH", "LOW", "MEDIUM"]
 SortOrderType = Literal["asc", "desc"]
 StandardsStatusType = Literal["DELETING", "FAILED", "INCOMPLETE", "PENDING", "READY"]
 StatusReasonCodeType = Literal["INTERNAL_ERROR", "NO_AVAILABLE_CONFIGURATION_RECORDER"]
 StringFilterComparisonType = Literal["EQUALS", "NOT_EQUALS", "PREFIX", "PREFIX_NOT_EQUALS"]
 ThreatIntelIndicatorCategoryType = Literal[
@@ -130,14 +147,15 @@
     "HASH_SHA512",
     "IPV4_ADDRESS",
     "IPV6_ADDRESS",
     "MUTEX",
     "PROCESS",
     "URL",
 ]
+UnprocessedErrorCodeType = Literal["ACCESS_DENIED", "INVALID_INPUT", "LIMIT_EXCEEDED", "NOT_FOUND"]
 VerificationStateType = Literal["BENIGN_POSITIVE", "FALSE_POSITIVE", "TRUE_POSITIVE", "UNKNOWN"]
 VulnerabilityFixAvailableType = Literal["NO", "PARTIAL", "YES"]
 WorkflowStateType = Literal["ASSIGNED", "DEFERRED", "IN_PROGRESS", "NEW", "RESOLVED"]
 WorkflowStatusType = Literal["NEW", "NOTIFIED", "RESOLVED", "SUPPRESSED"]
 SecurityHubServiceName = Literal["securityhub"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -150,23 +168,25 @@
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
@@ -176,30 +196,35 @@
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
@@ -225,14 +250,15 @@
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
@@ -277,51 +303,57 @@
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
@@ -334,14 +366,15 @@
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
@@ -353,28 +386,35 @@
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
@@ -402,56 +442,64 @@
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
     "scheduler",
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
@@ -475,39 +523,47 @@
 ]
 PaginatorName = Literal[
     "describe_action_targets",
     "describe_products",
     "describe_standards",
     "describe_standards_controls",
     "get_enabled_standards",
+    "get_finding_history",
     "get_findings",
     "get_insights",
     "list_enabled_products_for_import",
     "list_finding_aggregators",
     "list_invitations",
     "list_members",
     "list_organization_admin_accounts",
+    "list_security_control_definitions",
+    "list_standards_control_associations",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/literals.pyi` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,84 +14,103 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AdminStatusType",
+    "AssociationStatusType",
     "AutoEnableStandardsType",
+    "AutomationRulesActionTypeType",
     "AwsIamAccessKeyStatusType",
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType",
     "ComplianceStatusType",
+    "ControlFindingGeneratorType",
     "ControlStatusType",
     "DateRangeUnitType",
     "DescribeActionTargetsPaginatorName",
     "DescribeProductsPaginatorName",
     "DescribeStandardsControlsPaginatorName",
     "DescribeStandardsPaginatorName",
+    "FindingHistoryUpdateSourceTypeType",
     "GetEnabledStandardsPaginatorName",
+    "GetFindingHistoryPaginatorName",
     "GetFindingsPaginatorName",
     "GetInsightsPaginatorName",
     "IntegrationTypeType",
     "ListEnabledProductsForImportPaginatorName",
     "ListFindingAggregatorsPaginatorName",
     "ListInvitationsPaginatorName",
     "ListMembersPaginatorName",
     "ListOrganizationAdminAccountsPaginatorName",
+    "ListSecurityControlDefinitionsPaginatorName",
+    "ListStandardsControlAssociationsPaginatorName",
     "MalwareStateType",
     "MalwareTypeType",
     "MapFilterComparisonType",
     "NetworkDirectionType",
     "PartitionType",
     "RecordStateType",
+    "RegionAvailabilityStatusType",
+    "RuleStatusType",
     "SeverityLabelType",
     "SeverityRatingType",
     "SortOrderType",
     "StandardsStatusType",
     "StatusReasonCodeType",
     "StringFilterComparisonType",
     "ThreatIntelIndicatorCategoryType",
     "ThreatIntelIndicatorTypeType",
+    "UnprocessedErrorCodeType",
     "VerificationStateType",
     "VulnerabilityFixAvailableType",
     "WorkflowStateType",
     "WorkflowStatusType",
     "SecurityHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
+AssociationStatusType = Literal["DISABLED", "ENABLED"]
 AutoEnableStandardsType = Literal["DEFAULT", "NONE"]
+AutomationRulesActionTypeType = Literal["FINDING_FIELDS_UPDATE"]
 AwsIamAccessKeyStatusType = Literal["Active", "Inactive"]
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType = Literal["Prefix", "Suffix"]
 ComplianceStatusType = Literal["FAILED", "NOT_AVAILABLE", "PASSED", "WARNING"]
+ControlFindingGeneratorType = Literal["SECURITY_CONTROL", "STANDARD_CONTROL"]
 ControlStatusType = Literal["DISABLED", "ENABLED"]
 DateRangeUnitType = Literal["DAYS"]
 DescribeActionTargetsPaginatorName = Literal["describe_action_targets"]
 DescribeProductsPaginatorName = Literal["describe_products"]
 DescribeStandardsControlsPaginatorName = Literal["describe_standards_controls"]
 DescribeStandardsPaginatorName = Literal["describe_standards"]
+FindingHistoryUpdateSourceTypeType = Literal["BATCH_IMPORT_FINDINGS", "BATCH_UPDATE_FINDINGS"]
 GetEnabledStandardsPaginatorName = Literal["get_enabled_standards"]
+GetFindingHistoryPaginatorName = Literal["get_finding_history"]
 GetFindingsPaginatorName = Literal["get_findings"]
 GetInsightsPaginatorName = Literal["get_insights"]
 IntegrationTypeType = Literal[
     "RECEIVE_FINDINGS_FROM_SECURITY_HUB",
     "SEND_FINDINGS_TO_SECURITY_HUB",
     "UPDATE_FINDINGS_IN_SECURITY_HUB",
 ]
 ListEnabledProductsForImportPaginatorName = Literal["list_enabled_products_for_import"]
 ListFindingAggregatorsPaginatorName = Literal["list_finding_aggregators"]
 ListInvitationsPaginatorName = Literal["list_invitations"]
 ListMembersPaginatorName = Literal["list_members"]
 ListOrganizationAdminAccountsPaginatorName = Literal["list_organization_admin_accounts"]
+ListSecurityControlDefinitionsPaginatorName = Literal["list_security_control_definitions"]
+ListStandardsControlAssociationsPaginatorName = Literal["list_standards_control_associations"]
 MalwareStateType = Literal["OBSERVED", "REMOVAL_FAILED", "REMOVED"]
 MalwareTypeType = Literal[
     "ADWARE",
     "BLENDED_THREAT",
     "BOTNET_AGENT",
     "COIN_MINER",
     "EXPLOIT_KIT",
@@ -106,14 +125,16 @@
     "VIRUS",
     "WORM",
 ]
 MapFilterComparisonType = Literal["EQUALS", "NOT_EQUALS"]
 NetworkDirectionType = Literal["IN", "OUT"]
 PartitionType = Literal["aws", "aws-cn", "aws-us-gov"]
 RecordStateType = Literal["ACTIVE", "ARCHIVED"]
+RegionAvailabilityStatusType = Literal["AVAILABLE", "UNAVAILABLE"]
+RuleStatusType = Literal["DISABLED", "ENABLED"]
 SeverityLabelType = Literal["CRITICAL", "HIGH", "INFORMATIONAL", "LOW", "MEDIUM"]
 SeverityRatingType = Literal["CRITICAL", "HIGH", "LOW", "MEDIUM"]
 SortOrderType = Literal["asc", "desc"]
 StandardsStatusType = Literal["DELETING", "FAILED", "INCOMPLETE", "PENDING", "READY"]
 StatusReasonCodeType = Literal["INTERNAL_ERROR", "NO_AVAILABLE_CONFIGURATION_RECORDER"]
 StringFilterComparisonType = Literal["EQUALS", "NOT_EQUALS", "PREFIX", "PREFIX_NOT_EQUALS"]
 ThreatIntelIndicatorCategoryType = Literal[
@@ -128,14 +149,15 @@
     "HASH_SHA512",
     "IPV4_ADDRESS",
     "IPV6_ADDRESS",
     "MUTEX",
     "PROCESS",
     "URL",
 ]
+UnprocessedErrorCodeType = Literal["ACCESS_DENIED", "INVALID_INPUT", "LIMIT_EXCEEDED", "NOT_FOUND"]
 VerificationStateType = Literal["BENIGN_POSITIVE", "FALSE_POSITIVE", "TRUE_POSITIVE", "UNKNOWN"]
 VulnerabilityFixAvailableType = Literal["NO", "PARTIAL", "YES"]
 WorkflowStateType = Literal["ASSIGNED", "DEFERRED", "IN_PROGRESS", "NEW", "RESOLVED"]
 WorkflowStatusType = Literal["NEW", "NOTIFIED", "RESOLVED", "SUPPRESSED"]
 SecurityHubServiceName = Literal["securityhub"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -148,23 +170,25 @@
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
@@ -174,30 +198,35 @@
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
@@ -223,14 +252,15 @@
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
@@ -275,51 +305,57 @@
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
@@ -332,14 +368,15 @@
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
@@ -351,28 +388,35 @@
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
@@ -400,56 +444,64 @@
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
     "scheduler",
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
@@ -473,39 +525,47 @@
 ]
 PaginatorName = Literal[
     "describe_action_targets",
     "describe_products",
     "describe_standards",
     "describe_standards_controls",
     "get_enabled_standards",
+    "get_finding_history",
     "get_findings",
     "get_insights",
     "list_enabled_products_for_import",
     "list_finding_aggregators",
     "list_invitations",
     "list_members",
     "list_organization_admin_accounts",
+    "list_security_control_definitions",
+    "list_standards_control_associations",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/paginator.py` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/paginator.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,75 +11,89 @@
     from mypy_boto3_securityhub.client import SecurityHubClient
     from mypy_boto3_securityhub.paginator import (
         DescribeActionTargetsPaginator,
         DescribeProductsPaginator,
         DescribeStandardsPaginator,
         DescribeStandardsControlsPaginator,
         GetEnabledStandardsPaginator,
+        GetFindingHistoryPaginator,
         GetFindingsPaginator,
         GetInsightsPaginator,
         ListEnabledProductsForImportPaginator,
         ListFindingAggregatorsPaginator,
         ListInvitationsPaginator,
         ListMembersPaginator,
         ListOrganizationAdminAccountsPaginator,
+        ListSecurityControlDefinitionsPaginator,
+        ListStandardsControlAssociationsPaginator,
     )
 
     session = Session()
     client: SecurityHubClient = session.client("securityhub")
 
     describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator("describe_action_targets")
     describe_products_paginator: DescribeProductsPaginator = client.get_paginator("describe_products")
     describe_standards_paginator: DescribeStandardsPaginator = client.get_paginator("describe_standards")
     describe_standards_controls_paginator: DescribeStandardsControlsPaginator = client.get_paginator("describe_standards_controls")
     get_enabled_standards_paginator: GetEnabledStandardsPaginator = client.get_paginator("get_enabled_standards")
+    get_finding_history_paginator: GetFindingHistoryPaginator = client.get_paginator("get_finding_history")
     get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
     get_insights_paginator: GetInsightsPaginator = client.get_paginator("get_insights")
     list_enabled_products_for_import_paginator: ListEnabledProductsForImportPaginator = client.get_paginator("list_enabled_products_for_import")
     list_finding_aggregators_paginator: ListFindingAggregatorsPaginator = client.get_paginator("list_finding_aggregators")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
+    list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")
+    list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from datetime import datetime
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     AwsSecurityFindingFiltersTypeDef,
+    AwsSecurityFindingIdentifierTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
     DescribeStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
+    GetFindingHistoryResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetInsightsResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
+    ListSecurityControlDefinitionsResponseTypeDef,
+    ListStandardsControlAssociationsResponseTypeDef,
     PaginatorConfigTypeDef,
     SortCriterionTypeDef,
 )
 
 __all__ = (
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
     "DescribeStandardsPaginator",
     "DescribeStandardsControlsPaginator",
     "GetEnabledStandardsPaginator",
+    "GetFindingHistoryPaginator",
     "GetFindingsPaginator",
     "GetInsightsPaginator",
     "ListEnabledProductsForImportPaginator",
     "ListFindingAggregatorsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
+    "ListSecurityControlDefinitionsPaginator",
+    "ListStandardsControlAssociationsPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -95,60 +109,60 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeactiontargetspaginator)
     """
 
     def paginate(
         self,
         *,
         ActionTargetArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeActionTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeactiontargetspaginator)
         """
 
 
 class DescribeProductsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeproductspaginator)
     """
 
     def paginate(
-        self, *, ProductArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ProductArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeproductspaginator)
         """
 
 
 class DescribeStandardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardspaginator)
         """
 
 
 class DescribeStandardsControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardscontrolspaginator)
     """
 
     def paginate(
-        self, *, StandardsSubscriptionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, StandardsSubscriptionArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStandardsControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardscontrolspaginator)
         """
 
 
@@ -158,122 +172,172 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getenabledstandardspaginator)
     """
 
     def paginate(
         self,
         *,
         StandardsSubscriptionArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetEnabledStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getenabledstandardspaginator)
         """
 
 
+class GetFindingHistoryPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindinghistorypaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
+        StartTime: Union[datetime, str] = ...,
+        EndTime: Union[datetime, str] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[GetFindingHistoryResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindinghistorypaginator)
+        """
+
+
 class GetFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
         """
 
 
 class GetInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getinsightspaginator)
     """
 
     def paginate(
-        self, *, InsightArns: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InsightArns: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getinsightspaginator)
         """
 
 
 class ListEnabledProductsForImportPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listenabledproductsforimportpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnabledProductsForImportResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listenabledproductsforimportpaginator)
         """
 
 
 class ListFindingAggregatorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listfindingaggregatorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFindingAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listfindingaggregatorspaginator)
         """
 
 
 class ListInvitationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listinvitationspaginator)
         """
 
 
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, OnlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, OnlyAssociated: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listmemberspaginator)
         """
 
 
 class ListOrganizationAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
         """
+
+
+class ListSecurityControlDefinitionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
+    """
+
+    def paginate(
+        self, *, StandardsArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListSecurityControlDefinitionsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
+        """
+
+
+class ListStandardsControlAssociationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
+    """
+
+    def paginate(
+        self, *, SecurityControlId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListStandardsControlAssociationsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
+        """
```

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/paginator.pyi` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/paginator.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -11,75 +11,89 @@
     from mypy_boto3_securityhub.client import SecurityHubClient
     from mypy_boto3_securityhub.paginator import (
         DescribeActionTargetsPaginator,
         DescribeProductsPaginator,
         DescribeStandardsPaginator,
         DescribeStandardsControlsPaginator,
         GetEnabledStandardsPaginator,
+        GetFindingHistoryPaginator,
         GetFindingsPaginator,
         GetInsightsPaginator,
         ListEnabledProductsForImportPaginator,
         ListFindingAggregatorsPaginator,
         ListInvitationsPaginator,
         ListMembersPaginator,
         ListOrganizationAdminAccountsPaginator,
+        ListSecurityControlDefinitionsPaginator,
+        ListStandardsControlAssociationsPaginator,
     )
 
     session = Session()
     client: SecurityHubClient = session.client("securityhub")
 
     describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator("describe_action_targets")
     describe_products_paginator: DescribeProductsPaginator = client.get_paginator("describe_products")
     describe_standards_paginator: DescribeStandardsPaginator = client.get_paginator("describe_standards")
     describe_standards_controls_paginator: DescribeStandardsControlsPaginator = client.get_paginator("describe_standards_controls")
     get_enabled_standards_paginator: GetEnabledStandardsPaginator = client.get_paginator("get_enabled_standards")
+    get_finding_history_paginator: GetFindingHistoryPaginator = client.get_paginator("get_finding_history")
     get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
     get_insights_paginator: GetInsightsPaginator = client.get_paginator("get_insights")
     list_enabled_products_for_import_paginator: ListEnabledProductsForImportPaginator = client.get_paginator("list_enabled_products_for_import")
     list_finding_aggregators_paginator: ListFindingAggregatorsPaginator = client.get_paginator("list_finding_aggregators")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
+    list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")
+    list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from datetime import datetime
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     AwsSecurityFindingFiltersTypeDef,
+    AwsSecurityFindingIdentifierTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
     DescribeStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
+    GetFindingHistoryResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetInsightsResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
+    ListSecurityControlDefinitionsResponseTypeDef,
+    ListStandardsControlAssociationsResponseTypeDef,
     PaginatorConfigTypeDef,
     SortCriterionTypeDef,
 )
 
 __all__ = (
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
     "DescribeStandardsPaginator",
     "DescribeStandardsControlsPaginator",
     "GetEnabledStandardsPaginator",
+    "GetFindingHistoryPaginator",
     "GetFindingsPaginator",
     "GetInsightsPaginator",
     "ListEnabledProductsForImportPaginator",
     "ListFindingAggregatorsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
+    "ListSecurityControlDefinitionsPaginator",
+    "ListStandardsControlAssociationsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
@@ -92,57 +106,57 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeactiontargetspaginator)
     """
 
     def paginate(
         self,
         *,
         ActionTargetArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeActionTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeactiontargetspaginator)
         """
 
 class DescribeProductsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeproductspaginator)
     """
 
     def paginate(
-        self, *, ProductArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ProductArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeproductspaginator)
         """
 
 class DescribeStandardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardspaginator)
         """
 
 class DescribeStandardsControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardscontrolspaginator)
     """
 
     def paginate(
-        self, *, StandardsSubscriptionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, StandardsSubscriptionArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStandardsControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardscontrolspaginator)
         """
 
 class GetEnabledStandardsPaginator(Paginator):
@@ -151,115 +165,162 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getenabledstandardspaginator)
     """
 
     def paginate(
         self,
         *,
         StandardsSubscriptionArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetEnabledStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getenabledstandardspaginator)
         """
 
+class GetFindingHistoryPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindinghistorypaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
+        StartTime: Union[datetime, str] = ...,
+        EndTime: Union[datetime, str] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[GetFindingHistoryResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindinghistorypaginator)
+        """
+
 class GetFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
         """
 
 class GetInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getinsightspaginator)
     """
 
     def paginate(
-        self, *, InsightArns: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InsightArns: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getinsightspaginator)
         """
 
 class ListEnabledProductsForImportPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listenabledproductsforimportpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnabledProductsForImportResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listenabledproductsforimportpaginator)
         """
 
 class ListFindingAggregatorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listfindingaggregatorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFindingAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listfindingaggregatorspaginator)
         """
 
 class ListInvitationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listinvitationspaginator)
         """
 
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, OnlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, OnlyAssociated: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listmemberspaginator)
         """
 
 class ListOrganizationAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
         """
+
+class ListSecurityControlDefinitionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
+    """
+
+    def paginate(
+        self, *, StandardsArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListSecurityControlDefinitionsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
+        """
+
+class ListStandardsControlAssociationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
+    """
+
+    def paginate(
+        self, *, SecurityControlId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListStandardsControlAssociationsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
+        """
```

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/type_defs.py` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -9,38 +9,44 @@
     from mypy_boto3_securityhub.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef
 
     data: AcceptAdministratorInvitationRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdminStatusType,
+    AssociationStatusType,
     AutoEnableStandardsType,
     AwsIamAccessKeyStatusType,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
     ComplianceStatusType,
+    ControlFindingGeneratorType,
     ControlStatusType,
+    FindingHistoryUpdateSourceTypeType,
     IntegrationTypeType,
     MalwareStateType,
     MalwareTypeType,
     MapFilterComparisonType,
     NetworkDirectionType,
     PartitionType,
     RecordStateType,
+    RegionAvailabilityStatusType,
+    RuleStatusType,
     SeverityLabelType,
     SeverityRatingType,
     SortOrderType,
     StandardsStatusType,
     StatusReasonCodeType,
     StringFilterComparisonType,
     ThreatIntelIndicatorCategoryType,
     ThreatIntelIndicatorTypeType,
+    UnprocessedErrorCodeType,
     VerificationStateType,
     VulnerabilityFixAvailableType,
     WorkflowStateType,
     WorkflowStatusType,
 )
 
 if sys.version_info >= (3, 9):
@@ -48,15 +54,14 @@
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
     "AccountDetailsTypeDef",
     "ActionLocalIpDetailsTypeDef",
     "ActionLocalPortDetailsTypeDef",
     "CityTypeDef",
@@ -64,22 +69,41 @@
     "GeoLocationTypeDef",
     "IpOrganizationDetailsTypeDef",
     "ActionRemotePortDetailsTypeDef",
     "ActionTargetTypeDef",
     "DnsRequestActionTypeDef",
     "AdjustmentTypeDef",
     "AdminAccountTypeDef",
+    "AssociatedStandardTypeDef",
+    "AssociationStateDetailsTypeDef",
+    "NoteUpdateTypeDef",
+    "RelatedFindingTypeDef",
+    "SeverityUpdateTypeDef",
+    "WorkflowUpdateTypeDef",
+    "MapFilterTypeDef",
+    "NumberFilterTypeDef",
+    "StringFilterTypeDef",
+    "AutomationRulesMetadataTypeDef",
     "AvailabilityZoneTypeDef",
+    "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
+    "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
+    "AwsAmazonMqBrokerUsersDetailsTypeDef",
+    "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
     "AwsApiCallActionDomainDetailsTypeDef",
     "AwsApiGatewayAccessLogSettingsTypeDef",
     "AwsApiGatewayCanarySettingsTypeDef",
     "AwsApiGatewayEndpointConfigurationTypeDef",
     "AwsApiGatewayMethodSettingsTypeDef",
     "AwsCorsConfigurationTypeDef",
     "AwsApiGatewayV2RouteSettingsTypeDef",
+    "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
+    "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef",
+    "AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef",
+    "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef",
@@ -119,22 +143,53 @@
     "AwsDynamoDbTableRestoreSummaryTypeDef",
     "AwsDynamoDbTableSseDescriptionTypeDef",
     "AwsDynamoDbTableStreamSpecificationTypeDef",
     "AwsDynamoDbTableProjectionTypeDef",
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
     "AwsEc2EipDetailsTypeDef",
     "AwsEc2InstanceMetadataOptionsTypeDef",
+    "AwsEc2InstanceMonitoringDetailsTypeDef",
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataPlacementDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef",
     "AwsEc2NetworkAclAssociationTypeDef",
     "IcmpTypeCodeTypeDef",
     "PortRangeFromToTypeDef",
     "AwsEc2NetworkInterfaceAttachmentTypeDef",
     "AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef",
     "AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef",
     "AwsEc2NetworkInterfaceSecurityGroupTypeDef",
+    "PropagatingVgwSetDetailsTypeDef",
+    "RouteSetDetailsTypeDef",
     "AwsEc2SecurityGroupIpRangeTypeDef",
     "AwsEc2SecurityGroupIpv6RangeTypeDef",
     "AwsEc2SecurityGroupPrefixListIdTypeDef",
     "AwsEc2SecurityGroupUserIdGroupPairTypeDef",
     "Ipv6CidrBlockAssociationTypeDef",
     "AwsEc2TransitGatewayDetailsTypeDef",
     "AwsEc2VolumeAttachmentTypeDef",
@@ -211,14 +266,22 @@
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
     "AwsElbLoadBalancerHealthCheckTypeDef",
     "AwsElbLoadBalancerInstanceTypeDef",
     "AwsElbLoadBalancerSourceSecurityGroupTypeDef",
     "AwsElbLoadBalancerListenerTypeDef",
     "AwsElbv2LoadBalancerAttributeTypeDef",
     "LoadBalancerStateTypeDef",
+    "AwsEventSchemasRegistryDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef",
+    "AwsGuardDutyDetectorFeaturesDetailsTypeDef",
     "AwsIamAccessKeySessionContextAttributesTypeDef",
     "AwsIamAccessKeySessionContextSessionIssuerTypeDef",
     "AwsIamAttachedManagedPolicyTypeDef",
     "AwsIamGroupPolicyTypeDef",
     "AwsIamInstanceProfileRoleTypeDef",
     "AwsIamPermissionsBoundaryTypeDef",
     "AwsIamPolicyVersionTypeDef",
@@ -278,139 +341,189 @@
     "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef",
     "AwsS3BucketBucketVersioningConfigurationTypeDef",
     "AwsS3BucketLoggingConfigurationTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef",
+    "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef",
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
     "AwsS3BucketWebsiteConfigurationRedirectToTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef",
     "AwsS3ObjectDetailsTypeDef",
+    "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     "BooleanFilterTypeDef",
     "IpFilterTypeDef",
     "KeywordFilterTypeDef",
-    "MapFilterTypeDef",
-    "NumberFilterTypeDef",
-    "StringFilterTypeDef",
     "AwsSecurityFindingIdentifierTypeDef",
     "MalwareTypeDef",
     "NoteTypeDef",
     "PatchSummaryTypeDef",
     "ProcessDetailsTypeDef",
-    "RelatedFindingTypeDef",
     "SeverityTypeDef",
     "ThreatIntelIndicatorTypeDef",
     "WorkflowTypeDef",
     "AwsSnsTopicSubscriptionTypeDef",
     "AwsSqsQueueDetailsTypeDef",
     "AwsSsmComplianceSummaryTypeDef",
+    "AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef",
+    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef",
     "AwsWafRateBasedRuleMatchPredicateTypeDef",
     "AwsWafRegionalRateBasedRuleMatchPredicateTypeDef",
     "AwsWafRegionalRulePredicateListDetailsTypeDef",
     "AwsWafRegionalRuleGroupRulesActionDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListActionDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef",
     "AwsWafRulePredicateListDetailsTypeDef",
     "AwsWafRuleGroupRulesActionDetailsTypeDef",
     "WafActionTypeDef",
     "WafExcludedRuleTypeDef",
     "WafOverrideActionTypeDef",
+    "AwsWafv2CustomHttpHeaderTypeDef",
+    "AwsWafv2VisibilityConfigDetailsTypeDef",
+    "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
     "AwsXrayEncryptionConfigDetailsTypeDef",
+    "BatchDeleteAutomationRulesRequestRequestTypeDef",
+    "UnprocessedAutomationRuleTypeDef",
     "BatchDisableStandardsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StandardsSubscriptionRequestTypeDef",
+    "BatchGetAutomationRulesRequestRequestTypeDef",
+    "BatchGetSecurityControlsRequestRequestTypeDef",
+    "SecurityControlTypeDef",
+    "UnprocessedSecurityControlTypeDef",
+    "StandardsControlAssociationIdTypeDef",
+    "StandardsControlAssociationDetailTypeDef",
     "ImportFindingsErrorTypeDef",
-    "NoteUpdateTypeDef",
-    "SeverityUpdateTypeDef",
-    "WorkflowUpdateTypeDef",
+    "StandardsControlAssociationUpdateTypeDef",
     "CellTypeDef",
     "ClassificationStatusTypeDef",
     "StatusReasonTypeDef",
     "VolumeMountTypeDef",
     "CreateActionTargetRequestRequestTypeDef",
+    "CreateActionTargetResponseTypeDef",
+    "CreateAutomationRuleResponseTypeDef",
     "CreateFindingAggregatorRequestRequestTypeDef",
+    "CreateFindingAggregatorResponseTypeDef",
+    "CreateInsightResponseTypeDef",
     "ResultTypeDef",
     "DateRangeTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteActionTargetRequestRequestTypeDef",
+    "DeleteActionTargetResponseTypeDef",
     "DeleteFindingAggregatorRequestRequestTypeDef",
     "DeleteInsightRequestRequestTypeDef",
+    "DeleteInsightResponseTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
     "DescribeActionTargetsRequestRequestTypeDef",
     "DescribeHubRequestRequestTypeDef",
+    "DescribeHubResponseTypeDef",
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
     "DescribeProductsRequestRequestTypeDef",
     "ProductTypeDef",
+    "DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
     "DescribeStandardsControlsRequestRequestTypeDef",
     "StandardsControlTypeDef",
+    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
     "DescribeStandardsRequestRequestTypeDef",
-    "StandardTypeDef",
     "DisableImportFindingsForProductRequestRequestTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
     "EnableImportFindingsForProductRequestRequestTypeDef",
+    "EnableImportFindingsForProductResponseTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "EnableSecurityHubRequestRequestTypeDef",
     "FilePathsTypeDef",
     "FindingAggregatorTypeDef",
+    "FindingHistoryUpdateSourceTypeDef",
+    "FindingHistoryUpdateTypeDef",
     "FindingProviderSeverityTypeDef",
     "FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef",
     "FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef",
     "InvitationTypeDef",
+    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
     "GetEnabledStandardsRequestRequestTypeDef",
     "GetFindingAggregatorRequestRequestTypeDef",
+    "GetFindingAggregatorResponseTypeDef",
     "SortCriterionTypeDef",
     "GetInsightResultsRequestRequestTypeDef",
+    "GetInsightsRequestGetInsightsPaginateTypeDef",
     "GetInsightsRequestRequestTypeDef",
+    "GetInvitationsCountResponseTypeDef",
     "GetMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "InsightResultValueTypeDef",
     "InviteMembersRequestRequestTypeDef",
+    "ListAutomationRulesRequestRequestTypeDef",
+    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
     "ListEnabledProductsForImportRequestRequestTypeDef",
+    "ListEnabledProductsForImportResponseTypeDef",
+    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
     "ListFindingAggregatorsRequestRequestTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
+    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
+    "ListSecurityControlDefinitionsRequestRequestTypeDef",
+    "SecurityControlDefinitionTypeDef",
+    "ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
+    "ListStandardsControlAssociationsRequestRequestTypeDef",
+    "StandardsControlAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PortRangeTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
+    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
+    "ResponseMetadataTypeDef",
     "RuleGroupSourceListDetailsTypeDef",
     "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
     "RuleGroupVariablesIpSetsDetailsTypeDef",
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     "SoftwarePackageTypeDef",
+    "StandardsManagedByTypeDef",
     "StandardsStatusReasonTypeDef",
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateActionTargetRequestRequestTypeDef",
     "UpdateFindingAggregatorRequestRequestTypeDef",
+    "UpdateFindingAggregatorResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateSecurityHubConfigurationRequestRequestTypeDef",
     "UpdateStandardsControlRequestRequestTypeDef",
     "VulnerabilityVendorTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "ActionRemoteIpDetailsTypeDef",
+    "DescribeActionTargetsResponseTypeDef",
     "CvssTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "AssociationSetDetailsTypeDef",
+    "AutomationRulesFindingFieldsUpdateTypeDef",
+    "ListAutomationRulesResponseTypeDef",
+    "AwsAmazonMqBrokerLogsDetailsTypeDef",
     "AwsApiGatewayRestApiDetailsTypeDef",
     "AwsApiGatewayStageDetailsTypeDef",
     "AwsApiGatewayV2ApiDetailsTypeDef",
     "AwsApiGatewayV2StageDetailsTypeDef",
+    "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef",
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
     "AwsBackupBackupVaultDetailsTypeDef",
     "AwsBackupRecoveryPointDetailsTypeDef",
     "AwsCertificateManagerCertificateDomainValidationOptionTypeDef",
     "AwsCloudFormationStackDetailsTypeDef",
@@ -420,14 +533,19 @@
     "AwsCloudWatchAlarmDetailsTypeDef",
     "AwsCodeBuildProjectEnvironmentTypeDef",
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     "AwsDynamoDbTableLocalSecondaryIndexTypeDef",
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
     "AwsEc2NetworkAclEntryTypeDef",
     "AwsEc2NetworkInterfaceDetailsTypeDef",
     "AwsEc2SecurityGroupIpPermissionTypeDef",
     "AwsEc2SubnetDetailsTypeDef",
     "AwsEc2VolumeDetailsTypeDef",
     "AwsEc2VpcDetailsTypeDef",
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
@@ -448,14 +566,16 @@
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
     "AwsElbLoadBalancerPoliciesTypeDef",
     "AwsElbLoadBalancerAttributesTypeDef",
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
     "AwsElbv2LoadBalancerDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
     "AwsIamAccessKeySessionContextTypeDef",
     "AwsIamGroupDetailsTypeDef",
     "AwsIamInstanceProfileTypeDef",
     "AwsIamPolicyDetailsTypeDef",
     "AwsIamUserDetailsTypeDef",
     "AwsKinesisStreamDetailsTypeDef",
     "AwsLambdaFunctionEnvironmentTypeDef",
@@ -467,148 +587,165 @@
     "AwsRdsDbSnapshotDetailsTypeDef",
     "AwsRdsDbPendingModifiedValuesTypeDef",
     "AwsRdsDbSecurityGroupDetailsTypeDef",
     "AwsRdsDbSubnetGroupSubnetTypeDef",
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
+    "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
+    "AwsSageMakerNotebookInstanceDetailsTypeDef",
     "AwsSecretsManagerSecretDetailsTypeDef",
+    "BatchUpdateFindingsRequestRequestTypeDef",
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
+    "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    "GetFindingHistoryRequestRequestTypeDef",
     "AwsSnsTopicDetailsTypeDef",
     "AwsSsmPatchTypeDef",
+    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     "AwsWafRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRuleDetailsTypeDef",
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
     "AwsWafRuleDetailsTypeDef",
     "AwsWafRuleGroupRulesDetailsTypeDef",
     "AwsWafWebAclRuleTypeDef",
-    "CreateActionTargetResponseTypeDef",
-    "CreateFindingAggregatorResponseTypeDef",
-    "CreateInsightResponseTypeDef",
-    "DeleteActionTargetResponseTypeDef",
-    "DeleteInsightResponseTypeDef",
-    "DescribeActionTargetsResponseTypeDef",
-    "DescribeHubResponseTypeDef",
-    "DescribeOrganizationConfigurationResponseTypeDef",
-    "EnableImportFindingsForProductResponseTypeDef",
-    "GetFindingAggregatorResponseTypeDef",
-    "GetInvitationsCountResponseTypeDef",
-    "ListEnabledProductsForImportResponseTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateFindingAggregatorResponseTypeDef",
+    "AwsWafv2CustomRequestHandlingDetailsTypeDef",
+    "AwsWafv2CustomResponseDetailsTypeDef",
+    "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
+    "BatchDeleteAutomationRulesResponseTypeDef",
+    "BatchUpdateAutomationRulesResponseTypeDef",
     "BatchEnableStandardsRequestRequestTypeDef",
+    "BatchGetSecurityControlsResponseTypeDef",
+    "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
+    "UnprocessedStandardsControlAssociationTypeDef",
     "BatchImportFindingsResponseTypeDef",
-    "BatchUpdateFindingsRequestRequestTypeDef",
+    "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
+    "UnprocessedStandardsControlAssociationUpdateTypeDef",
     "ComplianceTypeDef",
     "ContainerDetailsTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "DateFilterTypeDef",
-    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
-    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
-    "DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
-    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
-    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
-    "GetInsightsRequestGetInsightsPaginateTypeDef",
-    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
-    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "DescribeProductsResponseTypeDef",
     "DescribeStandardsControlsResponseTypeDef",
-    "DescribeStandardsResponseTypeDef",
     "ThreatTypeDef",
     "ListFindingAggregatorsResponseTypeDef",
+    "FindingHistoryRecordTypeDef",
     "FindingProviderFieldsTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "InsightResultsTypeDef",
+    "ListSecurityControlDefinitionsResponseTypeDef",
+    "ListStandardsControlAssociationsResponseTypeDef",
     "NetworkPathComponentDetailsTypeDef",
     "NetworkTypeDef",
     "PageTypeDef",
     "RemediationTypeDef",
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
     "RuleGroupVariablesTypeDef",
+    "StandardTypeDef",
     "StandardsSubscriptionTypeDef",
     "StatelessCustomPublishMetricActionTypeDef",
     "AwsApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "VulnerabilityTypeDef",
+    "AwsEc2RouteTableDetailsTypeDef",
+    "AutomationRulesActionTypeDef",
+    "AwsAmazonMqBrokerDetailsTypeDef",
+    "AwsAppSyncGraphQlApiDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     "AwsBackupBackupPlanRuleDetailsTypeDef",
     "AwsCertificateManagerCertificateRenewalSummaryTypeDef",
     "AwsCloudFrontDistributionOriginItemTypeDef",
     "AwsCloudFrontDistributionOriginGroupTypeDef",
     "AwsCodeBuildProjectDetailsTypeDef",
     "AwsDynamoDbTableReplicaTypeDef",
+    "AwsEc2LaunchTemplateDataDetailsTypeDef",
     "AwsEc2NetworkAclDetailsTypeDef",
     "AwsEc2SecurityGroupDetailsTypeDef",
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
     "AwsEc2VpnConnectionDetailsTypeDef",
     "AwsEcsClusterConfigurationDetailsTypeDef",
     "AwsEcsServiceDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
     "AwsEcsTaskDetailsTypeDef",
     "AwsEfsAccessPointDetailsTypeDef",
     "AwsEksClusterDetailsTypeDef",
     "AwsElasticsearchDomainDetailsTypeDef",
     "AwsElbLoadBalancerDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
     "AwsIamAccessKeyDetailsTypeDef",
     "AwsIamRoleDetailsTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
     "AwsOpenSearchServiceDomainDetailsTypeDef",
     "AwsRdsDbSubnetGroupTypeDef",
     "AwsRedshiftClusterDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
+    "AwsS3BucketObjectLockConfigurationTypeDef",
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     "AwsS3BucketWebsiteConfigurationTypeDef",
     "BatchUpdateFindingsResponseTypeDef",
     "AwsSsmPatchComplianceDetailsTypeDef",
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     "AwsWafRegionalWebAclDetailsTypeDef",
     "AwsWafRuleGroupDetailsTypeDef",
     "AwsWafWebAclDetailsTypeDef",
+    "AwsWafv2ActionAllowDetailsTypeDef",
+    "AwsWafv2RulesActionCaptchaDetailsTypeDef",
+    "AwsWafv2RulesActionCountDetailsTypeDef",
+    "AwsWafv2ActionBlockDetailsTypeDef",
+    "BatchGetStandardsControlAssociationsResponseTypeDef",
+    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
+    "AutomationRulesFindingFiltersTypeDef",
     "AwsSecurityFindingFiltersTypeDef",
+    "GetFindingHistoryResponseTypeDef",
     "GetInsightResultsResponseTypeDef",
     "NetworkHeaderTypeDef",
     "OccurrencesTypeDef",
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
+    "DescribeStandardsResponseTypeDef",
     "BatchDisableStandardsResponseTypeDef",
     "BatchEnableStandardsResponseTypeDef",
     "GetEnabledStandardsResponseTypeDef",
     "StatelessCustomActionDefinitionTypeDef",
     "PortProbeActionTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     "AwsCertificateManagerCertificateDetailsTypeDef",
     "AwsCloudFrontDistributionOriginsTypeDef",
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
     "AwsDynamoDbTableDetailsTypeDef",
+    "AwsEc2LaunchTemplateDetailsTypeDef",
     "AwsEcsClusterDetailsTypeDef",
     "AwsEcsTaskDefinitionDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
     "AwsRdsDbInstanceDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
+    "AwsStepFunctionStateMachineDetailsTypeDef",
+    "AwsWafv2RulesActionDetailsTypeDef",
+    "AwsWafv2WebAclActionDetailsTypeDef",
+    "AutomationRulesConfigTypeDef",
+    "CreateAutomationRuleRequestRequestTypeDef",
+    "UpdateAutomationRulesRequestItemTypeDef",
     "CreateInsightRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "InsightTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "UpdateInsightRequestRequestTypeDef",
     "NetworkPathComponentTypeDef",
@@ -616,22 +753,28 @@
     "SensitiveDataDetectionsTypeDef",
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     "RuleGroupSourceCustomActionsDetailsTypeDef",
     "ActionTypeDef",
     "AwsBackupBackupPlanDetailsTypeDef",
     "AwsCloudFrontDistributionDetailsTypeDef",
+    "AwsGuardDutyDetectorDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationTypeDef",
+    "AwsWafv2RulesDetailsTypeDef",
+    "BatchGetAutomationRulesResponseTypeDef",
+    "BatchUpdateAutomationRulesRequestRequestTypeDef",
     "GetInsightsResponseTypeDef",
     "CustomDataIdentifiersResultTypeDef",
     "SensitiveDataResultTypeDef",
     "FirewallPolicyDetailsTypeDef",
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
+    "AwsWafv2RuleGroupDetailsTypeDef",
+    "AwsWafv2WebAclDetailsTypeDef",
     "ClassificationResultTypeDef",
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     "RuleGroupSourceTypeDef",
     "AwsS3BucketDetailsTypeDef",
     "DataClassificationDetailsTypeDef",
     "RuleGroupDetailsTypeDef",
     "AwsNetworkFirewallRuleGroupDetailsTypeDef",
@@ -668,19 +811,17 @@
     "_OptionalAccountDetailsTypeDef",
     {
         "Email": str,
     },
     total=False,
 )
 
-
 class AccountDetailsTypeDef(_RequiredAccountDetailsTypeDef, _OptionalAccountDetailsTypeDef):
     pass
 
-
 ActionLocalIpDetailsTypeDef = TypedDict(
     "ActionLocalIpDetailsTypeDef",
     {
         "IpAddressV4": str,
     },
     total=False,
 )
@@ -773,23 +914,173 @@
     {
         "AccountId": str,
         "Status": AdminStatusType,
     },
     total=False,
 )
 
+AssociatedStandardTypeDef = TypedDict(
+    "AssociatedStandardTypeDef",
+    {
+        "StandardsId": str,
+    },
+    total=False,
+)
+
+AssociationStateDetailsTypeDef = TypedDict(
+    "AssociationStateDetailsTypeDef",
+    {
+        "State": str,
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
+NoteUpdateTypeDef = TypedDict(
+    "NoteUpdateTypeDef",
+    {
+        "Text": str,
+        "UpdatedBy": str,
+    },
+)
+
+RelatedFindingTypeDef = TypedDict(
+    "RelatedFindingTypeDef",
+    {
+        "ProductArn": str,
+        "Id": str,
+    },
+)
+
+SeverityUpdateTypeDef = TypedDict(
+    "SeverityUpdateTypeDef",
+    {
+        "Normalized": int,
+        "Product": float,
+        "Label": SeverityLabelType,
+    },
+    total=False,
+)
+
+WorkflowUpdateTypeDef = TypedDict(
+    "WorkflowUpdateTypeDef",
+    {
+        "Status": WorkflowStatusType,
+    },
+    total=False,
+)
+
+MapFilterTypeDef = TypedDict(
+    "MapFilterTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "Comparison": MapFilterComparisonType,
+    },
+    total=False,
+)
+
+NumberFilterTypeDef = TypedDict(
+    "NumberFilterTypeDef",
+    {
+        "Gte": float,
+        "Lte": float,
+        "Eq": float,
+    },
+    total=False,
+)
+
+StringFilterTypeDef = TypedDict(
+    "StringFilterTypeDef",
+    {
+        "Value": str,
+        "Comparison": StringFilterComparisonType,
+    },
+    total=False,
+)
+
+AutomationRulesMetadataTypeDef = TypedDict(
+    "AutomationRulesMetadataTypeDef",
+    {
+        "RuleArn": str,
+        "RuleStatus": RuleStatusType,
+        "RuleOrder": int,
+        "RuleName": str,
+        "Description": str,
+        "IsTerminal": bool,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "CreatedBy": str,
+    },
+    total=False,
+)
+
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
     },
     total=False,
 )
 
+AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
+    {
+        "KmsKeyId": str,
+        "UseAwsOwnedKey": bool,
+    },
+    total=False,
+)
+
+AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
+    {
+        "Hosts": Sequence[str],
+        "RoleBase": str,
+        "RoleName": str,
+        "RoleSearchMatching": str,
+        "RoleSearchSubtree": bool,
+        "ServiceAccountUsername": str,
+        "UserBase": str,
+        "UserRoleName": str,
+        "UserSearchMatching": str,
+        "UserSearchSubtree": bool,
+    },
+    total=False,
+)
+
+AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
+    {
+        "DayOfWeek": str,
+        "TimeOfDay": str,
+        "TimeZone": str,
+    },
+    total=False,
+)
+
+AwsAmazonMqBrokerUsersDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerUsersDetailsTypeDef",
+    {
+        "PendingChange": str,
+        "Username": str,
+    },
+    total=False,
+)
+
+AwsAmazonMqBrokerLogsPendingDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
+    {
+        "Audit": bool,
+        "General": bool,
+    },
+    total=False,
+)
+
 AwsApiCallActionDomainDetailsTypeDef = TypedDict(
     "AwsApiCallActionDomainDetailsTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
@@ -862,14 +1153,56 @@
         "DataTraceEnabled": bool,
         "ThrottlingBurstLimit": int,
         "ThrottlingRateLimit": float,
     },
     total=False,
 )
 
+AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
+    {
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerUri": str,
+        "IdentityValidationExpression": str,
+    },
+    total=False,
+)
+
+AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef",
+    {
+        "AuthTtL": int,
+        "ClientId": str,
+        "IatTtL": int,
+        "Issuer": str,
+    },
+    total=False,
+)
+
+AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef",
+    {
+        "AppIdClientRegex": str,
+        "AwsRegion": str,
+        "DefaultAction": str,
+        "UserPoolId": str,
+    },
+    total=False,
+)
+
+AwsAppSyncGraphQlApiLogConfigDetailsTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
+    {
+        "CloudWatchLogsRoleArn": str,
+        "ExcludeVerboseContent": bool,
+        "FieldLogLevel": str,
+    },
+    total=False,
+)
+
 AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
@@ -1342,22 +1675,291 @@
         "HttpPutResponseHopLimit": int,
         "HttpTokens": str,
         "InstanceMetadataTags": str,
     },
     total=False,
 )
 
+AwsEc2InstanceMonitoringDetailsTypeDef = TypedDict(
+    "AwsEc2InstanceMonitoringDetailsTypeDef",
+    {
+        "State": str,
+    },
+    total=False,
+)
+
 AwsEc2InstanceNetworkInterfacesDetailsTypeDef = TypedDict(
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
     {
         "NetworkInterfaceId": str,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
+    {
+        "DeleteOnTermination": bool,
+        "Encrypted": bool,
+        "Iops": int,
+        "KmsKeyId": str,
+        "SnapshotId": str,
+        "Throughput": int,
+        "VolumeSize": int,
+        "VolumeType": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
+    {
+        "CapacityReservationId": str,
+        "CapacityReservationResourceGroupArn": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
+    {
+        "CoreCount": int,
+        "ThreadsPerCore": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
+    {
+        "CpuCredits": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
+    {
+        "Type": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef",
+    {
+        "Count": int,
+        "Type": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef",
+    {
+        "Configured": bool,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef",
+    {
+        "AutoRecovery": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef",
+    {
+        "HttpEndpoint": str,
+        "HttpProtocolIpv6": str,
+        "HttpTokens": str,
+        "HttpPutResponseHopLimit": int,
+        "InstanceMetadataTags": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataPlacementDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataPlacementDetailsTypeDef",
+    {
+        "Affinity": str,
+        "AvailabilityZone": str,
+        "GroupName": str,
+        "HostId": str,
+        "HostResourceGroupArn": str,
+        "PartitionNumber": int,
+        "SpreadDomain": str,
+        "Tenancy": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef",
+    {
+        "EnableResourceNameDnsAAAARecord": bool,
+        "EnableResourceNameDnsARecord": bool,
+        "HostnameType": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
+    {
+        "BlockDurationMinutes": int,
+        "InstanceInterruptionBehavior": str,
+        "MaxPrice": str,
+        "SpotInstanceType": str,
+        "ValidUntil": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
+    {
+        "Max": int,
+        "Min": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
+    {
+        "Max": int,
+        "Min": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
+    {
+        "Max": int,
+        "Min": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
+    {
+        "Max": float,
+        "Min": float,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef",
+    {
+        "Max": int,
+        "Min": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef",
+    {
+        "Max": int,
+        "Min": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef",
+    {
+        "Max": float,
+        "Min": float,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef",
+    {
+        "Max": int,
+        "Min": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
+    {
+        "Ipv4Prefix": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef",
+    {
+        "Ipv6Address": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef",
+    {
+        "Ipv6Prefix": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef",
+    {
+        "Primary": bool,
+        "PrivateIpAddress": str,
+    },
+    total=False,
+)
+
 AwsEc2NetworkAclAssociationTypeDef = TypedDict(
     "AwsEc2NetworkAclAssociationTypeDef",
     {
         "NetworkAclAssociationId": str,
         "NetworkAclId": str,
         "SubnetId": str,
     },
@@ -1418,14 +2020,45 @@
     {
         "GroupName": str,
         "GroupId": str,
     },
     total=False,
 )
 
+PropagatingVgwSetDetailsTypeDef = TypedDict(
+    "PropagatingVgwSetDetailsTypeDef",
+    {
+        "GatewayId": str,
+    },
+    total=False,
+)
+
+RouteSetDetailsTypeDef = TypedDict(
+    "RouteSetDetailsTypeDef",
+    {
+        "CarrierGatewayId": str,
+        "CoreNetworkArn": str,
+        "DestinationCidrBlock": str,
+        "DestinationIpv6CidrBlock": str,
+        "DestinationPrefixListId": str,
+        "EgressOnlyInternetGatewayId": str,
+        "GatewayId": str,
+        "InstanceId": str,
+        "InstanceOwnerId": str,
+        "LocalGatewayId": str,
+        "NatGatewayId": str,
+        "NetworkInterfaceId": str,
+        "Origin": str,
+        "State": str,
+        "TransitGatewayId": str,
+        "VpcPeeringConnectionId": str,
+    },
+    total=False,
+)
+
 AwsEc2SecurityGroupIpRangeTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpRangeTypeDef",
     {
         "CidrIp": str,
     },
     total=False,
 )
@@ -1998,14 +2631,15 @@
 )
 
 AwsEksClusterResourcesVpcConfigDetailsTypeDef = TypedDict(
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
+        "EndpointPublicAccess": bool,
     },
     total=False,
 )
 
 AwsEksClusterLoggingClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
     {
@@ -2240,14 +2874,82 @@
     {
         "Code": str,
         "Reason": str,
     },
     total=False,
 )
 
+AwsEventSchemasRegistryDetailsTypeDef = TypedDict(
+    "AwsEventSchemasRegistryDetailsTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef",
+    {
+        "Status": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef",
+    {
+        "Status": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef",
+    {
+        "Status": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef",
+    {
+        "Status": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef",
+    {
+        "Status": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef",
+    {
+        "Reason": str,
+        "Status": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorFeaturesDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorFeaturesDetailsTypeDef",
+    {
+        "Name": str,
+        "Status": str,
+    },
+    total=False,
+)
+
 AwsIamAccessKeySessionContextAttributesTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextAttributesTypeDef",
     {
         "MfaAuthenticated": bool,
         "CreationDate": str,
     },
     total=False,
@@ -2923,14 +3625,24 @@
     {
         "Name": AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
         "Value": str,
     },
     total=False,
 )
 
+AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef = TypedDict(
+    "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef",
+    {
+        "Days": int,
+        "Mode": str,
+        "Years": int,
+    },
+    total=False,
+)
+
 AwsS3BucketServerSideEncryptionByDefaultTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
     {
         "SSEAlgorithm": str,
         "KMSMasterKeyID": str,
     },
     total=False,
@@ -2975,14 +3687,22 @@
         "ContentType": str,
         "ServerSideEncryption": str,
         "SSEKMSKeyId": str,
     },
     total=False,
 )
 
+AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef = TypedDict(
+    "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
+    {
+        "MinimumInstanceMetadataServiceVersion": str,
+    },
+    total=False,
+)
+
 AwsSecretsManagerSecretRotationRulesTypeDef = TypedDict(
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     {
         "AutomaticallyAfterDays": int,
     },
     total=False,
 )
@@ -3007,43 +3727,14 @@
     "KeywordFilterTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-MapFilterTypeDef = TypedDict(
-    "MapFilterTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "Comparison": MapFilterComparisonType,
-    },
-    total=False,
-)
-
-NumberFilterTypeDef = TypedDict(
-    "NumberFilterTypeDef",
-    {
-        "Gte": float,
-        "Lte": float,
-        "Eq": float,
-    },
-    total=False,
-)
-
-StringFilterTypeDef = TypedDict(
-    "StringFilterTypeDef",
-    {
-        "Value": str,
-        "Comparison": StringFilterComparisonType,
-    },
-    total=False,
-)
-
 AwsSecurityFindingIdentifierTypeDef = TypedDict(
     "AwsSecurityFindingIdentifierTypeDef",
     {
         "Id": str,
         "ProductArn": str,
     },
 )
@@ -3060,19 +3751,17 @@
         "Type": MalwareTypeType,
         "Path": str,
         "State": MalwareStateType,
     },
     total=False,
 )
 
-
 class MalwareTypeDef(_RequiredMalwareTypeDef, _OptionalMalwareTypeDef):
     pass
 
-
 NoteTypeDef = TypedDict(
     "NoteTypeDef",
     {
         "Text": str,
         "UpdatedBy": str,
         "UpdatedAt": str,
     },
@@ -3097,40 +3786,30 @@
         "OperationEndTime": str,
         "RebootOption": str,
         "Operation": str,
     },
     total=False,
 )
 
-
 class PatchSummaryTypeDef(_RequiredPatchSummaryTypeDef, _OptionalPatchSummaryTypeDef):
     pass
 
-
 ProcessDetailsTypeDef = TypedDict(
     "ProcessDetailsTypeDef",
     {
         "Name": str,
         "Path": str,
         "Pid": int,
         "ParentPid": int,
         "LaunchedAt": str,
         "TerminatedAt": str,
     },
     total=False,
 )
 
-RelatedFindingTypeDef = TypedDict(
-    "RelatedFindingTypeDef",
-    {
-        "ProductArn": str,
-        "Id": str,
-    },
-)
-
 SeverityTypeDef = TypedDict(
     "SeverityTypeDef",
     {
         "Product": float,
         "Label": SeverityLabelType,
         "Normalized": int,
         "Original": str,
@@ -3200,14 +3879,30 @@
         "NonCompliantMediumCount": int,
         "NonCompliantUnspecifiedCount": int,
         "PatchGroup": str,
     },
     total=False,
 )
 
+AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef",
+    {
+        "LogGroupArn": str,
+    },
+    total=False,
+)
+
 AwsWafRateBasedRuleMatchPredicateTypeDef = TypedDict(
     "AwsWafRateBasedRuleMatchPredicateTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
@@ -3296,39 +3991,72 @@
     "WafOverrideActionTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
+AwsWafv2CustomHttpHeaderTypeDef = TypedDict(
+    "AwsWafv2CustomHttpHeaderTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+    total=False,
+)
+
+AwsWafv2VisibilityConfigDetailsTypeDef = TypedDict(
+    "AwsWafv2VisibilityConfigDetailsTypeDef",
+    {
+        "CloudWatchMetricsEnabled": bool,
+        "MetricName": str,
+        "SampledRequestsEnabled": bool,
+    },
+    total=False,
+)
+
+AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef = TypedDict(
+    "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
+    {
+        "ImmunityTime": int,
+    },
+    total=False,
+)
+
 AwsXrayEncryptionConfigDetailsTypeDef = TypedDict(
     "AwsXrayEncryptionConfigDetailsTypeDef",
     {
         "KeyId": str,
         "Status": str,
         "Type": str,
     },
     total=False,
 )
 
-BatchDisableStandardsRequestRequestTypeDef = TypedDict(
-    "BatchDisableStandardsRequestRequestTypeDef",
+BatchDeleteAutomationRulesRequestRequestTypeDef = TypedDict(
+    "BatchDeleteAutomationRulesRequestRequestTypeDef",
     {
-        "StandardsSubscriptionArns": Sequence[str],
+        "AutomationRulesArns": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UnprocessedAutomationRuleTypeDef = TypedDict(
+    "UnprocessedAutomationRuleTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "RuleArn": str,
+        "ErrorCode": int,
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
+BatchDisableStandardsRequestRequestTypeDef = TypedDict(
+    "BatchDisableStandardsRequestRequestTypeDef",
+    {
+        "StandardsSubscriptionArns": Sequence[str],
     },
 )
 
 _RequiredStandardsSubscriptionRequestTypeDef = TypedDict(
     "_RequiredStandardsSubscriptionRequestTypeDef",
     {
         "StandardsArn": str,
@@ -3338,56 +4066,133 @@
     "_OptionalStandardsSubscriptionRequestTypeDef",
     {
         "StandardsInput": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StandardsSubscriptionRequestTypeDef(
     _RequiredStandardsSubscriptionRequestTypeDef, _OptionalStandardsSubscriptionRequestTypeDef
 ):
     pass
 
+BatchGetAutomationRulesRequestRequestTypeDef = TypedDict(
+    "BatchGetAutomationRulesRequestRequestTypeDef",
+    {
+        "AutomationRulesArns": Sequence[str],
+    },
+)
 
-ImportFindingsErrorTypeDef = TypedDict(
-    "ImportFindingsErrorTypeDef",
+BatchGetSecurityControlsRequestRequestTypeDef = TypedDict(
+    "BatchGetSecurityControlsRequestRequestTypeDef",
     {
-        "Id": str,
-        "ErrorCode": str,
-        "ErrorMessage": str,
+        "SecurityControlIds": Sequence[str],
     },
 )
 
-NoteUpdateTypeDef = TypedDict(
-    "NoteUpdateTypeDef",
+SecurityControlTypeDef = TypedDict(
+    "SecurityControlTypeDef",
     {
-        "Text": str,
-        "UpdatedBy": str,
+        "SecurityControlId": str,
+        "SecurityControlArn": str,
+        "Title": str,
+        "Description": str,
+        "RemediationUrl": str,
+        "SeverityRating": SeverityRatingType,
+        "SecurityControlStatus": ControlStatusType,
     },
 )
 
-SeverityUpdateTypeDef = TypedDict(
-    "SeverityUpdateTypeDef",
+_RequiredUnprocessedSecurityControlTypeDef = TypedDict(
+    "_RequiredUnprocessedSecurityControlTypeDef",
     {
-        "Normalized": int,
-        "Product": float,
-        "Label": SeverityLabelType,
+        "SecurityControlId": str,
+        "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedSecurityControlTypeDef = TypedDict(
+    "_OptionalUnprocessedSecurityControlTypeDef",
+    {
+        "ErrorReason": str,
     },
     total=False,
 )
 
-WorkflowUpdateTypeDef = TypedDict(
-    "WorkflowUpdateTypeDef",
+class UnprocessedSecurityControlTypeDef(
+    _RequiredUnprocessedSecurityControlTypeDef, _OptionalUnprocessedSecurityControlTypeDef
+):
+    pass
+
+StandardsControlAssociationIdTypeDef = TypedDict(
+    "StandardsControlAssociationIdTypeDef",
     {
-        "Status": WorkflowStatusType,
+        "SecurityControlId": str,
+        "StandardsArn": str,
+    },
+)
+
+_RequiredStandardsControlAssociationDetailTypeDef = TypedDict(
+    "_RequiredStandardsControlAssociationDetailTypeDef",
+    {
+        "StandardsArn": str,
+        "SecurityControlId": str,
+        "SecurityControlArn": str,
+        "AssociationStatus": AssociationStatusType,
+    },
+)
+_OptionalStandardsControlAssociationDetailTypeDef = TypedDict(
+    "_OptionalStandardsControlAssociationDetailTypeDef",
+    {
+        "RelatedRequirements": List[str],
+        "UpdatedAt": datetime,
+        "UpdatedReason": str,
+        "StandardsControlTitle": str,
+        "StandardsControlDescription": str,
+        "StandardsControlArns": List[str],
     },
     total=False,
 )
 
+class StandardsControlAssociationDetailTypeDef(
+    _RequiredStandardsControlAssociationDetailTypeDef,
+    _OptionalStandardsControlAssociationDetailTypeDef,
+):
+    pass
+
+ImportFindingsErrorTypeDef = TypedDict(
+    "ImportFindingsErrorTypeDef",
+    {
+        "Id": str,
+        "ErrorCode": str,
+        "ErrorMessage": str,
+    },
+)
+
+_RequiredStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_RequiredStandardsControlAssociationUpdateTypeDef",
+    {
+        "StandardsArn": str,
+        "SecurityControlId": str,
+        "AssociationStatus": AssociationStatusType,
+    },
+)
+_OptionalStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_OptionalStandardsControlAssociationUpdateTypeDef",
+    {
+        "UpdatedReason": str,
+    },
+    total=False,
+)
+
+class StandardsControlAssociationUpdateTypeDef(
+    _RequiredStandardsControlAssociationUpdateTypeDef,
+    _OptionalStandardsControlAssociationUpdateTypeDef,
+):
+    pass
+
 CellTypeDef = TypedDict(
     "CellTypeDef",
     {
         "Column": int,
         "Row": int,
         "ColumnName": str,
         "CellReference": str,
@@ -3414,19 +4219,17 @@
     "_OptionalStatusReasonTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class StatusReasonTypeDef(_RequiredStatusReasonTypeDef, _OptionalStatusReasonTypeDef):
     pass
 
-
 VolumeMountTypeDef = TypedDict(
     "VolumeMountTypeDef",
     {
         "Name": str,
         "MountPath": str,
     },
     total=False,
@@ -3437,35 +4240,68 @@
     {
         "Name": str,
         "Description": str,
         "Id": str,
     },
 )
 
+CreateActionTargetResponseTypeDef = TypedDict(
+    "CreateActionTargetResponseTypeDef",
+    {
+        "ActionTargetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAutomationRuleResponseTypeDef = TypedDict(
+    "CreateAutomationRuleResponseTypeDef",
+    {
+        "RuleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFindingAggregatorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFindingAggregatorRequestRequestTypeDef",
     {
         "RegionLinkingMode": str,
     },
 )
 _OptionalCreateFindingAggregatorRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFindingAggregatorRequestRequestTypeDef",
     {
         "Regions": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateFindingAggregatorRequestRequestTypeDef(
     _RequiredCreateFindingAggregatorRequestRequestTypeDef,
     _OptionalCreateFindingAggregatorRequestRequestTypeDef,
 ):
     pass
 
+CreateFindingAggregatorResponseTypeDef = TypedDict(
+    "CreateFindingAggregatorResponseTypeDef",
+    {
+        "FindingAggregatorArn": str,
+        "FindingAggregationRegion": str,
+        "RegionLinkingMode": str,
+        "Regions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateInsightResponseTypeDef = TypedDict(
+    "CreateInsightResponseTypeDef",
+    {
+        "InsightArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ResultTypeDef = TypedDict(
     "ResultTypeDef",
     {
         "AccountId": str,
         "ProcessingResult": str,
     },
@@ -3491,48 +4327,63 @@
 DeleteActionTargetRequestRequestTypeDef = TypedDict(
     "DeleteActionTargetRequestRequestTypeDef",
     {
         "ActionTargetArn": str,
     },
 )
 
+DeleteActionTargetResponseTypeDef = TypedDict(
+    "DeleteActionTargetResponseTypeDef",
+    {
+        "ActionTargetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteFindingAggregatorRequestRequestTypeDef = TypedDict(
     "DeleteFindingAggregatorRequestRequestTypeDef",
     {
         "FindingAggregatorArn": str,
     },
 )
 
 DeleteInsightRequestRequestTypeDef = TypedDict(
     "DeleteInsightRequestRequestTypeDef",
     {
         "InsightArn": str,
     },
 )
 
+DeleteInsightResponseTypeDef = TypedDict(
+    "DeleteInsightResponseTypeDef",
+    {
+        "InsightArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteInvitationsRequestRequestTypeDef = TypedDict(
     "DeleteInvitationsRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
 DeleteMembersRequestRequestTypeDef = TypedDict(
     "DeleteMembersRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef = TypedDict(
+    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ActionTargetArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeActionTargetsRequestRequestTypeDef = TypedDict(
     "DescribeActionTargetsRequestRequestTypeDef",
     {
@@ -3547,14 +4398,44 @@
     "DescribeHubRequestRequestTypeDef",
     {
         "HubArn": str,
     },
     total=False,
 )
 
+DescribeHubResponseTypeDef = TypedDict(
+    "DescribeHubResponseTypeDef",
+    {
+        "HubArn": str,
+        "SubscribedAt": str,
+        "AutoEnableControls": bool,
+        "ControlFindingGenerator": ControlFindingGeneratorType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    {
+        "AutoEnable": bool,
+        "MemberAccountLimitReached": bool,
+        "AutoEnableStandards": AutoEnableStandardsType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeProductsRequestDescribeProductsPaginateTypeDef = TypedDict(
+    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
+    {
+        "ProductArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeProductsRequestRequestTypeDef = TypedDict(
     "DescribeProductsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ProductArn": str,
     },
@@ -3578,18 +4459,36 @@
         "MarketplaceUrl": str,
         "ActivationUrl": str,
         "ProductSubscriptionResourcePolicy": str,
     },
     total=False,
 )
 
-
 class ProductTypeDef(_RequiredProductTypeDef, _OptionalProductTypeDef):
     pass
 
+_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
+    {
+        "StandardsSubscriptionArn": str,
+    },
+)
+_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef(
+    _RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
+    _OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
+):
+    pass
 
 _RequiredDescribeStandardsControlsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeStandardsControlsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArn": str,
     },
 )
@@ -3598,22 +4497,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeStandardsControlsRequestRequestTypeDef(
     _RequiredDescribeStandardsControlsRequestRequestTypeDef,
     _OptionalDescribeStandardsControlsRequestRequestTypeDef,
 ):
     pass
 
-
 StandardsControlTypeDef = TypedDict(
     "StandardsControlTypeDef",
     {
         "StandardsControlArn": str,
         "ControlStatus": ControlStatusType,
         "DisabledReason": str,
         "ControlStatusUpdatedAt": datetime,
@@ -3623,30 +4520,27 @@
         "RemediationUrl": str,
         "SeverityRating": SeverityRatingType,
         "RelatedRequirements": List[str],
     },
     total=False,
 )
 
-DescribeStandardsRequestRequestTypeDef = TypedDict(
-    "DescribeStandardsRequestRequestTypeDef",
+DescribeStandardsRequestDescribeStandardsPaginateTypeDef = TypedDict(
+    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-StandardTypeDef = TypedDict(
-    "StandardTypeDef",
+DescribeStandardsRequestRequestTypeDef = TypedDict(
+    "DescribeStandardsRequestRequestTypeDef",
     {
-        "StandardsArn": str,
-        "Name": str,
-        "Description": str,
-        "EnabledByDefault": bool,
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
 DisableImportFindingsForProductRequestRequestTypeDef = TypedDict(
     "DisableImportFindingsForProductRequestRequestTypeDef",
     {
@@ -3671,26 +4565,35 @@
 EnableImportFindingsForProductRequestRequestTypeDef = TypedDict(
     "EnableImportFindingsForProductRequestRequestTypeDef",
     {
         "ProductArn": str,
     },
 )
 
+EnableImportFindingsForProductResponseTypeDef = TypedDict(
+    "EnableImportFindingsForProductResponseTypeDef",
+    {
+        "ProductSubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnableOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     {
         "AdminAccountId": str,
     },
 )
 
 EnableSecurityHubRequestRequestTypeDef = TypedDict(
     "EnableSecurityHubRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
         "EnableDefaultStandards": bool,
+        "ControlFindingGenerator": ControlFindingGeneratorType,
     },
     total=False,
 )
 
 FilePathsTypeDef = TypedDict(
     "FilePathsTypeDef",
     {
@@ -3706,14 +4609,33 @@
     "FindingAggregatorTypeDef",
     {
         "FindingAggregatorArn": str,
     },
     total=False,
 )
 
+FindingHistoryUpdateSourceTypeDef = TypedDict(
+    "FindingHistoryUpdateSourceTypeDef",
+    {
+        "Type": FindingHistoryUpdateSourceTypeType,
+        "Identity": str,
+    },
+    total=False,
+)
+
+FindingHistoryUpdateTypeDef = TypedDict(
+    "FindingHistoryUpdateTypeDef",
+    {
+        "UpdatedField": str,
+        "OldValue": str,
+        "NewValue": str,
+    },
+    total=False,
+)
+
 FindingProviderSeverityTypeDef = TypedDict(
     "FindingProviderSeverityTypeDef",
     {
         "Label": SeverityLabelType,
         "Original": str,
     },
     total=False,
@@ -3743,14 +4665,23 @@
         "InvitationId": str,
         "InvitedAt": datetime,
         "MemberStatus": str,
     },
     total=False,
 )
 
+GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef = TypedDict(
+    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
+    {
+        "StandardsSubscriptionArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetEnabledStandardsRequestRequestTypeDef = TypedDict(
     "GetEnabledStandardsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -3760,14 +4691,25 @@
 GetFindingAggregatorRequestRequestTypeDef = TypedDict(
     "GetFindingAggregatorRequestRequestTypeDef",
     {
         "FindingAggregatorArn": str,
     },
 )
 
+GetFindingAggregatorResponseTypeDef = TypedDict(
+    "GetFindingAggregatorResponseTypeDef",
+    {
+        "FindingAggregatorArn": str,
+        "FindingAggregationRegion": str,
+        "RegionLinkingMode": str,
+        "Regions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SortCriterionTypeDef = TypedDict(
     "SortCriterionTypeDef",
     {
         "Field": str,
         "SortOrder": SortOrderType,
     },
     total=False,
@@ -3776,24 +4718,41 @@
 GetInsightResultsRequestRequestTypeDef = TypedDict(
     "GetInsightResultsRequestRequestTypeDef",
     {
         "InsightArn": str,
     },
 )
 
+GetInsightsRequestGetInsightsPaginateTypeDef = TypedDict(
+    "GetInsightsRequestGetInsightsPaginateTypeDef",
+    {
+        "InsightArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetInsightsRequestRequestTypeDef = TypedDict(
     "GetInsightsRequestRequestTypeDef",
     {
         "InsightArns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "InvitationsCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMembersRequestRequestTypeDef = TypedDict(
     "GetMembersRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
@@ -3822,67 +4781,233 @@
 InviteMembersRequestRequestTypeDef = TypedDict(
     "InviteMembersRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
+ListAutomationRulesRequestRequestTypeDef = TypedDict(
+    "ListAutomationRulesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef = TypedDict(
+    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEnabledProductsForImportRequestRequestTypeDef = TypedDict(
     "ListEnabledProductsForImportRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListEnabledProductsForImportResponseTypeDef = TypedDict(
+    "ListEnabledProductsForImportResponseTypeDef",
+    {
+        "ProductSubscriptions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef = TypedDict(
+    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFindingAggregatorsRequestRequestTypeDef = TypedDict(
     "ListFindingAggregatorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
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
 
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "OnlyAssociated": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMembersRequestRequestTypeDef = TypedDict(
     "ListMembersRequestRequestTypeDef",
     {
         "OnlyAssociated": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
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
 )
 
+ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef = TypedDict(
+    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
+    {
+        "StandardsArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListSecurityControlDefinitionsRequestRequestTypeDef = TypedDict(
+    "ListSecurityControlDefinitionsRequestRequestTypeDef",
+    {
+        "StandardsArn": str,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+SecurityControlDefinitionTypeDef = TypedDict(
+    "SecurityControlDefinitionTypeDef",
+    {
+        "SecurityControlId": str,
+        "Title": str,
+        "Description": str,
+        "RemediationUrl": str,
+        "SeverityRating": SeverityRatingType,
+        "CurrentRegionAvailability": RegionAvailabilityStatusType,
+    },
+)
+
+_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
+    {
+        "SecurityControlId": str,
+    },
+)
+_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef(
+    _RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
+    _OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
+):
+    pass
+
+_RequiredListStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
+    "_RequiredListStandardsControlAssociationsRequestRequestTypeDef",
+    {
+        "SecurityControlId": str,
+    },
+)
+_OptionalListStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
+    "_OptionalListStandardsControlAssociationsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListStandardsControlAssociationsRequestRequestTypeDef(
+    _RequiredListStandardsControlAssociationsRequestRequestTypeDef,
+    _OptionalListStandardsControlAssociationsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStandardsControlAssociationSummaryTypeDef = TypedDict(
+    "_RequiredStandardsControlAssociationSummaryTypeDef",
+    {
+        "StandardsArn": str,
+        "SecurityControlId": str,
+        "SecurityControlArn": str,
+        "AssociationStatus": AssociationStatusType,
+    },
+)
+_OptionalStandardsControlAssociationSummaryTypeDef = TypedDict(
+    "_OptionalStandardsControlAssociationSummaryTypeDef",
+    {
+        "RelatedRequirements": List[str],
+        "UpdatedAt": datetime,
+        "UpdatedReason": str,
+        "StandardsControlTitle": str,
+        "StandardsControlDescription": str,
+    },
+    total=False,
+)
+
+class StandardsControlAssociationSummaryTypeDef(
+    _RequiredStandardsControlAssociationSummaryTypeDef,
+    _OptionalStandardsControlAssociationSummaryTypeDef,
+):
+    pass
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
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "Begin": int,
         "End": int,
     },
     total=False,
@@ -3903,23 +5028,44 @@
     {
         "JsonPath": str,
         "RecordIndex": int,
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
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Text": str,
         "Url": str,
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
 RuleGroupSourceListDetailsTypeDef = TypedDict(
     "RuleGroupSourceListDetailsTypeDef",
     {
         "GeneratedRulesType": str,
         "TargetTypes": Sequence[str],
         "Targets": Sequence[str],
     },
@@ -4015,14 +5161,25 @@
         "Epoch": str,
         "Release": str,
         "Architecture": str,
         "PackageManager": str,
         "FilePath": str,
         "FixedInVersion": str,
         "Remediation": str,
+        "SourceLayerHash": str,
+        "SourceLayerArn": str,
+    },
+    total=False,
+)
+
+StandardsManagedByTypeDef = TypedDict(
+    "StandardsManagedByTypeDef",
+    {
+        "Company": str,
+        "Product": str,
     },
     total=False,
 )
 
 StandardsStatusReasonTypeDef = TypedDict(
     "StandardsStatusReasonTypeDef",
     {
@@ -4065,22 +5222,20 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateActionTargetRequestRequestTypeDef(
     _RequiredUpdateActionTargetRequestRequestTypeDef,
     _OptionalUpdateActionTargetRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateFindingAggregatorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFindingAggregatorRequestRequestTypeDef",
     {
         "FindingAggregatorArn": str,
         "RegionLinkingMode": str,
     },
 )
@@ -4088,21 +5243,30 @@
     "_OptionalUpdateFindingAggregatorRequestRequestTypeDef",
     {
         "Regions": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateFindingAggregatorRequestRequestTypeDef(
     _RequiredUpdateFindingAggregatorRequestRequestTypeDef,
     _OptionalUpdateFindingAggregatorRequestRequestTypeDef,
 ):
     pass
 
+UpdateFindingAggregatorResponseTypeDef = TypedDict(
+    "UpdateFindingAggregatorResponseTypeDef",
+    {
+        "FindingAggregatorArn": str,
+        "FindingAggregationRegion": str,
+        "RegionLinkingMode": str,
+        "Regions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "AutoEnable": bool,
     },
 )
@@ -4110,26 +5274,25 @@
     "_OptionalUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "AutoEnableStandards": AutoEnableStandardsType,
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
 UpdateSecurityHubConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateSecurityHubConfigurationRequestRequestTypeDef",
     {
         "AutoEnableControls": bool,
+        "ControlFindingGenerator": ControlFindingGeneratorType,
     },
     total=False,
 )
 
 _RequiredUpdateStandardsControlRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStandardsControlRequestRequestTypeDef",
     {
@@ -4141,22 +5304,20 @@
     {
         "ControlStatus": ControlStatusType,
         "DisabledReason": str,
     },
     total=False,
 )
 
-
 class UpdateStandardsControlRequestRequestTypeDef(
     _RequiredUpdateStandardsControlRequestRequestTypeDef,
     _OptionalUpdateStandardsControlRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredVulnerabilityVendorTypeDef = TypedDict(
     "_RequiredVulnerabilityVendorTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalVulnerabilityVendorTypeDef = TypedDict(
@@ -4166,21 +5327,19 @@
         "VendorSeverity": str,
         "VendorCreatedAt": str,
         "VendorUpdatedAt": str,
     },
     total=False,
 )
 
-
 class VulnerabilityVendorTypeDef(
     _RequiredVulnerabilityVendorTypeDef, _OptionalVulnerabilityVendorTypeDef
 ):
     pass
 
-
 CreateMembersRequestRequestTypeDef = TypedDict(
     "CreateMembersRequestRequestTypeDef",
     {
         "AccountDetails": Sequence[AccountDetailsTypeDef],
     },
 )
 
@@ -4192,26 +5351,94 @@
         "Country": CountryTypeDef,
         "City": CityTypeDef,
         "GeoLocation": GeoLocationTypeDef,
     },
     total=False,
 )
 
+DescribeActionTargetsResponseTypeDef = TypedDict(
+    "DescribeActionTargetsResponseTypeDef",
+    {
+        "ActionTargets": List[ActionTargetTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CvssTypeDef = TypedDict(
     "CvssTypeDef",
     {
         "Version": str,
         "BaseScore": float,
         "BaseVector": str,
         "Source": str,
         "Adjustments": Sequence[AdjustmentTypeDef],
     },
     total=False,
 )
 
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AssociationSetDetailsTypeDef = TypedDict(
+    "AssociationSetDetailsTypeDef",
+    {
+        "AssociationState": AssociationStateDetailsTypeDef,
+        "GatewayId": str,
+        "Main": bool,
+        "RouteTableAssociationId": str,
+        "RouteTableId": str,
+        "SubnetId": str,
+    },
+    total=False,
+)
+
+AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
+    "AutomationRulesFindingFieldsUpdateTypeDef",
+    {
+        "Note": NoteUpdateTypeDef,
+        "Severity": SeverityUpdateTypeDef,
+        "VerificationState": VerificationStateType,
+        "Confidence": int,
+        "Criticality": int,
+        "Types": List[str],
+        "UserDefinedFields": Dict[str, str],
+        "Workflow": WorkflowUpdateTypeDef,
+        "RelatedFindings": List[RelatedFindingTypeDef],
+    },
+    total=False,
+)
+
+ListAutomationRulesResponseTypeDef = TypedDict(
+    "ListAutomationRulesResponseTypeDef",
+    {
+        "AutomationRulesMetadata": List[AutomationRulesMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AwsAmazonMqBrokerLogsDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLogsDetailsTypeDef",
+    {
+        "Audit": bool,
+        "General": bool,
+        "AuditLogGroup": str,
+        "GeneralLogGroup": str,
+        "Pending": AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsApiGatewayRestApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayRestApiDetailsTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "CreatedDate": str,
@@ -4280,14 +5507,25 @@
         "AutoDeploy": bool,
         "LastDeploymentStatusMessage": str,
         "ApiGatewayManaged": bool,
     },
     total=False,
 )
 
+AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
+    {
+        "AuthenticationType": str,
+        "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
+        "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
+        "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
     {
         "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
         ],
@@ -4517,14 +5755,118 @@
         "IamInstanceProfileArn": str,
         "VpcId": str,
         "SubnetId": str,
         "LaunchedAt": str,
         "NetworkInterfaces": Sequence[AwsEc2InstanceNetworkInterfacesDetailsTypeDef],
         "VirtualizationType": str,
         "MetadataOptions": AwsEc2InstanceMetadataOptionsTypeDef,
+        "Monitoring": AwsEc2InstanceMonitoringDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
+    {
+        "DeviceName": str,
+        "Ebs": AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
+        "NoDevice": str,
+        "VirtualName": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
+    {
+        "CapacityReservationPreference": str,
+        "CapacityReservationTarget": AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
+    {
+        "MarketType": str,
+        "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
+    {
+        "AcceleratorCount": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
+        ),
+        "AcceleratorManufacturers": Sequence[str],
+        "AcceleratorNames": Sequence[str],
+        "AcceleratorTotalMemoryMiB": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef
+        ),
+        "AcceleratorTypes": Sequence[str],
+        "BareMetal": str,
+        "BaselineEbsBandwidthMbps": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef
+        ),
+        "BurstablePerformance": str,
+        "CpuManufacturers": Sequence[str],
+        "ExcludedInstanceTypes": Sequence[str],
+        "InstanceGenerations": Sequence[str],
+        "LocalStorage": str,
+        "LocalStorageTypes": Sequence[str],
+        "MemoryGiBPerVCpu": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef
+        ),
+        "MemoryMiB": AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
+        "NetworkInterfaceCount": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef
+        ),
+        "OnDemandMaxPricePercentageOverLowestPrice": int,
+        "RequireHibernateSupport": bool,
+        "SpotMaxPricePercentageOverLowestPrice": int,
+        "TotalLocalStorageGB": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
+        ),
+        "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
+    {
+        "AssociateCarrierIpAddress": bool,
+        "AssociatePublicIpAddress": bool,
+        "DeleteOnTermination": bool,
+        "Description": str,
+        "DeviceIndex": int,
+        "Groups": Sequence[str],
+        "InterfaceType": str,
+        "Ipv4PrefixCount": int,
+        "Ipv4Prefixes": Sequence[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef
+        ],
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": Sequence[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef
+        ],
+        "Ipv6PrefixCount": int,
+        "Ipv6Prefixes": Sequence[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef
+        ],
+        "NetworkCardIndex": int,
+        "NetworkInterfaceId": str,
+        "PrivateIpAddress": str,
+        "PrivateIpAddresses": Sequence[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef
+        ],
+        "SecondaryPrivateIpAddressCount": int,
+        "SubnetId": str,
     },
     total=False,
 )
 
 AwsEc2NetworkAclEntryTypeDef = TypedDict(
     "AwsEc2NetworkAclEntryTypeDef",
     {
@@ -4672,15 +6014,17 @@
     total=False,
 )
 
 AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
     {
         "KmsKeyId": str,
-        "LogConfiguration": AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef,
+        "LogConfiguration": (
+            AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef
+        ),
         "Logging": str,
     },
     total=False,
 )
 
 AwsEcsContainerDetailsTypeDef = TypedDict(
     "AwsEcsContainerDetailsTypeDef",
@@ -4692,15 +6036,17 @@
     },
     total=False,
 )
 
 AwsEcsServiceDeploymentConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
     {
-        "DeploymentCircuitBreaker": AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef,
+        "DeploymentCircuitBreaker": (
+            AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef
+        ),
         "MaximumPercent": int,
         "MinimumHealthyPercent": int,
     },
     total=False,
 )
 
 AwsEcsServiceNetworkConfigurationDetailsTypeDef = TypedDict(
@@ -4710,15 +6056,17 @@
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
     {
-        "Capabilities": AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef,
+        "Capabilities": (
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef
+        ),
         "Devices": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef
         ],
         "InitProcessEnabled": bool,
         "MaxSwap": int,
         "SharedMemorySize": int,
         "Swappiness": int,
@@ -4752,15 +6100,17 @@
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
     {
-        "AuthorizationConfig": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef,
+        "AuthorizationConfig": (
+            AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef
+        ),
         "FilesystemId": str,
         "RootDirectory": str,
         "TransitEncryption": str,
         "TransitEncryptionPort": int,
     },
     total=False,
 )
@@ -4818,15 +6168,17 @@
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     {
         "DedicatedMasterCount": int,
         "DedicatedMasterEnabled": bool,
         "DedicatedMasterType": str,
         "InstanceCount": int,
         "InstanceType": str,
-        "ZoneAwarenessConfig": AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef,
+        "ZoneAwarenessConfig": (
+            AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef
+        ),
         "ZoneAwarenessEnabled": bool,
     },
     total=False,
 )
 
 AwsElasticsearchDomainLogPublishingOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
@@ -4883,14 +6235,30 @@
         "Type": str,
         "VpcId": str,
         "LoadBalancerAttributes": Sequence[AwsElbv2LoadBalancerAttributeTypeDef],
     },
     total=False,
 )
 
+AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
+    {
+        "AuditLogs": AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
+    {
+        "EbsVolumes": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsIamAccessKeySessionContextTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextTypeDef",
     {
         "Attributes": AwsIamAccessKeySessionContextAttributesTypeDef,
         "SessionIssuer": AwsIamAccessKeySessionContextSessionIssuerTypeDef,
     },
     total=False,
@@ -5006,15 +6374,17 @@
 AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
     {
         "InstanceCount": int,
         "WarmEnabled": bool,
         "WarmCount": int,
         "DedicatedMasterEnabled": bool,
-        "ZoneAwarenessConfig": AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef,
+        "ZoneAwarenessConfig": (
+            AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef
+        ),
         "DedicatedMasterCount": int,
         "InstanceType": str,
         "WarmType": str,
         "ZoneAwarenessEnabled": bool,
         "DedicatedMasterType": str,
     },
     total=False,
@@ -5178,14 +6548,22 @@
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     {
         "FilterRules": Sequence[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef],
     },
     total=False,
 )
 
+AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef = TypedDict(
+    "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
+    {
+        "DefaultRetention": AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsS3BucketServerSideEncryptionRuleTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": AwsS3BucketServerSideEncryptionByDefaultTypeDef,
     },
     total=False,
 )
@@ -5195,14 +6573,43 @@
     {
         "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
         "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     },
     total=False,
 )
 
+AwsSageMakerNotebookInstanceDetailsTypeDef = TypedDict(
+    "AwsSageMakerNotebookInstanceDetailsTypeDef",
+    {
+        "AcceleratorTypes": Sequence[str],
+        "AdditionalCodeRepositories": Sequence[str],
+        "DefaultCodeRepository": str,
+        "DirectInternetAccess": str,
+        "FailureReason": str,
+        "InstanceMetadataServiceConfiguration": (
+            AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef
+        ),
+        "InstanceType": str,
+        "KmsKeyId": str,
+        "NetworkInterfaceId": str,
+        "NotebookInstanceArn": str,
+        "NotebookInstanceLifecycleConfigName": str,
+        "NotebookInstanceName": str,
+        "NotebookInstanceStatus": str,
+        "PlatformIdentifier": str,
+        "RoleArn": str,
+        "RootAccess": str,
+        "SecurityGroups": Sequence[str],
+        "SubnetId": str,
+        "Url": str,
+        "VolumeSizeInGB": int,
+    },
+    total=False,
+)
+
 AwsSecretsManagerSecretDetailsTypeDef = TypedDict(
     "AwsSecretsManagerSecretDetailsTypeDef",
     {
         "RotationRules": AwsSecretsManagerSecretRotationRulesTypeDef,
         "RotationOccurredWithinFrequency": bool,
         "KmsKeyId": str,
         "RotationEnabled": bool,
@@ -5210,23 +6617,95 @@
         "Deleted": bool,
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+_RequiredBatchUpdateFindingsRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchUpdateFindingsRequestRequestTypeDef",
+    {
+        "FindingIdentifiers": Sequence[AwsSecurityFindingIdentifierTypeDef],
+    },
+)
+_OptionalBatchUpdateFindingsRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchUpdateFindingsRequestRequestTypeDef",
+    {
+        "Note": NoteUpdateTypeDef,
+        "Severity": SeverityUpdateTypeDef,
+        "VerificationState": VerificationStateType,
+        "Confidence": int,
+        "Criticality": int,
+        "Types": Sequence[str],
+        "UserDefinedFields": Mapping[str, str],
+        "Workflow": WorkflowUpdateTypeDef,
+        "RelatedFindings": Sequence[RelatedFindingTypeDef],
+    },
+    total=False,
+)
+
+class BatchUpdateFindingsRequestRequestTypeDef(
+    _RequiredBatchUpdateFindingsRequestRequestTypeDef,
+    _OptionalBatchUpdateFindingsRequestRequestTypeDef,
+):
+    pass
+
 BatchUpdateFindingsUnprocessedFindingTypeDef = TypedDict(
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
+_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+    },
+)
+_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef(
+    _RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    _OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+):
+    pass
+
+_RequiredGetFindingHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetFindingHistoryRequestRequestTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+    },
+)
+_OptionalGetFindingHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetFindingHistoryRequestRequestTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class GetFindingHistoryRequestRequestTypeDef(
+    _RequiredGetFindingHistoryRequestRequestTypeDef, _OptionalGetFindingHistoryRequestRequestTypeDef
+):
+    pass
+
 AwsSnsTopicDetailsTypeDef = TypedDict(
     "AwsSnsTopicDetailsTypeDef",
     {
         "KmsMasterKeyId": str,
         "Subscription": Sequence[AwsSnsTopicSubscriptionTypeDef],
         "TopicName": str,
         "Owner": str,
@@ -5245,14 +6724,22 @@
     "AwsSsmPatchTypeDef",
     {
         "ComplianceSummary": AwsSsmComplianceSummaryTypeDef,
     },
     total=False,
 )
 
+AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
+    {
+        "CloudWatchLogsLogGroup": AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsWafRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRateBasedRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
@@ -5340,203 +6827,148 @@
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
-CreateActionTargetResponseTypeDef = TypedDict(
-    "CreateActionTargetResponseTypeDef",
-    {
-        "ActionTargetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFindingAggregatorResponseTypeDef = TypedDict(
-    "CreateFindingAggregatorResponseTypeDef",
-    {
-        "FindingAggregatorArn": str,
-        "FindingAggregationRegion": str,
-        "RegionLinkingMode": str,
-        "Regions": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateInsightResponseTypeDef = TypedDict(
-    "CreateInsightResponseTypeDef",
-    {
-        "InsightArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteActionTargetResponseTypeDef = TypedDict(
-    "DeleteActionTargetResponseTypeDef",
-    {
-        "ActionTargetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteInsightResponseTypeDef = TypedDict(
-    "DeleteInsightResponseTypeDef",
+AwsWafv2CustomRequestHandlingDetailsTypeDef = TypedDict(
+    "AwsWafv2CustomRequestHandlingDetailsTypeDef",
     {
-        "InsightArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "InsertHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
+    total=False,
 )
 
-DescribeActionTargetsResponseTypeDef = TypedDict(
-    "DescribeActionTargetsResponseTypeDef",
+AwsWafv2CustomResponseDetailsTypeDef = TypedDict(
+    "AwsWafv2CustomResponseDetailsTypeDef",
     {
-        "ActionTargets": List[ActionTargetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CustomResponseBodyKey": str,
+        "ResponseCode": int,
+        "ResponseHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
+    total=False,
 )
 
-DescribeHubResponseTypeDef = TypedDict(
-    "DescribeHubResponseTypeDef",
+AwsWafv2WebAclCaptchaConfigDetailsTypeDef = TypedDict(
+    "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     {
-        "HubArn": str,
-        "SubscribedAt": str,
-        "AutoEnableControls": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ImmunityTimeProperty": AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     },
+    total=False,
 )
 
-DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
-    "DescribeOrganizationConfigurationResponseTypeDef",
+BatchDeleteAutomationRulesResponseTypeDef = TypedDict(
+    "BatchDeleteAutomationRulesResponseTypeDef",
     {
-        "AutoEnable": bool,
-        "MemberAccountLimitReached": bool,
-        "AutoEnableStandards": AutoEnableStandardsType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProcessedAutomationRules": List[str],
+        "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EnableImportFindingsForProductResponseTypeDef = TypedDict(
-    "EnableImportFindingsForProductResponseTypeDef",
+BatchUpdateAutomationRulesResponseTypeDef = TypedDict(
+    "BatchUpdateAutomationRulesResponseTypeDef",
     {
-        "ProductSubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProcessedAutomationRules": List[str],
+        "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetFindingAggregatorResponseTypeDef = TypedDict(
-    "GetFindingAggregatorResponseTypeDef",
+BatchEnableStandardsRequestRequestTypeDef = TypedDict(
+    "BatchEnableStandardsRequestRequestTypeDef",
     {
-        "FindingAggregatorArn": str,
-        "FindingAggregationRegion": str,
-        "RegionLinkingMode": str,
-        "Regions": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StandardsSubscriptionRequests": Sequence[StandardsSubscriptionRequestTypeDef],
     },
 )
 
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
+BatchGetSecurityControlsResponseTypeDef = TypedDict(
+    "BatchGetSecurityControlsResponseTypeDef",
     {
-        "InvitationsCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SecurityControls": List[SecurityControlTypeDef],
+        "UnprocessedIds": List[UnprocessedSecurityControlTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnabledProductsForImportResponseTypeDef = TypedDict(
-    "ListEnabledProductsForImportResponseTypeDef",
+BatchGetStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
+    "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
     {
-        "ProductSubscriptions": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StandardsControlAssociationIds": Sequence[StandardsControlAssociationIdTypeDef],
     },
 )
 
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
+_RequiredUnprocessedStandardsControlAssociationTypeDef = TypedDict(
+    "_RequiredUnprocessedStandardsControlAssociationTypeDef",
     {
-        "AdminAccounts": List[AdminAccountTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StandardsControlAssociationId": StandardsControlAssociationIdTypeDef,
+        "ErrorCode": UnprocessedErrorCodeType,
     },
 )
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_OptionalUnprocessedStandardsControlAssociationTypeDef = TypedDict(
+    "_OptionalUnprocessedStandardsControlAssociationTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFindingAggregatorResponseTypeDef = TypedDict(
-    "UpdateFindingAggregatorResponseTypeDef",
-    {
-        "FindingAggregatorArn": str,
-        "FindingAggregationRegion": str,
-        "RegionLinkingMode": str,
-        "Regions": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ErrorReason": str,
     },
+    total=False,
 )
 
-BatchEnableStandardsRequestRequestTypeDef = TypedDict(
-    "BatchEnableStandardsRequestRequestTypeDef",
-    {
-        "StandardsSubscriptionRequests": Sequence[StandardsSubscriptionRequestTypeDef],
-    },
-)
+class UnprocessedStandardsControlAssociationTypeDef(
+    _RequiredUnprocessedStandardsControlAssociationTypeDef,
+    _OptionalUnprocessedStandardsControlAssociationTypeDef,
+):
+    pass
 
 BatchImportFindingsResponseTypeDef = TypedDict(
     "BatchImportFindingsResponseTypeDef",
     {
         "FailedCount": int,
         "SuccessCount": int,
         "FailedFindings": List[ImportFindingsErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredBatchUpdateFindingsRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchUpdateFindingsRequestRequestTypeDef",
+BatchUpdateStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
+    "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
     {
-        "FindingIdentifiers": Sequence[AwsSecurityFindingIdentifierTypeDef],
+        "StandardsControlAssociationUpdates": Sequence[StandardsControlAssociationUpdateTypeDef],
     },
 )
-_OptionalBatchUpdateFindingsRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchUpdateFindingsRequestRequestTypeDef",
+
+_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef",
     {
-        "Note": NoteUpdateTypeDef,
-        "Severity": SeverityUpdateTypeDef,
-        "VerificationState": VerificationStateType,
-        "Confidence": int,
-        "Criticality": int,
-        "Types": Sequence[str],
-        "UserDefinedFields": Mapping[str, str],
-        "Workflow": WorkflowUpdateTypeDef,
-        "RelatedFindings": Sequence[RelatedFindingTypeDef],
+        "StandardsControlAssociationUpdate": StandardsControlAssociationUpdateTypeDef,
+        "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef",
+    {
+        "ErrorReason": str,
     },
     total=False,
 )
 
-
-class BatchUpdateFindingsRequestRequestTypeDef(
-    _RequiredBatchUpdateFindingsRequestRequestTypeDef,
-    _OptionalBatchUpdateFindingsRequestRequestTypeDef,
+class UnprocessedStandardsControlAssociationUpdateTypeDef(
+    _RequiredUnprocessedStandardsControlAssociationUpdateTypeDef,
+    _OptionalUnprocessedStandardsControlAssociationUpdateTypeDef,
 ):
     pass
 
-
 ComplianceTypeDef = TypedDict(
     "ComplianceTypeDef",
     {
         "Status": ComplianceStatusType,
         "RelatedRequirements": Sequence[str],
         "StatusReasons": Sequence[StatusReasonTypeDef],
+        "SecurityControlId": str,
+        "AssociatedStandards": Sequence[AssociatedStandardTypeDef],
     },
     total=False,
 )
 
 ContainerDetailsTypeDef = TypedDict(
     "ContainerDetailsTypeDef",
     {
@@ -5551,191 +6983,75 @@
     total=False,
 )
 
 CreateMembersResponseTypeDef = TypedDict(
     "CreateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteMembersResponseTypeDef = TypedDict(
     "DeleteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InviteMembersResponseTypeDef = TypedDict(
     "InviteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DateFilterTypeDef = TypedDict(
     "DateFilterTypeDef",
     {
         "Start": str,
         "End": str,
         "DateRange": DateRangeTypeDef,
     },
     total=False,
 )
 
-DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef = TypedDict(
-    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
-    {
-        "ActionTargetArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeProductsRequestDescribeProductsPaginateTypeDef = TypedDict(
-    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
-    {
-        "ProductArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
-    {
-        "StandardsSubscriptionArn": str,
-    },
-)
-_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef(
-    _RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
-    _OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
-):
-    pass
-
-
-DescribeStandardsRequestDescribeStandardsPaginateTypeDef = TypedDict(
-    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef = TypedDict(
-    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
-    {
-        "StandardsSubscriptionArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetInsightsRequestGetInsightsPaginateTypeDef = TypedDict(
-    "GetInsightsRequestGetInsightsPaginateTypeDef",
-    {
-        "InsightArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef = TypedDict(
-    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef = TypedDict(
-    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "OnlyAssociated": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeProductsResponseTypeDef = TypedDict(
     "DescribeProductsResponseTypeDef",
     {
         "Products": List[ProductTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStandardsControlsResponseTypeDef = TypedDict(
     "DescribeStandardsControlsResponseTypeDef",
     {
         "Controls": List[StandardsControlTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeStandardsResponseTypeDef = TypedDict(
-    "DescribeStandardsResponseTypeDef",
-    {
-        "Standards": List[StandardTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ThreatTypeDef = TypedDict(
     "ThreatTypeDef",
     {
         "Name": str,
@@ -5747,16 +7063,29 @@
 )
 
 ListFindingAggregatorsResponseTypeDef = TypedDict(
     "ListFindingAggregatorsResponseTypeDef",
     {
         "FindingAggregators": List[FindingAggregatorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FindingHistoryRecordTypeDef = TypedDict(
+    "FindingHistoryRecordTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+        "UpdateTime": datetime,
+        "FindingCreated": bool,
+        "UpdateSource": FindingHistoryUpdateSourceTypeDef,
+        "Updates": List[FindingHistoryUpdateTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
 FindingProviderFieldsTypeDef = TypedDict(
     "FindingProviderFieldsTypeDef",
     {
         "Confidence": int,
         "Criticality": int,
@@ -5767,62 +7096,80 @@
     total=False,
 )
 
 GetAdministratorAccountResponseTypeDef = TypedDict(
     "GetAdministratorAccountResponseTypeDef",
     {
         "Administrator": InvitationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "Master": InvitationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
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
 
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "UnprocessedAccounts": List[ResultTypeDef],
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
 
 InsightResultsTypeDef = TypedDict(
     "InsightResultsTypeDef",
     {
         "InsightArn": str,
         "GroupByAttribute": str,
         "ResultValues": List[InsightResultValueTypeDef],
     },
 )
 
+ListSecurityControlDefinitionsResponseTypeDef = TypedDict(
+    "ListSecurityControlDefinitionsResponseTypeDef",
+    {
+        "SecurityControlDefinitions": List[SecurityControlDefinitionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStandardsControlAssociationsResponseTypeDef = TypedDict(
+    "ListStandardsControlAssociationsResponseTypeDef",
+    {
+        "StandardsControlAssociationSummaries": List[StandardsControlAssociationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NetworkPathComponentDetailsTypeDef = TypedDict(
     "NetworkPathComponentDetailsTypeDef",
     {
         "Address": Sequence[str],
         "PortRanges": Sequence[PortRangeTypeDef],
     },
     total=False,
@@ -5895,14 +7242,26 @@
     {
         "IpSets": RuleGroupVariablesIpSetsDetailsTypeDef,
         "PortSets": RuleGroupVariablesPortSetsDetailsTypeDef,
     },
     total=False,
 )
 
+StandardTypeDef = TypedDict(
+    "StandardTypeDef",
+    {
+        "StandardsArn": str,
+        "Name": str,
+        "Description": str,
+        "EnabledByDefault": bool,
+        "StandardsManagedBy": StandardsManagedByTypeDef,
+    },
+    total=False,
+)
+
 _RequiredStandardsSubscriptionTypeDef = TypedDict(
     "_RequiredStandardsSubscriptionTypeDef",
     {
         "StandardsSubscriptionArn": str,
         "StandardsArn": str,
         "StandardsInput": Dict[str, str],
         "StandardsStatus": StandardsStatusType,
@@ -5912,21 +7271,19 @@
     "_OptionalStandardsSubscriptionTypeDef",
     {
         "StandardsStatusReason": StandardsStatusReasonTypeDef,
     },
     total=False,
 )
 
-
 class StandardsSubscriptionTypeDef(
     _RequiredStandardsSubscriptionTypeDef, _OptionalStandardsSubscriptionTypeDef
 ):
     pass
 
-
 StatelessCustomPublishMetricActionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[StatelessCustomPublishMetricActionDimensionTypeDef],
     },
     total=False,
 )
@@ -5984,24 +7341,94 @@
         "Vendor": VulnerabilityVendorTypeDef,
         "ReferenceUrls": Sequence[str],
         "FixAvailable": VulnerabilityFixAvailableType,
     },
     total=False,
 )
 
-
 class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
     pass
 
+AwsEc2RouteTableDetailsTypeDef = TypedDict(
+    "AwsEc2RouteTableDetailsTypeDef",
+    {
+        "AssociationSet": Sequence[AssociationSetDetailsTypeDef],
+        "OwnerId": str,
+        "PropagatingVgwSet": Sequence[PropagatingVgwSetDetailsTypeDef],
+        "RouteTableId": str,
+        "RouteSet": Sequence[RouteSetDetailsTypeDef],
+        "VpcId": str,
+    },
+    total=False,
+)
+
+AutomationRulesActionTypeDef = TypedDict(
+    "AutomationRulesActionTypeDef",
+    {
+        "Type": Literal["FINDING_FIELDS_UPDATE"],
+        "FindingFieldsUpdate": AutomationRulesFindingFieldsUpdateTypeDef,
+    },
+    total=False,
+)
+
+AwsAmazonMqBrokerDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerDetailsTypeDef",
+    {
+        "AuthenticationStrategy": str,
+        "AutoMinorVersionUpgrade": bool,
+        "BrokerArn": str,
+        "BrokerName": str,
+        "DeploymentMode": str,
+        "EncryptionOptions": AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
+        "EngineType": str,
+        "EngineVersion": str,
+        "HostInstanceType": str,
+        "BrokerId": str,
+        "LdapServerMetadata": AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
+        "Logs": AwsAmazonMqBrokerLogsDetailsTypeDef,
+        "MaintenanceWindowStartTime": AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
+        "PubliclyAccessible": bool,
+        "SecurityGroups": Sequence[str],
+        "StorageType": str,
+        "SubnetIds": Sequence[str],
+        "Users": Sequence[AwsAmazonMqBrokerUsersDetailsTypeDef],
+    },
+    total=False,
+)
+
+AwsAppSyncGraphQlApiDetailsTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiDetailsTypeDef",
+    {
+        "ApiId": str,
+        "Id": str,
+        "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
+        "Name": str,
+        "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
+        "XrayEnabled": bool,
+        "Arn": str,
+        "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
+        "AuthenticationType": str,
+        "LogConfig": AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
+        "AdditionalAuthenticationProviders": Sequence[
+            AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef
+        ],
+        "WafWebAclArn": str,
+    },
+    total=False,
+)
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     {
-        "InstancesDistribution": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
-        "LaunchTemplate": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
+        "InstancesDistribution": (
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
+        ),
+        "LaunchTemplate": (
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef
+        ),
     },
     total=False,
 )
 
 AwsAutoScalingLaunchConfigurationDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     {
@@ -6104,14 +7531,59 @@
         "RegionName": str,
         "ReplicaStatus": str,
         "ReplicaStatusDescription": str,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDataDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataDetailsTypeDef",
+    {
+        "BlockDeviceMappingSet": Sequence[
+            AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef
+        ],
+        "CapacityReservationSpecification": (
+            AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef
+        ),
+        "CpuOptions": AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
+        "CreditSpecification": AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
+        "DisableApiStop": bool,
+        "DisableApiTermination": bool,
+        "EbsOptimized": bool,
+        "ElasticGpuSpecificationSet": Sequence[
+            AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef
+        ],
+        "ElasticInferenceAcceleratorSet": Sequence[
+            AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef
+        ],
+        "EnclaveOptions": AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
+        "HibernationOptions": AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
+        "IamInstanceProfile": AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
+        "ImageId": str,
+        "InstanceInitiatedShutdownBehavior": str,
+        "InstanceMarketOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
+        "InstanceRequirements": AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
+        "InstanceType": str,
+        "KernelId": str,
+        "KeyName": str,
+        "LicenseSet": Sequence[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef],
+        "MaintenanceOptions": AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
+        "MetadataOptions": AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
+        "Monitoring": AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
+        "NetworkInterfaceSet": Sequence[AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef],
+        "Placement": AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
+        "PrivateDnsNameOptions": AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
+        "RamDiskId": str,
+        "SecurityGroupIdSet": Sequence[str],
+        "SecurityGroupSet": Sequence[str],
+        "UserData": str,
+    },
+    total=False,
+)
+
 AwsEc2NetworkAclDetailsTypeDef = TypedDict(
     "AwsEc2NetworkAclDetailsTypeDef",
     {
         "IsDefault": bool,
         "NetworkAclId": str,
         "OwnerId": str,
         "VpcId": str,
@@ -6163,15 +7635,17 @@
     },
     total=False,
 )
 
 AwsEcsClusterConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationDetailsTypeDef",
     {
-        "ExecuteCommandConfiguration": AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef,
+        "ExecuteCommandConfiguration": (
+            AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef
+        ),
     },
     total=False,
 )
 
 AwsEcsServiceDetailsTypeDef = TypedDict(
     "AwsEcsServiceDetailsTypeDef",
     {
@@ -6215,15 +7689,17 @@
         "EntryPoint": Sequence[str],
         "Environment": Sequence[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef],
         "EnvironmentFiles": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef
         ],
         "Essential": bool,
         "ExtraHosts": Sequence[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef],
-        "FirelensConfiguration": AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
+        "FirelensConfiguration": (
+            AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef
+        ),
         "HealthCheck": AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
         "Hostname": str,
         "Image": str,
         "Interactive": bool,
         "Links": Sequence[str],
         "LinuxParameters": AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef,
         "LogConfiguration": AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef,
@@ -6233,15 +7709,17 @@
         "Name": str,
         "PortMappings": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef
         ],
         "Privileged": bool,
         "PseudoTerminal": bool,
         "ReadonlyRootFilesystem": bool,
-        "RepositoryCredentials": AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef,
+        "RepositoryCredentials": (
+            AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef
+        ),
         "ResourceRequirements": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef
         ],
         "Secrets": Sequence[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef],
         "StartTimeout": int,
         "StopTimeout": int,
         "SystemControls": Sequence[
@@ -6254,15 +7732,17 @@
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
     {
-        "DockerVolumeConfiguration": AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
+        "DockerVolumeConfiguration": (
+            AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef
+        ),
         "EfsVolumeConfiguration": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
         "Host": AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
         "Name": str,
     },
     total=False,
 )
 
@@ -6317,15 +7797,17 @@
         "AccessPolicies": str,
         "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
         "DomainId": str,
         "DomainName": str,
         "Endpoint": str,
         "Endpoints": Mapping[str, str],
         "ElasticsearchVersion": str,
-        "ElasticsearchClusterConfig": AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
+        "ElasticsearchClusterConfig": (
+            AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef
+        ),
         "EncryptionAtRestOptions": AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
         "LogPublishingOptions": AwsElasticsearchDomainLogPublishingOptionsTypeDef,
         "NodeToNodeEncryptionOptions": AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
         "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
         "VPCOptions": AwsElasticsearchDomainVPCOptionsTypeDef,
     },
     total=False,
@@ -6351,14 +7833,23 @@
         "SourceSecurityGroup": AwsElbLoadBalancerSourceSecurityGroupTypeDef,
         "Subnets": Sequence[str],
         "VpcId": str,
     },
     total=False,
 )
 
+AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
+    {
+        "ScanEc2InstanceWithFindings": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
+        "ServiceRole": str,
+    },
+    total=False,
+)
+
 AwsIamAccessKeyDetailsTypeDef = TypedDict(
     "AwsIamAccessKeyDetailsTypeDef",
     {
         "UserName": str,
         "Status": AwsIamAccessKeyStatusType,
         "CreatedAt": str,
         "PrincipalId": str,
@@ -6405,29 +7896,33 @@
         "RevisionId": str,
         "Role": str,
         "Runtime": str,
         "Timeout": int,
         "TracingConfig": AwsLambdaFunctionTracingConfigTypeDef,
         "VpcConfig": AwsLambdaFunctionVpcConfigTypeDef,
         "Version": str,
+        "Architectures": Sequence[str],
+        "PackageType": str,
     },
     total=False,
 )
 
 AwsOpenSearchServiceDomainDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDetailsTypeDef",
     {
         "Arn": str,
         "AccessPolicies": str,
         "DomainName": str,
         "Id": str,
         "DomainEndpoint": str,
         "EngineVersion": str,
         "EncryptionAtRestOptions": AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
-        "NodeToNodeEncryptionOptions": AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef,
+        "NodeToNodeEncryptionOptions": (
+            AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef
+        ),
         "ServiceSoftwareOptions": AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
         "ClusterConfig": AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
         "DomainEndpointOptions": AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
         "VpcOptions": AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef,
         "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
         "DomainEndpoints": Mapping[str, str],
         "AdvancedSecurityOptions": AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
@@ -6516,14 +8011,23 @@
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     {
         "S3KeyFilter": AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     },
     total=False,
 )
 
+AwsS3BucketObjectLockConfigurationTypeDef = TypedDict(
+    "AwsS3BucketObjectLockConfigurationTypeDef",
+    {
+        "ObjectLockEnabled": str,
+        "Rule": AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsS3BucketServerSideEncryptionConfigurationTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     {
         "Rules": Sequence[AwsS3BucketServerSideEncryptionRuleTypeDef],
     },
     total=False,
 )
@@ -6540,26 +8044,38 @@
 )
 
 BatchUpdateFindingsResponseTypeDef = TypedDict(
     "BatchUpdateFindingsResponseTypeDef",
     {
         "ProcessedFindings": List[AwsSecurityFindingIdentifierTypeDef],
         "UnprocessedFindings": List[BatchUpdateFindingsUnprocessedFindingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AwsSsmPatchComplianceDetailsTypeDef = TypedDict(
     "AwsSsmPatchComplianceDetailsTypeDef",
     {
         "Patch": AwsSsmPatchTypeDef,
     },
     total=False,
 )
 
+AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
+    {
+        "Destinations": Sequence[
+            AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef
+        ],
+        "IncludeExecutionData": bool,
+        "Level": str,
+    },
+    total=False,
+)
+
 AwsWafRegionalRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
         "Rules": Sequence[AwsWafRegionalRuleGroupRulesDetailsTypeDef],
@@ -6597,14 +8113,105 @@
         "DefaultAction": str,
         "Rules": Sequence[AwsWafWebAclRuleTypeDef],
         "WebAclId": str,
     },
     total=False,
 )
 
+AwsWafv2ActionAllowDetailsTypeDef = TypedDict(
+    "AwsWafv2ActionAllowDetailsTypeDef",
+    {
+        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2RulesActionCaptchaDetailsTypeDef = TypedDict(
+    "AwsWafv2RulesActionCaptchaDetailsTypeDef",
+    {
+        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2RulesActionCountDetailsTypeDef = TypedDict(
+    "AwsWafv2RulesActionCountDetailsTypeDef",
+    {
+        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2ActionBlockDetailsTypeDef = TypedDict(
+    "AwsWafv2ActionBlockDetailsTypeDef",
+    {
+        "CustomResponse": AwsWafv2CustomResponseDetailsTypeDef,
+    },
+    total=False,
+)
+
+BatchGetStandardsControlAssociationsResponseTypeDef = TypedDict(
+    "BatchGetStandardsControlAssociationsResponseTypeDef",
+    {
+        "StandardsControlAssociationDetails": List[StandardsControlAssociationDetailTypeDef],
+        "UnprocessedAssociations": List[UnprocessedStandardsControlAssociationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchUpdateStandardsControlAssociationsResponseTypeDef = TypedDict(
+    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
+    {
+        "UnprocessedAssociationUpdates": List[UnprocessedStandardsControlAssociationUpdateTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AutomationRulesFindingFiltersTypeDef = TypedDict(
+    "AutomationRulesFindingFiltersTypeDef",
+    {
+        "ProductArn": List[StringFilterTypeDef],
+        "AwsAccountId": List[StringFilterTypeDef],
+        "Id": List[StringFilterTypeDef],
+        "GeneratorId": List[StringFilterTypeDef],
+        "Type": List[StringFilterTypeDef],
+        "FirstObservedAt": List[DateFilterTypeDef],
+        "LastObservedAt": List[DateFilterTypeDef],
+        "CreatedAt": List[DateFilterTypeDef],
+        "UpdatedAt": List[DateFilterTypeDef],
+        "Confidence": List[NumberFilterTypeDef],
+        "Criticality": List[NumberFilterTypeDef],
+        "Title": List[StringFilterTypeDef],
+        "Description": List[StringFilterTypeDef],
+        "SourceUrl": List[StringFilterTypeDef],
+        "ProductName": List[StringFilterTypeDef],
+        "CompanyName": List[StringFilterTypeDef],
+        "SeverityLabel": List[StringFilterTypeDef],
+        "ResourceType": List[StringFilterTypeDef],
+        "ResourceId": List[StringFilterTypeDef],
+        "ResourcePartition": List[StringFilterTypeDef],
+        "ResourceRegion": List[StringFilterTypeDef],
+        "ResourceTags": List[MapFilterTypeDef],
+        "ResourceDetailsOther": List[MapFilterTypeDef],
+        "ComplianceStatus": List[StringFilterTypeDef],
+        "ComplianceSecurityControlId": List[StringFilterTypeDef],
+        "ComplianceAssociatedStandardsId": List[StringFilterTypeDef],
+        "VerificationState": List[StringFilterTypeDef],
+        "WorkflowStatus": List[StringFilterTypeDef],
+        "RecordState": List[StringFilterTypeDef],
+        "RelatedFindingsProductArn": List[StringFilterTypeDef],
+        "RelatedFindingsId": List[StringFilterTypeDef],
+        "NoteText": List[StringFilterTypeDef],
+        "NoteUpdatedAt": List[DateFilterTypeDef],
+        "NoteUpdatedBy": List[StringFilterTypeDef],
+        "UserDefinedFields": List[MapFilterTypeDef],
+    },
+    total=False,
+)
+
 AwsSecurityFindingFiltersTypeDef = TypedDict(
     "AwsSecurityFindingFiltersTypeDef",
     {
         "ProductArn": Sequence[StringFilterTypeDef],
         "AwsAccountId": Sequence[StringFilterTypeDef],
         "Id": Sequence[StringFilterTypeDef],
         "GeneratorId": Sequence[StringFilterTypeDef],
@@ -6695,23 +8302,34 @@
         "FindingProviderFieldsCriticality": Sequence[NumberFilterTypeDef],
         "FindingProviderFieldsRelatedFindingsId": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsRelatedFindingsProductArn": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsSeverityLabel": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsSeverityOriginal": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsTypes": Sequence[StringFilterTypeDef],
         "Sample": Sequence[BooleanFilterTypeDef],
+        "ComplianceSecurityControlId": Sequence[StringFilterTypeDef],
+        "ComplianceAssociatedStandardsId": Sequence[StringFilterTypeDef],
     },
     total=False,
 )
 
+GetFindingHistoryResponseTypeDef = TypedDict(
+    "GetFindingHistoryResponseTypeDef",
+    {
+        "Records": List[FindingHistoryRecordTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetInsightResultsResponseTypeDef = TypedDict(
     "GetInsightResultsResponseTypeDef",
     {
         "InsightResults": InsightResultsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkHeaderTypeDef = TypedDict(
     "NetworkHeaderTypeDef",
     {
         "Protocol": str,
@@ -6738,36 +8356,45 @@
     {
         "Actions": Sequence[str],
         "MatchAttributes": RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     },
     total=False,
 )
 
+DescribeStandardsResponseTypeDef = TypedDict(
+    "DescribeStandardsResponseTypeDef",
+    {
+        "Standards": List[StandardTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchDisableStandardsResponseTypeDef = TypedDict(
     "BatchDisableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchEnableStandardsResponseTypeDef = TypedDict(
     "BatchEnableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEnabledStandardsResponseTypeDef = TypedDict(
     "GetEnabledStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StatelessCustomActionDefinitionTypeDef = TypedDict(
     "StatelessCustomActionDefinitionTypeDef",
     {
         "PublishMetricAction": StatelessCustomPublishMetricActionTypeDef,
@@ -6792,15 +8419,17 @@
         "HealthCheckType": str,
         "HealthCheckGracePeriod": int,
         "CreatedTime": str,
         "MixedInstancesPolicy": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
         "AvailabilityZones": Sequence[
             AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef
         ],
-        "LaunchTemplate": AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
+        "LaunchTemplate": (
+            AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
+        ),
         "CapacityRebalance": bool,
     },
     total=False,
 )
 
 AwsBackupBackupPlanBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
@@ -6882,14 +8511,26 @@
         "TableName": str,
         "TableSizeBytes": int,
         "TableStatus": str,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDetailsTypeDef",
+    {
+        "LaunchTemplateName": str,
+        "Id": str,
+        "LaunchTemplateData": AwsEc2LaunchTemplateDataDetailsTypeDef,
+        "DefaultVersionNumber": int,
+        "LatestVersionNumber": int,
+    },
+    total=False,
+)
+
 AwsEcsClusterDetailsTypeDef = TypedDict(
     "AwsEcsClusterDetailsTypeDef",
     {
         "ClusterArn": str,
         "ActiveServicesCount": int,
         "CapacityProviders": Sequence[str],
         "ClusterSettings": Sequence[AwsEcsClusterClusterSettingsDetailsTypeDef],
@@ -6922,14 +8563,27 @@
         "RequiresCompatibilities": Sequence[str],
         "TaskRoleArn": str,
         "Volumes": Sequence[AwsEcsTaskDefinitionVolumesDetailsTypeDef],
     },
     total=False,
 )
 
+AwsGuardDutyDetectorDataSourcesDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
+    {
+        "CloudTrail": AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef,
+        "DnsLogs": AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef,
+        "FlowLogs": AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef,
+        "Kubernetes": AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
+        "MalwareProtection": AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
+        "S3Logs": AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsRdsDbInstanceDetailsTypeDef = TypedDict(
     "AwsRdsDbInstanceDetailsTypeDef",
     {
         "AssociatedRoles": Sequence[AwsRdsDbInstanceAssociatedRoleTypeDef],
         "CACertificateIdentifier": str,
         "DBClusterIdentifier": str,
         "DBInstanceIdentifier": str,
@@ -7005,29 +8659,134 @@
         "Filter": AwsS3BucketNotificationConfigurationFilterTypeDef,
         "Destination": str,
         "Type": str,
     },
     total=False,
 )
 
+AwsStepFunctionStateMachineDetailsTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineDetailsTypeDef",
+    {
+        "Label": str,
+        "LoggingConfiguration": AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
+        "Name": str,
+        "RoleArn": str,
+        "StateMachineArn": str,
+        "Status": str,
+        "TracingConfiguration": AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
+        "Type": str,
+    },
+    total=False,
+)
+
+AwsWafv2RulesActionDetailsTypeDef = TypedDict(
+    "AwsWafv2RulesActionDetailsTypeDef",
+    {
+        "Allow": AwsWafv2ActionAllowDetailsTypeDef,
+        "Block": AwsWafv2ActionBlockDetailsTypeDef,
+        "Captcha": AwsWafv2RulesActionCaptchaDetailsTypeDef,
+        "Count": AwsWafv2RulesActionCountDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2WebAclActionDetailsTypeDef = TypedDict(
+    "AwsWafv2WebAclActionDetailsTypeDef",
+    {
+        "Allow": AwsWafv2ActionAllowDetailsTypeDef,
+        "Block": AwsWafv2ActionBlockDetailsTypeDef,
+    },
+    total=False,
+)
+
+AutomationRulesConfigTypeDef = TypedDict(
+    "AutomationRulesConfigTypeDef",
+    {
+        "RuleArn": str,
+        "RuleStatus": RuleStatusType,
+        "RuleOrder": int,
+        "RuleName": str,
+        "Description": str,
+        "IsTerminal": bool,
+        "Criteria": AutomationRulesFindingFiltersTypeDef,
+        "Actions": List[AutomationRulesActionTypeDef],
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "CreatedBy": str,
+    },
+    total=False,
+)
+
+_RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAutomationRuleRequestRequestTypeDef",
+    {
+        "RuleOrder": int,
+        "RuleName": str,
+        "Description": str,
+        "Criteria": AutomationRulesFindingFiltersTypeDef,
+        "Actions": Sequence[AutomationRulesActionTypeDef],
+    },
+)
+_OptionalCreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAutomationRuleRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "RuleStatus": RuleStatusType,
+        "IsTerminal": bool,
+    },
+    total=False,
+)
+
+class CreateAutomationRuleRequestRequestTypeDef(
+    _RequiredCreateAutomationRuleRequestRequestTypeDef,
+    _OptionalCreateAutomationRuleRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateAutomationRulesRequestItemTypeDef = TypedDict(
+    "_RequiredUpdateAutomationRulesRequestItemTypeDef",
+    {
+        "RuleArn": str,
+    },
+)
+_OptionalUpdateAutomationRulesRequestItemTypeDef = TypedDict(
+    "_OptionalUpdateAutomationRulesRequestItemTypeDef",
+    {
+        "RuleStatus": RuleStatusType,
+        "RuleOrder": int,
+        "Description": str,
+        "RuleName": str,
+        "IsTerminal": bool,
+        "Criteria": AutomationRulesFindingFiltersTypeDef,
+        "Actions": Sequence[AutomationRulesActionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateAutomationRulesRequestItemTypeDef(
+    _RequiredUpdateAutomationRulesRequestItemTypeDef,
+    _OptionalUpdateAutomationRulesRequestItemTypeDef,
+):
+    pass
+
 CreateInsightRequestRequestTypeDef = TypedDict(
     "CreateInsightRequestRequestTypeDef",
     {
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
 )
 
 GetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     {
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "SortCriteria": Sequence[SortCriterionTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetFindingsRequestRequestTypeDef = TypedDict(
     "GetFindingsRequestRequestTypeDef",
     {
@@ -7060,21 +8819,19 @@
     {
         "Note": NoteUpdateTypeDef,
         "RecordState": RecordStateType,
     },
     total=False,
 )
 
-
 class UpdateFindingsRequestRequestTypeDef(
     _RequiredUpdateFindingsRequestRequestTypeDef, _OptionalUpdateFindingsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateInsightRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInsightRequestRequestTypeDef",
     {
         "InsightArn": str,
     },
 )
 _OptionalUpdateInsightRequestRequestTypeDef = TypedDict(
@@ -7083,21 +8840,19 @@
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
     total=False,
 )
 
-
 class UpdateInsightRequestRequestTypeDef(
     _RequiredUpdateInsightRequestRequestTypeDef, _OptionalUpdateInsightRequestRequestTypeDef
 ):
     pass
 
-
 NetworkPathComponentTypeDef = TypedDict(
     "NetworkPathComponentTypeDef",
     {
         "ComponentId": str,
         "ComponentType": str,
         "Egress": NetworkHeaderTypeDef,
         "Ingress": NetworkHeaderTypeDef,
@@ -7191,18 +8946,32 @@
         "ViewerCertificate": AwsCloudFrontDistributionViewerCertificateTypeDef,
         "Status": str,
         "WebAclId": str,
     },
     total=False,
 )
 
+AwsGuardDutyDetectorDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDetailsTypeDef",
+    {
+        "DataSources": AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
+        "Features": Sequence[AwsGuardDutyDetectorFeaturesDetailsTypeDef],
+        "FindingPublishingFrequency": str,
+        "ServiceRole": str,
+        "Status": str,
+    },
+    total=False,
+)
+
 AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     {
-        "AbortIncompleteMultipartUpload": AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef,
+        "AbortIncompleteMultipartUpload": (
+            AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
+        ),
         "ExpirationDate": str,
         "ExpirationInDays": int,
         "ExpiredObjectDeleteMarker": bool,
         "Filter": AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
         "ID": str,
         "NoncurrentVersionExpirationInDays": int,
         "NoncurrentVersionTransitions": Sequence[
@@ -7221,20 +8990,48 @@
     "AwsS3BucketNotificationConfigurationTypeDef",
     {
         "Configurations": Sequence[AwsS3BucketNotificationConfigurationDetailTypeDef],
     },
     total=False,
 )
 
+AwsWafv2RulesDetailsTypeDef = TypedDict(
+    "AwsWafv2RulesDetailsTypeDef",
+    {
+        "Action": AwsWafv2RulesActionDetailsTypeDef,
+        "Name": str,
+        "OverrideAction": str,
+        "Priority": int,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
+BatchGetAutomationRulesResponseTypeDef = TypedDict(
+    "BatchGetAutomationRulesResponseTypeDef",
+    {
+        "Rules": List[AutomationRulesConfigTypeDef],
+        "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchUpdateAutomationRulesRequestRequestTypeDef = TypedDict(
+    "BatchUpdateAutomationRulesRequestRequestTypeDef",
+    {
+        "UpdateAutomationRulesRequestItems": Sequence[UpdateAutomationRulesRequestItemTypeDef],
+    },
+)
+
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "Insights": List[InsightTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CustomDataIdentifiersResultTypeDef = TypedDict(
     "CustomDataIdentifiersResultTypeDef",
     {
         "Detections": Sequence[CustomDataIdentifiersDetectionsTypeDef],
@@ -7282,14 +9079,46 @@
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
     {
         "Rules": Sequence[AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef],
     },
     total=False,
 )
 
+AwsWafv2RuleGroupDetailsTypeDef = TypedDict(
+    "AwsWafv2RuleGroupDetailsTypeDef",
+    {
+        "Capacity": int,
+        "Description": str,
+        "Id": str,
+        "Name": str,
+        "Arn": str,
+        "Rules": Sequence[AwsWafv2RulesDetailsTypeDef],
+        "Scope": str,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2WebAclDetailsTypeDef = TypedDict(
+    "AwsWafv2WebAclDetailsTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "ManagedbyFirewallManager": bool,
+        "Id": str,
+        "Capacity": int,
+        "CaptchaConfig": AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
+        "DefaultAction": AwsWafv2WebAclActionDetailsTypeDef,
+        "Description": str,
+        "Rules": Sequence[AwsWafv2RulesDetailsTypeDef],
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
 ClassificationResultTypeDef = TypedDict(
     "ClassificationResultTypeDef",
     {
         "MimeType": str,
         "SizeClassified": int,
         "AdditionalOccurrences": bool,
         "Status": ClassificationStatusTypeDef,
@@ -7313,15 +9142,17 @@
 
 RuleGroupSourceTypeDef = TypedDict(
     "RuleGroupSourceTypeDef",
     {
         "RulesSourceList": RuleGroupSourceListDetailsTypeDef,
         "RulesString": str,
         "StatefulRules": Sequence[RuleGroupSourceStatefulRulesDetailsTypeDef],
-        "StatelessRulesAndCustomActions": RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
+        "StatelessRulesAndCustomActions": (
+            RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef
+        ),
     },
     total=False,
 )
 
 AwsS3BucketDetailsTypeDef = TypedDict(
     "AwsS3BucketDetailsTypeDef",
     {
@@ -7333,14 +9164,15 @@
         "BucketLifecycleConfiguration": AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef,
         "PublicAccessBlockConfiguration": AwsS3AccountPublicAccessBlockDetailsTypeDef,
         "AccessControlList": str,
         "BucketLoggingConfiguration": AwsS3BucketLoggingConfigurationTypeDef,
         "BucketWebsiteConfiguration": AwsS3BucketWebsiteConfigurationTypeDef,
         "BucketNotificationConfiguration": AwsS3BucketNotificationConfigurationTypeDef,
         "BucketVersioningConfiguration": AwsS3BucketBucketVersioningConfigurationTypeDef,
+        "ObjectLockConfiguration": AwsS3BucketObjectLockConfigurationTypeDef,
     },
     total=False,
 )
 
 DataClassificationDetailsTypeDef = TypedDict(
     "DataClassificationDetailsTypeDef",
     {
@@ -7451,14 +9283,24 @@
         "AwsWafRegionalWebAcl": AwsWafRegionalWebAclDetailsTypeDef,
         "AwsWafRule": AwsWafRuleDetailsTypeDef,
         "AwsWafRuleGroup": AwsWafRuleGroupDetailsTypeDef,
         "AwsEcsTask": AwsEcsTaskDetailsTypeDef,
         "AwsBackupBackupVault": AwsBackupBackupVaultDetailsTypeDef,
         "AwsBackupBackupPlan": AwsBackupBackupPlanDetailsTypeDef,
         "AwsBackupRecoveryPoint": AwsBackupRecoveryPointDetailsTypeDef,
+        "AwsEc2LaunchTemplate": AwsEc2LaunchTemplateDetailsTypeDef,
+        "AwsSageMakerNotebookInstance": AwsSageMakerNotebookInstanceDetailsTypeDef,
+        "AwsWafv2WebAcl": AwsWafv2WebAclDetailsTypeDef,
+        "AwsWafv2RuleGroup": AwsWafv2RuleGroupDetailsTypeDef,
+        "AwsEc2RouteTable": AwsEc2RouteTableDetailsTypeDef,
+        "AwsAmazonMqBroker": AwsAmazonMqBrokerDetailsTypeDef,
+        "AwsAppSyncGraphQlApi": AwsAppSyncGraphQlApiDetailsTypeDef,
+        "AwsEventSchemasRegistry": AwsEventSchemasRegistryDetailsTypeDef,
+        "AwsGuardDutyDetector": AwsGuardDutyDetectorDetailsTypeDef,
+        "AwsStepFunctionStateMachine": AwsStepFunctionStateMachineDetailsTypeDef,
     },
     total=False,
 )
 
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
@@ -7475,19 +9317,17 @@
         "Tags": Mapping[str, str],
         "DataClassification": DataClassificationDetailsTypeDef,
         "Details": ResourceDetailsTypeDef,
     },
     total=False,
 )
 
-
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
-
 _RequiredAwsSecurityFindingTypeDef = TypedDict(
     "_RequiredAwsSecurityFindingTypeDef",
     {
         "SchemaVersion": str,
         "Id": str,
         "ProductArn": str,
         "GeneratorId": str,
@@ -7533,29 +9373,27 @@
         "Action": ActionTypeDef,
         "FindingProviderFields": FindingProviderFieldsTypeDef,
         "Sample": bool,
     },
     total=False,
 )
 
-
 class AwsSecurityFindingTypeDef(
     _RequiredAwsSecurityFindingTypeDef, _OptionalAwsSecurityFindingTypeDef
 ):
     pass
 
-
 BatchImportFindingsRequestRequestTypeDef = TypedDict(
     "BatchImportFindingsRequestRequestTypeDef",
     {
         "Findings": Sequence[AwsSecurityFindingTypeDef],
     },
 )
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "Findings": List[AwsSecurityFindingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/type_defs.pyi` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,38 +9,44 @@
     from mypy_boto3_securityhub.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef
 
     data: AcceptAdministratorInvitationRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdminStatusType,
+    AssociationStatusType,
     AutoEnableStandardsType,
     AwsIamAccessKeyStatusType,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
     ComplianceStatusType,
+    ControlFindingGeneratorType,
     ControlStatusType,
+    FindingHistoryUpdateSourceTypeType,
     IntegrationTypeType,
     MalwareStateType,
     MalwareTypeType,
     MapFilterComparisonType,
     NetworkDirectionType,
     PartitionType,
     RecordStateType,
+    RegionAvailabilityStatusType,
+    RuleStatusType,
     SeverityLabelType,
     SeverityRatingType,
     SortOrderType,
     StandardsStatusType,
     StatusReasonCodeType,
     StringFilterComparisonType,
     ThreatIntelIndicatorCategoryType,
     ThreatIntelIndicatorTypeType,
+    UnprocessedErrorCodeType,
     VerificationStateType,
     VulnerabilityFixAvailableType,
     WorkflowStateType,
     WorkflowStatusType,
 )
 
 if sys.version_info >= (3, 9):
@@ -48,14 +54,15 @@
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
     "AccountDetailsTypeDef",
     "ActionLocalIpDetailsTypeDef",
     "ActionLocalPortDetailsTypeDef",
     "CityTypeDef",
@@ -63,22 +70,41 @@
     "GeoLocationTypeDef",
     "IpOrganizationDetailsTypeDef",
     "ActionRemotePortDetailsTypeDef",
     "ActionTargetTypeDef",
     "DnsRequestActionTypeDef",
     "AdjustmentTypeDef",
     "AdminAccountTypeDef",
+    "AssociatedStandardTypeDef",
+    "AssociationStateDetailsTypeDef",
+    "NoteUpdateTypeDef",
+    "RelatedFindingTypeDef",
+    "SeverityUpdateTypeDef",
+    "WorkflowUpdateTypeDef",
+    "MapFilterTypeDef",
+    "NumberFilterTypeDef",
+    "StringFilterTypeDef",
+    "AutomationRulesMetadataTypeDef",
     "AvailabilityZoneTypeDef",
+    "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
+    "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
+    "AwsAmazonMqBrokerUsersDetailsTypeDef",
+    "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
     "AwsApiCallActionDomainDetailsTypeDef",
     "AwsApiGatewayAccessLogSettingsTypeDef",
     "AwsApiGatewayCanarySettingsTypeDef",
     "AwsApiGatewayEndpointConfigurationTypeDef",
     "AwsApiGatewayMethodSettingsTypeDef",
     "AwsCorsConfigurationTypeDef",
     "AwsApiGatewayV2RouteSettingsTypeDef",
+    "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
+    "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef",
+    "AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef",
+    "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef",
@@ -118,22 +144,53 @@
     "AwsDynamoDbTableRestoreSummaryTypeDef",
     "AwsDynamoDbTableSseDescriptionTypeDef",
     "AwsDynamoDbTableStreamSpecificationTypeDef",
     "AwsDynamoDbTableProjectionTypeDef",
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
     "AwsEc2EipDetailsTypeDef",
     "AwsEc2InstanceMetadataOptionsTypeDef",
+    "AwsEc2InstanceMonitoringDetailsTypeDef",
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataPlacementDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef",
     "AwsEc2NetworkAclAssociationTypeDef",
     "IcmpTypeCodeTypeDef",
     "PortRangeFromToTypeDef",
     "AwsEc2NetworkInterfaceAttachmentTypeDef",
     "AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef",
     "AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef",
     "AwsEc2NetworkInterfaceSecurityGroupTypeDef",
+    "PropagatingVgwSetDetailsTypeDef",
+    "RouteSetDetailsTypeDef",
     "AwsEc2SecurityGroupIpRangeTypeDef",
     "AwsEc2SecurityGroupIpv6RangeTypeDef",
     "AwsEc2SecurityGroupPrefixListIdTypeDef",
     "AwsEc2SecurityGroupUserIdGroupPairTypeDef",
     "Ipv6CidrBlockAssociationTypeDef",
     "AwsEc2TransitGatewayDetailsTypeDef",
     "AwsEc2VolumeAttachmentTypeDef",
@@ -210,14 +267,22 @@
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
     "AwsElbLoadBalancerHealthCheckTypeDef",
     "AwsElbLoadBalancerInstanceTypeDef",
     "AwsElbLoadBalancerSourceSecurityGroupTypeDef",
     "AwsElbLoadBalancerListenerTypeDef",
     "AwsElbv2LoadBalancerAttributeTypeDef",
     "LoadBalancerStateTypeDef",
+    "AwsEventSchemasRegistryDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef",
+    "AwsGuardDutyDetectorFeaturesDetailsTypeDef",
     "AwsIamAccessKeySessionContextAttributesTypeDef",
     "AwsIamAccessKeySessionContextSessionIssuerTypeDef",
     "AwsIamAttachedManagedPolicyTypeDef",
     "AwsIamGroupPolicyTypeDef",
     "AwsIamInstanceProfileRoleTypeDef",
     "AwsIamPermissionsBoundaryTypeDef",
     "AwsIamPolicyVersionTypeDef",
@@ -277,139 +342,189 @@
     "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef",
     "AwsS3BucketBucketVersioningConfigurationTypeDef",
     "AwsS3BucketLoggingConfigurationTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef",
+    "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef",
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
     "AwsS3BucketWebsiteConfigurationRedirectToTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef",
     "AwsS3ObjectDetailsTypeDef",
+    "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     "BooleanFilterTypeDef",
     "IpFilterTypeDef",
     "KeywordFilterTypeDef",
-    "MapFilterTypeDef",
-    "NumberFilterTypeDef",
-    "StringFilterTypeDef",
     "AwsSecurityFindingIdentifierTypeDef",
     "MalwareTypeDef",
     "NoteTypeDef",
     "PatchSummaryTypeDef",
     "ProcessDetailsTypeDef",
-    "RelatedFindingTypeDef",
     "SeverityTypeDef",
     "ThreatIntelIndicatorTypeDef",
     "WorkflowTypeDef",
     "AwsSnsTopicSubscriptionTypeDef",
     "AwsSqsQueueDetailsTypeDef",
     "AwsSsmComplianceSummaryTypeDef",
+    "AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef",
+    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef",
     "AwsWafRateBasedRuleMatchPredicateTypeDef",
     "AwsWafRegionalRateBasedRuleMatchPredicateTypeDef",
     "AwsWafRegionalRulePredicateListDetailsTypeDef",
     "AwsWafRegionalRuleGroupRulesActionDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListActionDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef",
     "AwsWafRulePredicateListDetailsTypeDef",
     "AwsWafRuleGroupRulesActionDetailsTypeDef",
     "WafActionTypeDef",
     "WafExcludedRuleTypeDef",
     "WafOverrideActionTypeDef",
+    "AwsWafv2CustomHttpHeaderTypeDef",
+    "AwsWafv2VisibilityConfigDetailsTypeDef",
+    "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
     "AwsXrayEncryptionConfigDetailsTypeDef",
+    "BatchDeleteAutomationRulesRequestRequestTypeDef",
+    "UnprocessedAutomationRuleTypeDef",
     "BatchDisableStandardsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StandardsSubscriptionRequestTypeDef",
+    "BatchGetAutomationRulesRequestRequestTypeDef",
+    "BatchGetSecurityControlsRequestRequestTypeDef",
+    "SecurityControlTypeDef",
+    "UnprocessedSecurityControlTypeDef",
+    "StandardsControlAssociationIdTypeDef",
+    "StandardsControlAssociationDetailTypeDef",
     "ImportFindingsErrorTypeDef",
-    "NoteUpdateTypeDef",
-    "SeverityUpdateTypeDef",
-    "WorkflowUpdateTypeDef",
+    "StandardsControlAssociationUpdateTypeDef",
     "CellTypeDef",
     "ClassificationStatusTypeDef",
     "StatusReasonTypeDef",
     "VolumeMountTypeDef",
     "CreateActionTargetRequestRequestTypeDef",
+    "CreateActionTargetResponseTypeDef",
+    "CreateAutomationRuleResponseTypeDef",
     "CreateFindingAggregatorRequestRequestTypeDef",
+    "CreateFindingAggregatorResponseTypeDef",
+    "CreateInsightResponseTypeDef",
     "ResultTypeDef",
     "DateRangeTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteActionTargetRequestRequestTypeDef",
+    "DeleteActionTargetResponseTypeDef",
     "DeleteFindingAggregatorRequestRequestTypeDef",
     "DeleteInsightRequestRequestTypeDef",
+    "DeleteInsightResponseTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
     "DescribeActionTargetsRequestRequestTypeDef",
     "DescribeHubRequestRequestTypeDef",
+    "DescribeHubResponseTypeDef",
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
     "DescribeProductsRequestRequestTypeDef",
     "ProductTypeDef",
+    "DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
     "DescribeStandardsControlsRequestRequestTypeDef",
     "StandardsControlTypeDef",
+    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
     "DescribeStandardsRequestRequestTypeDef",
-    "StandardTypeDef",
     "DisableImportFindingsForProductRequestRequestTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
     "EnableImportFindingsForProductRequestRequestTypeDef",
+    "EnableImportFindingsForProductResponseTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "EnableSecurityHubRequestRequestTypeDef",
     "FilePathsTypeDef",
     "FindingAggregatorTypeDef",
+    "FindingHistoryUpdateSourceTypeDef",
+    "FindingHistoryUpdateTypeDef",
     "FindingProviderSeverityTypeDef",
     "FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef",
     "FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef",
     "InvitationTypeDef",
+    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
     "GetEnabledStandardsRequestRequestTypeDef",
     "GetFindingAggregatorRequestRequestTypeDef",
+    "GetFindingAggregatorResponseTypeDef",
     "SortCriterionTypeDef",
     "GetInsightResultsRequestRequestTypeDef",
+    "GetInsightsRequestGetInsightsPaginateTypeDef",
     "GetInsightsRequestRequestTypeDef",
+    "GetInvitationsCountResponseTypeDef",
     "GetMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "InsightResultValueTypeDef",
     "InviteMembersRequestRequestTypeDef",
+    "ListAutomationRulesRequestRequestTypeDef",
+    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
     "ListEnabledProductsForImportRequestRequestTypeDef",
+    "ListEnabledProductsForImportResponseTypeDef",
+    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
     "ListFindingAggregatorsRequestRequestTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
+    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
+    "ListSecurityControlDefinitionsRequestRequestTypeDef",
+    "SecurityControlDefinitionTypeDef",
+    "ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
+    "ListStandardsControlAssociationsRequestRequestTypeDef",
+    "StandardsControlAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PortRangeTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
+    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
+    "ResponseMetadataTypeDef",
     "RuleGroupSourceListDetailsTypeDef",
     "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
     "RuleGroupVariablesIpSetsDetailsTypeDef",
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     "SoftwarePackageTypeDef",
+    "StandardsManagedByTypeDef",
     "StandardsStatusReasonTypeDef",
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateActionTargetRequestRequestTypeDef",
     "UpdateFindingAggregatorRequestRequestTypeDef",
+    "UpdateFindingAggregatorResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateSecurityHubConfigurationRequestRequestTypeDef",
     "UpdateStandardsControlRequestRequestTypeDef",
     "VulnerabilityVendorTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "ActionRemoteIpDetailsTypeDef",
+    "DescribeActionTargetsResponseTypeDef",
     "CvssTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "AssociationSetDetailsTypeDef",
+    "AutomationRulesFindingFieldsUpdateTypeDef",
+    "ListAutomationRulesResponseTypeDef",
+    "AwsAmazonMqBrokerLogsDetailsTypeDef",
     "AwsApiGatewayRestApiDetailsTypeDef",
     "AwsApiGatewayStageDetailsTypeDef",
     "AwsApiGatewayV2ApiDetailsTypeDef",
     "AwsApiGatewayV2StageDetailsTypeDef",
+    "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef",
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
     "AwsBackupBackupVaultDetailsTypeDef",
     "AwsBackupRecoveryPointDetailsTypeDef",
     "AwsCertificateManagerCertificateDomainValidationOptionTypeDef",
     "AwsCloudFormationStackDetailsTypeDef",
@@ -419,14 +534,19 @@
     "AwsCloudWatchAlarmDetailsTypeDef",
     "AwsCodeBuildProjectEnvironmentTypeDef",
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     "AwsDynamoDbTableLocalSecondaryIndexTypeDef",
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
     "AwsEc2NetworkAclEntryTypeDef",
     "AwsEc2NetworkInterfaceDetailsTypeDef",
     "AwsEc2SecurityGroupIpPermissionTypeDef",
     "AwsEc2SubnetDetailsTypeDef",
     "AwsEc2VolumeDetailsTypeDef",
     "AwsEc2VpcDetailsTypeDef",
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
@@ -447,14 +567,16 @@
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
     "AwsElbLoadBalancerPoliciesTypeDef",
     "AwsElbLoadBalancerAttributesTypeDef",
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
     "AwsElbv2LoadBalancerDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
     "AwsIamAccessKeySessionContextTypeDef",
     "AwsIamGroupDetailsTypeDef",
     "AwsIamInstanceProfileTypeDef",
     "AwsIamPolicyDetailsTypeDef",
     "AwsIamUserDetailsTypeDef",
     "AwsKinesisStreamDetailsTypeDef",
     "AwsLambdaFunctionEnvironmentTypeDef",
@@ -466,148 +588,165 @@
     "AwsRdsDbSnapshotDetailsTypeDef",
     "AwsRdsDbPendingModifiedValuesTypeDef",
     "AwsRdsDbSecurityGroupDetailsTypeDef",
     "AwsRdsDbSubnetGroupSubnetTypeDef",
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
+    "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
+    "AwsSageMakerNotebookInstanceDetailsTypeDef",
     "AwsSecretsManagerSecretDetailsTypeDef",
+    "BatchUpdateFindingsRequestRequestTypeDef",
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
+    "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    "GetFindingHistoryRequestRequestTypeDef",
     "AwsSnsTopicDetailsTypeDef",
     "AwsSsmPatchTypeDef",
+    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     "AwsWafRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRuleDetailsTypeDef",
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
     "AwsWafRuleDetailsTypeDef",
     "AwsWafRuleGroupRulesDetailsTypeDef",
     "AwsWafWebAclRuleTypeDef",
-    "CreateActionTargetResponseTypeDef",
-    "CreateFindingAggregatorResponseTypeDef",
-    "CreateInsightResponseTypeDef",
-    "DeleteActionTargetResponseTypeDef",
-    "DeleteInsightResponseTypeDef",
-    "DescribeActionTargetsResponseTypeDef",
-    "DescribeHubResponseTypeDef",
-    "DescribeOrganizationConfigurationResponseTypeDef",
-    "EnableImportFindingsForProductResponseTypeDef",
-    "GetFindingAggregatorResponseTypeDef",
-    "GetInvitationsCountResponseTypeDef",
-    "ListEnabledProductsForImportResponseTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateFindingAggregatorResponseTypeDef",
+    "AwsWafv2CustomRequestHandlingDetailsTypeDef",
+    "AwsWafv2CustomResponseDetailsTypeDef",
+    "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
+    "BatchDeleteAutomationRulesResponseTypeDef",
+    "BatchUpdateAutomationRulesResponseTypeDef",
     "BatchEnableStandardsRequestRequestTypeDef",
+    "BatchGetSecurityControlsResponseTypeDef",
+    "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
+    "UnprocessedStandardsControlAssociationTypeDef",
     "BatchImportFindingsResponseTypeDef",
-    "BatchUpdateFindingsRequestRequestTypeDef",
+    "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
+    "UnprocessedStandardsControlAssociationUpdateTypeDef",
     "ComplianceTypeDef",
     "ContainerDetailsTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "DateFilterTypeDef",
-    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
-    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
-    "DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
-    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
-    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
-    "GetInsightsRequestGetInsightsPaginateTypeDef",
-    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
-    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "DescribeProductsResponseTypeDef",
     "DescribeStandardsControlsResponseTypeDef",
-    "DescribeStandardsResponseTypeDef",
     "ThreatTypeDef",
     "ListFindingAggregatorsResponseTypeDef",
+    "FindingHistoryRecordTypeDef",
     "FindingProviderFieldsTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "InsightResultsTypeDef",
+    "ListSecurityControlDefinitionsResponseTypeDef",
+    "ListStandardsControlAssociationsResponseTypeDef",
     "NetworkPathComponentDetailsTypeDef",
     "NetworkTypeDef",
     "PageTypeDef",
     "RemediationTypeDef",
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
     "RuleGroupVariablesTypeDef",
+    "StandardTypeDef",
     "StandardsSubscriptionTypeDef",
     "StatelessCustomPublishMetricActionTypeDef",
     "AwsApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "VulnerabilityTypeDef",
+    "AwsEc2RouteTableDetailsTypeDef",
+    "AutomationRulesActionTypeDef",
+    "AwsAmazonMqBrokerDetailsTypeDef",
+    "AwsAppSyncGraphQlApiDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     "AwsBackupBackupPlanRuleDetailsTypeDef",
     "AwsCertificateManagerCertificateRenewalSummaryTypeDef",
     "AwsCloudFrontDistributionOriginItemTypeDef",
     "AwsCloudFrontDistributionOriginGroupTypeDef",
     "AwsCodeBuildProjectDetailsTypeDef",
     "AwsDynamoDbTableReplicaTypeDef",
+    "AwsEc2LaunchTemplateDataDetailsTypeDef",
     "AwsEc2NetworkAclDetailsTypeDef",
     "AwsEc2SecurityGroupDetailsTypeDef",
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
     "AwsEc2VpnConnectionDetailsTypeDef",
     "AwsEcsClusterConfigurationDetailsTypeDef",
     "AwsEcsServiceDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
     "AwsEcsTaskDetailsTypeDef",
     "AwsEfsAccessPointDetailsTypeDef",
     "AwsEksClusterDetailsTypeDef",
     "AwsElasticsearchDomainDetailsTypeDef",
     "AwsElbLoadBalancerDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
     "AwsIamAccessKeyDetailsTypeDef",
     "AwsIamRoleDetailsTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
     "AwsOpenSearchServiceDomainDetailsTypeDef",
     "AwsRdsDbSubnetGroupTypeDef",
     "AwsRedshiftClusterDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
+    "AwsS3BucketObjectLockConfigurationTypeDef",
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     "AwsS3BucketWebsiteConfigurationTypeDef",
     "BatchUpdateFindingsResponseTypeDef",
     "AwsSsmPatchComplianceDetailsTypeDef",
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     "AwsWafRegionalWebAclDetailsTypeDef",
     "AwsWafRuleGroupDetailsTypeDef",
     "AwsWafWebAclDetailsTypeDef",
+    "AwsWafv2ActionAllowDetailsTypeDef",
+    "AwsWafv2RulesActionCaptchaDetailsTypeDef",
+    "AwsWafv2RulesActionCountDetailsTypeDef",
+    "AwsWafv2ActionBlockDetailsTypeDef",
+    "BatchGetStandardsControlAssociationsResponseTypeDef",
+    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
+    "AutomationRulesFindingFiltersTypeDef",
     "AwsSecurityFindingFiltersTypeDef",
+    "GetFindingHistoryResponseTypeDef",
     "GetInsightResultsResponseTypeDef",
     "NetworkHeaderTypeDef",
     "OccurrencesTypeDef",
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
+    "DescribeStandardsResponseTypeDef",
     "BatchDisableStandardsResponseTypeDef",
     "BatchEnableStandardsResponseTypeDef",
     "GetEnabledStandardsResponseTypeDef",
     "StatelessCustomActionDefinitionTypeDef",
     "PortProbeActionTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     "AwsCertificateManagerCertificateDetailsTypeDef",
     "AwsCloudFrontDistributionOriginsTypeDef",
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
     "AwsDynamoDbTableDetailsTypeDef",
+    "AwsEc2LaunchTemplateDetailsTypeDef",
     "AwsEcsClusterDetailsTypeDef",
     "AwsEcsTaskDefinitionDetailsTypeDef",
+    "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
     "AwsRdsDbInstanceDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
+    "AwsStepFunctionStateMachineDetailsTypeDef",
+    "AwsWafv2RulesActionDetailsTypeDef",
+    "AwsWafv2WebAclActionDetailsTypeDef",
+    "AutomationRulesConfigTypeDef",
+    "CreateAutomationRuleRequestRequestTypeDef",
+    "UpdateAutomationRulesRequestItemTypeDef",
     "CreateInsightRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "InsightTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "UpdateInsightRequestRequestTypeDef",
     "NetworkPathComponentTypeDef",
@@ -615,22 +754,28 @@
     "SensitiveDataDetectionsTypeDef",
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     "RuleGroupSourceCustomActionsDetailsTypeDef",
     "ActionTypeDef",
     "AwsBackupBackupPlanDetailsTypeDef",
     "AwsCloudFrontDistributionDetailsTypeDef",
+    "AwsGuardDutyDetectorDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationTypeDef",
+    "AwsWafv2RulesDetailsTypeDef",
+    "BatchGetAutomationRulesResponseTypeDef",
+    "BatchUpdateAutomationRulesRequestRequestTypeDef",
     "GetInsightsResponseTypeDef",
     "CustomDataIdentifiersResultTypeDef",
     "SensitiveDataResultTypeDef",
     "FirewallPolicyDetailsTypeDef",
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
+    "AwsWafv2RuleGroupDetailsTypeDef",
+    "AwsWafv2WebAclDetailsTypeDef",
     "ClassificationResultTypeDef",
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     "RuleGroupSourceTypeDef",
     "AwsS3BucketDetailsTypeDef",
     "DataClassificationDetailsTypeDef",
     "RuleGroupDetailsTypeDef",
     "AwsNetworkFirewallRuleGroupDetailsTypeDef",
@@ -667,17 +812,19 @@
     "_OptionalAccountDetailsTypeDef",
     {
         "Email": str,
     },
     total=False,
 )
 
+
 class AccountDetailsTypeDef(_RequiredAccountDetailsTypeDef, _OptionalAccountDetailsTypeDef):
     pass
 
+
 ActionLocalIpDetailsTypeDef = TypedDict(
     "ActionLocalIpDetailsTypeDef",
     {
         "IpAddressV4": str,
     },
     total=False,
 )
@@ -770,23 +917,173 @@
     {
         "AccountId": str,
         "Status": AdminStatusType,
     },
     total=False,
 )
 
+AssociatedStandardTypeDef = TypedDict(
+    "AssociatedStandardTypeDef",
+    {
+        "StandardsId": str,
+    },
+    total=False,
+)
+
+AssociationStateDetailsTypeDef = TypedDict(
+    "AssociationStateDetailsTypeDef",
+    {
+        "State": str,
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
+NoteUpdateTypeDef = TypedDict(
+    "NoteUpdateTypeDef",
+    {
+        "Text": str,
+        "UpdatedBy": str,
+    },
+)
+
+RelatedFindingTypeDef = TypedDict(
+    "RelatedFindingTypeDef",
+    {
+        "ProductArn": str,
+        "Id": str,
+    },
+)
+
+SeverityUpdateTypeDef = TypedDict(
+    "SeverityUpdateTypeDef",
+    {
+        "Normalized": int,
+        "Product": float,
+        "Label": SeverityLabelType,
+    },
+    total=False,
+)
+
+WorkflowUpdateTypeDef = TypedDict(
+    "WorkflowUpdateTypeDef",
+    {
+        "Status": WorkflowStatusType,
+    },
+    total=False,
+)
+
+MapFilterTypeDef = TypedDict(
+    "MapFilterTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "Comparison": MapFilterComparisonType,
+    },
+    total=False,
+)
+
+NumberFilterTypeDef = TypedDict(
+    "NumberFilterTypeDef",
+    {
+        "Gte": float,
+        "Lte": float,
+        "Eq": float,
+    },
+    total=False,
+)
+
+StringFilterTypeDef = TypedDict(
+    "StringFilterTypeDef",
+    {
+        "Value": str,
+        "Comparison": StringFilterComparisonType,
+    },
+    total=False,
+)
+
+AutomationRulesMetadataTypeDef = TypedDict(
+    "AutomationRulesMetadataTypeDef",
+    {
+        "RuleArn": str,
+        "RuleStatus": RuleStatusType,
+        "RuleOrder": int,
+        "RuleName": str,
+        "Description": str,
+        "IsTerminal": bool,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "CreatedBy": str,
+    },
+    total=False,
+)
+
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
     },
     total=False,
 )
 
+AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
+    {
+        "KmsKeyId": str,
+        "UseAwsOwnedKey": bool,
+    },
+    total=False,
+)
+
+AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
+    {
+        "Hosts": Sequence[str],
+        "RoleBase": str,
+        "RoleName": str,
+        "RoleSearchMatching": str,
+        "RoleSearchSubtree": bool,
+        "ServiceAccountUsername": str,
+        "UserBase": str,
+        "UserRoleName": str,
+        "UserSearchMatching": str,
+        "UserSearchSubtree": bool,
+    },
+    total=False,
+)
+
+AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
+    {
+        "DayOfWeek": str,
+        "TimeOfDay": str,
+        "TimeZone": str,
+    },
+    total=False,
+)
+
+AwsAmazonMqBrokerUsersDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerUsersDetailsTypeDef",
+    {
+        "PendingChange": str,
+        "Username": str,
+    },
+    total=False,
+)
+
+AwsAmazonMqBrokerLogsPendingDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
+    {
+        "Audit": bool,
+        "General": bool,
+    },
+    total=False,
+)
+
 AwsApiCallActionDomainDetailsTypeDef = TypedDict(
     "AwsApiCallActionDomainDetailsTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
@@ -859,14 +1156,56 @@
         "DataTraceEnabled": bool,
         "ThrottlingBurstLimit": int,
         "ThrottlingRateLimit": float,
     },
     total=False,
 )
 
+AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
+    {
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerUri": str,
+        "IdentityValidationExpression": str,
+    },
+    total=False,
+)
+
+AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef",
+    {
+        "AuthTtL": int,
+        "ClientId": str,
+        "IatTtL": int,
+        "Issuer": str,
+    },
+    total=False,
+)
+
+AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef",
+    {
+        "AppIdClientRegex": str,
+        "AwsRegion": str,
+        "DefaultAction": str,
+        "UserPoolId": str,
+    },
+    total=False,
+)
+
+AwsAppSyncGraphQlApiLogConfigDetailsTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
+    {
+        "CloudWatchLogsRoleArn": str,
+        "ExcludeVerboseContent": bool,
+        "FieldLogLevel": str,
+    },
+    total=False,
+)
+
 AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
@@ -1339,22 +1678,291 @@
         "HttpPutResponseHopLimit": int,
         "HttpTokens": str,
         "InstanceMetadataTags": str,
     },
     total=False,
 )
 
+AwsEc2InstanceMonitoringDetailsTypeDef = TypedDict(
+    "AwsEc2InstanceMonitoringDetailsTypeDef",
+    {
+        "State": str,
+    },
+    total=False,
+)
+
 AwsEc2InstanceNetworkInterfacesDetailsTypeDef = TypedDict(
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
     {
         "NetworkInterfaceId": str,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
+    {
+        "DeleteOnTermination": bool,
+        "Encrypted": bool,
+        "Iops": int,
+        "KmsKeyId": str,
+        "SnapshotId": str,
+        "Throughput": int,
+        "VolumeSize": int,
+        "VolumeType": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
+    {
+        "CapacityReservationId": str,
+        "CapacityReservationResourceGroupArn": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
+    {
+        "CoreCount": int,
+        "ThreadsPerCore": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
+    {
+        "CpuCredits": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
+    {
+        "Type": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef",
+    {
+        "Count": int,
+        "Type": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef",
+    {
+        "Configured": bool,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef",
+    {
+        "AutoRecovery": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef",
+    {
+        "HttpEndpoint": str,
+        "HttpProtocolIpv6": str,
+        "HttpTokens": str,
+        "HttpPutResponseHopLimit": int,
+        "InstanceMetadataTags": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataPlacementDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataPlacementDetailsTypeDef",
+    {
+        "Affinity": str,
+        "AvailabilityZone": str,
+        "GroupName": str,
+        "HostId": str,
+        "HostResourceGroupArn": str,
+        "PartitionNumber": int,
+        "SpreadDomain": str,
+        "Tenancy": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef",
+    {
+        "EnableResourceNameDnsAAAARecord": bool,
+        "EnableResourceNameDnsARecord": bool,
+        "HostnameType": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
+    {
+        "BlockDurationMinutes": int,
+        "InstanceInterruptionBehavior": str,
+        "MaxPrice": str,
+        "SpotInstanceType": str,
+        "ValidUntil": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
+    {
+        "Max": int,
+        "Min": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
+    {
+        "Max": int,
+        "Min": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
+    {
+        "Max": int,
+        "Min": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
+    {
+        "Max": float,
+        "Min": float,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef",
+    {
+        "Max": int,
+        "Min": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef",
+    {
+        "Max": int,
+        "Min": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef",
+    {
+        "Max": float,
+        "Min": float,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef",
+    {
+        "Max": int,
+        "Min": int,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
+    {
+        "Ipv4Prefix": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef",
+    {
+        "Ipv6Address": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef",
+    {
+        "Ipv6Prefix": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef",
+    {
+        "Primary": bool,
+        "PrivateIpAddress": str,
+    },
+    total=False,
+)
+
 AwsEc2NetworkAclAssociationTypeDef = TypedDict(
     "AwsEc2NetworkAclAssociationTypeDef",
     {
         "NetworkAclAssociationId": str,
         "NetworkAclId": str,
         "SubnetId": str,
     },
@@ -1415,14 +2023,45 @@
     {
         "GroupName": str,
         "GroupId": str,
     },
     total=False,
 )
 
+PropagatingVgwSetDetailsTypeDef = TypedDict(
+    "PropagatingVgwSetDetailsTypeDef",
+    {
+        "GatewayId": str,
+    },
+    total=False,
+)
+
+RouteSetDetailsTypeDef = TypedDict(
+    "RouteSetDetailsTypeDef",
+    {
+        "CarrierGatewayId": str,
+        "CoreNetworkArn": str,
+        "DestinationCidrBlock": str,
+        "DestinationIpv6CidrBlock": str,
+        "DestinationPrefixListId": str,
+        "EgressOnlyInternetGatewayId": str,
+        "GatewayId": str,
+        "InstanceId": str,
+        "InstanceOwnerId": str,
+        "LocalGatewayId": str,
+        "NatGatewayId": str,
+        "NetworkInterfaceId": str,
+        "Origin": str,
+        "State": str,
+        "TransitGatewayId": str,
+        "VpcPeeringConnectionId": str,
+    },
+    total=False,
+)
+
 AwsEc2SecurityGroupIpRangeTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpRangeTypeDef",
     {
         "CidrIp": str,
     },
     total=False,
 )
@@ -1995,14 +2634,15 @@
 )
 
 AwsEksClusterResourcesVpcConfigDetailsTypeDef = TypedDict(
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
+        "EndpointPublicAccess": bool,
     },
     total=False,
 )
 
 AwsEksClusterLoggingClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
     {
@@ -2237,14 +2877,82 @@
     {
         "Code": str,
         "Reason": str,
     },
     total=False,
 )
 
+AwsEventSchemasRegistryDetailsTypeDef = TypedDict(
+    "AwsEventSchemasRegistryDetailsTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef",
+    {
+        "Status": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef",
+    {
+        "Status": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef",
+    {
+        "Status": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef",
+    {
+        "Status": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef",
+    {
+        "Status": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef",
+    {
+        "Reason": str,
+        "Status": str,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorFeaturesDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorFeaturesDetailsTypeDef",
+    {
+        "Name": str,
+        "Status": str,
+    },
+    total=False,
+)
+
 AwsIamAccessKeySessionContextAttributesTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextAttributesTypeDef",
     {
         "MfaAuthenticated": bool,
         "CreationDate": str,
     },
     total=False,
@@ -2920,14 +3628,24 @@
     {
         "Name": AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
         "Value": str,
     },
     total=False,
 )
 
+AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef = TypedDict(
+    "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef",
+    {
+        "Days": int,
+        "Mode": str,
+        "Years": int,
+    },
+    total=False,
+)
+
 AwsS3BucketServerSideEncryptionByDefaultTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
     {
         "SSEAlgorithm": str,
         "KMSMasterKeyID": str,
     },
     total=False,
@@ -2972,14 +3690,22 @@
         "ContentType": str,
         "ServerSideEncryption": str,
         "SSEKMSKeyId": str,
     },
     total=False,
 )
 
+AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef = TypedDict(
+    "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
+    {
+        "MinimumInstanceMetadataServiceVersion": str,
+    },
+    total=False,
+)
+
 AwsSecretsManagerSecretRotationRulesTypeDef = TypedDict(
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     {
         "AutomaticallyAfterDays": int,
     },
     total=False,
 )
@@ -3004,43 +3730,14 @@
     "KeywordFilterTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-MapFilterTypeDef = TypedDict(
-    "MapFilterTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "Comparison": MapFilterComparisonType,
-    },
-    total=False,
-)
-
-NumberFilterTypeDef = TypedDict(
-    "NumberFilterTypeDef",
-    {
-        "Gte": float,
-        "Lte": float,
-        "Eq": float,
-    },
-    total=False,
-)
-
-StringFilterTypeDef = TypedDict(
-    "StringFilterTypeDef",
-    {
-        "Value": str,
-        "Comparison": StringFilterComparisonType,
-    },
-    total=False,
-)
-
 AwsSecurityFindingIdentifierTypeDef = TypedDict(
     "AwsSecurityFindingIdentifierTypeDef",
     {
         "Id": str,
         "ProductArn": str,
     },
 )
@@ -3057,17 +3754,19 @@
         "Type": MalwareTypeType,
         "Path": str,
         "State": MalwareStateType,
     },
     total=False,
 )
 
+
 class MalwareTypeDef(_RequiredMalwareTypeDef, _OptionalMalwareTypeDef):
     pass
 
+
 NoteTypeDef = TypedDict(
     "NoteTypeDef",
     {
         "Text": str,
         "UpdatedBy": str,
         "UpdatedAt": str,
     },
@@ -3092,38 +3791,32 @@
         "OperationEndTime": str,
         "RebootOption": str,
         "Operation": str,
     },
     total=False,
 )
 
+
 class PatchSummaryTypeDef(_RequiredPatchSummaryTypeDef, _OptionalPatchSummaryTypeDef):
     pass
 
+
 ProcessDetailsTypeDef = TypedDict(
     "ProcessDetailsTypeDef",
     {
         "Name": str,
         "Path": str,
         "Pid": int,
         "ParentPid": int,
         "LaunchedAt": str,
         "TerminatedAt": str,
     },
     total=False,
 )
 
-RelatedFindingTypeDef = TypedDict(
-    "RelatedFindingTypeDef",
-    {
-        "ProductArn": str,
-        "Id": str,
-    },
-)
-
 SeverityTypeDef = TypedDict(
     "SeverityTypeDef",
     {
         "Product": float,
         "Label": SeverityLabelType,
         "Normalized": int,
         "Original": str,
@@ -3193,14 +3886,30 @@
         "NonCompliantMediumCount": int,
         "NonCompliantUnspecifiedCount": int,
         "PatchGroup": str,
     },
     total=False,
 )
 
+AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef",
+    {
+        "LogGroupArn": str,
+    },
+    total=False,
+)
+
 AwsWafRateBasedRuleMatchPredicateTypeDef = TypedDict(
     "AwsWafRateBasedRuleMatchPredicateTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
@@ -3289,39 +3998,72 @@
     "WafOverrideActionTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
+AwsWafv2CustomHttpHeaderTypeDef = TypedDict(
+    "AwsWafv2CustomHttpHeaderTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+    total=False,
+)
+
+AwsWafv2VisibilityConfigDetailsTypeDef = TypedDict(
+    "AwsWafv2VisibilityConfigDetailsTypeDef",
+    {
+        "CloudWatchMetricsEnabled": bool,
+        "MetricName": str,
+        "SampledRequestsEnabled": bool,
+    },
+    total=False,
+)
+
+AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef = TypedDict(
+    "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
+    {
+        "ImmunityTime": int,
+    },
+    total=False,
+)
+
 AwsXrayEncryptionConfigDetailsTypeDef = TypedDict(
     "AwsXrayEncryptionConfigDetailsTypeDef",
     {
         "KeyId": str,
         "Status": str,
         "Type": str,
     },
     total=False,
 )
 
-BatchDisableStandardsRequestRequestTypeDef = TypedDict(
-    "BatchDisableStandardsRequestRequestTypeDef",
+BatchDeleteAutomationRulesRequestRequestTypeDef = TypedDict(
+    "BatchDeleteAutomationRulesRequestRequestTypeDef",
     {
-        "StandardsSubscriptionArns": Sequence[str],
+        "AutomationRulesArns": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UnprocessedAutomationRuleTypeDef = TypedDict(
+    "UnprocessedAutomationRuleTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "RuleArn": str,
+        "ErrorCode": int,
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
+BatchDisableStandardsRequestRequestTypeDef = TypedDict(
+    "BatchDisableStandardsRequestRequestTypeDef",
+    {
+        "StandardsSubscriptionArns": Sequence[str],
     },
 )
 
 _RequiredStandardsSubscriptionRequestTypeDef = TypedDict(
     "_RequiredStandardsSubscriptionRequestTypeDef",
     {
         "StandardsArn": str,
@@ -3331,54 +4073,141 @@
     "_OptionalStandardsSubscriptionRequestTypeDef",
     {
         "StandardsInput": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StandardsSubscriptionRequestTypeDef(
     _RequiredStandardsSubscriptionRequestTypeDef, _OptionalStandardsSubscriptionRequestTypeDef
 ):
     pass
 
-ImportFindingsErrorTypeDef = TypedDict(
-    "ImportFindingsErrorTypeDef",
+
+BatchGetAutomationRulesRequestRequestTypeDef = TypedDict(
+    "BatchGetAutomationRulesRequestRequestTypeDef",
     {
-        "Id": str,
-        "ErrorCode": str,
-        "ErrorMessage": str,
+        "AutomationRulesArns": Sequence[str],
     },
 )
 
-NoteUpdateTypeDef = TypedDict(
-    "NoteUpdateTypeDef",
+BatchGetSecurityControlsRequestRequestTypeDef = TypedDict(
+    "BatchGetSecurityControlsRequestRequestTypeDef",
     {
-        "Text": str,
-        "UpdatedBy": str,
+        "SecurityControlIds": Sequence[str],
     },
 )
 
-SeverityUpdateTypeDef = TypedDict(
-    "SeverityUpdateTypeDef",
+SecurityControlTypeDef = TypedDict(
+    "SecurityControlTypeDef",
     {
-        "Normalized": int,
-        "Product": float,
-        "Label": SeverityLabelType,
+        "SecurityControlId": str,
+        "SecurityControlArn": str,
+        "Title": str,
+        "Description": str,
+        "RemediationUrl": str,
+        "SeverityRating": SeverityRatingType,
+        "SecurityControlStatus": ControlStatusType,
+    },
+)
+
+_RequiredUnprocessedSecurityControlTypeDef = TypedDict(
+    "_RequiredUnprocessedSecurityControlTypeDef",
+    {
+        "SecurityControlId": str,
+        "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedSecurityControlTypeDef = TypedDict(
+    "_OptionalUnprocessedSecurityControlTypeDef",
+    {
+        "ErrorReason": str,
     },
     total=False,
 )
 
-WorkflowUpdateTypeDef = TypedDict(
-    "WorkflowUpdateTypeDef",
+
+class UnprocessedSecurityControlTypeDef(
+    _RequiredUnprocessedSecurityControlTypeDef, _OptionalUnprocessedSecurityControlTypeDef
+):
+    pass
+
+
+StandardsControlAssociationIdTypeDef = TypedDict(
+    "StandardsControlAssociationIdTypeDef",
     {
-        "Status": WorkflowStatusType,
+        "SecurityControlId": str,
+        "StandardsArn": str,
+    },
+)
+
+_RequiredStandardsControlAssociationDetailTypeDef = TypedDict(
+    "_RequiredStandardsControlAssociationDetailTypeDef",
+    {
+        "StandardsArn": str,
+        "SecurityControlId": str,
+        "SecurityControlArn": str,
+        "AssociationStatus": AssociationStatusType,
+    },
+)
+_OptionalStandardsControlAssociationDetailTypeDef = TypedDict(
+    "_OptionalStandardsControlAssociationDetailTypeDef",
+    {
+        "RelatedRequirements": List[str],
+        "UpdatedAt": datetime,
+        "UpdatedReason": str,
+        "StandardsControlTitle": str,
+        "StandardsControlDescription": str,
+        "StandardsControlArns": List[str],
     },
     total=False,
 )
 
+
+class StandardsControlAssociationDetailTypeDef(
+    _RequiredStandardsControlAssociationDetailTypeDef,
+    _OptionalStandardsControlAssociationDetailTypeDef,
+):
+    pass
+
+
+ImportFindingsErrorTypeDef = TypedDict(
+    "ImportFindingsErrorTypeDef",
+    {
+        "Id": str,
+        "ErrorCode": str,
+        "ErrorMessage": str,
+    },
+)
+
+_RequiredStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_RequiredStandardsControlAssociationUpdateTypeDef",
+    {
+        "StandardsArn": str,
+        "SecurityControlId": str,
+        "AssociationStatus": AssociationStatusType,
+    },
+)
+_OptionalStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_OptionalStandardsControlAssociationUpdateTypeDef",
+    {
+        "UpdatedReason": str,
+    },
+    total=False,
+)
+
+
+class StandardsControlAssociationUpdateTypeDef(
+    _RequiredStandardsControlAssociationUpdateTypeDef,
+    _OptionalStandardsControlAssociationUpdateTypeDef,
+):
+    pass
+
+
 CellTypeDef = TypedDict(
     "CellTypeDef",
     {
         "Column": int,
         "Row": int,
         "ColumnName": str,
         "CellReference": str,
@@ -3405,17 +4234,19 @@
     "_OptionalStatusReasonTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class StatusReasonTypeDef(_RequiredStatusReasonTypeDef, _OptionalStatusReasonTypeDef):
     pass
 
+
 VolumeMountTypeDef = TypedDict(
     "VolumeMountTypeDef",
     {
         "Name": str,
         "MountPath": str,
     },
     total=False,
@@ -3426,34 +4257,71 @@
     {
         "Name": str,
         "Description": str,
         "Id": str,
     },
 )
 
+CreateActionTargetResponseTypeDef = TypedDict(
+    "CreateActionTargetResponseTypeDef",
+    {
+        "ActionTargetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAutomationRuleResponseTypeDef = TypedDict(
+    "CreateAutomationRuleResponseTypeDef",
+    {
+        "RuleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFindingAggregatorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFindingAggregatorRequestRequestTypeDef",
     {
         "RegionLinkingMode": str,
     },
 )
 _OptionalCreateFindingAggregatorRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFindingAggregatorRequestRequestTypeDef",
     {
         "Regions": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateFindingAggregatorRequestRequestTypeDef(
     _RequiredCreateFindingAggregatorRequestRequestTypeDef,
     _OptionalCreateFindingAggregatorRequestRequestTypeDef,
 ):
     pass
 
+
+CreateFindingAggregatorResponseTypeDef = TypedDict(
+    "CreateFindingAggregatorResponseTypeDef",
+    {
+        "FindingAggregatorArn": str,
+        "FindingAggregationRegion": str,
+        "RegionLinkingMode": str,
+        "Regions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateInsightResponseTypeDef = TypedDict(
+    "CreateInsightResponseTypeDef",
+    {
+        "InsightArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResultTypeDef = TypedDict(
     "ResultTypeDef",
     {
         "AccountId": str,
         "ProcessingResult": str,
     },
     total=False,
@@ -3478,48 +4346,63 @@
 DeleteActionTargetRequestRequestTypeDef = TypedDict(
     "DeleteActionTargetRequestRequestTypeDef",
     {
         "ActionTargetArn": str,
     },
 )
 
+DeleteActionTargetResponseTypeDef = TypedDict(
+    "DeleteActionTargetResponseTypeDef",
+    {
+        "ActionTargetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteFindingAggregatorRequestRequestTypeDef = TypedDict(
     "DeleteFindingAggregatorRequestRequestTypeDef",
     {
         "FindingAggregatorArn": str,
     },
 )
 
 DeleteInsightRequestRequestTypeDef = TypedDict(
     "DeleteInsightRequestRequestTypeDef",
     {
         "InsightArn": str,
     },
 )
 
+DeleteInsightResponseTypeDef = TypedDict(
+    "DeleteInsightResponseTypeDef",
+    {
+        "InsightArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteInvitationsRequestRequestTypeDef = TypedDict(
     "DeleteInvitationsRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
 DeleteMembersRequestRequestTypeDef = TypedDict(
     "DeleteMembersRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef = TypedDict(
+    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ActionTargetArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeActionTargetsRequestRequestTypeDef = TypedDict(
     "DescribeActionTargetsRequestRequestTypeDef",
     {
@@ -3534,14 +4417,44 @@
     "DescribeHubRequestRequestTypeDef",
     {
         "HubArn": str,
     },
     total=False,
 )
 
+DescribeHubResponseTypeDef = TypedDict(
+    "DescribeHubResponseTypeDef",
+    {
+        "HubArn": str,
+        "SubscribedAt": str,
+        "AutoEnableControls": bool,
+        "ControlFindingGenerator": ControlFindingGeneratorType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    {
+        "AutoEnable": bool,
+        "MemberAccountLimitReached": bool,
+        "AutoEnableStandards": AutoEnableStandardsType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeProductsRequestDescribeProductsPaginateTypeDef = TypedDict(
+    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
+    {
+        "ProductArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeProductsRequestRequestTypeDef = TypedDict(
     "DescribeProductsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ProductArn": str,
     },
@@ -3565,17 +4478,41 @@
         "MarketplaceUrl": str,
         "ActivationUrl": str,
         "ProductSubscriptionResourcePolicy": str,
     },
     total=False,
 )
 
+
 class ProductTypeDef(_RequiredProductTypeDef, _OptionalProductTypeDef):
     pass
 
+
+_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
+    {
+        "StandardsSubscriptionArn": str,
+    },
+)
+_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef(
+    _RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
+    _OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeStandardsControlsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeStandardsControlsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArn": str,
     },
 )
 _OptionalDescribeStandardsControlsRequestRequestTypeDef = TypedDict(
@@ -3583,20 +4520,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeStandardsControlsRequestRequestTypeDef(
     _RequiredDescribeStandardsControlsRequestRequestTypeDef,
     _OptionalDescribeStandardsControlsRequestRequestTypeDef,
 ):
     pass
 
+
 StandardsControlTypeDef = TypedDict(
     "StandardsControlTypeDef",
     {
         "StandardsControlArn": str,
         "ControlStatus": ControlStatusType,
         "DisabledReason": str,
         "ControlStatusUpdatedAt": datetime,
@@ -3606,30 +4545,27 @@
         "RemediationUrl": str,
         "SeverityRating": SeverityRatingType,
         "RelatedRequirements": List[str],
     },
     total=False,
 )
 
-DescribeStandardsRequestRequestTypeDef = TypedDict(
-    "DescribeStandardsRequestRequestTypeDef",
+DescribeStandardsRequestDescribeStandardsPaginateTypeDef = TypedDict(
+    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-StandardTypeDef = TypedDict(
-    "StandardTypeDef",
+DescribeStandardsRequestRequestTypeDef = TypedDict(
+    "DescribeStandardsRequestRequestTypeDef",
     {
-        "StandardsArn": str,
-        "Name": str,
-        "Description": str,
-        "EnabledByDefault": bool,
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
 DisableImportFindingsForProductRequestRequestTypeDef = TypedDict(
     "DisableImportFindingsForProductRequestRequestTypeDef",
     {
@@ -3654,26 +4590,35 @@
 EnableImportFindingsForProductRequestRequestTypeDef = TypedDict(
     "EnableImportFindingsForProductRequestRequestTypeDef",
     {
         "ProductArn": str,
     },
 )
 
+EnableImportFindingsForProductResponseTypeDef = TypedDict(
+    "EnableImportFindingsForProductResponseTypeDef",
+    {
+        "ProductSubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnableOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     {
         "AdminAccountId": str,
     },
 )
 
 EnableSecurityHubRequestRequestTypeDef = TypedDict(
     "EnableSecurityHubRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
         "EnableDefaultStandards": bool,
+        "ControlFindingGenerator": ControlFindingGeneratorType,
     },
     total=False,
 )
 
 FilePathsTypeDef = TypedDict(
     "FilePathsTypeDef",
     {
@@ -3689,14 +4634,33 @@
     "FindingAggregatorTypeDef",
     {
         "FindingAggregatorArn": str,
     },
     total=False,
 )
 
+FindingHistoryUpdateSourceTypeDef = TypedDict(
+    "FindingHistoryUpdateSourceTypeDef",
+    {
+        "Type": FindingHistoryUpdateSourceTypeType,
+        "Identity": str,
+    },
+    total=False,
+)
+
+FindingHistoryUpdateTypeDef = TypedDict(
+    "FindingHistoryUpdateTypeDef",
+    {
+        "UpdatedField": str,
+        "OldValue": str,
+        "NewValue": str,
+    },
+    total=False,
+)
+
 FindingProviderSeverityTypeDef = TypedDict(
     "FindingProviderSeverityTypeDef",
     {
         "Label": SeverityLabelType,
         "Original": str,
     },
     total=False,
@@ -3726,14 +4690,23 @@
         "InvitationId": str,
         "InvitedAt": datetime,
         "MemberStatus": str,
     },
     total=False,
 )
 
+GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef = TypedDict(
+    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
+    {
+        "StandardsSubscriptionArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetEnabledStandardsRequestRequestTypeDef = TypedDict(
     "GetEnabledStandardsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -3743,14 +4716,25 @@
 GetFindingAggregatorRequestRequestTypeDef = TypedDict(
     "GetFindingAggregatorRequestRequestTypeDef",
     {
         "FindingAggregatorArn": str,
     },
 )
 
+GetFindingAggregatorResponseTypeDef = TypedDict(
+    "GetFindingAggregatorResponseTypeDef",
+    {
+        "FindingAggregatorArn": str,
+        "FindingAggregationRegion": str,
+        "RegionLinkingMode": str,
+        "Regions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SortCriterionTypeDef = TypedDict(
     "SortCriterionTypeDef",
     {
         "Field": str,
         "SortOrder": SortOrderType,
     },
     total=False,
@@ -3759,24 +4743,41 @@
 GetInsightResultsRequestRequestTypeDef = TypedDict(
     "GetInsightResultsRequestRequestTypeDef",
     {
         "InsightArn": str,
     },
 )
 
+GetInsightsRequestGetInsightsPaginateTypeDef = TypedDict(
+    "GetInsightsRequestGetInsightsPaginateTypeDef",
+    {
+        "InsightArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetInsightsRequestRequestTypeDef = TypedDict(
     "GetInsightsRequestRequestTypeDef",
     {
         "InsightArns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "InvitationsCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMembersRequestRequestTypeDef = TypedDict(
     "GetMembersRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
@@ -3805,67 +4806,239 @@
 InviteMembersRequestRequestTypeDef = TypedDict(
     "InviteMembersRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
+ListAutomationRulesRequestRequestTypeDef = TypedDict(
+    "ListAutomationRulesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef = TypedDict(
+    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEnabledProductsForImportRequestRequestTypeDef = TypedDict(
     "ListEnabledProductsForImportRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListEnabledProductsForImportResponseTypeDef = TypedDict(
+    "ListEnabledProductsForImportResponseTypeDef",
+    {
+        "ProductSubscriptions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef = TypedDict(
+    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFindingAggregatorsRequestRequestTypeDef = TypedDict(
     "ListFindingAggregatorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
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
 
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "OnlyAssociated": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMembersRequestRequestTypeDef = TypedDict(
     "ListMembersRequestRequestTypeDef",
     {
         "OnlyAssociated": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
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
 )
 
+ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef = TypedDict(
+    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
+    {
+        "StandardsArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListSecurityControlDefinitionsRequestRequestTypeDef = TypedDict(
+    "ListSecurityControlDefinitionsRequestRequestTypeDef",
+    {
+        "StandardsArn": str,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+SecurityControlDefinitionTypeDef = TypedDict(
+    "SecurityControlDefinitionTypeDef",
+    {
+        "SecurityControlId": str,
+        "Title": str,
+        "Description": str,
+        "RemediationUrl": str,
+        "SeverityRating": SeverityRatingType,
+        "CurrentRegionAvailability": RegionAvailabilityStatusType,
+    },
+)
+
+_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
+    {
+        "SecurityControlId": str,
+    },
+)
+_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef(
+    _RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
+    _OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
+    "_RequiredListStandardsControlAssociationsRequestRequestTypeDef",
+    {
+        "SecurityControlId": str,
+    },
+)
+_OptionalListStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
+    "_OptionalListStandardsControlAssociationsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListStandardsControlAssociationsRequestRequestTypeDef(
+    _RequiredListStandardsControlAssociationsRequestRequestTypeDef,
+    _OptionalListStandardsControlAssociationsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStandardsControlAssociationSummaryTypeDef = TypedDict(
+    "_RequiredStandardsControlAssociationSummaryTypeDef",
+    {
+        "StandardsArn": str,
+        "SecurityControlId": str,
+        "SecurityControlArn": str,
+        "AssociationStatus": AssociationStatusType,
+    },
+)
+_OptionalStandardsControlAssociationSummaryTypeDef = TypedDict(
+    "_OptionalStandardsControlAssociationSummaryTypeDef",
+    {
+        "RelatedRequirements": List[str],
+        "UpdatedAt": datetime,
+        "UpdatedReason": str,
+        "StandardsControlTitle": str,
+        "StandardsControlDescription": str,
+    },
+    total=False,
+)
+
+
+class StandardsControlAssociationSummaryTypeDef(
+    _RequiredStandardsControlAssociationSummaryTypeDef,
+    _OptionalStandardsControlAssociationSummaryTypeDef,
+):
+    pass
+
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
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "Begin": int,
         "End": int,
     },
     total=False,
@@ -3886,23 +5059,44 @@
     {
         "JsonPath": str,
         "RecordIndex": int,
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
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Text": str,
         "Url": str,
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
 RuleGroupSourceListDetailsTypeDef = TypedDict(
     "RuleGroupSourceListDetailsTypeDef",
     {
         "GeneratedRulesType": str,
         "TargetTypes": Sequence[str],
         "Targets": Sequence[str],
     },
@@ -3998,14 +5192,25 @@
         "Epoch": str,
         "Release": str,
         "Architecture": str,
         "PackageManager": str,
         "FilePath": str,
         "FixedInVersion": str,
         "Remediation": str,
+        "SourceLayerHash": str,
+        "SourceLayerArn": str,
+    },
+    total=False,
+)
+
+StandardsManagedByTypeDef = TypedDict(
+    "StandardsManagedByTypeDef",
+    {
+        "Company": str,
+        "Product": str,
     },
     total=False,
 )
 
 StandardsStatusReasonTypeDef = TypedDict(
     "StandardsStatusReasonTypeDef",
     {
@@ -4048,20 +5253,22 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateActionTargetRequestRequestTypeDef(
     _RequiredUpdateActionTargetRequestRequestTypeDef,
     _OptionalUpdateActionTargetRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateFindingAggregatorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFindingAggregatorRequestRequestTypeDef",
     {
         "FindingAggregatorArn": str,
         "RegionLinkingMode": str,
     },
 )
@@ -4069,44 +5276,60 @@
     "_OptionalUpdateFindingAggregatorRequestRequestTypeDef",
     {
         "Regions": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateFindingAggregatorRequestRequestTypeDef(
     _RequiredUpdateFindingAggregatorRequestRequestTypeDef,
     _OptionalUpdateFindingAggregatorRequestRequestTypeDef,
 ):
     pass
 
+
+UpdateFindingAggregatorResponseTypeDef = TypedDict(
+    "UpdateFindingAggregatorResponseTypeDef",
+    {
+        "FindingAggregatorArn": str,
+        "FindingAggregationRegion": str,
+        "RegionLinkingMode": str,
+        "Regions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "AutoEnable": bool,
     },
 )
 _OptionalUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "AutoEnableStandards": AutoEnableStandardsType,
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
 UpdateSecurityHubConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateSecurityHubConfigurationRequestRequestTypeDef",
     {
         "AutoEnableControls": bool,
+        "ControlFindingGenerator": ControlFindingGeneratorType,
     },
     total=False,
 )
 
 _RequiredUpdateStandardsControlRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStandardsControlRequestRequestTypeDef",
     {
@@ -4118,20 +5341,22 @@
     {
         "ControlStatus": ControlStatusType,
         "DisabledReason": str,
     },
     total=False,
 )
 
+
 class UpdateStandardsControlRequestRequestTypeDef(
     _RequiredUpdateStandardsControlRequestRequestTypeDef,
     _OptionalUpdateStandardsControlRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredVulnerabilityVendorTypeDef = TypedDict(
     "_RequiredVulnerabilityVendorTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalVulnerabilityVendorTypeDef = TypedDict(
@@ -4141,19 +5366,21 @@
         "VendorSeverity": str,
         "VendorCreatedAt": str,
         "VendorUpdatedAt": str,
     },
     total=False,
 )
 
+
 class VulnerabilityVendorTypeDef(
     _RequiredVulnerabilityVendorTypeDef, _OptionalVulnerabilityVendorTypeDef
 ):
     pass
 
+
 CreateMembersRequestRequestTypeDef = TypedDict(
     "CreateMembersRequestRequestTypeDef",
     {
         "AccountDetails": Sequence[AccountDetailsTypeDef],
     },
 )
 
@@ -4165,26 +5392,94 @@
         "Country": CountryTypeDef,
         "City": CityTypeDef,
         "GeoLocation": GeoLocationTypeDef,
     },
     total=False,
 )
 
+DescribeActionTargetsResponseTypeDef = TypedDict(
+    "DescribeActionTargetsResponseTypeDef",
+    {
+        "ActionTargets": List[ActionTargetTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CvssTypeDef = TypedDict(
     "CvssTypeDef",
     {
         "Version": str,
         "BaseScore": float,
         "BaseVector": str,
         "Source": str,
         "Adjustments": Sequence[AdjustmentTypeDef],
     },
     total=False,
 )
 
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AssociationSetDetailsTypeDef = TypedDict(
+    "AssociationSetDetailsTypeDef",
+    {
+        "AssociationState": AssociationStateDetailsTypeDef,
+        "GatewayId": str,
+        "Main": bool,
+        "RouteTableAssociationId": str,
+        "RouteTableId": str,
+        "SubnetId": str,
+    },
+    total=False,
+)
+
+AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
+    "AutomationRulesFindingFieldsUpdateTypeDef",
+    {
+        "Note": NoteUpdateTypeDef,
+        "Severity": SeverityUpdateTypeDef,
+        "VerificationState": VerificationStateType,
+        "Confidence": int,
+        "Criticality": int,
+        "Types": List[str],
+        "UserDefinedFields": Dict[str, str],
+        "Workflow": WorkflowUpdateTypeDef,
+        "RelatedFindings": List[RelatedFindingTypeDef],
+    },
+    total=False,
+)
+
+ListAutomationRulesResponseTypeDef = TypedDict(
+    "ListAutomationRulesResponseTypeDef",
+    {
+        "AutomationRulesMetadata": List[AutomationRulesMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AwsAmazonMqBrokerLogsDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLogsDetailsTypeDef",
+    {
+        "Audit": bool,
+        "General": bool,
+        "AuditLogGroup": str,
+        "GeneralLogGroup": str,
+        "Pending": AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsApiGatewayRestApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayRestApiDetailsTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "CreatedDate": str,
@@ -4253,14 +5548,25 @@
         "AutoDeploy": bool,
         "LastDeploymentStatusMessage": str,
         "ApiGatewayManaged": bool,
     },
     total=False,
 )
 
+AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
+    {
+        "AuthenticationType": str,
+        "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
+        "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
+        "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
     {
         "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
         ],
@@ -4490,14 +5796,118 @@
         "IamInstanceProfileArn": str,
         "VpcId": str,
         "SubnetId": str,
         "LaunchedAt": str,
         "NetworkInterfaces": Sequence[AwsEc2InstanceNetworkInterfacesDetailsTypeDef],
         "VirtualizationType": str,
         "MetadataOptions": AwsEc2InstanceMetadataOptionsTypeDef,
+        "Monitoring": AwsEc2InstanceMonitoringDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
+    {
+        "DeviceName": str,
+        "Ebs": AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
+        "NoDevice": str,
+        "VirtualName": str,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
+    {
+        "CapacityReservationPreference": str,
+        "CapacityReservationTarget": AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
+    {
+        "MarketType": str,
+        "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
+    {
+        "AcceleratorCount": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
+        ),
+        "AcceleratorManufacturers": Sequence[str],
+        "AcceleratorNames": Sequence[str],
+        "AcceleratorTotalMemoryMiB": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef
+        ),
+        "AcceleratorTypes": Sequence[str],
+        "BareMetal": str,
+        "BaselineEbsBandwidthMbps": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef
+        ),
+        "BurstablePerformance": str,
+        "CpuManufacturers": Sequence[str],
+        "ExcludedInstanceTypes": Sequence[str],
+        "InstanceGenerations": Sequence[str],
+        "LocalStorage": str,
+        "LocalStorageTypes": Sequence[str],
+        "MemoryGiBPerVCpu": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef
+        ),
+        "MemoryMiB": AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
+        "NetworkInterfaceCount": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef
+        ),
+        "OnDemandMaxPricePercentageOverLowestPrice": int,
+        "RequireHibernateSupport": bool,
+        "SpotMaxPricePercentageOverLowestPrice": int,
+        "TotalLocalStorageGB": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
+        ),
+        "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
+    {
+        "AssociateCarrierIpAddress": bool,
+        "AssociatePublicIpAddress": bool,
+        "DeleteOnTermination": bool,
+        "Description": str,
+        "DeviceIndex": int,
+        "Groups": Sequence[str],
+        "InterfaceType": str,
+        "Ipv4PrefixCount": int,
+        "Ipv4Prefixes": Sequence[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef
+        ],
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": Sequence[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef
+        ],
+        "Ipv6PrefixCount": int,
+        "Ipv6Prefixes": Sequence[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef
+        ],
+        "NetworkCardIndex": int,
+        "NetworkInterfaceId": str,
+        "PrivateIpAddress": str,
+        "PrivateIpAddresses": Sequence[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef
+        ],
+        "SecondaryPrivateIpAddressCount": int,
+        "SubnetId": str,
     },
     total=False,
 )
 
 AwsEc2NetworkAclEntryTypeDef = TypedDict(
     "AwsEc2NetworkAclEntryTypeDef",
     {
@@ -4645,15 +6055,17 @@
     total=False,
 )
 
 AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
     {
         "KmsKeyId": str,
-        "LogConfiguration": AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef,
+        "LogConfiguration": (
+            AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef
+        ),
         "Logging": str,
     },
     total=False,
 )
 
 AwsEcsContainerDetailsTypeDef = TypedDict(
     "AwsEcsContainerDetailsTypeDef",
@@ -4665,15 +6077,17 @@
     },
     total=False,
 )
 
 AwsEcsServiceDeploymentConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
     {
-        "DeploymentCircuitBreaker": AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef,
+        "DeploymentCircuitBreaker": (
+            AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef
+        ),
         "MaximumPercent": int,
         "MinimumHealthyPercent": int,
     },
     total=False,
 )
 
 AwsEcsServiceNetworkConfigurationDetailsTypeDef = TypedDict(
@@ -4683,15 +6097,17 @@
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
     {
-        "Capabilities": AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef,
+        "Capabilities": (
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef
+        ),
         "Devices": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef
         ],
         "InitProcessEnabled": bool,
         "MaxSwap": int,
         "SharedMemorySize": int,
         "Swappiness": int,
@@ -4725,15 +6141,17 @@
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
     {
-        "AuthorizationConfig": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef,
+        "AuthorizationConfig": (
+            AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef
+        ),
         "FilesystemId": str,
         "RootDirectory": str,
         "TransitEncryption": str,
         "TransitEncryptionPort": int,
     },
     total=False,
 )
@@ -4791,15 +6209,17 @@
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     {
         "DedicatedMasterCount": int,
         "DedicatedMasterEnabled": bool,
         "DedicatedMasterType": str,
         "InstanceCount": int,
         "InstanceType": str,
-        "ZoneAwarenessConfig": AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef,
+        "ZoneAwarenessConfig": (
+            AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef
+        ),
         "ZoneAwarenessEnabled": bool,
     },
     total=False,
 )
 
 AwsElasticsearchDomainLogPublishingOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
@@ -4856,14 +6276,30 @@
         "Type": str,
         "VpcId": str,
         "LoadBalancerAttributes": Sequence[AwsElbv2LoadBalancerAttributeTypeDef],
     },
     total=False,
 )
 
+AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
+    {
+        "AuditLogs": AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
+    {
+        "EbsVolumes": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsIamAccessKeySessionContextTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextTypeDef",
     {
         "Attributes": AwsIamAccessKeySessionContextAttributesTypeDef,
         "SessionIssuer": AwsIamAccessKeySessionContextSessionIssuerTypeDef,
     },
     total=False,
@@ -4979,15 +6415,17 @@
 AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
     {
         "InstanceCount": int,
         "WarmEnabled": bool,
         "WarmCount": int,
         "DedicatedMasterEnabled": bool,
-        "ZoneAwarenessConfig": AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef,
+        "ZoneAwarenessConfig": (
+            AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef
+        ),
         "DedicatedMasterCount": int,
         "InstanceType": str,
         "WarmType": str,
         "ZoneAwarenessEnabled": bool,
         "DedicatedMasterType": str,
     },
     total=False,
@@ -5151,14 +6589,22 @@
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     {
         "FilterRules": Sequence[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef],
     },
     total=False,
 )
 
+AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef = TypedDict(
+    "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
+    {
+        "DefaultRetention": AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsS3BucketServerSideEncryptionRuleTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": AwsS3BucketServerSideEncryptionByDefaultTypeDef,
     },
     total=False,
 )
@@ -5168,14 +6614,43 @@
     {
         "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
         "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     },
     total=False,
 )
 
+AwsSageMakerNotebookInstanceDetailsTypeDef = TypedDict(
+    "AwsSageMakerNotebookInstanceDetailsTypeDef",
+    {
+        "AcceleratorTypes": Sequence[str],
+        "AdditionalCodeRepositories": Sequence[str],
+        "DefaultCodeRepository": str,
+        "DirectInternetAccess": str,
+        "FailureReason": str,
+        "InstanceMetadataServiceConfiguration": (
+            AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef
+        ),
+        "InstanceType": str,
+        "KmsKeyId": str,
+        "NetworkInterfaceId": str,
+        "NotebookInstanceArn": str,
+        "NotebookInstanceLifecycleConfigName": str,
+        "NotebookInstanceName": str,
+        "NotebookInstanceStatus": str,
+        "PlatformIdentifier": str,
+        "RoleArn": str,
+        "RootAccess": str,
+        "SecurityGroups": Sequence[str],
+        "SubnetId": str,
+        "Url": str,
+        "VolumeSizeInGB": int,
+    },
+    total=False,
+)
+
 AwsSecretsManagerSecretDetailsTypeDef = TypedDict(
     "AwsSecretsManagerSecretDetailsTypeDef",
     {
         "RotationRules": AwsSecretsManagerSecretRotationRulesTypeDef,
         "RotationOccurredWithinFrequency": bool,
         "KmsKeyId": str,
         "RotationEnabled": bool,
@@ -5183,23 +6658,101 @@
         "Deleted": bool,
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+_RequiredBatchUpdateFindingsRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchUpdateFindingsRequestRequestTypeDef",
+    {
+        "FindingIdentifiers": Sequence[AwsSecurityFindingIdentifierTypeDef],
+    },
+)
+_OptionalBatchUpdateFindingsRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchUpdateFindingsRequestRequestTypeDef",
+    {
+        "Note": NoteUpdateTypeDef,
+        "Severity": SeverityUpdateTypeDef,
+        "VerificationState": VerificationStateType,
+        "Confidence": int,
+        "Criticality": int,
+        "Types": Sequence[str],
+        "UserDefinedFields": Mapping[str, str],
+        "Workflow": WorkflowUpdateTypeDef,
+        "RelatedFindings": Sequence[RelatedFindingTypeDef],
+    },
+    total=False,
+)
+
+
+class BatchUpdateFindingsRequestRequestTypeDef(
+    _RequiredBatchUpdateFindingsRequestRequestTypeDef,
+    _OptionalBatchUpdateFindingsRequestRequestTypeDef,
+):
+    pass
+
+
 BatchUpdateFindingsUnprocessedFindingTypeDef = TypedDict(
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
+_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+    },
+)
+_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef(
+    _RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    _OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetFindingHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetFindingHistoryRequestRequestTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+    },
+)
+_OptionalGetFindingHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetFindingHistoryRequestRequestTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class GetFindingHistoryRequestRequestTypeDef(
+    _RequiredGetFindingHistoryRequestRequestTypeDef, _OptionalGetFindingHistoryRequestRequestTypeDef
+):
+    pass
+
+
 AwsSnsTopicDetailsTypeDef = TypedDict(
     "AwsSnsTopicDetailsTypeDef",
     {
         "KmsMasterKeyId": str,
         "Subscription": Sequence[AwsSnsTopicSubscriptionTypeDef],
         "TopicName": str,
         "Owner": str,
@@ -5218,14 +6771,22 @@
     "AwsSsmPatchTypeDef",
     {
         "ComplianceSummary": AwsSsmComplianceSummaryTypeDef,
     },
     total=False,
 )
 
+AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
+    {
+        "CloudWatchLogsLogGroup": AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsWafRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRateBasedRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
@@ -5313,201 +6874,152 @@
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
-CreateActionTargetResponseTypeDef = TypedDict(
-    "CreateActionTargetResponseTypeDef",
+AwsWafv2CustomRequestHandlingDetailsTypeDef = TypedDict(
+    "AwsWafv2CustomRequestHandlingDetailsTypeDef",
     {
-        "ActionTargetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFindingAggregatorResponseTypeDef = TypedDict(
-    "CreateFindingAggregatorResponseTypeDef",
-    {
-        "FindingAggregatorArn": str,
-        "FindingAggregationRegion": str,
-        "RegionLinkingMode": str,
-        "Regions": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateInsightResponseTypeDef = TypedDict(
-    "CreateInsightResponseTypeDef",
-    {
-        "InsightArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteActionTargetResponseTypeDef = TypedDict(
-    "DeleteActionTargetResponseTypeDef",
-    {
-        "ActionTargetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "InsertHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
+    total=False,
 )
 
-DeleteInsightResponseTypeDef = TypedDict(
-    "DeleteInsightResponseTypeDef",
+AwsWafv2CustomResponseDetailsTypeDef = TypedDict(
+    "AwsWafv2CustomResponseDetailsTypeDef",
     {
-        "InsightArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CustomResponseBodyKey": str,
+        "ResponseCode": int,
+        "ResponseHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
+    total=False,
 )
 
-DescribeActionTargetsResponseTypeDef = TypedDict(
-    "DescribeActionTargetsResponseTypeDef",
+AwsWafv2WebAclCaptchaConfigDetailsTypeDef = TypedDict(
+    "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     {
-        "ActionTargets": List[ActionTargetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ImmunityTimeProperty": AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     },
+    total=False,
 )
 
-DescribeHubResponseTypeDef = TypedDict(
-    "DescribeHubResponseTypeDef",
+BatchDeleteAutomationRulesResponseTypeDef = TypedDict(
+    "BatchDeleteAutomationRulesResponseTypeDef",
     {
-        "HubArn": str,
-        "SubscribedAt": str,
-        "AutoEnableControls": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProcessedAutomationRules": List[str],
+        "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
-    "DescribeOrganizationConfigurationResponseTypeDef",
+BatchUpdateAutomationRulesResponseTypeDef = TypedDict(
+    "BatchUpdateAutomationRulesResponseTypeDef",
     {
-        "AutoEnable": bool,
-        "MemberAccountLimitReached": bool,
-        "AutoEnableStandards": AutoEnableStandardsType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProcessedAutomationRules": List[str],
+        "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EnableImportFindingsForProductResponseTypeDef = TypedDict(
-    "EnableImportFindingsForProductResponseTypeDef",
+BatchEnableStandardsRequestRequestTypeDef = TypedDict(
+    "BatchEnableStandardsRequestRequestTypeDef",
     {
-        "ProductSubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StandardsSubscriptionRequests": Sequence[StandardsSubscriptionRequestTypeDef],
     },
 )
 
-GetFindingAggregatorResponseTypeDef = TypedDict(
-    "GetFindingAggregatorResponseTypeDef",
+BatchGetSecurityControlsResponseTypeDef = TypedDict(
+    "BatchGetSecurityControlsResponseTypeDef",
     {
-        "FindingAggregatorArn": str,
-        "FindingAggregationRegion": str,
-        "RegionLinkingMode": str,
-        "Regions": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SecurityControls": List[SecurityControlTypeDef],
+        "UnprocessedIds": List[UnprocessedSecurityControlTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
+BatchGetStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
+    "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
     {
-        "InvitationsCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StandardsControlAssociationIds": Sequence[StandardsControlAssociationIdTypeDef],
     },
 )
 
-ListEnabledProductsForImportResponseTypeDef = TypedDict(
-    "ListEnabledProductsForImportResponseTypeDef",
+_RequiredUnprocessedStandardsControlAssociationTypeDef = TypedDict(
+    "_RequiredUnprocessedStandardsControlAssociationTypeDef",
     {
-        "ProductSubscriptions": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StandardsControlAssociationId": StandardsControlAssociationIdTypeDef,
+        "ErrorCode": UnprocessedErrorCodeType,
     },
 )
-
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
+_OptionalUnprocessedStandardsControlAssociationTypeDef = TypedDict(
+    "_OptionalUnprocessedStandardsControlAssociationTypeDef",
     {
-        "AdminAccounts": List[AdminAccountTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ErrorReason": str,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateFindingAggregatorResponseTypeDef = TypedDict(
-    "UpdateFindingAggregatorResponseTypeDef",
-    {
-        "FindingAggregatorArn": str,
-        "FindingAggregationRegion": str,
-        "RegionLinkingMode": str,
-        "Regions": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UnprocessedStandardsControlAssociationTypeDef(
+    _RequiredUnprocessedStandardsControlAssociationTypeDef,
+    _OptionalUnprocessedStandardsControlAssociationTypeDef,
+):
+    pass
 
-BatchEnableStandardsRequestRequestTypeDef = TypedDict(
-    "BatchEnableStandardsRequestRequestTypeDef",
-    {
-        "StandardsSubscriptionRequests": Sequence[StandardsSubscriptionRequestTypeDef],
-    },
-)
 
 BatchImportFindingsResponseTypeDef = TypedDict(
     "BatchImportFindingsResponseTypeDef",
     {
         "FailedCount": int,
         "SuccessCount": int,
         "FailedFindings": List[ImportFindingsErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredBatchUpdateFindingsRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchUpdateFindingsRequestRequestTypeDef",
+BatchUpdateStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
+    "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
     {
-        "FindingIdentifiers": Sequence[AwsSecurityFindingIdentifierTypeDef],
+        "StandardsControlAssociationUpdates": Sequence[StandardsControlAssociationUpdateTypeDef],
     },
 )
-_OptionalBatchUpdateFindingsRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchUpdateFindingsRequestRequestTypeDef",
+
+_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef",
     {
-        "Note": NoteUpdateTypeDef,
-        "Severity": SeverityUpdateTypeDef,
-        "VerificationState": VerificationStateType,
-        "Confidence": int,
-        "Criticality": int,
-        "Types": Sequence[str],
-        "UserDefinedFields": Mapping[str, str],
-        "Workflow": WorkflowUpdateTypeDef,
-        "RelatedFindings": Sequence[RelatedFindingTypeDef],
+        "StandardsControlAssociationUpdate": StandardsControlAssociationUpdateTypeDef,
+        "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef",
+    {
+        "ErrorReason": str,
     },
     total=False,
 )
 
-class BatchUpdateFindingsRequestRequestTypeDef(
-    _RequiredBatchUpdateFindingsRequestRequestTypeDef,
-    _OptionalBatchUpdateFindingsRequestRequestTypeDef,
+
+class UnprocessedStandardsControlAssociationUpdateTypeDef(
+    _RequiredUnprocessedStandardsControlAssociationUpdateTypeDef,
+    _OptionalUnprocessedStandardsControlAssociationUpdateTypeDef,
 ):
     pass
 
+
 ComplianceTypeDef = TypedDict(
     "ComplianceTypeDef",
     {
         "Status": ComplianceStatusType,
         "RelatedRequirements": Sequence[str],
         "StatusReasons": Sequence[StatusReasonTypeDef],
+        "SecurityControlId": str,
+        "AssociatedStandards": Sequence[AssociatedStandardTypeDef],
     },
     total=False,
 )
 
 ContainerDetailsTypeDef = TypedDict(
     "ContainerDetailsTypeDef",
     {
@@ -5522,189 +7034,75 @@
     total=False,
 )
 
 CreateMembersResponseTypeDef = TypedDict(
     "CreateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteMembersResponseTypeDef = TypedDict(
     "DeleteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InviteMembersResponseTypeDef = TypedDict(
     "InviteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DateFilterTypeDef = TypedDict(
     "DateFilterTypeDef",
     {
         "Start": str,
         "End": str,
         "DateRange": DateRangeTypeDef,
     },
     total=False,
 )
 
-DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef = TypedDict(
-    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
-    {
-        "ActionTargetArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeProductsRequestDescribeProductsPaginateTypeDef = TypedDict(
-    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
-    {
-        "ProductArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
-    {
-        "StandardsSubscriptionArn": str,
-    },
-)
-_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef(
-    _RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
-    _OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
-):
-    pass
-
-DescribeStandardsRequestDescribeStandardsPaginateTypeDef = TypedDict(
-    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef = TypedDict(
-    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
-    {
-        "StandardsSubscriptionArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetInsightsRequestGetInsightsPaginateTypeDef = TypedDict(
-    "GetInsightsRequestGetInsightsPaginateTypeDef",
-    {
-        "InsightArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef = TypedDict(
-    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef = TypedDict(
-    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "OnlyAssociated": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeProductsResponseTypeDef = TypedDict(
     "DescribeProductsResponseTypeDef",
     {
         "Products": List[ProductTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStandardsControlsResponseTypeDef = TypedDict(
     "DescribeStandardsControlsResponseTypeDef",
     {
         "Controls": List[StandardsControlTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeStandardsResponseTypeDef = TypedDict(
-    "DescribeStandardsResponseTypeDef",
-    {
-        "Standards": List[StandardTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ThreatTypeDef = TypedDict(
     "ThreatTypeDef",
     {
         "Name": str,
@@ -5716,16 +7114,29 @@
 )
 
 ListFindingAggregatorsResponseTypeDef = TypedDict(
     "ListFindingAggregatorsResponseTypeDef",
     {
         "FindingAggregators": List[FindingAggregatorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FindingHistoryRecordTypeDef = TypedDict(
+    "FindingHistoryRecordTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+        "UpdateTime": datetime,
+        "FindingCreated": bool,
+        "UpdateSource": FindingHistoryUpdateSourceTypeDef,
+        "Updates": List[FindingHistoryUpdateTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
 FindingProviderFieldsTypeDef = TypedDict(
     "FindingProviderFieldsTypeDef",
     {
         "Confidence": int,
         "Criticality": int,
@@ -5736,62 +7147,80 @@
     total=False,
 )
 
 GetAdministratorAccountResponseTypeDef = TypedDict(
     "GetAdministratorAccountResponseTypeDef",
     {
         "Administrator": InvitationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "Master": InvitationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
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
 
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "UnprocessedAccounts": List[ResultTypeDef],
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
 
 InsightResultsTypeDef = TypedDict(
     "InsightResultsTypeDef",
     {
         "InsightArn": str,
         "GroupByAttribute": str,
         "ResultValues": List[InsightResultValueTypeDef],
     },
 )
 
+ListSecurityControlDefinitionsResponseTypeDef = TypedDict(
+    "ListSecurityControlDefinitionsResponseTypeDef",
+    {
+        "SecurityControlDefinitions": List[SecurityControlDefinitionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStandardsControlAssociationsResponseTypeDef = TypedDict(
+    "ListStandardsControlAssociationsResponseTypeDef",
+    {
+        "StandardsControlAssociationSummaries": List[StandardsControlAssociationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NetworkPathComponentDetailsTypeDef = TypedDict(
     "NetworkPathComponentDetailsTypeDef",
     {
         "Address": Sequence[str],
         "PortRanges": Sequence[PortRangeTypeDef],
     },
     total=False,
@@ -5864,14 +7293,26 @@
     {
         "IpSets": RuleGroupVariablesIpSetsDetailsTypeDef,
         "PortSets": RuleGroupVariablesPortSetsDetailsTypeDef,
     },
     total=False,
 )
 
+StandardTypeDef = TypedDict(
+    "StandardTypeDef",
+    {
+        "StandardsArn": str,
+        "Name": str,
+        "Description": str,
+        "EnabledByDefault": bool,
+        "StandardsManagedBy": StandardsManagedByTypeDef,
+    },
+    total=False,
+)
+
 _RequiredStandardsSubscriptionTypeDef = TypedDict(
     "_RequiredStandardsSubscriptionTypeDef",
     {
         "StandardsSubscriptionArn": str,
         "StandardsArn": str,
         "StandardsInput": Dict[str, str],
         "StandardsStatus": StandardsStatusType,
@@ -5881,19 +7322,21 @@
     "_OptionalStandardsSubscriptionTypeDef",
     {
         "StandardsStatusReason": StandardsStatusReasonTypeDef,
     },
     total=False,
 )
 
+
 class StandardsSubscriptionTypeDef(
     _RequiredStandardsSubscriptionTypeDef, _OptionalStandardsSubscriptionTypeDef
 ):
     pass
 
+
 StatelessCustomPublishMetricActionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[StatelessCustomPublishMetricActionDimensionTypeDef],
     },
     total=False,
 )
@@ -5951,22 +7394,96 @@
         "Vendor": VulnerabilityVendorTypeDef,
         "ReferenceUrls": Sequence[str],
         "FixAvailable": VulnerabilityFixAvailableType,
     },
     total=False,
 )
 
+
 class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
     pass
 
+
+AwsEc2RouteTableDetailsTypeDef = TypedDict(
+    "AwsEc2RouteTableDetailsTypeDef",
+    {
+        "AssociationSet": Sequence[AssociationSetDetailsTypeDef],
+        "OwnerId": str,
+        "PropagatingVgwSet": Sequence[PropagatingVgwSetDetailsTypeDef],
+        "RouteTableId": str,
+        "RouteSet": Sequence[RouteSetDetailsTypeDef],
+        "VpcId": str,
+    },
+    total=False,
+)
+
+AutomationRulesActionTypeDef = TypedDict(
+    "AutomationRulesActionTypeDef",
+    {
+        "Type": Literal["FINDING_FIELDS_UPDATE"],
+        "FindingFieldsUpdate": AutomationRulesFindingFieldsUpdateTypeDef,
+    },
+    total=False,
+)
+
+AwsAmazonMqBrokerDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerDetailsTypeDef",
+    {
+        "AuthenticationStrategy": str,
+        "AutoMinorVersionUpgrade": bool,
+        "BrokerArn": str,
+        "BrokerName": str,
+        "DeploymentMode": str,
+        "EncryptionOptions": AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
+        "EngineType": str,
+        "EngineVersion": str,
+        "HostInstanceType": str,
+        "BrokerId": str,
+        "LdapServerMetadata": AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
+        "Logs": AwsAmazonMqBrokerLogsDetailsTypeDef,
+        "MaintenanceWindowStartTime": AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
+        "PubliclyAccessible": bool,
+        "SecurityGroups": Sequence[str],
+        "StorageType": str,
+        "SubnetIds": Sequence[str],
+        "Users": Sequence[AwsAmazonMqBrokerUsersDetailsTypeDef],
+    },
+    total=False,
+)
+
+AwsAppSyncGraphQlApiDetailsTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiDetailsTypeDef",
+    {
+        "ApiId": str,
+        "Id": str,
+        "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
+        "Name": str,
+        "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
+        "XrayEnabled": bool,
+        "Arn": str,
+        "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
+        "AuthenticationType": str,
+        "LogConfig": AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
+        "AdditionalAuthenticationProviders": Sequence[
+            AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef
+        ],
+        "WafWebAclArn": str,
+    },
+    total=False,
+)
+
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     {
-        "InstancesDistribution": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
-        "LaunchTemplate": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
+        "InstancesDistribution": (
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
+        ),
+        "LaunchTemplate": (
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef
+        ),
     },
     total=False,
 )
 
 AwsAutoScalingLaunchConfigurationDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     {
@@ -6069,14 +7586,59 @@
         "RegionName": str,
         "ReplicaStatus": str,
         "ReplicaStatusDescription": str,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDataDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataDetailsTypeDef",
+    {
+        "BlockDeviceMappingSet": Sequence[
+            AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef
+        ],
+        "CapacityReservationSpecification": (
+            AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef
+        ),
+        "CpuOptions": AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
+        "CreditSpecification": AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
+        "DisableApiStop": bool,
+        "DisableApiTermination": bool,
+        "EbsOptimized": bool,
+        "ElasticGpuSpecificationSet": Sequence[
+            AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef
+        ],
+        "ElasticInferenceAcceleratorSet": Sequence[
+            AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef
+        ],
+        "EnclaveOptions": AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
+        "HibernationOptions": AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
+        "IamInstanceProfile": AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
+        "ImageId": str,
+        "InstanceInitiatedShutdownBehavior": str,
+        "InstanceMarketOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
+        "InstanceRequirements": AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
+        "InstanceType": str,
+        "KernelId": str,
+        "KeyName": str,
+        "LicenseSet": Sequence[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef],
+        "MaintenanceOptions": AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
+        "MetadataOptions": AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
+        "Monitoring": AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
+        "NetworkInterfaceSet": Sequence[AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef],
+        "Placement": AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
+        "PrivateDnsNameOptions": AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
+        "RamDiskId": str,
+        "SecurityGroupIdSet": Sequence[str],
+        "SecurityGroupSet": Sequence[str],
+        "UserData": str,
+    },
+    total=False,
+)
+
 AwsEc2NetworkAclDetailsTypeDef = TypedDict(
     "AwsEc2NetworkAclDetailsTypeDef",
     {
         "IsDefault": bool,
         "NetworkAclId": str,
         "OwnerId": str,
         "VpcId": str,
@@ -6128,15 +7690,17 @@
     },
     total=False,
 )
 
 AwsEcsClusterConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationDetailsTypeDef",
     {
-        "ExecuteCommandConfiguration": AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef,
+        "ExecuteCommandConfiguration": (
+            AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef
+        ),
     },
     total=False,
 )
 
 AwsEcsServiceDetailsTypeDef = TypedDict(
     "AwsEcsServiceDetailsTypeDef",
     {
@@ -6180,15 +7744,17 @@
         "EntryPoint": Sequence[str],
         "Environment": Sequence[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef],
         "EnvironmentFiles": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef
         ],
         "Essential": bool,
         "ExtraHosts": Sequence[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef],
-        "FirelensConfiguration": AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
+        "FirelensConfiguration": (
+            AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef
+        ),
         "HealthCheck": AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
         "Hostname": str,
         "Image": str,
         "Interactive": bool,
         "Links": Sequence[str],
         "LinuxParameters": AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef,
         "LogConfiguration": AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef,
@@ -6198,15 +7764,17 @@
         "Name": str,
         "PortMappings": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef
         ],
         "Privileged": bool,
         "PseudoTerminal": bool,
         "ReadonlyRootFilesystem": bool,
-        "RepositoryCredentials": AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef,
+        "RepositoryCredentials": (
+            AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef
+        ),
         "ResourceRequirements": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef
         ],
         "Secrets": Sequence[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef],
         "StartTimeout": int,
         "StopTimeout": int,
         "SystemControls": Sequence[
@@ -6219,15 +7787,17 @@
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
     {
-        "DockerVolumeConfiguration": AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
+        "DockerVolumeConfiguration": (
+            AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef
+        ),
         "EfsVolumeConfiguration": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
         "Host": AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
         "Name": str,
     },
     total=False,
 )
 
@@ -6282,15 +7852,17 @@
         "AccessPolicies": str,
         "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
         "DomainId": str,
         "DomainName": str,
         "Endpoint": str,
         "Endpoints": Mapping[str, str],
         "ElasticsearchVersion": str,
-        "ElasticsearchClusterConfig": AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
+        "ElasticsearchClusterConfig": (
+            AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef
+        ),
         "EncryptionAtRestOptions": AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
         "LogPublishingOptions": AwsElasticsearchDomainLogPublishingOptionsTypeDef,
         "NodeToNodeEncryptionOptions": AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
         "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
         "VPCOptions": AwsElasticsearchDomainVPCOptionsTypeDef,
     },
     total=False,
@@ -6316,14 +7888,23 @@
         "SourceSecurityGroup": AwsElbLoadBalancerSourceSecurityGroupTypeDef,
         "Subnets": Sequence[str],
         "VpcId": str,
     },
     total=False,
 )
 
+AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
+    {
+        "ScanEc2InstanceWithFindings": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
+        "ServiceRole": str,
+    },
+    total=False,
+)
+
 AwsIamAccessKeyDetailsTypeDef = TypedDict(
     "AwsIamAccessKeyDetailsTypeDef",
     {
         "UserName": str,
         "Status": AwsIamAccessKeyStatusType,
         "CreatedAt": str,
         "PrincipalId": str,
@@ -6370,29 +7951,33 @@
         "RevisionId": str,
         "Role": str,
         "Runtime": str,
         "Timeout": int,
         "TracingConfig": AwsLambdaFunctionTracingConfigTypeDef,
         "VpcConfig": AwsLambdaFunctionVpcConfigTypeDef,
         "Version": str,
+        "Architectures": Sequence[str],
+        "PackageType": str,
     },
     total=False,
 )
 
 AwsOpenSearchServiceDomainDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDetailsTypeDef",
     {
         "Arn": str,
         "AccessPolicies": str,
         "DomainName": str,
         "Id": str,
         "DomainEndpoint": str,
         "EngineVersion": str,
         "EncryptionAtRestOptions": AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
-        "NodeToNodeEncryptionOptions": AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef,
+        "NodeToNodeEncryptionOptions": (
+            AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef
+        ),
         "ServiceSoftwareOptions": AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
         "ClusterConfig": AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
         "DomainEndpointOptions": AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
         "VpcOptions": AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef,
         "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
         "DomainEndpoints": Mapping[str, str],
         "AdvancedSecurityOptions": AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
@@ -6481,14 +8066,23 @@
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     {
         "S3KeyFilter": AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     },
     total=False,
 )
 
+AwsS3BucketObjectLockConfigurationTypeDef = TypedDict(
+    "AwsS3BucketObjectLockConfigurationTypeDef",
+    {
+        "ObjectLockEnabled": str,
+        "Rule": AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsS3BucketServerSideEncryptionConfigurationTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     {
         "Rules": Sequence[AwsS3BucketServerSideEncryptionRuleTypeDef],
     },
     total=False,
 )
@@ -6505,26 +8099,38 @@
 )
 
 BatchUpdateFindingsResponseTypeDef = TypedDict(
     "BatchUpdateFindingsResponseTypeDef",
     {
         "ProcessedFindings": List[AwsSecurityFindingIdentifierTypeDef],
         "UnprocessedFindings": List[BatchUpdateFindingsUnprocessedFindingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AwsSsmPatchComplianceDetailsTypeDef = TypedDict(
     "AwsSsmPatchComplianceDetailsTypeDef",
     {
         "Patch": AwsSsmPatchTypeDef,
     },
     total=False,
 )
 
+AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
+    {
+        "Destinations": Sequence[
+            AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef
+        ],
+        "IncludeExecutionData": bool,
+        "Level": str,
+    },
+    total=False,
+)
+
 AwsWafRegionalRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
         "Rules": Sequence[AwsWafRegionalRuleGroupRulesDetailsTypeDef],
@@ -6562,14 +8168,105 @@
         "DefaultAction": str,
         "Rules": Sequence[AwsWafWebAclRuleTypeDef],
         "WebAclId": str,
     },
     total=False,
 )
 
+AwsWafv2ActionAllowDetailsTypeDef = TypedDict(
+    "AwsWafv2ActionAllowDetailsTypeDef",
+    {
+        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2RulesActionCaptchaDetailsTypeDef = TypedDict(
+    "AwsWafv2RulesActionCaptchaDetailsTypeDef",
+    {
+        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2RulesActionCountDetailsTypeDef = TypedDict(
+    "AwsWafv2RulesActionCountDetailsTypeDef",
+    {
+        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2ActionBlockDetailsTypeDef = TypedDict(
+    "AwsWafv2ActionBlockDetailsTypeDef",
+    {
+        "CustomResponse": AwsWafv2CustomResponseDetailsTypeDef,
+    },
+    total=False,
+)
+
+BatchGetStandardsControlAssociationsResponseTypeDef = TypedDict(
+    "BatchGetStandardsControlAssociationsResponseTypeDef",
+    {
+        "StandardsControlAssociationDetails": List[StandardsControlAssociationDetailTypeDef],
+        "UnprocessedAssociations": List[UnprocessedStandardsControlAssociationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchUpdateStandardsControlAssociationsResponseTypeDef = TypedDict(
+    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
+    {
+        "UnprocessedAssociationUpdates": List[UnprocessedStandardsControlAssociationUpdateTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AutomationRulesFindingFiltersTypeDef = TypedDict(
+    "AutomationRulesFindingFiltersTypeDef",
+    {
+        "ProductArn": List[StringFilterTypeDef],
+        "AwsAccountId": List[StringFilterTypeDef],
+        "Id": List[StringFilterTypeDef],
+        "GeneratorId": List[StringFilterTypeDef],
+        "Type": List[StringFilterTypeDef],
+        "FirstObservedAt": List[DateFilterTypeDef],
+        "LastObservedAt": List[DateFilterTypeDef],
+        "CreatedAt": List[DateFilterTypeDef],
+        "UpdatedAt": List[DateFilterTypeDef],
+        "Confidence": List[NumberFilterTypeDef],
+        "Criticality": List[NumberFilterTypeDef],
+        "Title": List[StringFilterTypeDef],
+        "Description": List[StringFilterTypeDef],
+        "SourceUrl": List[StringFilterTypeDef],
+        "ProductName": List[StringFilterTypeDef],
+        "CompanyName": List[StringFilterTypeDef],
+        "SeverityLabel": List[StringFilterTypeDef],
+        "ResourceType": List[StringFilterTypeDef],
+        "ResourceId": List[StringFilterTypeDef],
+        "ResourcePartition": List[StringFilterTypeDef],
+        "ResourceRegion": List[StringFilterTypeDef],
+        "ResourceTags": List[MapFilterTypeDef],
+        "ResourceDetailsOther": List[MapFilterTypeDef],
+        "ComplianceStatus": List[StringFilterTypeDef],
+        "ComplianceSecurityControlId": List[StringFilterTypeDef],
+        "ComplianceAssociatedStandardsId": List[StringFilterTypeDef],
+        "VerificationState": List[StringFilterTypeDef],
+        "WorkflowStatus": List[StringFilterTypeDef],
+        "RecordState": List[StringFilterTypeDef],
+        "RelatedFindingsProductArn": List[StringFilterTypeDef],
+        "RelatedFindingsId": List[StringFilterTypeDef],
+        "NoteText": List[StringFilterTypeDef],
+        "NoteUpdatedAt": List[DateFilterTypeDef],
+        "NoteUpdatedBy": List[StringFilterTypeDef],
+        "UserDefinedFields": List[MapFilterTypeDef],
+    },
+    total=False,
+)
+
 AwsSecurityFindingFiltersTypeDef = TypedDict(
     "AwsSecurityFindingFiltersTypeDef",
     {
         "ProductArn": Sequence[StringFilterTypeDef],
         "AwsAccountId": Sequence[StringFilterTypeDef],
         "Id": Sequence[StringFilterTypeDef],
         "GeneratorId": Sequence[StringFilterTypeDef],
@@ -6660,23 +8357,34 @@
         "FindingProviderFieldsCriticality": Sequence[NumberFilterTypeDef],
         "FindingProviderFieldsRelatedFindingsId": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsRelatedFindingsProductArn": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsSeverityLabel": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsSeverityOriginal": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsTypes": Sequence[StringFilterTypeDef],
         "Sample": Sequence[BooleanFilterTypeDef],
+        "ComplianceSecurityControlId": Sequence[StringFilterTypeDef],
+        "ComplianceAssociatedStandardsId": Sequence[StringFilterTypeDef],
     },
     total=False,
 )
 
+GetFindingHistoryResponseTypeDef = TypedDict(
+    "GetFindingHistoryResponseTypeDef",
+    {
+        "Records": List[FindingHistoryRecordTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetInsightResultsResponseTypeDef = TypedDict(
     "GetInsightResultsResponseTypeDef",
     {
         "InsightResults": InsightResultsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkHeaderTypeDef = TypedDict(
     "NetworkHeaderTypeDef",
     {
         "Protocol": str,
@@ -6703,36 +8411,45 @@
     {
         "Actions": Sequence[str],
         "MatchAttributes": RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     },
     total=False,
 )
 
+DescribeStandardsResponseTypeDef = TypedDict(
+    "DescribeStandardsResponseTypeDef",
+    {
+        "Standards": List[StandardTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchDisableStandardsResponseTypeDef = TypedDict(
     "BatchDisableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchEnableStandardsResponseTypeDef = TypedDict(
     "BatchEnableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEnabledStandardsResponseTypeDef = TypedDict(
     "GetEnabledStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StatelessCustomActionDefinitionTypeDef = TypedDict(
     "StatelessCustomActionDefinitionTypeDef",
     {
         "PublishMetricAction": StatelessCustomPublishMetricActionTypeDef,
@@ -6757,15 +8474,17 @@
         "HealthCheckType": str,
         "HealthCheckGracePeriod": int,
         "CreatedTime": str,
         "MixedInstancesPolicy": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
         "AvailabilityZones": Sequence[
             AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef
         ],
-        "LaunchTemplate": AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
+        "LaunchTemplate": (
+            AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
+        ),
         "CapacityRebalance": bool,
     },
     total=False,
 )
 
 AwsBackupBackupPlanBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
@@ -6847,14 +8566,26 @@
         "TableName": str,
         "TableSizeBytes": int,
         "TableStatus": str,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDetailsTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDetailsTypeDef",
+    {
+        "LaunchTemplateName": str,
+        "Id": str,
+        "LaunchTemplateData": AwsEc2LaunchTemplateDataDetailsTypeDef,
+        "DefaultVersionNumber": int,
+        "LatestVersionNumber": int,
+    },
+    total=False,
+)
+
 AwsEcsClusterDetailsTypeDef = TypedDict(
     "AwsEcsClusterDetailsTypeDef",
     {
         "ClusterArn": str,
         "ActiveServicesCount": int,
         "CapacityProviders": Sequence[str],
         "ClusterSettings": Sequence[AwsEcsClusterClusterSettingsDetailsTypeDef],
@@ -6887,14 +8618,27 @@
         "RequiresCompatibilities": Sequence[str],
         "TaskRoleArn": str,
         "Volumes": Sequence[AwsEcsTaskDefinitionVolumesDetailsTypeDef],
     },
     total=False,
 )
 
+AwsGuardDutyDetectorDataSourcesDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
+    {
+        "CloudTrail": AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef,
+        "DnsLogs": AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef,
+        "FlowLogs": AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef,
+        "Kubernetes": AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
+        "MalwareProtection": AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
+        "S3Logs": AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsRdsDbInstanceDetailsTypeDef = TypedDict(
     "AwsRdsDbInstanceDetailsTypeDef",
     {
         "AssociatedRoles": Sequence[AwsRdsDbInstanceAssociatedRoleTypeDef],
         "CACertificateIdentifier": str,
         "DBClusterIdentifier": str,
         "DBInstanceIdentifier": str,
@@ -6970,29 +8714,138 @@
         "Filter": AwsS3BucketNotificationConfigurationFilterTypeDef,
         "Destination": str,
         "Type": str,
     },
     total=False,
 )
 
+AwsStepFunctionStateMachineDetailsTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineDetailsTypeDef",
+    {
+        "Label": str,
+        "LoggingConfiguration": AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
+        "Name": str,
+        "RoleArn": str,
+        "StateMachineArn": str,
+        "Status": str,
+        "TracingConfiguration": AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
+        "Type": str,
+    },
+    total=False,
+)
+
+AwsWafv2RulesActionDetailsTypeDef = TypedDict(
+    "AwsWafv2RulesActionDetailsTypeDef",
+    {
+        "Allow": AwsWafv2ActionAllowDetailsTypeDef,
+        "Block": AwsWafv2ActionBlockDetailsTypeDef,
+        "Captcha": AwsWafv2RulesActionCaptchaDetailsTypeDef,
+        "Count": AwsWafv2RulesActionCountDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2WebAclActionDetailsTypeDef = TypedDict(
+    "AwsWafv2WebAclActionDetailsTypeDef",
+    {
+        "Allow": AwsWafv2ActionAllowDetailsTypeDef,
+        "Block": AwsWafv2ActionBlockDetailsTypeDef,
+    },
+    total=False,
+)
+
+AutomationRulesConfigTypeDef = TypedDict(
+    "AutomationRulesConfigTypeDef",
+    {
+        "RuleArn": str,
+        "RuleStatus": RuleStatusType,
+        "RuleOrder": int,
+        "RuleName": str,
+        "Description": str,
+        "IsTerminal": bool,
+        "Criteria": AutomationRulesFindingFiltersTypeDef,
+        "Actions": List[AutomationRulesActionTypeDef],
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "CreatedBy": str,
+    },
+    total=False,
+)
+
+_RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAutomationRuleRequestRequestTypeDef",
+    {
+        "RuleOrder": int,
+        "RuleName": str,
+        "Description": str,
+        "Criteria": AutomationRulesFindingFiltersTypeDef,
+        "Actions": Sequence[AutomationRulesActionTypeDef],
+    },
+)
+_OptionalCreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAutomationRuleRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "RuleStatus": RuleStatusType,
+        "IsTerminal": bool,
+    },
+    total=False,
+)
+
+
+class CreateAutomationRuleRequestRequestTypeDef(
+    _RequiredCreateAutomationRuleRequestRequestTypeDef,
+    _OptionalCreateAutomationRuleRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateAutomationRulesRequestItemTypeDef = TypedDict(
+    "_RequiredUpdateAutomationRulesRequestItemTypeDef",
+    {
+        "RuleArn": str,
+    },
+)
+_OptionalUpdateAutomationRulesRequestItemTypeDef = TypedDict(
+    "_OptionalUpdateAutomationRulesRequestItemTypeDef",
+    {
+        "RuleStatus": RuleStatusType,
+        "RuleOrder": int,
+        "Description": str,
+        "RuleName": str,
+        "IsTerminal": bool,
+        "Criteria": AutomationRulesFindingFiltersTypeDef,
+        "Actions": Sequence[AutomationRulesActionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateAutomationRulesRequestItemTypeDef(
+    _RequiredUpdateAutomationRulesRequestItemTypeDef,
+    _OptionalUpdateAutomationRulesRequestItemTypeDef,
+):
+    pass
+
+
 CreateInsightRequestRequestTypeDef = TypedDict(
     "CreateInsightRequestRequestTypeDef",
     {
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
 )
 
 GetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     {
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "SortCriteria": Sequence[SortCriterionTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetFindingsRequestRequestTypeDef = TypedDict(
     "GetFindingsRequestRequestTypeDef",
     {
@@ -7025,19 +8878,21 @@
     {
         "Note": NoteUpdateTypeDef,
         "RecordState": RecordStateType,
     },
     total=False,
 )
 
+
 class UpdateFindingsRequestRequestTypeDef(
     _RequiredUpdateFindingsRequestRequestTypeDef, _OptionalUpdateFindingsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateInsightRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInsightRequestRequestTypeDef",
     {
         "InsightArn": str,
     },
 )
 _OptionalUpdateInsightRequestRequestTypeDef = TypedDict(
@@ -7046,19 +8901,21 @@
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
     total=False,
 )
 
+
 class UpdateInsightRequestRequestTypeDef(
     _RequiredUpdateInsightRequestRequestTypeDef, _OptionalUpdateInsightRequestRequestTypeDef
 ):
     pass
 
+
 NetworkPathComponentTypeDef = TypedDict(
     "NetworkPathComponentTypeDef",
     {
         "ComponentId": str,
         "ComponentType": str,
         "Egress": NetworkHeaderTypeDef,
         "Ingress": NetworkHeaderTypeDef,
@@ -7152,18 +9009,32 @@
         "ViewerCertificate": AwsCloudFrontDistributionViewerCertificateTypeDef,
         "Status": str,
         "WebAclId": str,
     },
     total=False,
 )
 
+AwsGuardDutyDetectorDetailsTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDetailsTypeDef",
+    {
+        "DataSources": AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
+        "Features": Sequence[AwsGuardDutyDetectorFeaturesDetailsTypeDef],
+        "FindingPublishingFrequency": str,
+        "ServiceRole": str,
+        "Status": str,
+    },
+    total=False,
+)
+
 AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     {
-        "AbortIncompleteMultipartUpload": AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef,
+        "AbortIncompleteMultipartUpload": (
+            AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
+        ),
         "ExpirationDate": str,
         "ExpirationInDays": int,
         "ExpiredObjectDeleteMarker": bool,
         "Filter": AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
         "ID": str,
         "NoncurrentVersionExpirationInDays": int,
         "NoncurrentVersionTransitions": Sequence[
@@ -7182,20 +9053,48 @@
     "AwsS3BucketNotificationConfigurationTypeDef",
     {
         "Configurations": Sequence[AwsS3BucketNotificationConfigurationDetailTypeDef],
     },
     total=False,
 )
 
+AwsWafv2RulesDetailsTypeDef = TypedDict(
+    "AwsWafv2RulesDetailsTypeDef",
+    {
+        "Action": AwsWafv2RulesActionDetailsTypeDef,
+        "Name": str,
+        "OverrideAction": str,
+        "Priority": int,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
+BatchGetAutomationRulesResponseTypeDef = TypedDict(
+    "BatchGetAutomationRulesResponseTypeDef",
+    {
+        "Rules": List[AutomationRulesConfigTypeDef],
+        "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchUpdateAutomationRulesRequestRequestTypeDef = TypedDict(
+    "BatchUpdateAutomationRulesRequestRequestTypeDef",
+    {
+        "UpdateAutomationRulesRequestItems": Sequence[UpdateAutomationRulesRequestItemTypeDef],
+    },
+)
+
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "Insights": List[InsightTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CustomDataIdentifiersResultTypeDef = TypedDict(
     "CustomDataIdentifiersResultTypeDef",
     {
         "Detections": Sequence[CustomDataIdentifiersDetectionsTypeDef],
@@ -7243,14 +9142,46 @@
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
     {
         "Rules": Sequence[AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef],
     },
     total=False,
 )
 
+AwsWafv2RuleGroupDetailsTypeDef = TypedDict(
+    "AwsWafv2RuleGroupDetailsTypeDef",
+    {
+        "Capacity": int,
+        "Description": str,
+        "Id": str,
+        "Name": str,
+        "Arn": str,
+        "Rules": Sequence[AwsWafv2RulesDetailsTypeDef],
+        "Scope": str,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2WebAclDetailsTypeDef = TypedDict(
+    "AwsWafv2WebAclDetailsTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "ManagedbyFirewallManager": bool,
+        "Id": str,
+        "Capacity": int,
+        "CaptchaConfig": AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
+        "DefaultAction": AwsWafv2WebAclActionDetailsTypeDef,
+        "Description": str,
+        "Rules": Sequence[AwsWafv2RulesDetailsTypeDef],
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
 ClassificationResultTypeDef = TypedDict(
     "ClassificationResultTypeDef",
     {
         "MimeType": str,
         "SizeClassified": int,
         "AdditionalOccurrences": bool,
         "Status": ClassificationStatusTypeDef,
@@ -7274,15 +9205,17 @@
 
 RuleGroupSourceTypeDef = TypedDict(
     "RuleGroupSourceTypeDef",
     {
         "RulesSourceList": RuleGroupSourceListDetailsTypeDef,
         "RulesString": str,
         "StatefulRules": Sequence[RuleGroupSourceStatefulRulesDetailsTypeDef],
-        "StatelessRulesAndCustomActions": RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
+        "StatelessRulesAndCustomActions": (
+            RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef
+        ),
     },
     total=False,
 )
 
 AwsS3BucketDetailsTypeDef = TypedDict(
     "AwsS3BucketDetailsTypeDef",
     {
@@ -7294,14 +9227,15 @@
         "BucketLifecycleConfiguration": AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef,
         "PublicAccessBlockConfiguration": AwsS3AccountPublicAccessBlockDetailsTypeDef,
         "AccessControlList": str,
         "BucketLoggingConfiguration": AwsS3BucketLoggingConfigurationTypeDef,
         "BucketWebsiteConfiguration": AwsS3BucketWebsiteConfigurationTypeDef,
         "BucketNotificationConfiguration": AwsS3BucketNotificationConfigurationTypeDef,
         "BucketVersioningConfiguration": AwsS3BucketBucketVersioningConfigurationTypeDef,
+        "ObjectLockConfiguration": AwsS3BucketObjectLockConfigurationTypeDef,
     },
     total=False,
 )
 
 DataClassificationDetailsTypeDef = TypedDict(
     "DataClassificationDetailsTypeDef",
     {
@@ -7412,14 +9346,24 @@
         "AwsWafRegionalWebAcl": AwsWafRegionalWebAclDetailsTypeDef,
         "AwsWafRule": AwsWafRuleDetailsTypeDef,
         "AwsWafRuleGroup": AwsWafRuleGroupDetailsTypeDef,
         "AwsEcsTask": AwsEcsTaskDetailsTypeDef,
         "AwsBackupBackupVault": AwsBackupBackupVaultDetailsTypeDef,
         "AwsBackupBackupPlan": AwsBackupBackupPlanDetailsTypeDef,
         "AwsBackupRecoveryPoint": AwsBackupRecoveryPointDetailsTypeDef,
+        "AwsEc2LaunchTemplate": AwsEc2LaunchTemplateDetailsTypeDef,
+        "AwsSageMakerNotebookInstance": AwsSageMakerNotebookInstanceDetailsTypeDef,
+        "AwsWafv2WebAcl": AwsWafv2WebAclDetailsTypeDef,
+        "AwsWafv2RuleGroup": AwsWafv2RuleGroupDetailsTypeDef,
+        "AwsEc2RouteTable": AwsEc2RouteTableDetailsTypeDef,
+        "AwsAmazonMqBroker": AwsAmazonMqBrokerDetailsTypeDef,
+        "AwsAppSyncGraphQlApi": AwsAppSyncGraphQlApiDetailsTypeDef,
+        "AwsEventSchemasRegistry": AwsEventSchemasRegistryDetailsTypeDef,
+        "AwsGuardDutyDetector": AwsGuardDutyDetectorDetailsTypeDef,
+        "AwsStepFunctionStateMachine": AwsStepFunctionStateMachineDetailsTypeDef,
     },
     total=False,
 )
 
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
@@ -7436,17 +9380,19 @@
         "Tags": Mapping[str, str],
         "DataClassification": DataClassificationDetailsTypeDef,
         "Details": ResourceDetailsTypeDef,
     },
     total=False,
 )
 
+
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
+
 _RequiredAwsSecurityFindingTypeDef = TypedDict(
     "_RequiredAwsSecurityFindingTypeDef",
     {
         "SchemaVersion": str,
         "Id": str,
         "ProductArn": str,
         "GeneratorId": str,
@@ -7492,27 +9438,29 @@
         "Action": ActionTypeDef,
         "FindingProviderFields": FindingProviderFieldsTypeDef,
         "Sample": bool,
     },
     total=False,
 )
 
+
 class AwsSecurityFindingTypeDef(
     _RequiredAwsSecurityFindingTypeDef, _OptionalAwsSecurityFindingTypeDef
 ):
     pass
 
+
 BatchImportFindingsRequestRequestTypeDef = TypedDict(
     "BatchImportFindingsRequestRequestTypeDef",
     {
         "Findings": Sequence[AwsSecurityFindingTypeDef],
     },
 )
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "Findings": List[AwsSecurityFindingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/PKG-INFO` & `mypy-boto3-securityhub-1.27.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-securityhub
-Version: 1.26.8
-Summary: Type annotations for boto3.SecurityHub 1.26.8 service generated with mypy-boto3-builder 7.11.10
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 securityhub type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-securityhub"></a>
 
 # mypy-boto3-securityhub
 
 [![PyPI - mypy-boto3-securityhub](https://img.shields.io/pypi/v/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securityhub?color=blue)](https://pypistats.org/packages/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,21 +252,24 @@
 from mypy_boto3_securityhub import SecurityHubClient
 from mypy_boto3_securityhub.paginator import (
     DescribeActionTargetsPaginator,
     DescribeProductsPaginator,
     DescribeStandardsPaginator,
     DescribeStandardsControlsPaginator,
     GetEnabledStandardsPaginator,
+    GetFindingHistoryPaginator,
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
+    ListSecurityControlDefinitionsPaginator,
+    ListStandardsControlAssociationsPaginator,
 )
 
 client: SecurityHubClient = Session().client("securityhub")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator(
@@ -309,72 +281,91 @@
 )
 describe_standards_controls_paginator: DescribeStandardsControlsPaginator = client.get_paginator(
     "describe_standards_controls"
 )
 get_enabled_standards_paginator: GetEnabledStandardsPaginator = client.get_paginator(
     "get_enabled_standards"
 )
+get_finding_history_paginator: GetFindingHistoryPaginator = client.get_paginator(
+    "get_finding_history"
+)
 get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
 get_insights_paginator: GetInsightsPaginator = client.get_paginator("get_insights")
 list_enabled_products_for_import_paginator: ListEnabledProductsForImportPaginator = (
     client.get_paginator("list_enabled_products_for_import")
 )
 list_finding_aggregators_paginator: ListFindingAggregatorsPaginator = client.get_paginator(
     "list_finding_aggregators"
 )
 list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
 list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
 list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = (
     client.get_paginator("list_organization_admin_accounts")
 )
+list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = (
+    client.get_paginator("list_security_control_definitions")
+)
+list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = (
+    client.get_paginator("list_standards_control_associations")
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_securityhub.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_securityhub.literals import (
     AdminStatusType,
+    AssociationStatusType,
     AutoEnableStandardsType,
+    AutomationRulesActionTypeType,
     AwsIamAccessKeyStatusType,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
     ComplianceStatusType,
+    ControlFindingGeneratorType,
     ControlStatusType,
     DateRangeUnitType,
     DescribeActionTargetsPaginatorName,
     DescribeProductsPaginatorName,
     DescribeStandardsControlsPaginatorName,
     DescribeStandardsPaginatorName,
+    FindingHistoryUpdateSourceTypeType,
     GetEnabledStandardsPaginatorName,
+    GetFindingHistoryPaginatorName,
     GetFindingsPaginatorName,
     GetInsightsPaginatorName,
     IntegrationTypeType,
     ListEnabledProductsForImportPaginatorName,
     ListFindingAggregatorsPaginatorName,
     ListInvitationsPaginatorName,
     ListMembersPaginatorName,
     ListOrganizationAdminAccountsPaginatorName,
+    ListSecurityControlDefinitionsPaginatorName,
+    ListStandardsControlAssociationsPaginatorName,
     MalwareStateType,
     MalwareTypeType,
     MapFilterComparisonType,
     NetworkDirectionType,
     PartitionType,
     RecordStateType,
+    RegionAvailabilityStatusType,
+    RuleStatusType,
     SeverityLabelType,
     SeverityRatingType,
     SortOrderType,
     StandardsStatusType,
     StatusReasonCodeType,
     StringFilterComparisonType,
     ThreatIntelIndicatorCategoryType,
     ThreatIntelIndicatorTypeType,
+    UnprocessedErrorCodeType,
     VerificationStateType,
     VulnerabilityFixAvailableType,
     WorkflowStateType,
     WorkflowStatusType,
     SecurityHubServiceName,
     ServiceName,
     ResourceServiceName,
@@ -406,22 +397,41 @@
     GeoLocationTypeDef,
     IpOrganizationDetailsTypeDef,
     ActionRemotePortDetailsTypeDef,
     ActionTargetTypeDef,
     DnsRequestActionTypeDef,
     AdjustmentTypeDef,
     AdminAccountTypeDef,
+    AssociatedStandardTypeDef,
+    AssociationStateDetailsTypeDef,
+    NoteUpdateTypeDef,
+    RelatedFindingTypeDef,
+    SeverityUpdateTypeDef,
+    WorkflowUpdateTypeDef,
+    MapFilterTypeDef,
+    NumberFilterTypeDef,
+    StringFilterTypeDef,
+    AutomationRulesMetadataTypeDef,
     AvailabilityZoneTypeDef,
+    AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
+    AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
+    AwsAmazonMqBrokerUsersDetailsTypeDef,
+    AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
     AwsApiCallActionDomainDetailsTypeDef,
     AwsApiGatewayAccessLogSettingsTypeDef,
     AwsApiGatewayCanarySettingsTypeDef,
     AwsApiGatewayEndpointConfigurationTypeDef,
     AwsApiGatewayMethodSettingsTypeDef,
     AwsCorsConfigurationTypeDef,
     AwsApiGatewayV2RouteSettingsTypeDef,
+    AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
+    AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
+    AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
+    AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
@@ -461,22 +471,53 @@
     AwsDynamoDbTableRestoreSummaryTypeDef,
     AwsDynamoDbTableSseDescriptionTypeDef,
     AwsDynamoDbTableStreamSpecificationTypeDef,
     AwsDynamoDbTableProjectionTypeDef,
     AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     AwsEc2EipDetailsTypeDef,
     AwsEc2InstanceMetadataOptionsTypeDef,
+    AwsEc2InstanceMonitoringDetailsTypeDef,
     AwsEc2InstanceNetworkInterfacesDetailsTypeDef,
+    AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
+    AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
+    AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
+    AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
+    AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef,
     AwsEc2NetworkAclAssociationTypeDef,
     IcmpTypeCodeTypeDef,
     PortRangeFromToTypeDef,
     AwsEc2NetworkInterfaceAttachmentTypeDef,
     AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef,
     AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef,
     AwsEc2NetworkInterfaceSecurityGroupTypeDef,
+    PropagatingVgwSetDetailsTypeDef,
+    RouteSetDetailsTypeDef,
     AwsEc2SecurityGroupIpRangeTypeDef,
     AwsEc2SecurityGroupIpv6RangeTypeDef,
     AwsEc2SecurityGroupPrefixListIdTypeDef,
     AwsEc2SecurityGroupUserIdGroupPairTypeDef,
     Ipv6CidrBlockAssociationTypeDef,
     AwsEc2TransitGatewayDetailsTypeDef,
     AwsEc2VolumeAttachmentTypeDef,
@@ -553,14 +594,22 @@
     AwsElbLoadBalancerBackendServerDescriptionTypeDef,
     AwsElbLoadBalancerHealthCheckTypeDef,
     AwsElbLoadBalancerInstanceTypeDef,
     AwsElbLoadBalancerSourceSecurityGroupTypeDef,
     AwsElbLoadBalancerListenerTypeDef,
     AwsElbv2LoadBalancerAttributeTypeDef,
     LoadBalancerStateTypeDef,
+    AwsEventSchemasRegistryDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef,
+    AwsGuardDutyDetectorFeaturesDetailsTypeDef,
     AwsIamAccessKeySessionContextAttributesTypeDef,
     AwsIamAccessKeySessionContextSessionIssuerTypeDef,
     AwsIamAttachedManagedPolicyTypeDef,
     AwsIamGroupPolicyTypeDef,
     AwsIamInstanceProfileRoleTypeDef,
     AwsIamPermissionsBoundaryTypeDef,
     AwsIamPolicyVersionTypeDef,
@@ -620,139 +669,189 @@
     AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef,
     AwsS3BucketBucketVersioningConfigurationTypeDef,
     AwsS3BucketLoggingConfigurationTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef,
+    AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef,
     AwsS3BucketServerSideEncryptionByDefaultTypeDef,
     AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     AwsS3ObjectDetailsTypeDef,
+    AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef,
     AwsSecretsManagerSecretRotationRulesTypeDef,
     BooleanFilterTypeDef,
     IpFilterTypeDef,
     KeywordFilterTypeDef,
-    MapFilterTypeDef,
-    NumberFilterTypeDef,
-    StringFilterTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     MalwareTypeDef,
     NoteTypeDef,
     PatchSummaryTypeDef,
     ProcessDetailsTypeDef,
-    RelatedFindingTypeDef,
     SeverityTypeDef,
     ThreatIntelIndicatorTypeDef,
     WorkflowTypeDef,
     AwsSnsTopicSubscriptionTypeDef,
     AwsSqsQueueDetailsTypeDef,
     AwsSsmComplianceSummaryTypeDef,
+    AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
+    AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
     AwsWafRateBasedRuleMatchPredicateTypeDef,
     AwsWafRegionalRateBasedRuleMatchPredicateTypeDef,
     AwsWafRegionalRulePredicateListDetailsTypeDef,
     AwsWafRegionalRuleGroupRulesActionDetailsTypeDef,
     AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
     AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
     AwsWafRulePredicateListDetailsTypeDef,
     AwsWafRuleGroupRulesActionDetailsTypeDef,
     WafActionTypeDef,
     WafExcludedRuleTypeDef,
     WafOverrideActionTypeDef,
+    AwsWafv2CustomHttpHeaderTypeDef,
+    AwsWafv2VisibilityConfigDetailsTypeDef,
+    AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     AwsXrayEncryptionConfigDetailsTypeDef,
+    BatchDeleteAutomationRulesRequestRequestTypeDef,
+    UnprocessedAutomationRuleTypeDef,
     BatchDisableStandardsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StandardsSubscriptionRequestTypeDef,
+    BatchGetAutomationRulesRequestRequestTypeDef,
+    BatchGetSecurityControlsRequestRequestTypeDef,
+    SecurityControlTypeDef,
+    UnprocessedSecurityControlTypeDef,
+    StandardsControlAssociationIdTypeDef,
+    StandardsControlAssociationDetailTypeDef,
     ImportFindingsErrorTypeDef,
-    NoteUpdateTypeDef,
-    SeverityUpdateTypeDef,
-    WorkflowUpdateTypeDef,
+    StandardsControlAssociationUpdateTypeDef,
     CellTypeDef,
     ClassificationStatusTypeDef,
     StatusReasonTypeDef,
     VolumeMountTypeDef,
     CreateActionTargetRequestRequestTypeDef,
+    CreateActionTargetResponseTypeDef,
+    CreateAutomationRuleResponseTypeDef,
     CreateFindingAggregatorRequestRequestTypeDef,
+    CreateFindingAggregatorResponseTypeDef,
+    CreateInsightResponseTypeDef,
     ResultTypeDef,
     DateRangeTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteActionTargetRequestRequestTypeDef,
+    DeleteActionTargetResponseTypeDef,
     DeleteFindingAggregatorRequestRequestTypeDef,
     DeleteInsightRequestRequestTypeDef,
+    DeleteInsightResponseTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
     DescribeActionTargetsRequestRequestTypeDef,
     DescribeHubRequestRequestTypeDef,
+    DescribeHubResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    DescribeProductsRequestDescribeProductsPaginateTypeDef,
     DescribeProductsRequestRequestTypeDef,
     ProductTypeDef,
+    DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
     DescribeStandardsControlsRequestRequestTypeDef,
     StandardsControlTypeDef,
+    DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
     DescribeStandardsRequestRequestTypeDef,
-    StandardTypeDef,
     DisableImportFindingsForProductRequestRequestTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     EnableImportFindingsForProductRequestRequestTypeDef,
+    EnableImportFindingsForProductResponseTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     EnableSecurityHubRequestRequestTypeDef,
     FilePathsTypeDef,
     FindingAggregatorTypeDef,
+    FindingHistoryUpdateSourceTypeDef,
+    FindingHistoryUpdateTypeDef,
     FindingProviderSeverityTypeDef,
     FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef,
     FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef,
     InvitationTypeDef,
+    GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
     GetEnabledStandardsRequestRequestTypeDef,
     GetFindingAggregatorRequestRequestTypeDef,
+    GetFindingAggregatorResponseTypeDef,
     SortCriterionTypeDef,
     GetInsightResultsRequestRequestTypeDef,
+    GetInsightsRequestGetInsightsPaginateTypeDef,
     GetInsightsRequestRequestTypeDef,
+    GetInvitationsCountResponseTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     InsightResultValueTypeDef,
     InviteMembersRequestRequestTypeDef,
+    ListAutomationRulesRequestRequestTypeDef,
+    ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
     ListEnabledProductsForImportRequestRequestTypeDef,
+    ListEnabledProductsForImportResponseTypeDef,
+    ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
     ListFindingAggregatorsRequestRequestTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
+    ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
+    ListSecurityControlDefinitionsRequestRequestTypeDef,
+    SecurityControlDefinitionTypeDef,
+    ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
+    ListStandardsControlAssociationsRequestRequestTypeDef,
+    StandardsControlAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PortRangeTypeDef,
     RangeTypeDef,
     RecordTypeDef,
+    PaginatorConfigTypeDef,
     RecommendationTypeDef,
+    ResponseMetadataTypeDef,
     RuleGroupSourceListDetailsTypeDef,
     RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
     RuleGroupSourceStatefulRulesOptionsDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef,
     RuleGroupVariablesIpSetsDetailsTypeDef,
     RuleGroupVariablesPortSetsDetailsTypeDef,
     SoftwarePackageTypeDef,
+    StandardsManagedByTypeDef,
     StandardsStatusReasonTypeDef,
     StatelessCustomPublishMetricActionDimensionTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateActionTargetRequestRequestTypeDef,
     UpdateFindingAggregatorRequestRequestTypeDef,
+    UpdateFindingAggregatorResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateSecurityHubConfigurationRequestRequestTypeDef,
     UpdateStandardsControlRequestRequestTypeDef,
     VulnerabilityVendorTypeDef,
     CreateMembersRequestRequestTypeDef,
     ActionRemoteIpDetailsTypeDef,
+    DescribeActionTargetsResponseTypeDef,
     CvssTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    AssociationSetDetailsTypeDef,
+    AutomationRulesFindingFieldsUpdateTypeDef,
+    ListAutomationRulesResponseTypeDef,
+    AwsAmazonMqBrokerLogsDetailsTypeDef,
     AwsApiGatewayRestApiDetailsTypeDef,
     AwsApiGatewayStageDetailsTypeDef,
     AwsApiGatewayV2ApiDetailsTypeDef,
     AwsApiGatewayV2StageDetailsTypeDef,
+    AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef,
     AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef,
     AwsBackupBackupVaultDetailsTypeDef,
     AwsBackupRecoveryPointDetailsTypeDef,
     AwsCertificateManagerCertificateDomainValidationOptionTypeDef,
     AwsCloudFormationStackDetailsTypeDef,
@@ -762,14 +861,19 @@
     AwsCloudWatchAlarmDetailsTypeDef,
     AwsCodeBuildProjectEnvironmentTypeDef,
     AwsCodeBuildProjectLogsConfigDetailsTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexTypeDef,
     AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef,
     AwsEc2InstanceDetailsTypeDef,
+    AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef,
+    AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef,
     AwsEc2NetworkAclEntryTypeDef,
     AwsEc2NetworkInterfaceDetailsTypeDef,
     AwsEc2SecurityGroupIpPermissionTypeDef,
     AwsEc2SubnetDetailsTypeDef,
     AwsEc2VolumeDetailsTypeDef,
     AwsEc2VpcDetailsTypeDef,
     AwsEc2VpcEndpointServiceDetailsTypeDef,
@@ -790,14 +894,16 @@
     AwsElasticBeanstalkEnvironmentDetailsTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsTypeDef,
     AwsElbLoadBalancerPoliciesTypeDef,
     AwsElbLoadBalancerAttributesTypeDef,
     AwsElbLoadBalancerListenerDescriptionTypeDef,
     AwsElbv2LoadBalancerDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
     AwsIamAccessKeySessionContextTypeDef,
     AwsIamGroupDetailsTypeDef,
     AwsIamInstanceProfileTypeDef,
     AwsIamPolicyDetailsTypeDef,
     AwsIamUserDetailsTypeDef,
     AwsKinesisStreamDetailsTypeDef,
     AwsLambdaFunctionEnvironmentTypeDef,
@@ -809,148 +915,165 @@
     AwsRdsDbSnapshotDetailsTypeDef,
     AwsRdsDbPendingModifiedValuesTypeDef,
     AwsRdsDbSecurityGroupDetailsTypeDef,
     AwsRdsDbSubnetGroupSubnetTypeDef,
     AwsRedshiftClusterClusterParameterGroupTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
+    AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
     AwsS3BucketServerSideEncryptionRuleTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
+    AwsSageMakerNotebookInstanceDetailsTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
+    BatchUpdateFindingsRequestRequestTypeDef,
     BatchUpdateFindingsUnprocessedFindingTypeDef,
+    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    GetFindingHistoryRequestRequestTypeDef,
     AwsSnsTopicDetailsTypeDef,
     AwsSsmPatchTypeDef,
+    AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRuleDetailsTypeDef,
     AwsWafRegionalRuleGroupRulesDetailsTypeDef,
     AwsWafRegionalWebAclRulesListDetailsTypeDef,
     AwsWafRuleDetailsTypeDef,
     AwsWafRuleGroupRulesDetailsTypeDef,
     AwsWafWebAclRuleTypeDef,
-    CreateActionTargetResponseTypeDef,
-    CreateFindingAggregatorResponseTypeDef,
-    CreateInsightResponseTypeDef,
-    DeleteActionTargetResponseTypeDef,
-    DeleteInsightResponseTypeDef,
-    DescribeActionTargetsResponseTypeDef,
-    DescribeHubResponseTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
-    EnableImportFindingsForProductResponseTypeDef,
-    GetFindingAggregatorResponseTypeDef,
-    GetInvitationsCountResponseTypeDef,
-    ListEnabledProductsForImportResponseTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateFindingAggregatorResponseTypeDef,
+    AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    AwsWafv2CustomResponseDetailsTypeDef,
+    AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
+    BatchDeleteAutomationRulesResponseTypeDef,
+    BatchUpdateAutomationRulesResponseTypeDef,
     BatchEnableStandardsRequestRequestTypeDef,
+    BatchGetSecurityControlsResponseTypeDef,
+    BatchGetStandardsControlAssociationsRequestRequestTypeDef,
+    UnprocessedStandardsControlAssociationTypeDef,
     BatchImportFindingsResponseTypeDef,
-    BatchUpdateFindingsRequestRequestTypeDef,
+    BatchUpdateStandardsControlAssociationsRequestRequestTypeDef,
+    UnprocessedStandardsControlAssociationUpdateTypeDef,
     ComplianceTypeDef,
     ContainerDetailsTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     DateFilterTypeDef,
-    DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
-    DescribeProductsRequestDescribeProductsPaginateTypeDef,
-    DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
-    DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
-    GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
-    GetInsightsRequestGetInsightsPaginateTypeDef,
-    ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
-    ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
-    DescribeStandardsResponseTypeDef,
     ThreatTypeDef,
     ListFindingAggregatorsResponseTypeDef,
+    FindingHistoryRecordTypeDef,
     FindingProviderFieldsTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
+    ListSecurityControlDefinitionsResponseTypeDef,
+    ListStandardsControlAssociationsResponseTypeDef,
     NetworkPathComponentDetailsTypeDef,
     NetworkTypeDef,
     PageTypeDef,
     RemediationTypeDef,
     RuleGroupSourceStatefulRulesDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     RuleGroupVariablesTypeDef,
+    StandardTypeDef,
     StandardsSubscriptionTypeDef,
     StatelessCustomPublishMetricActionTypeDef,
     AwsApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     VulnerabilityTypeDef,
+    AwsEc2RouteTableDetailsTypeDef,
+    AutomationRulesActionTypeDef,
+    AwsAmazonMqBrokerDetailsTypeDef,
+    AwsAppSyncGraphQlApiDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsTypeDef,
     AwsBackupBackupPlanRuleDetailsTypeDef,
     AwsCertificateManagerCertificateRenewalSummaryTypeDef,
     AwsCloudFrontDistributionOriginItemTypeDef,
     AwsCloudFrontDistributionOriginGroupTypeDef,
     AwsCodeBuildProjectDetailsTypeDef,
     AwsDynamoDbTableReplicaTypeDef,
+    AwsEc2LaunchTemplateDataDetailsTypeDef,
     AwsEc2NetworkAclDetailsTypeDef,
     AwsEc2SecurityGroupDetailsTypeDef,
     AwsEc2VpcPeeringConnectionDetailsTypeDef,
     AwsEc2VpnConnectionDetailsTypeDef,
     AwsEcsClusterConfigurationDetailsTypeDef,
     AwsEcsServiceDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesDetailsTypeDef,
     AwsEcsTaskDetailsTypeDef,
     AwsEfsAccessPointDetailsTypeDef,
     AwsEksClusterDetailsTypeDef,
     AwsElasticsearchDomainDetailsTypeDef,
     AwsElbLoadBalancerDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
     AwsIamAccessKeyDetailsTypeDef,
     AwsIamRoleDetailsTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     AwsOpenSearchServiceDomainDetailsTypeDef,
     AwsRdsDbSubnetGroupTypeDef,
     AwsRedshiftClusterDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
     AwsS3BucketNotificationConfigurationFilterTypeDef,
+    AwsS3BucketObjectLockConfigurationTypeDef,
     AwsS3BucketServerSideEncryptionConfigurationTypeDef,
     AwsS3BucketWebsiteConfigurationTypeDef,
     BatchUpdateFindingsResponseTypeDef,
     AwsSsmPatchComplianceDetailsTypeDef,
+    AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
     AwsWafRegionalRuleGroupDetailsTypeDef,
     AwsWafRegionalWebAclDetailsTypeDef,
     AwsWafRuleGroupDetailsTypeDef,
     AwsWafWebAclDetailsTypeDef,
+    AwsWafv2ActionAllowDetailsTypeDef,
+    AwsWafv2RulesActionCaptchaDetailsTypeDef,
+    AwsWafv2RulesActionCountDetailsTypeDef,
+    AwsWafv2ActionBlockDetailsTypeDef,
+    BatchGetStandardsControlAssociationsResponseTypeDef,
+    BatchUpdateStandardsControlAssociationsResponseTypeDef,
+    AutomationRulesFindingFiltersTypeDef,
     AwsSecurityFindingFiltersTypeDef,
+    GetFindingHistoryResponseTypeDef,
     GetInsightResultsResponseTypeDef,
     NetworkHeaderTypeDef,
     OccurrencesTypeDef,
     RuleGroupSourceStatelessRuleDefinitionTypeDef,
+    DescribeStandardsResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     StatelessCustomActionDefinitionTypeDef,
     PortProbeActionTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
     AwsCloudFrontDistributionOriginsTypeDef,
     AwsCloudFrontDistributionOriginGroupsTypeDef,
     AwsDynamoDbTableDetailsTypeDef,
+    AwsEc2LaunchTemplateDetailsTypeDef,
     AwsEcsClusterDetailsTypeDef,
     AwsEcsTaskDefinitionDetailsTypeDef,
+    AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
     AwsRdsDbInstanceDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
     AwsS3BucketNotificationConfigurationDetailTypeDef,
+    AwsStepFunctionStateMachineDetailsTypeDef,
+    AwsWafv2RulesActionDetailsTypeDef,
+    AwsWafv2WebAclActionDetailsTypeDef,
+    AutomationRulesConfigTypeDef,
+    CreateAutomationRuleRequestRequestTypeDef,
+    UpdateAutomationRulesRequestItemTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     InsightTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
     NetworkPathComponentTypeDef,
@@ -958,22 +1081,28 @@
     SensitiveDataDetectionsTypeDef,
     RuleGroupSourceStatelessRulesDetailsTypeDef,
     FirewallPolicyStatelessCustomActionsDetailsTypeDef,
     RuleGroupSourceCustomActionsDetailsTypeDef,
     ActionTypeDef,
     AwsBackupBackupPlanDetailsTypeDef,
     AwsCloudFrontDistributionDetailsTypeDef,
+    AwsGuardDutyDetectorDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef,
     AwsS3BucketNotificationConfigurationTypeDef,
+    AwsWafv2RulesDetailsTypeDef,
+    BatchGetAutomationRulesResponseTypeDef,
+    BatchUpdateAutomationRulesRequestRequestTypeDef,
     GetInsightsResponseTypeDef,
     CustomDataIdentifiersResultTypeDef,
     SensitiveDataResultTypeDef,
     FirewallPolicyDetailsTypeDef,
     RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef,
+    AwsWafv2RuleGroupDetailsTypeDef,
+    AwsWafv2WebAclDetailsTypeDef,
     ClassificationResultTypeDef,
     AwsNetworkFirewallFirewallPolicyDetailsTypeDef,
     RuleGroupSourceTypeDef,
     AwsS3BucketDetailsTypeDef,
     DataClassificationDetailsTypeDef,
     RuleGroupDetailsTypeDef,
     AwsNetworkFirewallRuleGroupDetailsTypeDef,
@@ -992,42 +1121,42 @@
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

### Comparing `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/SOURCES.txt` & `mypy-boto3-securityhub-1.27.0/mypy_boto3_securityhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.26.8/setup.py` & `mypy-boto3-securityhub-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-securityhub.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-securityhub",
-    version="1.26.8",
+    version="1.27.0",
     packages=["mypy_boto3_securityhub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SecurityHub 1.26.8 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.SecurityHub 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
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
     keywords="boto3 securityhub type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_securityhub": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_securityhub": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/",
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


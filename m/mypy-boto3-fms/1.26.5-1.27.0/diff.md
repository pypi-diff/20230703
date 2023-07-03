# Comparing `tmp/mypy-boto3-fms-1.26.5.tar.gz` & `tmp/mypy-boto3-fms-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fms-1.26.5.tar", last modified: Tue Nov  8 20:33:28 2022, max compression
+gzip compressed data, was "mypy-boto3-fms-1.27.0.tar", last modified: Mon Jul  3 19:50:47 2023, max compression
```

## Comparing `mypy-boto3-fms-1.26.5.tar` & `mypy-boto3-fms-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 20:33:28.885201 mypy-boto3-fms-1.26.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    19587 2022-11-08 20:33:28.877201 mypy-boto3-fms-1.26.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18168 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 20:33:28.873201 mypy-boto3-fms-1.26.5/mypy_boto3_fms/
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27532 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    27481 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11468 2022-11-08 20:33:03.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    11466 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7438 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7429 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    54548 2022-11-08 20:33:03.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    54483 2022-11-08 20:33:03.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 20:33:28.877201 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    19587 2022-11-08 20:33:28.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-11-08 20:33:28.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 20:33:28.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 20:33:28.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-08 20:33:28.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-08 20:33:28.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-08 20:33:28.885201 mypy-boto3-fms-1.26.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.571271 mypy-boto3-fms-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:51.000000 mypy-boto3-fms-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20839 2023-07-03 19:50:47.571271 mypy-boto3-fms-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-07-03 19:37:51.000000 mypy-boto3-fms-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.567271 mypy-boto3-fms-1.27.0/mypy_boto3_fms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-03 19:37:51.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-03 19:37:51.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:37:51.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30820 2023-07-03 19:37:51.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30763 2023-07-03 19:37:51.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12996 2023-07-03 19:37:52.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-07-03 19:37:52.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-03 19:37:51.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-03 19:37:51.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:51.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59433 2023-07-03 19:37:53.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59366 2023-07-03 19:37:52.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:51.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.571271 mypy-boto3-fms-1.27.0/mypy_boto3_fms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20839 2023-07-03 19:50:47.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:50:47.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:47.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:47.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:47.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:47.000000 mypy-boto3-fms-1.27.0/mypy_boto3_fms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:47.571271 mypy-boto3-fms-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:37:51.000000 mypy-boto3-fms-1.27.0/setup.py
```

### Comparing `mypy-boto3-fms-1.26.5/LICENSE` & `mypy-boto3-fms-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-fms-1.26.5/PKG-INFO` & `mypy-boto3-fms-1.27.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.26.5
-Summary: Type annotations for boto3.FMS 1.26.5 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.FMS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
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
 
 <a id="mypy-boto3-fms"></a>
 
 # mypy-boto3-fms
 
 [![PyPI - mypy-boto3-fms](https://img.shields.io/pypi/v/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fms?color=blue)](https://pypistats.org/packages/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.26.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,26 +278,34 @@
 `mypy_boto3_fms.paginator` module contains type annotations for all paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_fms import FMSClient
 from mypy_boto3_fms.paginator import (
+    ListAdminAccountsForOrganizationPaginator,
+    ListAdminsManagingAccountPaginator,
     ListAppsListsPaginator,
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 
 client: FMSClient = Session().client("fms")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+list_admin_accounts_for_organization_paginator: ListAdminAccountsForOrganizationPaginator = (
+    client.get_paginator("list_admin_accounts_for_organization")
+)
+list_admins_managing_account_paginator: ListAdminsManagingAccountPaginator = client.get_paginator(
+    "list_admins_managing_account"
+)
 list_apps_lists_paginator: ListAppsListsPaginator = client.get_paginator("list_apps_lists")
 list_compliance_status_paginator: ListComplianceStatusPaginator = client.get_paginator(
     "list_compliance_status"
 )
 list_member_accounts_paginator: ListMemberAccountsPaginator = client.get_paginator(
     "list_member_accounts"
 )
@@ -316,28 +325,33 @@
 `mypy_boto3_fms.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_fms.literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
+    CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
     FailedItemReasonType,
     FirewallDeploymentModelType,
+    ListAdminAccountsForOrganizationPaginatorName,
+    ListAdminsManagingAccountPaginatorName,
     ListAppsListsPaginatorName,
     ListComplianceStatusPaginatorName,
     ListMemberAccountsPaginatorName,
     ListPoliciesPaginatorName,
     ListProtocolsListsPaginatorName,
     ListThirdPartyFirewallFirewallPoliciesPaginatorName,
     MarketplaceSubscriptionOnboardingStatusType,
     NetworkFirewallOverrideActionType,
+    OrganizationStatusType,
     PolicyComplianceStatusTypeType,
     RemediationActionTypeType,
+    ResourceSetStatusType,
     RuleOrderType,
     SecurityServiceTypeType,
     TargetTypeType,
     ThirdPartyFirewallAssociationStatusType,
     ThirdPartyFirewallType,
     ViolationReasonType,
     FMSServiceName,
@@ -357,116 +371,129 @@
 ### Typed dictionaries
 
 `mypy_boto3_fms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_fms.type_defs import (
+    AccountScopeTypeDef,
     ActionTargetTypeDef,
+    AdminAccountSummaryTypeDef,
+    OrganizationalUnitScopeTypeDef,
+    PolicyTypeScopeTypeDef,
+    RegionScopeTypeDef,
     AppTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateThirdPartyFirewallResponseTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
     FailedItemTypeDef,
     BatchDisassociateResourceRequestRequestTypeDef,
     ComplianceViolatorTypeDef,
     DeleteAppsListRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     DeleteProtocolsListRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
     DisassociateThirdPartyFirewallRequestRequestTypeDef,
+    DisassociateThirdPartyFirewallResponseTypeDef,
     DiscoveredResourceTypeDef,
     DnsDuplicateRuleGroupViolationTypeDef,
     DnsRuleGroupLimitExceededViolationTypeDef,
     DnsRuleGroupPriorityConflictViolationTypeDef,
+    EmptyResponseMetadataTypeDef,
     EvaluationResultTypeDef,
     ExpectedRouteTypeDef,
     FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
     FirewallSubnetIsOutOfScopeViolationTypeDef,
     FirewallSubnetMissingVPCEndpointViolationTypeDef,
+    GetAdminAccountResponseTypeDef,
+    GetAdminScopeRequestRequestTypeDef,
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
+    GetNotificationChannelResponseTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetProtectionStatusRequestRequestTypeDef,
+    GetProtectionStatusResponseTypeDef,
     GetProtocolsListRequestRequestTypeDef,
     ProtocolsListDataTypeDef,
     GetResourceSetRequestRequestTypeDef,
     ResourceSetTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
+    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    ListAdminAccountsForOrganizationRequestRequestTypeDef,
+    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
+    ListAdminsManagingAccountRequestRequestTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
+    ListAppsListsRequestListAppsListsPaginateTypeDef,
     ListAppsListsRequestRequestTypeDef,
+    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     ListComplianceStatusRequestRequestTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
+    ListMemberAccountsResponseTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     PolicySummaryTypeDef,
+    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
     ListProtocolsListsRequestRequestTypeDef,
     ProtocolsListDataSummaryTypeDef,
     ListResourceSetResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ResourceSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
+    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     ThirdPartyFirewallFirewallPolicyTypeDef,
     RouteTypeDef,
     NetworkFirewallMissingExpectedRTViolationTypeDef,
     NetworkFirewallMissingFirewallViolationTypeDef,
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
+    PaginatorConfigTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
     ResourceTagTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
+    ResponseMetadataTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
     EC2CreateRouteActionTypeDef,
     EC2CreateRouteTableActionTypeDef,
     EC2DeleteRouteActionTypeDef,
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    AdminScopeTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
-    AssociateThirdPartyFirewallResponseTypeDef,
-    DisassociateThirdPartyFirewallResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAdminAccountResponseTypeDef,
-    GetNotificationChannelResponseTypeDef,
-    GetProtectionStatusResponseTypeDef,
-    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
-    ListMemberAccountsResponseTypeDef,
     AwsEc2InstanceViolationTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     PolicyComplianceDetailTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     PolicyComplianceStatusTypeDef,
     NetworkFirewallMissingExpectedRoutesViolationTypeDef,
     GetProtocolsListResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     GetResourceSetResponseTypeDef,
     PutResourceSetResponseTypeDef,
-    ListAppsListsRequestListAppsListsPaginateTypeDef,
-    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
-    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
-    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutProtocolsListRequestRequestTypeDef,
     PutResourceSetRequestRequestTypeDef,
@@ -478,14 +505,16 @@
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
     PolicyOptionTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
+    GetAdminScopeResponseTypeDef,
+    PutAdminAccountRequestRequestTypeDef,
     ListAppsListsResponseTypeDef,
     GetAppsListResponseTypeDef,
     PutAppsListRequestRequestTypeDef,
     PutAppsListResponseTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
@@ -501,53 +530,53 @@
     PossibleRemediationActionsTypeDef,
     ResourceViolationTypeDef,
     ViolationDetailTypeDef,
     GetViolationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> ActionTargetTypeDef:
+def get_structure() -> AccountScopeTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-fms-1.26.5/README.md` & `mypy-boto3-fms-1.27.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-fms"></a>
 
 # mypy-boto3-fms
 
 [![PyPI - mypy-boto3-fms](https://img.shields.io/pypi/v/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fms?color=blue)](https://pypistats.org/packages/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.26.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -246,26 +246,34 @@
 `mypy_boto3_fms.paginator` module contains type annotations for all paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_fms import FMSClient
 from mypy_boto3_fms.paginator import (
+    ListAdminAccountsForOrganizationPaginator,
+    ListAdminsManagingAccountPaginator,
     ListAppsListsPaginator,
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 
 client: FMSClient = Session().client("fms")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+list_admin_accounts_for_organization_paginator: ListAdminAccountsForOrganizationPaginator = (
+    client.get_paginator("list_admin_accounts_for_organization")
+)
+list_admins_managing_account_paginator: ListAdminsManagingAccountPaginator = client.get_paginator(
+    "list_admins_managing_account"
+)
 list_apps_lists_paginator: ListAppsListsPaginator = client.get_paginator("list_apps_lists")
 list_compliance_status_paginator: ListComplianceStatusPaginator = client.get_paginator(
     "list_compliance_status"
 )
 list_member_accounts_paginator: ListMemberAccountsPaginator = client.get_paginator(
     "list_member_accounts"
 )
@@ -285,28 +293,33 @@
 `mypy_boto3_fms.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_fms.literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
+    CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
     FailedItemReasonType,
     FirewallDeploymentModelType,
+    ListAdminAccountsForOrganizationPaginatorName,
+    ListAdminsManagingAccountPaginatorName,
     ListAppsListsPaginatorName,
     ListComplianceStatusPaginatorName,
     ListMemberAccountsPaginatorName,
     ListPoliciesPaginatorName,
     ListProtocolsListsPaginatorName,
     ListThirdPartyFirewallFirewallPoliciesPaginatorName,
     MarketplaceSubscriptionOnboardingStatusType,
     NetworkFirewallOverrideActionType,
+    OrganizationStatusType,
     PolicyComplianceStatusTypeType,
     RemediationActionTypeType,
+    ResourceSetStatusType,
     RuleOrderType,
     SecurityServiceTypeType,
     TargetTypeType,
     ThirdPartyFirewallAssociationStatusType,
     ThirdPartyFirewallType,
     ViolationReasonType,
     FMSServiceName,
@@ -326,116 +339,129 @@
 ### Typed dictionaries
 
 `mypy_boto3_fms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_fms.type_defs import (
+    AccountScopeTypeDef,
     ActionTargetTypeDef,
+    AdminAccountSummaryTypeDef,
+    OrganizationalUnitScopeTypeDef,
+    PolicyTypeScopeTypeDef,
+    RegionScopeTypeDef,
     AppTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateThirdPartyFirewallResponseTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
     FailedItemTypeDef,
     BatchDisassociateResourceRequestRequestTypeDef,
     ComplianceViolatorTypeDef,
     DeleteAppsListRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     DeleteProtocolsListRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
     DisassociateThirdPartyFirewallRequestRequestTypeDef,
+    DisassociateThirdPartyFirewallResponseTypeDef,
     DiscoveredResourceTypeDef,
     DnsDuplicateRuleGroupViolationTypeDef,
     DnsRuleGroupLimitExceededViolationTypeDef,
     DnsRuleGroupPriorityConflictViolationTypeDef,
+    EmptyResponseMetadataTypeDef,
     EvaluationResultTypeDef,
     ExpectedRouteTypeDef,
     FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
     FirewallSubnetIsOutOfScopeViolationTypeDef,
     FirewallSubnetMissingVPCEndpointViolationTypeDef,
+    GetAdminAccountResponseTypeDef,
+    GetAdminScopeRequestRequestTypeDef,
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
+    GetNotificationChannelResponseTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetProtectionStatusRequestRequestTypeDef,
+    GetProtectionStatusResponseTypeDef,
     GetProtocolsListRequestRequestTypeDef,
     ProtocolsListDataTypeDef,
     GetResourceSetRequestRequestTypeDef,
     ResourceSetTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
+    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    ListAdminAccountsForOrganizationRequestRequestTypeDef,
+    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
+    ListAdminsManagingAccountRequestRequestTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
+    ListAppsListsRequestListAppsListsPaginateTypeDef,
     ListAppsListsRequestRequestTypeDef,
+    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     ListComplianceStatusRequestRequestTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
+    ListMemberAccountsResponseTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     PolicySummaryTypeDef,
+    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
     ListProtocolsListsRequestRequestTypeDef,
     ProtocolsListDataSummaryTypeDef,
     ListResourceSetResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ResourceSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
+    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     ThirdPartyFirewallFirewallPolicyTypeDef,
     RouteTypeDef,
     NetworkFirewallMissingExpectedRTViolationTypeDef,
     NetworkFirewallMissingFirewallViolationTypeDef,
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
+    PaginatorConfigTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
     ResourceTagTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
+    ResponseMetadataTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
     EC2CreateRouteActionTypeDef,
     EC2CreateRouteTableActionTypeDef,
     EC2DeleteRouteActionTypeDef,
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    AdminScopeTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
-    AssociateThirdPartyFirewallResponseTypeDef,
-    DisassociateThirdPartyFirewallResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAdminAccountResponseTypeDef,
-    GetNotificationChannelResponseTypeDef,
-    GetProtectionStatusResponseTypeDef,
-    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
-    ListMemberAccountsResponseTypeDef,
     AwsEc2InstanceViolationTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     PolicyComplianceDetailTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     PolicyComplianceStatusTypeDef,
     NetworkFirewallMissingExpectedRoutesViolationTypeDef,
     GetProtocolsListResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     GetResourceSetResponseTypeDef,
     PutResourceSetResponseTypeDef,
-    ListAppsListsRequestListAppsListsPaginateTypeDef,
-    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
-    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
-    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutProtocolsListRequestRequestTypeDef,
     PutResourceSetRequestRequestTypeDef,
@@ -447,14 +473,16 @@
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
     PolicyOptionTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
+    GetAdminScopeResponseTypeDef,
+    PutAdminAccountRequestRequestTypeDef,
     ListAppsListsResponseTypeDef,
     GetAppsListResponseTypeDef,
     PutAppsListRequestRequestTypeDef,
     PutAppsListResponseTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
@@ -470,53 +498,53 @@
     PossibleRemediationActionsTypeDef,
     ResourceViolationTypeDef,
     ViolationDetailTypeDef,
     GetViolationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> ActionTargetTypeDef:
+def get_structure() -> AccountScopeTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-fms-1.26.5/mypy_boto3_fms/__main__.py` & `mypy-boto3-fms-1.27.0/mypy_boto3_fms/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FMS 1.26.5\nVersion:         1.26.5\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.FMS 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.5")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-fms-1.26.5/mypy_boto3_fms/client.py` & `mypy-boto3-fms-1.27.0/mypy_boto3_fms/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,39 +15,46 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
+from .literals import ThirdPartyFirewallType
 from .paginator import (
+    ListAdminAccountsForOrganizationPaginator,
+    ListAdminsManagingAccountPaginator,
     ListAppsListsPaginator,
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 from .type_defs import (
+    AdminScopeTypeDef,
     AppsListDataTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
+    GetAdminScopeResponseTypeDef,
     GetAppsListResponseTypeDef,
     GetComplianceDetailResponseTypeDef,
     GetNotificationChannelResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProtectionStatusResponseTypeDef,
     GetProtocolsListResponseTypeDef,
     GetResourceSetResponseTypeDef,
     GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsResponseTypeDef,
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
     ListAppsListsResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
@@ -106,22 +113,22 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#exceptions)
         """
 
     def associate_admin_account(self, *, AdminAccount: str) -> EmptyResponseMetadataTypeDef:
         """
-        Sets the Firewall Manager administrator account.
+        Sets a Firewall Manager default administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.associate_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#associate_admin_account)
         """
 
     def associate_third_party_firewall(
-        self, *, ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
+        self, *, ThirdPartyFirewall: ThirdPartyFirewallType
     ) -> AssociateThirdPartyFirewallResponseTypeDef:
         """
         Sets the Firewall Manager policy administrator as a tenant administrator of a
         third-party firewall service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.associate_third_party_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#associate_third_party_firewall)
@@ -197,31 +204,30 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_protocols_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#delete_protocols_list)
         """
 
     def delete_resource_set(self, *, Identifier: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the specified  ResourceSet .
+        Deletes the specified  ResourceSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#delete_resource_set)
         """
 
     def disassociate_admin_account(self) -> EmptyResponseMetadataTypeDef:
         """
-        Disassociates the account that has been set as the Firewall Manager
-        administrator account.
+        Disassociates an Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.disassociate_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#disassociate_admin_account)
         """
 
     def disassociate_third_party_firewall(
-        self, *, ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
+        self, *, ThirdPartyFirewall: ThirdPartyFirewallType
     ) -> DisassociateThirdPartyFirewallResponseTypeDef:
         """
         Disassociates a Firewall Manager policy administrator from a third-party
         firewall tenant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.disassociate_third_party_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#disassociate_third_party_firewall)
@@ -240,20 +246,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#generate_presigned_url)
         """
 
     def get_admin_account(self) -> GetAdminAccountResponseTypeDef:
         """
         Returns the Organizations account that is associated with Firewall Manager as
-        the Firewall Manager administrator.
+        the Firewall Manager default administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_admin_account)
         """
 
+    def get_admin_scope(self, *, AdminAccount: str) -> GetAdminScopeResponseTypeDef:
+        """
+        Returns information about the specified account's administrative scope.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_admin_scope)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_admin_scope)
+        """
+
     def get_apps_list(self, *, ListId: str, DefaultList: bool = ...) -> GetAppsListResponseTypeDef:
         """
         Returns information about the specified Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_apps_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_apps_list)
         """
@@ -318,15 +332,15 @@
         Gets information about a specific resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_resource_set)
         """
 
     def get_third_party_firewall_association_status(
-        self, *, ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
+        self, *, ThirdPartyFirewall: ThirdPartyFirewallType
     ) -> GetThirdPartyFirewallAssociationStatusResponseTypeDef:
         """
         The onboarding status of a Firewall Manager admin account to third-party
         firewall vendor tenant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_third_party_firewall_association_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_third_party_firewall_association_status)
@@ -339,14 +353,36 @@
         Retrieves violations for a resource based on the specified Firewall Manager
         policy and Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_violation_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_violation_details)
         """
 
+    def list_admin_accounts_for_organization(
+        self, *, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListAdminAccountsForOrganizationResponseTypeDef:
+        """
+        Returns a `AdminAccounts` object that lists the Firewall Manager administrators
+        within the organization that are onboarded to Firewall Manager by
+        AssociateAdminAccount.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_admin_accounts_for_organization)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_admin_accounts_for_organization)
+        """
+
+    def list_admins_managing_account(
+        self, *, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListAdminsManagingAccountResponseTypeDef:
+        """
+        Lists the accounts that are managing the specified Organizations member account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_admins_managing_account)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_admins_managing_account)
+        """
+
     def list_apps_lists(
         self, *, MaxResults: int, DefaultLists: bool = ..., NextToken: str = ...
     ) -> ListAppsListsResponseTypeDef:
         """
         Returns an array of `AppsListDataSummary` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_apps_lists)
@@ -435,28 +471,34 @@
         Retrieves the list of tags for the specified Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_tags_for_resource)
         """
 
     def list_third_party_firewall_firewall_policies(
-        self,
-        *,
-        ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
-        MaxResults: int,
-        NextToken: str = ...
+        self, *, ThirdPartyFirewall: ThirdPartyFirewallType, MaxResults: int, NextToken: str = ...
     ) -> ListThirdPartyFirewallFirewallPoliciesResponseTypeDef:
         """
         Retrieves a list of all of the third-party firewall policies that are associated
         with the third-party firewall administrator's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_third_party_firewall_firewall_policies)
         """
 
+    def put_admin_account(
+        self, *, AdminAccount: str, AdminScope: AdminScopeTypeDef = ...
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Creates or updates an Firewall Manager administrator account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_admin_account)
+        """
+
     def put_apps_list(
         self, *, AppsList: AppsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutAppsListResponseTypeDef:
         """
         Creates an Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)
@@ -517,14 +559,32 @@
         Removes one or more tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#untag_resource)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_admin_accounts_for_organization"]
+    ) -> ListAdminAccountsForOrganizationPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_admins_managing_account"]
+    ) -> ListAdminsManagingAccountPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_apps_lists"]) -> ListAppsListsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_paginator)
         """
 
     @overload
```

### Comparing `mypy-boto3-fms-1.26.5/mypy_boto3_fms/client.pyi` & `mypy-boto3-fms-1.27.0/mypy_boto3_fms/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,39 +15,46 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
+from .literals import ThirdPartyFirewallType
 from .paginator import (
+    ListAdminAccountsForOrganizationPaginator,
+    ListAdminsManagingAccountPaginator,
     ListAppsListsPaginator,
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 from .type_defs import (
+    AdminScopeTypeDef,
     AppsListDataTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
+    GetAdminScopeResponseTypeDef,
     GetAppsListResponseTypeDef,
     GetComplianceDetailResponseTypeDef,
     GetNotificationChannelResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProtectionStatusResponseTypeDef,
     GetProtocolsListResponseTypeDef,
     GetResourceSetResponseTypeDef,
     GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsResponseTypeDef,
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
     ListAppsListsResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
@@ -101,21 +108,21 @@
         FMSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#exceptions)
         """
     def associate_admin_account(self, *, AdminAccount: str) -> EmptyResponseMetadataTypeDef:
         """
-        Sets the Firewall Manager administrator account.
+        Sets a Firewall Manager default administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.associate_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#associate_admin_account)
         """
     def associate_third_party_firewall(
-        self, *, ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
+        self, *, ThirdPartyFirewall: ThirdPartyFirewallType
     ) -> AssociateThirdPartyFirewallResponseTypeDef:
         """
         Sets the Firewall Manager policy administrator as a tenant administrator of a
         third-party firewall service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.associate_third_party_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#associate_third_party_firewall)
@@ -182,29 +189,28 @@
         Permanently deletes an Firewall Manager protocols list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_protocols_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#delete_protocols_list)
         """
     def delete_resource_set(self, *, Identifier: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the specified  ResourceSet .
+        Deletes the specified  ResourceSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#delete_resource_set)
         """
     def disassociate_admin_account(self) -> EmptyResponseMetadataTypeDef:
         """
-        Disassociates the account that has been set as the Firewall Manager
-        administrator account.
+        Disassociates an Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.disassociate_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#disassociate_admin_account)
         """
     def disassociate_third_party_firewall(
-        self, *, ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
+        self, *, ThirdPartyFirewall: ThirdPartyFirewallType
     ) -> DisassociateThirdPartyFirewallResponseTypeDef:
         """
         Disassociates a Firewall Manager policy administrator from a third-party
         firewall tenant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.disassociate_third_party_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#disassociate_third_party_firewall)
@@ -221,19 +227,26 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#generate_presigned_url)
         """
     def get_admin_account(self) -> GetAdminAccountResponseTypeDef:
         """
         Returns the Organizations account that is associated with Firewall Manager as
-        the Firewall Manager administrator.
+        the Firewall Manager default administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_admin_account)
         """
+    def get_admin_scope(self, *, AdminAccount: str) -> GetAdminScopeResponseTypeDef:
+        """
+        Returns information about the specified account's administrative scope.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_admin_scope)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_admin_scope)
+        """
     def get_apps_list(self, *, ListId: str, DefaultList: bool = ...) -> GetAppsListResponseTypeDef:
         """
         Returns information about the specified Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_apps_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_apps_list)
         """
@@ -291,15 +304,15 @@
         """
         Gets information about a specific resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_resource_set)
         """
     def get_third_party_firewall_association_status(
-        self, *, ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
+        self, *, ThirdPartyFirewall: ThirdPartyFirewallType
     ) -> GetThirdPartyFirewallAssociationStatusResponseTypeDef:
         """
         The onboarding status of a Firewall Manager admin account to third-party
         firewall vendor tenant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_third_party_firewall_association_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_third_party_firewall_association_status)
@@ -310,14 +323,34 @@
         """
         Retrieves violations for a resource based on the specified Firewall Manager
         policy and Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_violation_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_violation_details)
         """
+    def list_admin_accounts_for_organization(
+        self, *, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListAdminAccountsForOrganizationResponseTypeDef:
+        """
+        Returns a `AdminAccounts` object that lists the Firewall Manager administrators
+        within the organization that are onboarded to Firewall Manager by
+        AssociateAdminAccount.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_admin_accounts_for_organization)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_admin_accounts_for_organization)
+        """
+    def list_admins_managing_account(
+        self, *, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListAdminsManagingAccountResponseTypeDef:
+        """
+        Lists the accounts that are managing the specified Organizations member account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_admins_managing_account)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_admins_managing_account)
+        """
     def list_apps_lists(
         self, *, MaxResults: int, DefaultLists: bool = ..., NextToken: str = ...
     ) -> ListAppsListsResponseTypeDef:
         """
         Returns an array of `AppsListDataSummary` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_apps_lists)
@@ -397,27 +430,32 @@
         """
         Retrieves the list of tags for the specified Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_tags_for_resource)
         """
     def list_third_party_firewall_firewall_policies(
-        self,
-        *,
-        ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
-        MaxResults: int,
-        NextToken: str = ...
+        self, *, ThirdPartyFirewall: ThirdPartyFirewallType, MaxResults: int, NextToken: str = ...
     ) -> ListThirdPartyFirewallFirewallPoliciesResponseTypeDef:
         """
         Retrieves a list of all of the third-party firewall policies that are associated
         with the third-party firewall administrator's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_third_party_firewall_firewall_policies)
         """
+    def put_admin_account(
+        self, *, AdminAccount: str, AdminScope: AdminScopeTypeDef = ...
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Creates or updates an Firewall Manager administrator account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_admin_account)
+        """
     def put_apps_list(
         self, *, AppsList: AppsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutAppsListResponseTypeDef:
         """
         Creates an Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)
@@ -471,14 +509,30 @@
         """
         Removes one or more tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#untag_resource)
         """
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_admin_accounts_for_organization"]
+    ) -> ListAdminAccountsForOrganizationPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_admins_managing_account"]
+    ) -> ListAdminsManagingAccountPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_paginator)
+        """
+    @overload
     def get_paginator(self, operation_name: Literal["list_apps_lists"]) -> ListAppsListsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_paginator)
         """
     @overload
     def get_paginator(
```

### Comparing `mypy-boto3-fms-1.26.5/mypy_boto3_fms/literals.py` & `mypy-boto3-fms-1.27.0/mypy_boto3_fms/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,33 @@
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AccountRoleStatusType",
     "CustomerPolicyScopeIdTypeType",
+    "CustomerPolicyStatusType",
     "DependentServiceNameType",
     "DestinationTypeType",
     "FailedItemReasonType",
     "FirewallDeploymentModelType",
+    "ListAdminAccountsForOrganizationPaginatorName",
+    "ListAdminsManagingAccountPaginatorName",
     "ListAppsListsPaginatorName",
     "ListComplianceStatusPaginatorName",
     "ListMemberAccountsPaginatorName",
     "ListPoliciesPaginatorName",
     "ListProtocolsListsPaginatorName",
     "ListThirdPartyFirewallFirewallPoliciesPaginatorName",
     "MarketplaceSubscriptionOnboardingStatusType",
     "NetworkFirewallOverrideActionType",
+    "OrganizationStatusType",
     "PolicyComplianceStatusTypeType",
     "RemediationActionTypeType",
+    "ResourceSetStatusType",
     "RuleOrderType",
     "SecurityServiceTypeType",
     "TargetTypeType",
     "ThirdPartyFirewallAssociationStatusType",
     "ThirdPartyFirewallType",
     "ViolationReasonType",
     "FMSServiceName",
@@ -48,37 +53,44 @@
     "PaginatorName",
     "RegionName",
 )
 
 
 AccountRoleStatusType = Literal["CREATING", "DELETED", "DELETING", "PENDING_DELETION", "READY"]
 CustomerPolicyScopeIdTypeType = Literal["ACCOUNT", "ORG_UNIT"]
+CustomerPolicyStatusType = Literal["ACTIVE", "OUT_OF_ADMIN_SCOPE"]
 DependentServiceNameType = Literal["AWSCONFIG", "AWSSHIELD_ADVANCED", "AWSVPC", "AWSWAF"]
 DestinationTypeType = Literal["IPV4", "IPV6", "PREFIX_LIST"]
 FailedItemReasonType = Literal[
     "NOT_VALID_ACCOUNT_ID",
     "NOT_VALID_ARN",
     "NOT_VALID_PARTITION",
     "NOT_VALID_REGION",
     "NOT_VALID_RESOURCE_TYPE",
     "NOT_VALID_SERVICE",
 ]
 FirewallDeploymentModelType = Literal["CENTRALIZED", "DISTRIBUTED"]
+ListAdminAccountsForOrganizationPaginatorName = Literal["list_admin_accounts_for_organization"]
+ListAdminsManagingAccountPaginatorName = Literal["list_admins_managing_account"]
 ListAppsListsPaginatorName = Literal["list_apps_lists"]
 ListComplianceStatusPaginatorName = Literal["list_compliance_status"]
 ListMemberAccountsPaginatorName = Literal["list_member_accounts"]
 ListPoliciesPaginatorName = Literal["list_policies"]
 ListProtocolsListsPaginatorName = Literal["list_protocols_lists"]
 ListThirdPartyFirewallFirewallPoliciesPaginatorName = Literal[
     "list_third_party_firewall_firewall_policies"
 ]
 MarketplaceSubscriptionOnboardingStatusType = Literal["COMPLETE", "NOT_COMPLETE", "NO_SUBSCRIPTION"]
 NetworkFirewallOverrideActionType = Literal["DROP_TO_ALERT"]
+OrganizationStatusType = Literal[
+    "OFFBOARDING", "OFFBOARDING_COMPLETE", "ONBOARDING", "ONBOARDING_COMPLETE"
+]
 PolicyComplianceStatusTypeType = Literal["COMPLIANT", "NON_COMPLIANT"]
 RemediationActionTypeType = Literal["MODIFY", "REMOVE"]
+ResourceSetStatusType = Literal["ACTIVE", "OUT_OF_ADMIN_SCOPE"]
 RuleOrderType = Literal["DEFAULT_ACTION_ORDER", "STRICT_ORDER"]
 SecurityServiceTypeType = Literal[
     "DNS_FIREWALL",
     "IMPORT_NETWORK_FIREWALL",
     "NETWORK_FIREWALL",
     "SECURITY_GROUPS_COMMON",
     "SECURITY_GROUPS_CONTENT_AUDIT",
@@ -99,15 +111,15 @@
     "TRANSIT_GATEWAY",
     "VPC_ENDPOINT",
     "VPC_PEERING_CONNECTION",
 ]
 ThirdPartyFirewallAssociationStatusType = Literal[
     "NOT_EXIST", "OFFBOARDING", "OFFBOARD_COMPLETE", "ONBOARDING", "ONBOARD_COMPLETE"
 ]
-ThirdPartyFirewallType = Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
+ThirdPartyFirewallType = Literal["FORTIGATE_CLOUD_NATIVE_FIREWALL", "PALO_ALTO_NETWORKS_CLOUD_NGFW"]
 ViolationReasonType = Literal[
     "BLACK_HOLE_ROUTE_DETECTED",
     "BLACK_HOLE_ROUTE_DETECTED_IN_FIREWALL_SUBNET",
     "FIREWALL_SUBNET_IS_OUT_OF_SCOPE",
     "FIREWALL_SUBNET_MISSING_EXPECTED_ROUTE",
     "FIREWALL_SUBNET_MISSING_VPCE_ENDPOINT",
     "FMS_CREATED_SECURITY_GROUP_EDITED",
@@ -146,23 +158,25 @@
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
@@ -172,30 +186,35 @@
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
@@ -221,14 +240,15 @@
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
@@ -273,51 +293,57 @@
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
@@ -330,14 +356,15 @@
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
@@ -349,28 +376,35 @@
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
@@ -398,55 +432,64 @@
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
@@ -465,37 +508,45 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
+    "list_admin_accounts_for_organization",
+    "list_admins_managing_account",
     "list_apps_lists",
     "list_compliance_status",
     "list_member_accounts",
     "list_policies",
     "list_protocols_lists",
     "list_third_party_firewall_firewall_policies",
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
+    "ap-southeast-3",
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

### Comparing `mypy-boto3-fms-1.26.5/mypy_boto3_fms/literals.pyi` & `mypy-boto3-fms-1.27.0/mypy_boto3_fms/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -17,28 +17,33 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AccountRoleStatusType",
     "CustomerPolicyScopeIdTypeType",
+    "CustomerPolicyStatusType",
     "DependentServiceNameType",
     "DestinationTypeType",
     "FailedItemReasonType",
     "FirewallDeploymentModelType",
+    "ListAdminAccountsForOrganizationPaginatorName",
+    "ListAdminsManagingAccountPaginatorName",
     "ListAppsListsPaginatorName",
     "ListComplianceStatusPaginatorName",
     "ListMemberAccountsPaginatorName",
     "ListPoliciesPaginatorName",
     "ListProtocolsListsPaginatorName",
     "ListThirdPartyFirewallFirewallPoliciesPaginatorName",
     "MarketplaceSubscriptionOnboardingStatusType",
     "NetworkFirewallOverrideActionType",
+    "OrganizationStatusType",
     "PolicyComplianceStatusTypeType",
     "RemediationActionTypeType",
+    "ResourceSetStatusType",
     "RuleOrderType",
     "SecurityServiceTypeType",
     "TargetTypeType",
     "ThirdPartyFirewallAssociationStatusType",
     "ThirdPartyFirewallType",
     "ViolationReasonType",
     "FMSServiceName",
@@ -46,37 +51,44 @@
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AccountRoleStatusType = Literal["CREATING", "DELETED", "DELETING", "PENDING_DELETION", "READY"]
 CustomerPolicyScopeIdTypeType = Literal["ACCOUNT", "ORG_UNIT"]
+CustomerPolicyStatusType = Literal["ACTIVE", "OUT_OF_ADMIN_SCOPE"]
 DependentServiceNameType = Literal["AWSCONFIG", "AWSSHIELD_ADVANCED", "AWSVPC", "AWSWAF"]
 DestinationTypeType = Literal["IPV4", "IPV6", "PREFIX_LIST"]
 FailedItemReasonType = Literal[
     "NOT_VALID_ACCOUNT_ID",
     "NOT_VALID_ARN",
     "NOT_VALID_PARTITION",
     "NOT_VALID_REGION",
     "NOT_VALID_RESOURCE_TYPE",
     "NOT_VALID_SERVICE",
 ]
 FirewallDeploymentModelType = Literal["CENTRALIZED", "DISTRIBUTED"]
+ListAdminAccountsForOrganizationPaginatorName = Literal["list_admin_accounts_for_organization"]
+ListAdminsManagingAccountPaginatorName = Literal["list_admins_managing_account"]
 ListAppsListsPaginatorName = Literal["list_apps_lists"]
 ListComplianceStatusPaginatorName = Literal["list_compliance_status"]
 ListMemberAccountsPaginatorName = Literal["list_member_accounts"]
 ListPoliciesPaginatorName = Literal["list_policies"]
 ListProtocolsListsPaginatorName = Literal["list_protocols_lists"]
 ListThirdPartyFirewallFirewallPoliciesPaginatorName = Literal[
     "list_third_party_firewall_firewall_policies"
 ]
 MarketplaceSubscriptionOnboardingStatusType = Literal["COMPLETE", "NOT_COMPLETE", "NO_SUBSCRIPTION"]
 NetworkFirewallOverrideActionType = Literal["DROP_TO_ALERT"]
+OrganizationStatusType = Literal[
+    "OFFBOARDING", "OFFBOARDING_COMPLETE", "ONBOARDING", "ONBOARDING_COMPLETE"
+]
 PolicyComplianceStatusTypeType = Literal["COMPLIANT", "NON_COMPLIANT"]
 RemediationActionTypeType = Literal["MODIFY", "REMOVE"]
+ResourceSetStatusType = Literal["ACTIVE", "OUT_OF_ADMIN_SCOPE"]
 RuleOrderType = Literal["DEFAULT_ACTION_ORDER", "STRICT_ORDER"]
 SecurityServiceTypeType = Literal[
     "DNS_FIREWALL",
     "IMPORT_NETWORK_FIREWALL",
     "NETWORK_FIREWALL",
     "SECURITY_GROUPS_COMMON",
     "SECURITY_GROUPS_CONTENT_AUDIT",
@@ -97,15 +109,15 @@
     "TRANSIT_GATEWAY",
     "VPC_ENDPOINT",
     "VPC_PEERING_CONNECTION",
 ]
 ThirdPartyFirewallAssociationStatusType = Literal[
     "NOT_EXIST", "OFFBOARDING", "OFFBOARD_COMPLETE", "ONBOARDING", "ONBOARD_COMPLETE"
 ]
-ThirdPartyFirewallType = Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
+ThirdPartyFirewallType = Literal["FORTIGATE_CLOUD_NATIVE_FIREWALL", "PALO_ALTO_NETWORKS_CLOUD_NGFW"]
 ViolationReasonType = Literal[
     "BLACK_HOLE_ROUTE_DETECTED",
     "BLACK_HOLE_ROUTE_DETECTED_IN_FIREWALL_SUBNET",
     "FIREWALL_SUBNET_IS_OUT_OF_SCOPE",
     "FIREWALL_SUBNET_MISSING_EXPECTED_ROUTE",
     "FIREWALL_SUBNET_MISSING_VPCE_ENDPOINT",
     "FMS_CREATED_SECURITY_GROUP_EDITED",
@@ -144,23 +156,25 @@
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
@@ -170,30 +184,35 @@
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
@@ -219,14 +238,15 @@
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
@@ -271,51 +291,57 @@
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
@@ -328,14 +354,15 @@
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
@@ -347,28 +374,35 @@
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
@@ -396,55 +430,64 @@
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
@@ -463,37 +506,45 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
+    "list_admin_accounts_for_organization",
+    "list_admins_managing_account",
     "list_apps_lists",
     "list_compliance_status",
     "list_member_accounts",
     "list_policies",
     "list_protocols_lists",
     "list_third_party_firewall_firewall_policies",
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
+    "ap-southeast-3",
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

### Comparing `mypy-boto3-fms-1.26.5/mypy_boto3_fms/paginator.py` & `mypy-boto3-fms-1.27.0/mypy_boto3_fms/paginator.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,55 +6,57 @@
 Usage::
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_fms.client import FMSClient
     from mypy_boto3_fms.paginator import (
+        ListAdminAccountsForOrganizationPaginator,
+        ListAdminsManagingAccountPaginator,
         ListAppsListsPaginator,
         ListComplianceStatusPaginator,
         ListMemberAccountsPaginator,
         ListPoliciesPaginator,
         ListProtocolsListsPaginator,
         ListThirdPartyFirewallFirewallPoliciesPaginator,
     )
 
     session = Session()
     client: FMSClient = session.client("fms")
 
+    list_admin_accounts_for_organization_paginator: ListAdminAccountsForOrganizationPaginator = client.get_paginator("list_admin_accounts_for_organization")
+    list_admins_managing_account_paginator: ListAdminsManagingAccountPaginator = client.get_paginator("list_admins_managing_account")
     list_apps_lists_paginator: ListAppsListsPaginator = client.get_paginator("list_apps_lists")
     list_compliance_status_paginator: ListComplianceStatusPaginator = client.get_paginator("list_compliance_status")
     list_member_accounts_paginator: ListMemberAccountsPaginator = client.get_paginator("list_member_accounts")
     list_policies_paginator: ListPoliciesPaginator = client.get_paginator("list_policies")
     list_protocols_lists_paginator: ListProtocolsListsPaginator = client.get_paginator("list_protocols_lists")
     list_third_party_firewall_firewall_policies_paginator: ListThirdPartyFirewallFirewallPoliciesPaginator = client.get_paginator("list_third_party_firewall_firewall_policies")
     ```
 """
-import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
+from .literals import ThirdPartyFirewallType
 from .type_defs import (
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
     ListAppsListsResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
-if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
-
 __all__ = (
+    "ListAdminAccountsForOrganizationPaginator",
+    "ListAdminsManagingAccountPaginator",
     "ListAppsListsPaginator",
     "ListComplianceStatusPaginator",
     "ListMemberAccountsPaginator",
     "ListPoliciesPaginator",
     "ListProtocolsListsPaginator",
     "ListThirdPartyFirewallFirewallPoliciesPaginator",
 )
@@ -66,82 +68,112 @@
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
 
+class ListAdminAccountsForOrganizationPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminAccountsForOrganization)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminaccountsfororganizationpaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListAdminAccountsForOrganizationResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminAccountsForOrganization.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminaccountsfororganizationpaginator)
+        """
+
+
+class ListAdminsManagingAccountPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminsManagingAccount)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminsmanagingaccountpaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListAdminsManagingAccountResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminsManagingAccount.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminsmanagingaccountpaginator)
+        """
+
+
 class ListAppsListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listappslistspaginator)
     """
 
     def paginate(
-        self, *, DefaultLists: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DefaultLists: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAppsListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listappslistspaginator)
         """
 
 
 class ListComplianceStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listcompliancestatuspaginator)
     """
 
     def paginate(
-        self, *, PolicyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PolicyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComplianceStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listcompliancestatuspaginator)
         """
 
 
 class ListMemberAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listmemberaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMemberAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listmemberaccountspaginator)
         """
 
 
 class ListPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listpoliciespaginator)
         """
 
 
 class ListProtocolsListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listprotocolslistspaginator)
     """
 
     def paginate(
-        self, *, DefaultLists: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DefaultLists: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProtocolsListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listprotocolslistspaginator)
         """
 
 
@@ -150,14 +182,14 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
-        ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        ThirdPartyFirewall: ThirdPartyFirewallType,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
         """
```

### Comparing `mypy-boto3-fms-1.26.5/mypy_boto3_fms/paginator.pyi` & `mypy-boto3-fms-1.27.0/mypy_boto3_fms/paginator.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -6,54 +6,57 @@
 Usage::
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_fms.client import FMSClient
     from mypy_boto3_fms.paginator import (
+        ListAdminAccountsForOrganizationPaginator,
+        ListAdminsManagingAccountPaginator,
         ListAppsListsPaginator,
         ListComplianceStatusPaginator,
         ListMemberAccountsPaginator,
         ListPoliciesPaginator,
         ListProtocolsListsPaginator,
         ListThirdPartyFirewallFirewallPoliciesPaginator,
     )
 
     session = Session()
     client: FMSClient = session.client("fms")
 
+    list_admin_accounts_for_organization_paginator: ListAdminAccountsForOrganizationPaginator = client.get_paginator("list_admin_accounts_for_organization")
+    list_admins_managing_account_paginator: ListAdminsManagingAccountPaginator = client.get_paginator("list_admins_managing_account")
     list_apps_lists_paginator: ListAppsListsPaginator = client.get_paginator("list_apps_lists")
     list_compliance_status_paginator: ListComplianceStatusPaginator = client.get_paginator("list_compliance_status")
     list_member_accounts_paginator: ListMemberAccountsPaginator = client.get_paginator("list_member_accounts")
     list_policies_paginator: ListPoliciesPaginator = client.get_paginator("list_policies")
     list_protocols_lists_paginator: ListProtocolsListsPaginator = client.get_paginator("list_protocols_lists")
     list_third_party_firewall_firewall_policies_paginator: ListThirdPartyFirewallFirewallPoliciesPaginator = client.get_paginator("list_third_party_firewall_firewall_policies")
     ```
 """
-import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
+from .literals import ThirdPartyFirewallType
 from .type_defs import (
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
     ListAppsListsResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
-if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
 __all__ = (
+    "ListAdminAccountsForOrganizationPaginator",
+    "ListAdminsManagingAccountPaginator",
     "ListAppsListsPaginator",
     "ListComplianceStatusPaginator",
     "ListMemberAccountsPaginator",
     "ListPoliciesPaginator",
     "ListProtocolsListsPaginator",
     "ListThirdPartyFirewallFirewallPoliciesPaginator",
 )
@@ -62,78 +65,106 @@
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+class ListAdminAccountsForOrganizationPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminAccountsForOrganization)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminaccountsfororganizationpaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListAdminAccountsForOrganizationResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminAccountsForOrganization.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminaccountsfororganizationpaginator)
+        """
+
+class ListAdminsManagingAccountPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminsManagingAccount)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminsmanagingaccountpaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListAdminsManagingAccountResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminsManagingAccount.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminsmanagingaccountpaginator)
+        """
+
 class ListAppsListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listappslistspaginator)
     """
 
     def paginate(
-        self, *, DefaultLists: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DefaultLists: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAppsListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listappslistspaginator)
         """
 
 class ListComplianceStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listcompliancestatuspaginator)
     """
 
     def paginate(
-        self, *, PolicyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PolicyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComplianceStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listcompliancestatuspaginator)
         """
 
 class ListMemberAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listmemberaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMemberAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listmemberaccountspaginator)
         """
 
 class ListPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listpoliciespaginator)
         """
 
 class ListProtocolsListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listprotocolslistspaginator)
     """
 
     def paginate(
-        self, *, DefaultLists: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DefaultLists: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProtocolsListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listprotocolslistspaginator)
         """
 
 class ListThirdPartyFirewallFirewallPoliciesPaginator(Paginator):
@@ -141,14 +172,14 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
-        ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        ThirdPartyFirewall: ThirdPartyFirewallType,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
         """
```

### Comparing `mypy-boto3-fms-1.26.5/mypy_boto3_fms/type_defs.py` & `mypy-boto3-fms-1.27.0/mypy_boto3_fms/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,153 +2,170 @@
 Type annotations for fms service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_fms.type_defs import ActionTargetTypeDef
+    from mypy_boto3_fms.type_defs import AccountScopeTypeDef
 
-    data: ActionTargetTypeDef = {...}
+    data: AccountScopeTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
+    CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
     FailedItemReasonType,
     FirewallDeploymentModelType,
     MarketplaceSubscriptionOnboardingStatusType,
+    OrganizationStatusType,
     PolicyComplianceStatusTypeType,
     RemediationActionTypeType,
+    ResourceSetStatusType,
     RuleOrderType,
     SecurityServiceTypeType,
     TargetTypeType,
     ThirdPartyFirewallAssociationStatusType,
+    ThirdPartyFirewallType,
     ViolationReasonType,
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
+    "AccountScopeTypeDef",
     "ActionTargetTypeDef",
+    "AdminAccountSummaryTypeDef",
+    "OrganizationalUnitScopeTypeDef",
+    "PolicyTypeScopeTypeDef",
+    "RegionScopeTypeDef",
     "AppTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateThirdPartyFirewallResponseTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
     "FailedItemTypeDef",
     "BatchDisassociateResourceRequestRequestTypeDef",
     "ComplianceViolatorTypeDef",
     "DeleteAppsListRequestRequestTypeDef",
     "DeletePolicyRequestRequestTypeDef",
     "DeleteProtocolsListRequestRequestTypeDef",
     "DeleteResourceSetRequestRequestTypeDef",
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
+    "DisassociateThirdPartyFirewallResponseTypeDef",
     "DiscoveredResourceTypeDef",
     "DnsDuplicateRuleGroupViolationTypeDef",
     "DnsRuleGroupLimitExceededViolationTypeDef",
     "DnsRuleGroupPriorityConflictViolationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EvaluationResultTypeDef",
     "ExpectedRouteTypeDef",
     "FMSPolicyUpdateFirewallCreationConfigActionTypeDef",
     "FirewallSubnetIsOutOfScopeViolationTypeDef",
     "FirewallSubnetMissingVPCEndpointViolationTypeDef",
+    "GetAdminAccountResponseTypeDef",
+    "GetAdminScopeRequestRequestTypeDef",
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
+    "GetNotificationChannelResponseTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetProtectionStatusRequestRequestTypeDef",
+    "GetProtectionStatusResponseTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
     "ProtocolsListDataTypeDef",
     "GetResourceSetRequestRequestTypeDef",
     "ResourceSetTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
+    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
+    "ListAdminAccountsForOrganizationRequestRequestTypeDef",
+    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
+    "ListAdminsManagingAccountRequestRequestTypeDef",
+    "ListAdminsManagingAccountResponseTypeDef",
+    "ListAppsListsRequestListAppsListsPaginateTypeDef",
     "ListAppsListsRequestRequestTypeDef",
+    "ListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     "ListComplianceStatusRequestRequestTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
+    "ListMemberAccountsResponseTypeDef",
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
     "PolicySummaryTypeDef",
+    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
     "ListProtocolsListsRequestRequestTypeDef",
     "ProtocolsListDataSummaryTypeDef",
     "ListResourceSetResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ResourceSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
+    "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     "RouteTypeDef",
     "NetworkFirewallMissingExpectedRTViolationTypeDef",
     "NetworkFirewallMissingFirewallViolationTypeDef",
     "NetworkFirewallMissingSubnetViolationTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupTypeDef",
     "NetworkFirewallPolicyTypeDef",
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
+    "PaginatorConfigTypeDef",
     "ThirdPartyFirewallPolicyTypeDef",
     "ResourceTagTypeDef",
     "PutNotificationChannelRequestRequestTypeDef",
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     "ThirdPartyFirewallMissingFirewallViolationTypeDef",
     "ThirdPartyFirewallMissingSubnetViolationTypeDef",
+    "ResponseMetadataTypeDef",
     "SecurityGroupRuleDescriptionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
     "EC2CreateRouteActionTypeDef",
     "EC2CreateRouteTableActionTypeDef",
     "EC2DeleteRouteActionTypeDef",
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
+    "ListAdminAccountsForOrganizationResponseTypeDef",
+    "AdminScopeTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
-    "AssociateThirdPartyFirewallResponseTypeDef",
-    "DisassociateThirdPartyFirewallResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAdminAccountResponseTypeDef",
-    "GetNotificationChannelResponseTypeDef",
-    "GetProtectionStatusResponseTypeDef",
-    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
-    "ListMemberAccountsResponseTypeDef",
     "AwsEc2InstanceViolationTypeDef",
     "BatchAssociateResourceResponseTypeDef",
     "BatchDisassociateResourceResponseTypeDef",
     "PolicyComplianceDetailTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "PolicyComplianceStatusTypeDef",
     "NetworkFirewallMissingExpectedRoutesViolationTypeDef",
     "GetProtocolsListResponseTypeDef",
     "PutProtocolsListResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "PutResourceSetResponseTypeDef",
-    "ListAppsListsRequestListAppsListsPaginateTypeDef",
-    "ListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
-    "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListProtocolsListsResponseTypeDef",
     "ListResourceSetResourcesResponseTypeDef",
     "ListResourceSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutProtocolsListRequestRequestTypeDef",
     "PutResourceSetRequestRequestTypeDef",
@@ -160,14 +177,16 @@
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
     "PolicyOptionTypeDef",
     "SecurityGroupRemediationActionTypeDef",
     "RemediationActionTypeDef",
+    "GetAdminScopeResponseTypeDef",
+    "PutAdminAccountRequestRequestTypeDef",
     "ListAppsListsResponseTypeDef",
     "GetAppsListResponseTypeDef",
     "PutAppsListRequestRequestTypeDef",
     "PutAppsListResponseTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
@@ -182,23 +201,71 @@
     "PutPolicyResponseTypeDef",
     "PossibleRemediationActionsTypeDef",
     "ResourceViolationTypeDef",
     "ViolationDetailTypeDef",
     "GetViolationDetailsResponseTypeDef",
 )
 
+AccountScopeTypeDef = TypedDict(
+    "AccountScopeTypeDef",
+    {
+        "Accounts": List[str],
+        "AllAccountsEnabled": bool,
+        "ExcludeSpecifiedAccounts": bool,
+    },
+    total=False,
+)
+
 ActionTargetTypeDef = TypedDict(
     "ActionTargetTypeDef",
     {
         "ResourceId": str,
         "Description": str,
     },
     total=False,
 )
 
+AdminAccountSummaryTypeDef = TypedDict(
+    "AdminAccountSummaryTypeDef",
+    {
+        "AdminAccount": str,
+        "DefaultAdmin": bool,
+        "Status": OrganizationStatusType,
+    },
+    total=False,
+)
+
+OrganizationalUnitScopeTypeDef = TypedDict(
+    "OrganizationalUnitScopeTypeDef",
+    {
+        "OrganizationalUnits": List[str],
+        "AllOrganizationalUnitsEnabled": bool,
+        "ExcludeSpecifiedOrganizationalUnits": bool,
+    },
+    total=False,
+)
+
+PolicyTypeScopeTypeDef = TypedDict(
+    "PolicyTypeScopeTypeDef",
+    {
+        "PolicyTypes": List[SecurityServiceTypeType],
+        "AllPolicyTypesEnabled": bool,
+    },
+    total=False,
+)
+
+RegionScopeTypeDef = TypedDict(
+    "RegionScopeTypeDef",
+    {
+        "Regions": List[str],
+        "AllRegionsEnabled": bool,
+    },
+    total=False,
+)
+
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
@@ -210,26 +277,23 @@
         "AdminAccount": str,
     },
 )
 
 AssociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
+    "AssociateThirdPartyFirewallResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AwsEc2NetworkInterfaceViolationTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceViolationTypeDef",
     {
         "ViolationTarget": str,
@@ -324,15 +388,23 @@
         "Identifier": str,
     },
 )
 
 DisassociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
+    },
+)
+
+DisassociateThirdPartyFirewallResponseTypeDef = TypedDict(
+    "DisassociateThirdPartyFirewallResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DiscoveredResourceTypeDef = TypedDict(
     "DiscoveredResourceTypeDef",
     {
         "URI": str,
@@ -370,14 +442,21 @@
         "ConflictingPriority": int,
         "ConflictingPolicyId": str,
         "UnavailablePriorities": List[int],
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
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "ComplianceStatus": PolicyComplianceStatusTypeType,
         "ViolatorCount": int,
         "EvaluationLimitExceeded": bool,
     },
@@ -425,14 +504,30 @@
         "VpcId": str,
         "SubnetAvailabilityZone": str,
         "SubnetAvailabilityZoneId": str,
     },
     total=False,
 )
 
+GetAdminAccountResponseTypeDef = TypedDict(
+    "GetAdminAccountResponseTypeDef",
+    {
+        "AdminAccount": str,
+        "RoleStatus": AccountRoleStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetAdminScopeRequestRequestTypeDef = TypedDict(
+    "GetAdminScopeRequestRequestTypeDef",
+    {
+        "AdminAccount": str,
+    },
+)
+
 _RequiredGetAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetAppsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetAppsListRequestRequestTypeDef = TypedDict(
@@ -454,14 +549,23 @@
     "GetComplianceDetailRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
     },
 )
 
+GetNotificationChannelResponseTypeDef = TypedDict(
+    "GetNotificationChannelResponseTypeDef",
+    {
+        "SnsTopicArn": str,
+        "SnsRoleName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 
@@ -487,14 +591,25 @@
 class GetProtectionStatusRequestRequestTypeDef(
     _RequiredGetProtectionStatusRequestRequestTypeDef,
     _OptionalGetProtectionStatusRequestRequestTypeDef,
 ):
     pass
 
 
+GetProtectionStatusResponseTypeDef = TypedDict(
+    "GetProtectionStatusResponseTypeDef",
+    {
+        "AdminAccountId": str,
+        "ServiceType": SecurityServiceTypeType,
+        "Data": str,
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetProtocolsListRequestRequestTypeDef = TypedDict(
@@ -555,46 +670,98 @@
 _OptionalResourceSetTypeDef = TypedDict(
     "_OptionalResourceSetTypeDef",
     {
         "Id": str,
         "Description": str,
         "UpdateToken": str,
         "LastUpdateTime": datetime,
+        "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
 
 class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
     pass
 
 
 GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
+    },
+)
+
+GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
+    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetViolationDetailsRequestRequestTypeDef = TypedDict(
     "GetViolationDetailsRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
         "ResourceId": str,
         "ResourceType": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListAdminAccountsForOrganizationRequestRequestTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef = TypedDict(
+    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListAdminsManagingAccountRequestRequestTypeDef = TypedDict(
+    "ListAdminsManagingAccountRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListAdminsManagingAccountResponseTypeDef = TypedDict(
+    "ListAdminsManagingAccountResponseTypeDef",
+    {
+        "AdminAccounts": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAppsListsRequestListAppsListsPaginateTypeDef = TypedDict(
+    "ListAppsListsRequestListAppsListsPaginateTypeDef",
+    {
+        "DefaultLists": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 _RequiredListAppsListsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppsListsRequestRequestTypeDef",
     {
@@ -613,14 +780,36 @@
 
 class ListAppsListsRequestRequestTypeDef(
     _RequiredListAppsListsRequestRequestTypeDef, _OptionalListAppsListsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
+    "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    {
+        "PolicyId": str,
+    },
+)
+_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
+    "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
+    _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+    _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListComplianceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListComplianceStatusRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalListComplianceStatusRequestRequestTypeDef = TypedDict(
@@ -660,23 +849,48 @@
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
 
+ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListMemberAccountsResponseTypeDef = TypedDict(
+    "ListMemberAccountsResponseTypeDef",
+    {
+        "MemberAccounts": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPoliciesRequestRequestTypeDef = TypedDict(
     "ListPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -688,14 +902,24 @@
         "PolicyArn": str,
         "PolicyId": str,
         "PolicyName": str,
         "ResourceType": str,
         "SecurityServiceType": SecurityServiceTypeType,
         "RemediationEnabled": bool,
         "DeleteUnusedFMManagedResources": bool,
+        "PolicyStatus": CustomerPolicyStatusType,
+    },
+    total=False,
+)
+
+ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = TypedDict(
+    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
+    {
+        "DefaultLists": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 _RequiredListProtocolsListsRequestRequestTypeDef = TypedDict(
     "_RequiredListProtocolsListsRequestRequestTypeDef",
     {
@@ -784,14 +1008,15 @@
 ResourceSetSummaryTypeDef = TypedDict(
     "ResourceSetSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "LastUpdateTime": datetime,
+        "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
@@ -803,18 +1028,40 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
+    {
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
+    },
+)
+_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
+    _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+    _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
         "MaxResults": int,
     },
 )
 _OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
@@ -914,14 +1161,24 @@
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
     {
         "Action": Literal["DROP_TO_ALERT"],
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
 ThirdPartyFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallPolicyTypeDef",
     {
         "FirewallDeploymentModel": FirewallDeploymentModelType,
     },
     total=False,
 )
@@ -983,14 +1240,25 @@
         "VPC": str,
         "AvailabilityZone": str,
         "TargetViolationReason": str,
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
 SecurityGroupRuleDescriptionTypeDef = TypedDict(
     "SecurityGroupRuleDescriptionTypeDef",
     {
         "IPV4Range": str,
         "IPV6Range": str,
         "PrefixListId": str,
         "Protocol": str,
@@ -1168,14 +1436,34 @@
 class EC2ReplaceRouteTableAssociationActionTypeDef(
     _RequiredEC2ReplaceRouteTableAssociationActionTypeDef,
     _OptionalEC2ReplaceRouteTableAssociationActionTypeDef,
 ):
     pass
 
 
+ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AdminScopeTypeDef = TypedDict(
+    "AdminScopeTypeDef",
+    {
+        "AccountScope": AccountScopeTypeDef,
+        "OrganizationalUnitScope": OrganizationalUnitScopeTypeDef,
+        "RegionScope": RegionScopeTypeDef,
+        "PolicyTypeScope": PolicyTypeScopeTypeDef,
+    },
+    total=False,
+)
+
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "AppsList": List[AppTypeDef],
@@ -1203,108 +1491,38 @@
 )
 
 
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
 
-AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
-    "AssociateThirdPartyFirewallResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateThirdPartyFirewallResponseTypeDef = TypedDict(
-    "DisassociateThirdPartyFirewallResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
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
-GetAdminAccountResponseTypeDef = TypedDict(
-    "GetAdminAccountResponseTypeDef",
-    {
-        "AdminAccount": str,
-        "RoleStatus": AccountRoleStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetNotificationChannelResponseTypeDef = TypedDict(
-    "GetNotificationChannelResponseTypeDef",
-    {
-        "SnsTopicArn": str,
-        "SnsRoleName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProtectionStatusResponseTypeDef = TypedDict(
-    "GetProtectionStatusResponseTypeDef",
-    {
-        "AdminAccountId": str,
-        "ServiceType": SecurityServiceTypeType,
-        "Data": str,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
-    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListMemberAccountsResponseTypeDef = TypedDict(
-    "ListMemberAccountsResponseTypeDef",
-    {
-        "MemberAccounts": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AwsEc2InstanceViolationTypeDef = TypedDict(
     "AwsEc2InstanceViolationTypeDef",
     {
         "ViolationTarget": str,
         "AwsEc2NetworkInterfaceViolations": List[AwsEc2NetworkInterfaceViolationTypeDef],
     },
     total=False,
 )
 
 BatchAssociateResourceResponseTypeDef = TypedDict(
     "BatchAssociateResourceResponseTypeDef",
     {
         "ResourceSetIdentifier": str,
         "FailedItems": List[FailedItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisassociateResourceResponseTypeDef = TypedDict(
     "BatchDisassociateResourceResponseTypeDef",
     {
         "ResourceSetIdentifier": str,
         "FailedItems": List[FailedItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PolicyComplianceDetailTypeDef = TypedDict(
     "PolicyComplianceDetailTypeDef",
     {
         "PolicyOwner": str,
@@ -1319,15 +1537,15 @@
 )
 
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "Items": List[DiscoveredResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PolicyComplianceStatusTypeDef = TypedDict(
     "PolicyComplianceStatusTypeDef",
     {
         "PolicyOwner": str,
@@ -1352,164 +1570,86 @@
 )
 
 GetProtocolsListResponseTypeDef = TypedDict(
     "GetProtocolsListResponseTypeDef",
     {
         "ProtocolsList": ProtocolsListDataTypeDef,
         "ProtocolsListArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutProtocolsListResponseTypeDef = TypedDict(
     "PutProtocolsListResponseTypeDef",
     {
         "ProtocolsList": ProtocolsListDataTypeDef,
         "ProtocolsListArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
         "ResourceSet": ResourceSetTypeDef,
         "ResourceSetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutResourceSetResponseTypeDef = TypedDict(
     "PutResourceSetResponseTypeDef",
     {
         "ResourceSet": ResourceSetTypeDef,
         "ResourceSetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppsListsRequestListAppsListsPaginateTypeDef = TypedDict(
-    "ListAppsListsRequestListAppsListsPaginateTypeDef",
-    {
-        "DefaultLists": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
-    "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    {
-        "PolicyId": str,
-    },
-)
-_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
-    "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
-    _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-    _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-):
-    pass
-
-
-ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = TypedDict(
-    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
-    {
-        "DefaultLists": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
-    {
-        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
-    _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
-    _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
-):
-    pass
-
 
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "PolicyList": List[PolicySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProtocolsListsResponseTypeDef = TypedDict(
     "ListProtocolsListsResponseTypeDef",
     {
         "ProtocolsLists": List[ProtocolsListDataSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceSetResourcesResponseTypeDef = TypedDict(
     "ListResourceSetResourcesResponseTypeDef",
     {
         "Items": List[ResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "ResourceSets": List[ResourceSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutProtocolsListRequestRequestTypeDef",
     {
         "ProtocolsList": ProtocolsListDataTypeDef,
@@ -1560,15 +1700,15 @@
 )
 
 ListThirdPartyFirewallFirewallPoliciesResponseTypeDef = TypedDict(
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     {
         "ThirdPartyFirewallFirewallPolicies": List[ThirdPartyFirewallFirewallPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkFirewallBlackHoleRouteDetectedViolationTypeDef = TypedDict(
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     {
         "ViolationTarget": str,
@@ -1704,34 +1844,66 @@
         "EC2CreateRouteAction": EC2CreateRouteActionTypeDef,
         "EC2ReplaceRouteAction": EC2ReplaceRouteActionTypeDef,
         "EC2DeleteRouteAction": EC2DeleteRouteActionTypeDef,
         "EC2CopyRouteTableAction": EC2CopyRouteTableActionTypeDef,
         "EC2ReplaceRouteTableAssociationAction": EC2ReplaceRouteTableAssociationActionTypeDef,
         "EC2AssociateRouteTableAction": EC2AssociateRouteTableActionTypeDef,
         "EC2CreateRouteTableAction": EC2CreateRouteTableActionTypeDef,
-        "FMSPolicyUpdateFirewallCreationConfigAction": FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
+        "FMSPolicyUpdateFirewallCreationConfigAction": (
+            FMSPolicyUpdateFirewallCreationConfigActionTypeDef
+        ),
     },
     total=False,
 )
 
+GetAdminScopeResponseTypeDef = TypedDict(
+    "GetAdminScopeResponseTypeDef",
+    {
+        "AdminScope": AdminScopeTypeDef,
+        "Status": OrganizationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredPutAdminAccountRequestRequestTypeDef = TypedDict(
+    "_RequiredPutAdminAccountRequestRequestTypeDef",
+    {
+        "AdminAccount": str,
+    },
+)
+_OptionalPutAdminAccountRequestRequestTypeDef = TypedDict(
+    "_OptionalPutAdminAccountRequestRequestTypeDef",
+    {
+        "AdminScope": AdminScopeTypeDef,
+    },
+    total=False,
+)
+
+
+class PutAdminAccountRequestRequestTypeDef(
+    _RequiredPutAdminAccountRequestRequestTypeDef, _OptionalPutAdminAccountRequestRequestTypeDef
+):
+    pass
+
+
 ListAppsListsResponseTypeDef = TypedDict(
     "ListAppsListsResponseTypeDef",
     {
         "AppsLists": List[AppsListDataSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppsListResponseTypeDef = TypedDict(
     "GetAppsListResponseTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
         "AppsListArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
@@ -1753,32 +1925,32 @@
 
 
 PutAppsListResponseTypeDef = TypedDict(
     "PutAppsListResponseTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
         "AppsListArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListComplianceStatusResponseTypeDef = TypedDict(
     "ListComplianceStatusResponseTypeDef",
     {
         "PolicyComplianceStatusList": List[PolicyComplianceStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkFirewallPolicyDescriptionTypeDef = TypedDict(
     "NetworkFirewallPolicyDescriptionTypeDef",
     {
         "StatelessRuleGroups": List[StatelessRuleGroupTypeDef],
@@ -1862,14 +2034,15 @@
         "ResourceTypeList": List[str],
         "ResourceTags": List[ResourceTagTypeDef],
         "DeleteUnusedFMManagedResources": bool,
         "IncludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
         "ExcludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
         "ResourceSetIds": List[str],
         "PolicyDescription": str,
+        "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
 
 class PolicyTypeDef(_RequiredPolicyTypeDef, _OptionalPolicyTypeDef):
     pass
@@ -1898,15 +2071,15 @@
 
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "PolicyArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
@@ -1928,15 +2101,15 @@
 
 
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "PolicyArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PossibleRemediationActionsTypeDef = TypedDict(
     "PossibleRemediationActionsTypeDef",
     {
         "Description": str,
@@ -1949,32 +2122,52 @@
     "ResourceViolationTypeDef",
     {
         "AwsVPCSecurityGroupViolation": AwsVPCSecurityGroupViolationTypeDef,
         "AwsEc2NetworkInterfaceViolation": AwsEc2NetworkInterfaceViolationTypeDef,
         "AwsEc2InstanceViolation": AwsEc2InstanceViolationTypeDef,
         "NetworkFirewallMissingFirewallViolation": NetworkFirewallMissingFirewallViolationTypeDef,
         "NetworkFirewallMissingSubnetViolation": NetworkFirewallMissingSubnetViolationTypeDef,
-        "NetworkFirewallMissingExpectedRTViolation": NetworkFirewallMissingExpectedRTViolationTypeDef,
+        "NetworkFirewallMissingExpectedRTViolation": (
+            NetworkFirewallMissingExpectedRTViolationTypeDef
+        ),
         "NetworkFirewallPolicyModifiedViolation": NetworkFirewallPolicyModifiedViolationTypeDef,
-        "NetworkFirewallInternetTrafficNotInspectedViolation": NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
-        "NetworkFirewallInvalidRouteConfigurationViolation": NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
-        "NetworkFirewallBlackHoleRouteDetectedViolation": NetworkFirewallBlackHoleRouteDetectedViolationTypeDef,
-        "NetworkFirewallUnexpectedFirewallRoutesViolation": NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
-        "NetworkFirewallUnexpectedGatewayRoutesViolation": NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
-        "NetworkFirewallMissingExpectedRoutesViolation": NetworkFirewallMissingExpectedRoutesViolationTypeDef,
+        "NetworkFirewallInternetTrafficNotInspectedViolation": (
+            NetworkFirewallInternetTrafficNotInspectedViolationTypeDef
+        ),
+        "NetworkFirewallInvalidRouteConfigurationViolation": (
+            NetworkFirewallInvalidRouteConfigurationViolationTypeDef
+        ),
+        "NetworkFirewallBlackHoleRouteDetectedViolation": (
+            NetworkFirewallBlackHoleRouteDetectedViolationTypeDef
+        ),
+        "NetworkFirewallUnexpectedFirewallRoutesViolation": (
+            NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef
+        ),
+        "NetworkFirewallUnexpectedGatewayRoutesViolation": (
+            NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef
+        ),
+        "NetworkFirewallMissingExpectedRoutesViolation": (
+            NetworkFirewallMissingExpectedRoutesViolationTypeDef
+        ),
         "DnsRuleGroupPriorityConflictViolation": DnsRuleGroupPriorityConflictViolationTypeDef,
         "DnsDuplicateRuleGroupViolation": DnsDuplicateRuleGroupViolationTypeDef,
         "DnsRuleGroupLimitExceededViolation": DnsRuleGroupLimitExceededViolationTypeDef,
         "PossibleRemediationActions": PossibleRemediationActionsTypeDef,
         "FirewallSubnetIsOutOfScopeViolation": FirewallSubnetIsOutOfScopeViolationTypeDef,
         "RouteHasOutOfScopeEndpointViolation": RouteHasOutOfScopeEndpointViolationTypeDef,
-        "ThirdPartyFirewallMissingFirewallViolation": ThirdPartyFirewallMissingFirewallViolationTypeDef,
+        "ThirdPartyFirewallMissingFirewallViolation": (
+            ThirdPartyFirewallMissingFirewallViolationTypeDef
+        ),
         "ThirdPartyFirewallMissingSubnetViolation": ThirdPartyFirewallMissingSubnetViolationTypeDef,
-        "ThirdPartyFirewallMissingExpectedRouteTableViolation": ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
-        "FirewallSubnetMissingVPCEndpointViolation": FirewallSubnetMissingVPCEndpointViolationTypeDef,
+        "ThirdPartyFirewallMissingExpectedRouteTableViolation": (
+            ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef
+        ),
+        "FirewallSubnetMissingVPCEndpointViolation": (
+            FirewallSubnetMissingVPCEndpointViolationTypeDef
+        ),
     },
     total=False,
 )
 
 _RequiredViolationDetailTypeDef = TypedDict(
     "_RequiredViolationDetailTypeDef",
     {
@@ -1999,10 +2192,10 @@
     pass
 
 
 GetViolationDetailsResponseTypeDef = TypedDict(
     "GetViolationDetailsResponseTypeDef",
     {
         "ViolationDetail": ViolationDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fms-1.26.5/mypy_boto3_fms/type_defs.pyi` & `mypy-boto3-fms-1.27.0/mypy_boto3_fms/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,152 +2,169 @@
 Type annotations for fms service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_fms.type_defs import ActionTargetTypeDef
+    from mypy_boto3_fms.type_defs import AccountScopeTypeDef
 
-    data: ActionTargetTypeDef = {...}
+    data: AccountScopeTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
+    CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
     FailedItemReasonType,
     FirewallDeploymentModelType,
     MarketplaceSubscriptionOnboardingStatusType,
+    OrganizationStatusType,
     PolicyComplianceStatusTypeType,
     RemediationActionTypeType,
+    ResourceSetStatusType,
     RuleOrderType,
     SecurityServiceTypeType,
     TargetTypeType,
     ThirdPartyFirewallAssociationStatusType,
+    ThirdPartyFirewallType,
     ViolationReasonType,
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
+    "AccountScopeTypeDef",
     "ActionTargetTypeDef",
+    "AdminAccountSummaryTypeDef",
+    "OrganizationalUnitScopeTypeDef",
+    "PolicyTypeScopeTypeDef",
+    "RegionScopeTypeDef",
     "AppTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateThirdPartyFirewallResponseTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
     "FailedItemTypeDef",
     "BatchDisassociateResourceRequestRequestTypeDef",
     "ComplianceViolatorTypeDef",
     "DeleteAppsListRequestRequestTypeDef",
     "DeletePolicyRequestRequestTypeDef",
     "DeleteProtocolsListRequestRequestTypeDef",
     "DeleteResourceSetRequestRequestTypeDef",
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
+    "DisassociateThirdPartyFirewallResponseTypeDef",
     "DiscoveredResourceTypeDef",
     "DnsDuplicateRuleGroupViolationTypeDef",
     "DnsRuleGroupLimitExceededViolationTypeDef",
     "DnsRuleGroupPriorityConflictViolationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EvaluationResultTypeDef",
     "ExpectedRouteTypeDef",
     "FMSPolicyUpdateFirewallCreationConfigActionTypeDef",
     "FirewallSubnetIsOutOfScopeViolationTypeDef",
     "FirewallSubnetMissingVPCEndpointViolationTypeDef",
+    "GetAdminAccountResponseTypeDef",
+    "GetAdminScopeRequestRequestTypeDef",
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
+    "GetNotificationChannelResponseTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetProtectionStatusRequestRequestTypeDef",
+    "GetProtectionStatusResponseTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
     "ProtocolsListDataTypeDef",
     "GetResourceSetRequestRequestTypeDef",
     "ResourceSetTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
+    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
+    "ListAdminAccountsForOrganizationRequestRequestTypeDef",
+    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
+    "ListAdminsManagingAccountRequestRequestTypeDef",
+    "ListAdminsManagingAccountResponseTypeDef",
+    "ListAppsListsRequestListAppsListsPaginateTypeDef",
     "ListAppsListsRequestRequestTypeDef",
+    "ListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     "ListComplianceStatusRequestRequestTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
+    "ListMemberAccountsResponseTypeDef",
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
     "PolicySummaryTypeDef",
+    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
     "ListProtocolsListsRequestRequestTypeDef",
     "ProtocolsListDataSummaryTypeDef",
     "ListResourceSetResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ResourceSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
+    "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     "RouteTypeDef",
     "NetworkFirewallMissingExpectedRTViolationTypeDef",
     "NetworkFirewallMissingFirewallViolationTypeDef",
     "NetworkFirewallMissingSubnetViolationTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupTypeDef",
     "NetworkFirewallPolicyTypeDef",
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
+    "PaginatorConfigTypeDef",
     "ThirdPartyFirewallPolicyTypeDef",
     "ResourceTagTypeDef",
     "PutNotificationChannelRequestRequestTypeDef",
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     "ThirdPartyFirewallMissingFirewallViolationTypeDef",
     "ThirdPartyFirewallMissingSubnetViolationTypeDef",
+    "ResponseMetadataTypeDef",
     "SecurityGroupRuleDescriptionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
     "EC2CreateRouteActionTypeDef",
     "EC2CreateRouteTableActionTypeDef",
     "EC2DeleteRouteActionTypeDef",
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
+    "ListAdminAccountsForOrganizationResponseTypeDef",
+    "AdminScopeTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
-    "AssociateThirdPartyFirewallResponseTypeDef",
-    "DisassociateThirdPartyFirewallResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAdminAccountResponseTypeDef",
-    "GetNotificationChannelResponseTypeDef",
-    "GetProtectionStatusResponseTypeDef",
-    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
-    "ListMemberAccountsResponseTypeDef",
     "AwsEc2InstanceViolationTypeDef",
     "BatchAssociateResourceResponseTypeDef",
     "BatchDisassociateResourceResponseTypeDef",
     "PolicyComplianceDetailTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "PolicyComplianceStatusTypeDef",
     "NetworkFirewallMissingExpectedRoutesViolationTypeDef",
     "GetProtocolsListResponseTypeDef",
     "PutProtocolsListResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "PutResourceSetResponseTypeDef",
-    "ListAppsListsRequestListAppsListsPaginateTypeDef",
-    "ListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
-    "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListProtocolsListsResponseTypeDef",
     "ListResourceSetResourcesResponseTypeDef",
     "ListResourceSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutProtocolsListRequestRequestTypeDef",
     "PutResourceSetRequestRequestTypeDef",
@@ -159,14 +176,16 @@
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
     "PolicyOptionTypeDef",
     "SecurityGroupRemediationActionTypeDef",
     "RemediationActionTypeDef",
+    "GetAdminScopeResponseTypeDef",
+    "PutAdminAccountRequestRequestTypeDef",
     "ListAppsListsResponseTypeDef",
     "GetAppsListResponseTypeDef",
     "PutAppsListRequestRequestTypeDef",
     "PutAppsListResponseTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
@@ -181,23 +200,71 @@
     "PutPolicyResponseTypeDef",
     "PossibleRemediationActionsTypeDef",
     "ResourceViolationTypeDef",
     "ViolationDetailTypeDef",
     "GetViolationDetailsResponseTypeDef",
 )
 
+AccountScopeTypeDef = TypedDict(
+    "AccountScopeTypeDef",
+    {
+        "Accounts": List[str],
+        "AllAccountsEnabled": bool,
+        "ExcludeSpecifiedAccounts": bool,
+    },
+    total=False,
+)
+
 ActionTargetTypeDef = TypedDict(
     "ActionTargetTypeDef",
     {
         "ResourceId": str,
         "Description": str,
     },
     total=False,
 )
 
+AdminAccountSummaryTypeDef = TypedDict(
+    "AdminAccountSummaryTypeDef",
+    {
+        "AdminAccount": str,
+        "DefaultAdmin": bool,
+        "Status": OrganizationStatusType,
+    },
+    total=False,
+)
+
+OrganizationalUnitScopeTypeDef = TypedDict(
+    "OrganizationalUnitScopeTypeDef",
+    {
+        "OrganizationalUnits": List[str],
+        "AllOrganizationalUnitsEnabled": bool,
+        "ExcludeSpecifiedOrganizationalUnits": bool,
+    },
+    total=False,
+)
+
+PolicyTypeScopeTypeDef = TypedDict(
+    "PolicyTypeScopeTypeDef",
+    {
+        "PolicyTypes": List[SecurityServiceTypeType],
+        "AllPolicyTypesEnabled": bool,
+    },
+    total=False,
+)
+
+RegionScopeTypeDef = TypedDict(
+    "RegionScopeTypeDef",
+    {
+        "Regions": List[str],
+        "AllRegionsEnabled": bool,
+    },
+    total=False,
+)
+
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
@@ -209,26 +276,23 @@
         "AdminAccount": str,
     },
 )
 
 AssociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
+    "AssociateThirdPartyFirewallResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AwsEc2NetworkInterfaceViolationTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceViolationTypeDef",
     {
         "ViolationTarget": str,
@@ -321,15 +385,23 @@
         "Identifier": str,
     },
 )
 
 DisassociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
+    },
+)
+
+DisassociateThirdPartyFirewallResponseTypeDef = TypedDict(
+    "DisassociateThirdPartyFirewallResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DiscoveredResourceTypeDef = TypedDict(
     "DiscoveredResourceTypeDef",
     {
         "URI": str,
@@ -367,14 +439,21 @@
         "ConflictingPriority": int,
         "ConflictingPolicyId": str,
         "UnavailablePriorities": List[int],
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
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "ComplianceStatus": PolicyComplianceStatusTypeType,
         "ViolatorCount": int,
         "EvaluationLimitExceeded": bool,
     },
@@ -422,14 +501,30 @@
         "VpcId": str,
         "SubnetAvailabilityZone": str,
         "SubnetAvailabilityZoneId": str,
     },
     total=False,
 )
 
+GetAdminAccountResponseTypeDef = TypedDict(
+    "GetAdminAccountResponseTypeDef",
+    {
+        "AdminAccount": str,
+        "RoleStatus": AccountRoleStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetAdminScopeRequestRequestTypeDef = TypedDict(
+    "GetAdminScopeRequestRequestTypeDef",
+    {
+        "AdminAccount": str,
+    },
+)
+
 _RequiredGetAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetAppsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetAppsListRequestRequestTypeDef = TypedDict(
@@ -449,14 +544,23 @@
     "GetComplianceDetailRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
     },
 )
 
+GetNotificationChannelResponseTypeDef = TypedDict(
+    "GetNotificationChannelResponseTypeDef",
+    {
+        "SnsTopicArn": str,
+        "SnsRoleName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 
@@ -480,14 +584,25 @@
 
 class GetProtectionStatusRequestRequestTypeDef(
     _RequiredGetProtectionStatusRequestRequestTypeDef,
     _OptionalGetProtectionStatusRequestRequestTypeDef,
 ):
     pass
 
+GetProtectionStatusResponseTypeDef = TypedDict(
+    "GetProtectionStatusResponseTypeDef",
+    {
+        "AdminAccountId": str,
+        "ServiceType": SecurityServiceTypeType,
+        "Data": str,
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetProtocolsListRequestRequestTypeDef = TypedDict(
@@ -544,44 +659,96 @@
 _OptionalResourceSetTypeDef = TypedDict(
     "_OptionalResourceSetTypeDef",
     {
         "Id": str,
         "Description": str,
         "UpdateToken": str,
         "LastUpdateTime": datetime,
+        "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
 class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
     pass
 
 GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
+    },
+)
+
+GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
+    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetViolationDetailsRequestRequestTypeDef = TypedDict(
     "GetViolationDetailsRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
         "ResourceId": str,
         "ResourceType": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListAdminAccountsForOrganizationRequestRequestTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef = TypedDict(
+    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListAdminsManagingAccountRequestRequestTypeDef = TypedDict(
+    "ListAdminsManagingAccountRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListAdminsManagingAccountResponseTypeDef = TypedDict(
+    "ListAdminsManagingAccountResponseTypeDef",
+    {
+        "AdminAccounts": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAppsListsRequestListAppsListsPaginateTypeDef = TypedDict(
+    "ListAppsListsRequestListAppsListsPaginateTypeDef",
+    {
+        "DefaultLists": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 _RequiredListAppsListsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppsListsRequestRequestTypeDef",
     {
@@ -598,14 +765,34 @@
 )
 
 class ListAppsListsRequestRequestTypeDef(
     _RequiredListAppsListsRequestRequestTypeDef, _OptionalListAppsListsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
+    "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    {
+        "PolicyId": str,
+    },
+)
+_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
+    "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
+    _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+    _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+):
+    pass
+
 _RequiredListComplianceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListComplianceStatusRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalListComplianceStatusRequestRequestTypeDef = TypedDict(
@@ -641,23 +828,48 @@
 
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
+ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListMemberAccountsResponseTypeDef = TypedDict(
+    "ListMemberAccountsResponseTypeDef",
+    {
+        "MemberAccounts": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPoliciesRequestRequestTypeDef = TypedDict(
     "ListPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -669,14 +881,24 @@
         "PolicyArn": str,
         "PolicyId": str,
         "PolicyName": str,
         "ResourceType": str,
         "SecurityServiceType": SecurityServiceTypeType,
         "RemediationEnabled": bool,
         "DeleteUnusedFMManagedResources": bool,
+        "PolicyStatus": CustomerPolicyStatusType,
+    },
+    total=False,
+)
+
+ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = TypedDict(
+    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
+    {
+        "DefaultLists": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 _RequiredListProtocolsListsRequestRequestTypeDef = TypedDict(
     "_RequiredListProtocolsListsRequestRequestTypeDef",
     {
@@ -759,14 +981,15 @@
 ResourceSetSummaryTypeDef = TypedDict(
     "ResourceSetSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "LastUpdateTime": datetime,
+        "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
@@ -778,18 +1001,38 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
+    {
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
+    },
+)
+_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
+    _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+    _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+):
+    pass
+
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
         "MaxResults": int,
     },
 )
 _OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
@@ -887,14 +1130,24 @@
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
     {
         "Action": Literal["DROP_TO_ALERT"],
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
 ThirdPartyFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallPolicyTypeDef",
     {
         "FirewallDeploymentModel": FirewallDeploymentModelType,
     },
     total=False,
 )
@@ -954,14 +1207,25 @@
         "VPC": str,
         "AvailabilityZone": str,
         "TargetViolationReason": str,
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
 SecurityGroupRuleDescriptionTypeDef = TypedDict(
     "SecurityGroupRuleDescriptionTypeDef",
     {
         "IPV4Range": str,
         "IPV6Range": str,
         "PrefixListId": str,
         "Protocol": str,
@@ -1125,14 +1389,34 @@
 
 class EC2ReplaceRouteTableAssociationActionTypeDef(
     _RequiredEC2ReplaceRouteTableAssociationActionTypeDef,
     _OptionalEC2ReplaceRouteTableAssociationActionTypeDef,
 ):
     pass
 
+ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AdminScopeTypeDef = TypedDict(
+    "AdminScopeTypeDef",
+    {
+        "AccountScope": AccountScopeTypeDef,
+        "OrganizationalUnitScope": OrganizationalUnitScopeTypeDef,
+        "RegionScope": RegionScopeTypeDef,
+        "PolicyTypeScope": PolicyTypeScopeTypeDef,
+    },
+    total=False,
+)
+
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "AppsList": List[AppTypeDef],
@@ -1158,108 +1442,38 @@
     },
     total=False,
 )
 
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
-AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
-    "AssociateThirdPartyFirewallResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateThirdPartyFirewallResponseTypeDef = TypedDict(
-    "DisassociateThirdPartyFirewallResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
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
-GetAdminAccountResponseTypeDef = TypedDict(
-    "GetAdminAccountResponseTypeDef",
-    {
-        "AdminAccount": str,
-        "RoleStatus": AccountRoleStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetNotificationChannelResponseTypeDef = TypedDict(
-    "GetNotificationChannelResponseTypeDef",
-    {
-        "SnsTopicArn": str,
-        "SnsRoleName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProtectionStatusResponseTypeDef = TypedDict(
-    "GetProtectionStatusResponseTypeDef",
-    {
-        "AdminAccountId": str,
-        "ServiceType": SecurityServiceTypeType,
-        "Data": str,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
-    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListMemberAccountsResponseTypeDef = TypedDict(
-    "ListMemberAccountsResponseTypeDef",
-    {
-        "MemberAccounts": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AwsEc2InstanceViolationTypeDef = TypedDict(
     "AwsEc2InstanceViolationTypeDef",
     {
         "ViolationTarget": str,
         "AwsEc2NetworkInterfaceViolations": List[AwsEc2NetworkInterfaceViolationTypeDef],
     },
     total=False,
 )
 
 BatchAssociateResourceResponseTypeDef = TypedDict(
     "BatchAssociateResourceResponseTypeDef",
     {
         "ResourceSetIdentifier": str,
         "FailedItems": List[FailedItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisassociateResourceResponseTypeDef = TypedDict(
     "BatchDisassociateResourceResponseTypeDef",
     {
         "ResourceSetIdentifier": str,
         "FailedItems": List[FailedItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PolicyComplianceDetailTypeDef = TypedDict(
     "PolicyComplianceDetailTypeDef",
     {
         "PolicyOwner": str,
@@ -1274,15 +1488,15 @@
 )
 
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "Items": List[DiscoveredResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PolicyComplianceStatusTypeDef = TypedDict(
     "PolicyComplianceStatusTypeDef",
     {
         "PolicyOwner": str,
@@ -1307,160 +1521,86 @@
 )
 
 GetProtocolsListResponseTypeDef = TypedDict(
     "GetProtocolsListResponseTypeDef",
     {
         "ProtocolsList": ProtocolsListDataTypeDef,
         "ProtocolsListArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutProtocolsListResponseTypeDef = TypedDict(
     "PutProtocolsListResponseTypeDef",
     {
         "ProtocolsList": ProtocolsListDataTypeDef,
         "ProtocolsListArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
         "ResourceSet": ResourceSetTypeDef,
         "ResourceSetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutResourceSetResponseTypeDef = TypedDict(
     "PutResourceSetResponseTypeDef",
     {
         "ResourceSet": ResourceSetTypeDef,
         "ResourceSetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppsListsRequestListAppsListsPaginateTypeDef = TypedDict(
-    "ListAppsListsRequestListAppsListsPaginateTypeDef",
-    {
-        "DefaultLists": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
-    "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    {
-        "PolicyId": str,
-    },
-)
-_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
-    "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
-    _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-    _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-):
-    pass
-
-ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = TypedDict(
-    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
-    {
-        "DefaultLists": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
-    {
-        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
-    },
-)
-_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
-class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
-    _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
-    _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
-):
-    pass
-
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "PolicyList": List[PolicySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProtocolsListsResponseTypeDef = TypedDict(
     "ListProtocolsListsResponseTypeDef",
     {
         "ProtocolsLists": List[ProtocolsListDataSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceSetResourcesResponseTypeDef = TypedDict(
     "ListResourceSetResourcesResponseTypeDef",
     {
         "Items": List[ResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "ResourceSets": List[ResourceSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutProtocolsListRequestRequestTypeDef",
     {
         "ProtocolsList": ProtocolsListDataTypeDef,
@@ -1507,15 +1647,15 @@
 )
 
 ListThirdPartyFirewallFirewallPoliciesResponseTypeDef = TypedDict(
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     {
         "ThirdPartyFirewallFirewallPolicies": List[ThirdPartyFirewallFirewallPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkFirewallBlackHoleRouteDetectedViolationTypeDef = TypedDict(
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     {
         "ViolationTarget": str,
@@ -1651,34 +1791,64 @@
         "EC2CreateRouteAction": EC2CreateRouteActionTypeDef,
         "EC2ReplaceRouteAction": EC2ReplaceRouteActionTypeDef,
         "EC2DeleteRouteAction": EC2DeleteRouteActionTypeDef,
         "EC2CopyRouteTableAction": EC2CopyRouteTableActionTypeDef,
         "EC2ReplaceRouteTableAssociationAction": EC2ReplaceRouteTableAssociationActionTypeDef,
         "EC2AssociateRouteTableAction": EC2AssociateRouteTableActionTypeDef,
         "EC2CreateRouteTableAction": EC2CreateRouteTableActionTypeDef,
-        "FMSPolicyUpdateFirewallCreationConfigAction": FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
+        "FMSPolicyUpdateFirewallCreationConfigAction": (
+            FMSPolicyUpdateFirewallCreationConfigActionTypeDef
+        ),
     },
     total=False,
 )
 
+GetAdminScopeResponseTypeDef = TypedDict(
+    "GetAdminScopeResponseTypeDef",
+    {
+        "AdminScope": AdminScopeTypeDef,
+        "Status": OrganizationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredPutAdminAccountRequestRequestTypeDef = TypedDict(
+    "_RequiredPutAdminAccountRequestRequestTypeDef",
+    {
+        "AdminAccount": str,
+    },
+)
+_OptionalPutAdminAccountRequestRequestTypeDef = TypedDict(
+    "_OptionalPutAdminAccountRequestRequestTypeDef",
+    {
+        "AdminScope": AdminScopeTypeDef,
+    },
+    total=False,
+)
+
+class PutAdminAccountRequestRequestTypeDef(
+    _RequiredPutAdminAccountRequestRequestTypeDef, _OptionalPutAdminAccountRequestRequestTypeDef
+):
+    pass
+
 ListAppsListsResponseTypeDef = TypedDict(
     "ListAppsListsResponseTypeDef",
     {
         "AppsLists": List[AppsListDataSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppsListResponseTypeDef = TypedDict(
     "GetAppsListResponseTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
         "AppsListArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
@@ -1698,32 +1868,32 @@
     pass
 
 PutAppsListResponseTypeDef = TypedDict(
     "PutAppsListResponseTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
         "AppsListArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListComplianceStatusResponseTypeDef = TypedDict(
     "ListComplianceStatusResponseTypeDef",
     {
         "PolicyComplianceStatusList": List[PolicyComplianceStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkFirewallPolicyDescriptionTypeDef = TypedDict(
     "NetworkFirewallPolicyDescriptionTypeDef",
     {
         "StatelessRuleGroups": List[StatelessRuleGroupTypeDef],
@@ -1805,14 +1975,15 @@
         "ResourceTypeList": List[str],
         "ResourceTags": List[ResourceTagTypeDef],
         "DeleteUnusedFMManagedResources": bool,
         "IncludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
         "ExcludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
         "ResourceSetIds": List[str],
         "PolicyDescription": str,
+        "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
 class PolicyTypeDef(_RequiredPolicyTypeDef, _OptionalPolicyTypeDef):
     pass
 
@@ -1837,15 +2008,15 @@
     pass
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "PolicyArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
@@ -1865,15 +2036,15 @@
     pass
 
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "PolicyArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PossibleRemediationActionsTypeDef = TypedDict(
     "PossibleRemediationActionsTypeDef",
     {
         "Description": str,
@@ -1886,32 +2057,52 @@
     "ResourceViolationTypeDef",
     {
         "AwsVPCSecurityGroupViolation": AwsVPCSecurityGroupViolationTypeDef,
         "AwsEc2NetworkInterfaceViolation": AwsEc2NetworkInterfaceViolationTypeDef,
         "AwsEc2InstanceViolation": AwsEc2InstanceViolationTypeDef,
         "NetworkFirewallMissingFirewallViolation": NetworkFirewallMissingFirewallViolationTypeDef,
         "NetworkFirewallMissingSubnetViolation": NetworkFirewallMissingSubnetViolationTypeDef,
-        "NetworkFirewallMissingExpectedRTViolation": NetworkFirewallMissingExpectedRTViolationTypeDef,
+        "NetworkFirewallMissingExpectedRTViolation": (
+            NetworkFirewallMissingExpectedRTViolationTypeDef
+        ),
         "NetworkFirewallPolicyModifiedViolation": NetworkFirewallPolicyModifiedViolationTypeDef,
-        "NetworkFirewallInternetTrafficNotInspectedViolation": NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
-        "NetworkFirewallInvalidRouteConfigurationViolation": NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
-        "NetworkFirewallBlackHoleRouteDetectedViolation": NetworkFirewallBlackHoleRouteDetectedViolationTypeDef,
-        "NetworkFirewallUnexpectedFirewallRoutesViolation": NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
-        "NetworkFirewallUnexpectedGatewayRoutesViolation": NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
-        "NetworkFirewallMissingExpectedRoutesViolation": NetworkFirewallMissingExpectedRoutesViolationTypeDef,
+        "NetworkFirewallInternetTrafficNotInspectedViolation": (
+            NetworkFirewallInternetTrafficNotInspectedViolationTypeDef
+        ),
+        "NetworkFirewallInvalidRouteConfigurationViolation": (
+            NetworkFirewallInvalidRouteConfigurationViolationTypeDef
+        ),
+        "NetworkFirewallBlackHoleRouteDetectedViolation": (
+            NetworkFirewallBlackHoleRouteDetectedViolationTypeDef
+        ),
+        "NetworkFirewallUnexpectedFirewallRoutesViolation": (
+            NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef
+        ),
+        "NetworkFirewallUnexpectedGatewayRoutesViolation": (
+            NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef
+        ),
+        "NetworkFirewallMissingExpectedRoutesViolation": (
+            NetworkFirewallMissingExpectedRoutesViolationTypeDef
+        ),
         "DnsRuleGroupPriorityConflictViolation": DnsRuleGroupPriorityConflictViolationTypeDef,
         "DnsDuplicateRuleGroupViolation": DnsDuplicateRuleGroupViolationTypeDef,
         "DnsRuleGroupLimitExceededViolation": DnsRuleGroupLimitExceededViolationTypeDef,
         "PossibleRemediationActions": PossibleRemediationActionsTypeDef,
         "FirewallSubnetIsOutOfScopeViolation": FirewallSubnetIsOutOfScopeViolationTypeDef,
         "RouteHasOutOfScopeEndpointViolation": RouteHasOutOfScopeEndpointViolationTypeDef,
-        "ThirdPartyFirewallMissingFirewallViolation": ThirdPartyFirewallMissingFirewallViolationTypeDef,
+        "ThirdPartyFirewallMissingFirewallViolation": (
+            ThirdPartyFirewallMissingFirewallViolationTypeDef
+        ),
         "ThirdPartyFirewallMissingSubnetViolation": ThirdPartyFirewallMissingSubnetViolationTypeDef,
-        "ThirdPartyFirewallMissingExpectedRouteTableViolation": ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
-        "FirewallSubnetMissingVPCEndpointViolation": FirewallSubnetMissingVPCEndpointViolationTypeDef,
+        "ThirdPartyFirewallMissingExpectedRouteTableViolation": (
+            ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef
+        ),
+        "FirewallSubnetMissingVPCEndpointViolation": (
+            FirewallSubnetMissingVPCEndpointViolationTypeDef
+        ),
     },
     total=False,
 )
 
 _RequiredViolationDetailTypeDef = TypedDict(
     "_RequiredViolationDetailTypeDef",
     {
@@ -1934,10 +2125,10 @@
 class ViolationDetailTypeDef(_RequiredViolationDetailTypeDef, _OptionalViolationDetailTypeDef):
     pass
 
 GetViolationDetailsResponseTypeDef = TypedDict(
     "GetViolationDetailsResponseTypeDef",
     {
         "ViolationDetail": ViolationDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/PKG-INFO` & `mypy-boto3-fms-1.27.0/mypy_boto3_fms.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.26.5
-Summary: Type annotations for boto3.FMS 1.26.5 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.FMS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
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
 
 <a id="mypy-boto3-fms"></a>
 
 # mypy-boto3-fms
 
 [![PyPI - mypy-boto3-fms](https://img.shields.io/pypi/v/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fms?color=blue)](https://pypistats.org/packages/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.26.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,26 +278,34 @@
 `mypy_boto3_fms.paginator` module contains type annotations for all paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_fms import FMSClient
 from mypy_boto3_fms.paginator import (
+    ListAdminAccountsForOrganizationPaginator,
+    ListAdminsManagingAccountPaginator,
     ListAppsListsPaginator,
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 
 client: FMSClient = Session().client("fms")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+list_admin_accounts_for_organization_paginator: ListAdminAccountsForOrganizationPaginator = (
+    client.get_paginator("list_admin_accounts_for_organization")
+)
+list_admins_managing_account_paginator: ListAdminsManagingAccountPaginator = client.get_paginator(
+    "list_admins_managing_account"
+)
 list_apps_lists_paginator: ListAppsListsPaginator = client.get_paginator("list_apps_lists")
 list_compliance_status_paginator: ListComplianceStatusPaginator = client.get_paginator(
     "list_compliance_status"
 )
 list_member_accounts_paginator: ListMemberAccountsPaginator = client.get_paginator(
     "list_member_accounts"
 )
@@ -316,28 +325,33 @@
 `mypy_boto3_fms.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_fms.literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
+    CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
     FailedItemReasonType,
     FirewallDeploymentModelType,
+    ListAdminAccountsForOrganizationPaginatorName,
+    ListAdminsManagingAccountPaginatorName,
     ListAppsListsPaginatorName,
     ListComplianceStatusPaginatorName,
     ListMemberAccountsPaginatorName,
     ListPoliciesPaginatorName,
     ListProtocolsListsPaginatorName,
     ListThirdPartyFirewallFirewallPoliciesPaginatorName,
     MarketplaceSubscriptionOnboardingStatusType,
     NetworkFirewallOverrideActionType,
+    OrganizationStatusType,
     PolicyComplianceStatusTypeType,
     RemediationActionTypeType,
+    ResourceSetStatusType,
     RuleOrderType,
     SecurityServiceTypeType,
     TargetTypeType,
     ThirdPartyFirewallAssociationStatusType,
     ThirdPartyFirewallType,
     ViolationReasonType,
     FMSServiceName,
@@ -357,116 +371,129 @@
 ### Typed dictionaries
 
 `mypy_boto3_fms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_fms.type_defs import (
+    AccountScopeTypeDef,
     ActionTargetTypeDef,
+    AdminAccountSummaryTypeDef,
+    OrganizationalUnitScopeTypeDef,
+    PolicyTypeScopeTypeDef,
+    RegionScopeTypeDef,
     AppTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateThirdPartyFirewallResponseTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
     FailedItemTypeDef,
     BatchDisassociateResourceRequestRequestTypeDef,
     ComplianceViolatorTypeDef,
     DeleteAppsListRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     DeleteProtocolsListRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
     DisassociateThirdPartyFirewallRequestRequestTypeDef,
+    DisassociateThirdPartyFirewallResponseTypeDef,
     DiscoveredResourceTypeDef,
     DnsDuplicateRuleGroupViolationTypeDef,
     DnsRuleGroupLimitExceededViolationTypeDef,
     DnsRuleGroupPriorityConflictViolationTypeDef,
+    EmptyResponseMetadataTypeDef,
     EvaluationResultTypeDef,
     ExpectedRouteTypeDef,
     FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
     FirewallSubnetIsOutOfScopeViolationTypeDef,
     FirewallSubnetMissingVPCEndpointViolationTypeDef,
+    GetAdminAccountResponseTypeDef,
+    GetAdminScopeRequestRequestTypeDef,
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
+    GetNotificationChannelResponseTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetProtectionStatusRequestRequestTypeDef,
+    GetProtectionStatusResponseTypeDef,
     GetProtocolsListRequestRequestTypeDef,
     ProtocolsListDataTypeDef,
     GetResourceSetRequestRequestTypeDef,
     ResourceSetTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
+    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    ListAdminAccountsForOrganizationRequestRequestTypeDef,
+    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
+    ListAdminsManagingAccountRequestRequestTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
+    ListAppsListsRequestListAppsListsPaginateTypeDef,
     ListAppsListsRequestRequestTypeDef,
+    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     ListComplianceStatusRequestRequestTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
+    ListMemberAccountsResponseTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     PolicySummaryTypeDef,
+    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
     ListProtocolsListsRequestRequestTypeDef,
     ProtocolsListDataSummaryTypeDef,
     ListResourceSetResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ResourceSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
+    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     ThirdPartyFirewallFirewallPolicyTypeDef,
     RouteTypeDef,
     NetworkFirewallMissingExpectedRTViolationTypeDef,
     NetworkFirewallMissingFirewallViolationTypeDef,
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
+    PaginatorConfigTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
     ResourceTagTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
+    ResponseMetadataTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
     EC2CreateRouteActionTypeDef,
     EC2CreateRouteTableActionTypeDef,
     EC2DeleteRouteActionTypeDef,
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    AdminScopeTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
-    AssociateThirdPartyFirewallResponseTypeDef,
-    DisassociateThirdPartyFirewallResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAdminAccountResponseTypeDef,
-    GetNotificationChannelResponseTypeDef,
-    GetProtectionStatusResponseTypeDef,
-    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
-    ListMemberAccountsResponseTypeDef,
     AwsEc2InstanceViolationTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     PolicyComplianceDetailTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     PolicyComplianceStatusTypeDef,
     NetworkFirewallMissingExpectedRoutesViolationTypeDef,
     GetProtocolsListResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     GetResourceSetResponseTypeDef,
     PutResourceSetResponseTypeDef,
-    ListAppsListsRequestListAppsListsPaginateTypeDef,
-    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
-    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
-    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutProtocolsListRequestRequestTypeDef,
     PutResourceSetRequestRequestTypeDef,
@@ -478,14 +505,16 @@
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
     PolicyOptionTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
+    GetAdminScopeResponseTypeDef,
+    PutAdminAccountRequestRequestTypeDef,
     ListAppsListsResponseTypeDef,
     GetAppsListResponseTypeDef,
     PutAppsListRequestRequestTypeDef,
     PutAppsListResponseTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
@@ -501,53 +530,53 @@
     PossibleRemediationActionsTypeDef,
     ResourceViolationTypeDef,
     ViolationDetailTypeDef,
     GetViolationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> ActionTargetTypeDef:
+def get_structure() -> AccountScopeTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/SOURCES.txt` & `mypy-boto3-fms-1.27.0/mypy_boto3_fms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.26.5/setup.py` & `mypy-boto3-fms-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-fms.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fms",
-    version="1.26.5",
+    version="1.27.0",
     packages=["mypy_boto3_fms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FMS 1.26.5 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.FMS 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 fms type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_fms": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_fms": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/",
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


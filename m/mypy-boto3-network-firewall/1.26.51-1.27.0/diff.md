# Comparing `tmp/mypy-boto3-network-firewall-1.26.51.tar.gz` & `tmp/mypy-boto3-network-firewall-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-network-firewall-1.26.51.tar", last modified: Tue Jan 17 20:24:22 2023, max compression
+gzip compressed data, was "mypy-boto3-network-firewall-1.27.0.tar", last modified: Mon Jul  3 19:51:10 2023, max compression
```

## Comparing `mypy-boto3-network-firewall-1.26.51.tar` & `mypy-boto3-network-firewall-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:22.383515 mypy-boto3-network-firewall-1.26.51/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18260 2023-01-17 20:24:22.383515 mypy-boto3-network-firewall-1.26.51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:22.383515 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27559 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39734 2023-01-17 20:24:13.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39684 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:22.383515 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18260 2023-01-17 20:24:22.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-01-17 20:24:22.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 20:24:22.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 20:24:22.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-17 20:24:22.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-17 20:24:22.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 20:24:22.383515 mypy-boto3-network-firewall-1.26.51/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.819728 mypy-boto3-network-firewall-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-07-03 19:51:10.819728 mypy-boto3-network-firewall-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17929 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.819728 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32089 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32041 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47527 2023-07-03 19:42:43.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47471 2023-07-03 19:42:43.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.819728 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-07-03 19:51:10.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-03 19:51:10.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:10.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 19:51:10.000000 mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:10.819728 mypy-boto3-network-firewall-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-03 19:42:42.000000 mypy-boto3-network-firewall-1.27.0/setup.py
```

### Comparing `mypy-boto3-network-firewall-1.26.51/LICENSE` & `mypy-boto3-network-firewall-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-network-firewall-1.26.51/PKG-INFO` & `mypy-boto3-network-firewall-1.27.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-network-firewall
-Version: 1.26.51
-Summary: Type annotations for boto3.NetworkFirewall 1.26.51 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.NetworkFirewall 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-network-firewall"></a>
 
 # mypy-boto3-network-firewall
 
 [![PyPI - mypy-boto3-network-firewall](https://img.shields.io/pypi/v/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-network-firewall?color=blue)](https://pypistats.org/packages/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.26.51](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,26 +284,30 @@
 from boto3.session import Session
 
 from mypy_boto3_network_firewall import NetworkFirewallClient
 from mypy_boto3_network_firewall.paginator import (
     ListFirewallPoliciesPaginator,
     ListFirewallsPaginator,
     ListRuleGroupsPaginator,
+    ListTLSInspectionConfigurationsPaginator,
     ListTagsForResourcePaginator,
 )
 
 client: NetworkFirewallClient = Session().client("network-firewall")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_firewall_policies_paginator: ListFirewallPoliciesPaginator = client.get_paginator(
     "list_firewall_policies"
 )
 list_firewalls_paginator: ListFirewallsPaginator = client.get_paginator("list_firewalls")
 list_rule_groups_paginator: ListRuleGroupsPaginator = client.get_paginator("list_rule_groups")
+list_tls_inspection_configurations_paginator: ListTLSInspectionConfigurationsPaginator = (
+    client.get_paginator("list_tls_inspection_configurations")
+)
 list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator(
     "list_tags_for_resource"
 )
 ```
 
 <a id="literals"></a>
 
@@ -319,14 +323,15 @@
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
     IPAddressTypeType,
     ListFirewallPoliciesPaginatorName,
     ListFirewallsPaginatorName,
     ListRuleGroupsPaginatorName,
+    ListTLSInspectionConfigurationsPaginatorName,
     ListTagsForResourcePaginatorName,
     LogDestinationTypeType,
     LogTypeType,
     OverrideActionType,
     PerObjectSyncStatusType,
     ResourceManagedStatusType,
     ResourceManagedTypeType,
@@ -358,66 +363,77 @@
 `mypy_boto3_network_firewall.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_network_firewall.type_defs import (
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateFirewallPolicyResponseTypeDef,
     SubnetMappingTypeDef,
     AttachmentTypeDef,
     IPSetMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     TagTypeDef,
     SourceMetadataTypeDef,
     DeleteFirewallPolicyRequestRequestTypeDef,
     DeleteFirewallRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
+    DeleteTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallRequestRequestTypeDef,
     DescribeLoggingConfigurationRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataRequestRequestTypeDef,
     StatefulRuleOptionsTypeDef,
     DescribeRuleGroupRequestRequestTypeDef,
+    DescribeTLSInspectionConfigurationRequestRequestTypeDef,
     DimensionTypeDef,
     DisassociateSubnetsRequestRequestTypeDef,
     FirewallMetadataTypeDef,
     FirewallPolicyMetadataTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupReferenceTypeDef,
     HeaderTypeDef,
     IPSetReferenceTypeDef,
     IPSetTypeDef,
-    PaginatorConfigTypeDef,
+    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
     ListFirewallPoliciesRequestRequestTypeDef,
+    ListFirewallsRequestListFirewallsPaginateTypeDef,
     ListFirewallsRequestRequestTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupMetadataTypeDef,
+    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
+    ListTLSInspectionConfigurationsRequestRequestTypeDef,
+    TLSInspectionConfigurationMetadataTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     LogDestinationConfigTypeDef,
     PortRangeTypeDef,
     TCPFlagFieldTypeDef,
+    PaginatorConfigTypeDef,
     PerObjectStatusTypeDef,
     PortSetTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RuleOptionTypeDef,
     RulesSourceListTypeDef,
+    ServerCertificateTypeDef,
     StatefulRuleGroupOverrideTypeDef,
+    TlsCertificateDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionRequestRequestTypeDef,
-    UpdateFirewallDescriptionRequestRequestTypeDef,
-    UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
-    UpdateSubnetChangeProtectionRequestRequestTypeDef,
-    AssociateFirewallPolicyResponseTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
+    UpdateFirewallDescriptionRequestRequestTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
+    UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
+    UpdateSubnetChangeProtectionRequestRequestTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
     AssociateSubnetsRequestRequestTypeDef,
     AssociateSubnetsResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     CIDRSummaryTypeDef,
     UpdateFirewallEncryptionConfigurationRequestRequestTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
@@ -428,44 +444,52 @@
     TagResourceRequestRequestTypeDef,
     RuleGroupResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     PublishMetricActionTypeDef,
     ListFirewallsResponseTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ReferenceSetsTypeDef,
-    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
-    ListFirewallsRequestListFirewallsPaginateTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    PolicyVariablesTypeDef,
     ListRuleGroupsResponseTypeDef,
+    ListTLSInspectionConfigurationsResponseTypeDef,
     LoggingConfigurationTypeDef,
+    ServerCertificateScopeTypeDef,
     MatchAttributesTypeDef,
     SyncStateTypeDef,
     RuleVariablesTypeDef,
     StatefulRuleTypeDef,
     StatefulRuleGroupReferenceTypeDef,
+    TLSInspectionConfigurationResponseTypeDef,
     CapacityUsageSummaryTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     DeleteRuleGroupResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    ServerCertificateConfigurationTypeDef,
     RuleDefinitionTypeDef,
+    CreateTLSInspectionConfigurationResponseTypeDef,
+    DeleteTLSInspectionConfigurationResponseTypeDef,
+    UpdateTLSInspectionConfigurationResponseTypeDef,
     FirewallStatusTypeDef,
     CustomActionTypeDef,
+    TLSInspectionConfigurationTypeDef,
     StatelessRuleTypeDef,
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
     FirewallPolicyTypeDef,
+    CreateTLSInspectionConfigurationRequestRequestTypeDef,
+    DescribeTLSInspectionConfigurationResponseTypeDef,
+    UpdateTLSInspectionConfigurationRequestRequestTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
     CreateFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
     RulesSourceTypeDef,
     RuleGroupTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
@@ -481,42 +505,42 @@
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

### Comparing `mypy-boto3-network-firewall-1.26.51/README.md` & `mypy-boto3-network-firewall-1.27.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-network-firewall"></a>
 
 # mypy-boto3-network-firewall
 
 [![PyPI - mypy-boto3-network-firewall](https://img.shields.io/pypi/v/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-network-firewall?color=blue)](https://pypistats.org/packages/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.26.51](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
 
@@ -252,26 +252,30 @@
 from boto3.session import Session
 
 from mypy_boto3_network_firewall import NetworkFirewallClient
 from mypy_boto3_network_firewall.paginator import (
     ListFirewallPoliciesPaginator,
     ListFirewallsPaginator,
     ListRuleGroupsPaginator,
+    ListTLSInspectionConfigurationsPaginator,
     ListTagsForResourcePaginator,
 )
 
 client: NetworkFirewallClient = Session().client("network-firewall")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_firewall_policies_paginator: ListFirewallPoliciesPaginator = client.get_paginator(
     "list_firewall_policies"
 )
 list_firewalls_paginator: ListFirewallsPaginator = client.get_paginator("list_firewalls")
 list_rule_groups_paginator: ListRuleGroupsPaginator = client.get_paginator("list_rule_groups")
+list_tls_inspection_configurations_paginator: ListTLSInspectionConfigurationsPaginator = (
+    client.get_paginator("list_tls_inspection_configurations")
+)
 list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator(
     "list_tags_for_resource"
 )
 ```
 
 <a id="literals"></a>
 
@@ -287,14 +291,15 @@
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
     IPAddressTypeType,
     ListFirewallPoliciesPaginatorName,
     ListFirewallsPaginatorName,
     ListRuleGroupsPaginatorName,
+    ListTLSInspectionConfigurationsPaginatorName,
     ListTagsForResourcePaginatorName,
     LogDestinationTypeType,
     LogTypeType,
     OverrideActionType,
     PerObjectSyncStatusType,
     ResourceManagedStatusType,
     ResourceManagedTypeType,
@@ -326,66 +331,77 @@
 `mypy_boto3_network_firewall.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_network_firewall.type_defs import (
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateFirewallPolicyResponseTypeDef,
     SubnetMappingTypeDef,
     AttachmentTypeDef,
     IPSetMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     TagTypeDef,
     SourceMetadataTypeDef,
     DeleteFirewallPolicyRequestRequestTypeDef,
     DeleteFirewallRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
+    DeleteTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallRequestRequestTypeDef,
     DescribeLoggingConfigurationRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataRequestRequestTypeDef,
     StatefulRuleOptionsTypeDef,
     DescribeRuleGroupRequestRequestTypeDef,
+    DescribeTLSInspectionConfigurationRequestRequestTypeDef,
     DimensionTypeDef,
     DisassociateSubnetsRequestRequestTypeDef,
     FirewallMetadataTypeDef,
     FirewallPolicyMetadataTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupReferenceTypeDef,
     HeaderTypeDef,
     IPSetReferenceTypeDef,
     IPSetTypeDef,
-    PaginatorConfigTypeDef,
+    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
     ListFirewallPoliciesRequestRequestTypeDef,
+    ListFirewallsRequestListFirewallsPaginateTypeDef,
     ListFirewallsRequestRequestTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupMetadataTypeDef,
+    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
+    ListTLSInspectionConfigurationsRequestRequestTypeDef,
+    TLSInspectionConfigurationMetadataTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     LogDestinationConfigTypeDef,
     PortRangeTypeDef,
     TCPFlagFieldTypeDef,
+    PaginatorConfigTypeDef,
     PerObjectStatusTypeDef,
     PortSetTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RuleOptionTypeDef,
     RulesSourceListTypeDef,
+    ServerCertificateTypeDef,
     StatefulRuleGroupOverrideTypeDef,
+    TlsCertificateDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionRequestRequestTypeDef,
-    UpdateFirewallDescriptionRequestRequestTypeDef,
-    UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
-    UpdateSubnetChangeProtectionRequestRequestTypeDef,
-    AssociateFirewallPolicyResponseTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
+    UpdateFirewallDescriptionRequestRequestTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
+    UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
+    UpdateSubnetChangeProtectionRequestRequestTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
     AssociateSubnetsRequestRequestTypeDef,
     AssociateSubnetsResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     CIDRSummaryTypeDef,
     UpdateFirewallEncryptionConfigurationRequestRequestTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
@@ -396,44 +412,52 @@
     TagResourceRequestRequestTypeDef,
     RuleGroupResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     PublishMetricActionTypeDef,
     ListFirewallsResponseTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ReferenceSetsTypeDef,
-    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
-    ListFirewallsRequestListFirewallsPaginateTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    PolicyVariablesTypeDef,
     ListRuleGroupsResponseTypeDef,
+    ListTLSInspectionConfigurationsResponseTypeDef,
     LoggingConfigurationTypeDef,
+    ServerCertificateScopeTypeDef,
     MatchAttributesTypeDef,
     SyncStateTypeDef,
     RuleVariablesTypeDef,
     StatefulRuleTypeDef,
     StatefulRuleGroupReferenceTypeDef,
+    TLSInspectionConfigurationResponseTypeDef,
     CapacityUsageSummaryTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     DeleteRuleGroupResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    ServerCertificateConfigurationTypeDef,
     RuleDefinitionTypeDef,
+    CreateTLSInspectionConfigurationResponseTypeDef,
+    DeleteTLSInspectionConfigurationResponseTypeDef,
+    UpdateTLSInspectionConfigurationResponseTypeDef,
     FirewallStatusTypeDef,
     CustomActionTypeDef,
+    TLSInspectionConfigurationTypeDef,
     StatelessRuleTypeDef,
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
     FirewallPolicyTypeDef,
+    CreateTLSInspectionConfigurationRequestRequestTypeDef,
+    DescribeTLSInspectionConfigurationResponseTypeDef,
+    UpdateTLSInspectionConfigurationRequestRequestTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
     CreateFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
     RulesSourceTypeDef,
     RuleGroupTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
@@ -449,42 +473,42 @@
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

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/__init__.py` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,39 +6,43 @@
     ```python
     from boto3.session import Session
     from mypy_boto3_network_firewall import (
         Client,
         ListFirewallPoliciesPaginator,
         ListFirewallsPaginator,
         ListRuleGroupsPaginator,
+        ListTLSInspectionConfigurationsPaginator,
         ListTagsForResourcePaginator,
         NetworkFirewallClient,
     )
 
     session = Session()
     client: NetworkFirewallClient = session.client("network-firewall")
 
     list_firewall_policies_paginator: ListFirewallPoliciesPaginator = client.get_paginator("list_firewall_policies")
     list_firewalls_paginator: ListFirewallsPaginator = client.get_paginator("list_firewalls")
     list_rule_groups_paginator: ListRuleGroupsPaginator = client.get_paginator("list_rule_groups")
+    list_tls_inspection_configurations_paginator: ListTLSInspectionConfigurationsPaginator = client.get_paginator("list_tls_inspection_configurations")
     list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
 from .client import NetworkFirewallClient
 from .paginator import (
     ListFirewallPoliciesPaginator,
     ListFirewallsPaginator,
     ListRuleGroupsPaginator,
     ListTagsForResourcePaginator,
+    ListTLSInspectionConfigurationsPaginator,
 )
 
 Client = NetworkFirewallClient
 
 
 __all__ = (
     "Client",
     "ListFirewallPoliciesPaginator",
     "ListFirewallsPaginator",
     "ListRuleGroupsPaginator",
+    "ListTLSInspectionConfigurationsPaginator",
     "ListTagsForResourcePaginator",
     "NetworkFirewallClient",
 )
```

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/__init__.pyi` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/__init__.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -6,38 +6,42 @@
     ```python
     from boto3.session import Session
     from mypy_boto3_network_firewall import (
         Client,
         ListFirewallPoliciesPaginator,
         ListFirewallsPaginator,
         ListRuleGroupsPaginator,
+        ListTLSInspectionConfigurationsPaginator,
         ListTagsForResourcePaginator,
         NetworkFirewallClient,
     )
 
     session = Session()
     client: NetworkFirewallClient = session.client("network-firewall")
 
     list_firewall_policies_paginator: ListFirewallPoliciesPaginator = client.get_paginator("list_firewall_policies")
     list_firewalls_paginator: ListFirewallsPaginator = client.get_paginator("list_firewalls")
     list_rule_groups_paginator: ListRuleGroupsPaginator = client.get_paginator("list_rule_groups")
+    list_tls_inspection_configurations_paginator: ListTLSInspectionConfigurationsPaginator = client.get_paginator("list_tls_inspection_configurations")
     list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
 from .client import NetworkFirewallClient
 from .paginator import (
     ListFirewallPoliciesPaginator,
     ListFirewallsPaginator,
     ListRuleGroupsPaginator,
     ListTagsForResourcePaginator,
+    ListTLSInspectionConfigurationsPaginator,
 )
 
 Client = NetworkFirewallClient
 
 __all__ = (
     "Client",
     "ListFirewallPoliciesPaginator",
     "ListFirewallsPaginator",
     "ListRuleGroupsPaginator",
+    "ListTLSInspectionConfigurationsPaginator",
     "ListTagsForResourcePaginator",
     "NetworkFirewallClient",
 )
```

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/__main__.py` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.NetworkFirewall 1.26.51\nVersion:         1.26.51\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.NetworkFirewall 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.51")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/client.py` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/client.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -20,69 +20,73 @@
 
 from .literals import ResourceManagedStatusType, ResourceManagedTypeType, RuleGroupTypeType
 from .paginator import (
     ListFirewallPoliciesPaginator,
     ListFirewallsPaginator,
     ListRuleGroupsPaginator,
     ListTagsForResourcePaginator,
+    ListTLSInspectionConfigurationsPaginator,
 )
 from .type_defs import (
     AssociateFirewallPolicyResponseTypeDef,
     AssociateSubnetsResponseTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     CreateFirewallResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
+    CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DeleteRuleGroupResponseTypeDef,
+    DeleteTLSInspectionConfigurationResponseTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
     DescribeFirewallResponseTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     DescribeRuleGroupResponseTypeDef,
+    DescribeTLSInspectionConfigurationResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     EncryptionConfigurationTypeDef,
     FirewallPolicyTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListTLSInspectionConfigurationsResponseTypeDef,
     LoggingConfigurationTypeDef,
     RuleGroupTypeDef,
     SourceMetadataTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
+    TLSInspectionConfigurationTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
+    UpdateTLSInspectionConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("NetworkFirewallClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InsufficientCapacityException: Type[BotocoreClientError]
     InternalServerError: Type[BotocoreClientError]
     InvalidOperationException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     InvalidResourcePolicyException: Type[BotocoreClientError]
@@ -90,15 +94,14 @@
     LimitExceededException: Type[BotocoreClientError]
     LogDestinationPermissionException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceOwnerCheckException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
-
 class NetworkFirewallClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/)
     """
 
     meta: ClientMeta
@@ -107,61 +110,56 @@
     def exceptions(self) -> Exceptions:
         """
         NetworkFirewallClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#exceptions)
         """
-
     def associate_firewall_policy(
         self,
         *,
         FirewallPolicyArn: str,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> AssociateFirewallPolicyResponseTypeDef:
         """
         Associates a  FirewallPolicy to a  Firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.associate_firewall_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#associate_firewall_policy)
         """
-
     def associate_subnets(
         self,
         *,
         SubnetMappings: Sequence[SubnetMappingTypeDef],
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> AssociateSubnetsResponseTypeDef:
         """
         Associates the specified subnets in the Amazon VPC to the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.associate_subnets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#associate_subnets)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#close)
         """
-
     def create_firewall(
         self,
         *,
         FirewallName: str,
         FirewallPolicyArn: str,
         VpcId: str,
         SubnetMappings: Sequence[SubnetMappingTypeDef],
@@ -175,15 +173,14 @@
         """
         Creates an Network Firewall  Firewall and accompanying  FirewallStatus for a
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_firewall)
         """
-
     def create_firewall_policy(
         self,
         *,
         FirewallPolicyName: str,
         FirewallPolicy: FirewallPolicyTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
@@ -192,15 +189,14 @@
     ) -> CreateFirewallPolicyResponseTypeDef:
         """
         Creates the firewall policy for the firewall according to the specifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_firewall_policy)
         """
-
     def create_rule_group(
         self,
         *,
         RuleGroupName: str,
         Type: RuleGroupTypeType,
         Capacity: int,
         RuleGroup: RuleGroupTypeDef = ...,
@@ -214,163 +210,181 @@
         """
         Creates the specified stateless or stateful rule group, which includes the rules
         for network traffic inspection, a capacity setting, and tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_rule_group)
         """
+    def create_tls_inspection_configuration(
+        self,
+        *,
+        TLSInspectionConfigurationName: str,
+        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
+        Description: str = ...,
+        Tags: Sequence[TagTypeDef] = ...,
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+    ) -> CreateTLSInspectionConfigurationResponseTypeDef:
+        """
+        Creates an Network Firewall TLS inspection configuration.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_tls_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_tls_inspection_configuration)
+        """
     def delete_firewall(
         self, *, FirewallName: str = ..., FirewallArn: str = ...
     ) -> DeleteFirewallResponseTypeDef:
         """
         Deletes the specified  Firewall and its  FirewallStatus.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#delete_firewall)
         """
-
     def delete_firewall_policy(
         self, *, FirewallPolicyName: str = ..., FirewallPolicyArn: str = ...
     ) -> DeleteFirewallPolicyResponseTypeDef:
         """
         Deletes the specified  FirewallPolicy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_firewall_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#delete_firewall_policy)
         """
-
     def delete_resource_policy(self, *, ResourceArn: str) -> Dict[str, Any]:
         """
         Deletes a resource policy that you created in a  PutResourcePolicy request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#delete_resource_policy)
         """
-
     def delete_rule_group(
         self, *, RuleGroupName: str = ..., RuleGroupArn: str = ..., Type: RuleGroupTypeType = ...
     ) -> DeleteRuleGroupResponseTypeDef:
         """
         Deletes the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#delete_rule_group)
         """
+    def delete_tls_inspection_configuration(
+        self, *, TLSInspectionConfigurationArn: str = ..., TLSInspectionConfigurationName: str = ...
+    ) -> DeleteTLSInspectionConfigurationResponseTypeDef:
+        """
+        Deletes the specified  TLSInspectionConfiguration.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_tls_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#delete_tls_inspection_configuration)
+        """
     def describe_firewall(
         self, *, FirewallName: str = ..., FirewallArn: str = ...
     ) -> DescribeFirewallResponseTypeDef:
         """
         Returns the data objects for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_firewall)
         """
-
     def describe_firewall_policy(
         self, *, FirewallPolicyName: str = ..., FirewallPolicyArn: str = ...
     ) -> DescribeFirewallPolicyResponseTypeDef:
         """
         Returns the data objects for the specified firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_firewall_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_firewall_policy)
         """
-
     def describe_logging_configuration(
         self, *, FirewallArn: str = ..., FirewallName: str = ...
     ) -> DescribeLoggingConfigurationResponseTypeDef:
         """
         Returns the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_logging_configuration)
         """
-
     def describe_resource_policy(
         self, *, ResourceArn: str
     ) -> DescribeResourcePolicyResponseTypeDef:
         """
         Retrieves a resource policy that you created in a  PutResourcePolicy request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_resource_policy)
         """
-
     def describe_rule_group(
         self, *, RuleGroupName: str = ..., RuleGroupArn: str = ..., Type: RuleGroupTypeType = ...
     ) -> DescribeRuleGroupResponseTypeDef:
         """
         Returns the data objects for the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_rule_group)
         """
-
     def describe_rule_group_metadata(
         self, *, RuleGroupName: str = ..., RuleGroupArn: str = ..., Type: RuleGroupTypeType = ...
     ) -> DescribeRuleGroupMetadataResponseTypeDef:
         """
         High-level information about a rule group, returned by operations like create
         and describe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_rule_group_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_rule_group_metadata)
         """
+    def describe_tls_inspection_configuration(
+        self, *, TLSInspectionConfigurationArn: str = ..., TLSInspectionConfigurationName: str = ...
+    ) -> DescribeTLSInspectionConfigurationResponseTypeDef:
+        """
+        Returns the data objects for the specified TLS inspection configuration.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_tls_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_tls_inspection_configuration)
+        """
     def disassociate_subnets(
         self,
         *,
         SubnetIds: Sequence[str],
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> DisassociateSubnetsResponseTypeDef:
         """
         Removes the specified subnet associations from the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.disassociate_subnets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#disassociate_subnets)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#generate_presigned_url)
         """
-
     def list_firewall_policies(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListFirewallPoliciesResponseTypeDef:
         """
         Retrieves the metadata for the firewall policies that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_firewall_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#list_firewall_policies)
         """
-
     def list_firewalls(
         self, *, NextToken: str = ..., VpcIds: Sequence[str] = ..., MaxResults: int = ...
     ) -> ListFirewallsResponseTypeDef:
         """
         Retrieves the metadata for the firewalls that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_firewalls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#list_firewalls)
         """
-
     def list_rule_groups(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
@@ -378,95 +392,97 @@
     ) -> ListRuleGroupsResponseTypeDef:
         """
         Retrieves the metadata for the rule groups that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_rule_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#list_rule_groups)
         """
-
     def list_tags_for_resource(
         self, *, ResourceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves the tags associated with the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#list_tags_for_resource)
         """
+    def list_tls_inspection_configurations(
+        self, *, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListTLSInspectionConfigurationsResponseTypeDef:
+        """
+        Retrieves the metadata for the TLS inspection configurations that you have
+        defined.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_tls_inspection_configurations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#list_tls_inspection_configurations)
+        """
     def put_resource_policy(self, *, ResourceArn: str, Policy: str) -> Dict[str, Any]:
         """
         Creates or updates an IAM policy for your rule group or firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#put_resource_policy)
         """
-
     def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds the specified tags to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the tags with the specified keys from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#untag_resource)
         """
-
     def update_firewall_delete_protection(
         self,
         *,
         DeleteProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> UpdateFirewallDeleteProtectionResponseTypeDef:
         """
-        Modifies the flag, `DeleteProtection` , which indicates whether it is possible
-        to delete the firewall.
+        Modifies the flag, `DeleteProtection`, which indicates whether it is possible to
+        delete the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_delete_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_delete_protection)
         """
-
     def update_firewall_description(
         self,
         *,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...,
         Description: str = ...
     ) -> UpdateFirewallDescriptionResponseTypeDef:
         """
         Modifies the description for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_description)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_description)
         """
-
     def update_firewall_encryption_configuration(
         self,
         *,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateFirewallEncryptionConfigurationResponseTypeDef:
         """
         A complex type that contains settings for encryption of your firewall resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_encryption_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_encryption_configuration)
         """
-
     def update_firewall_policy(
         self,
         *,
         UpdateToken: str,
         FirewallPolicy: FirewallPolicyTypeDef,
         FirewallPolicyArn: str = ...,
         FirewallPolicyName: str = ...,
@@ -476,45 +492,42 @@
     ) -> UpdateFirewallPolicyResponseTypeDef:
         """
         Updates the properties of the specified firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_policy)
         """
-
     def update_firewall_policy_change_protection(
         self,
         *,
         FirewallPolicyChangeProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> UpdateFirewallPolicyChangeProtectionResponseTypeDef:
         """
-        Modifies the flag, `ChangeProtection` , which indicates whether it is possible
-        to change the firewall.
+        Modifies the flag, `ChangeProtection`, which indicates whether it is possible to
+        change the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_policy_change_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_policy_change_protection)
         """
-
     def update_logging_configuration(
         self,
         *,
         FirewallArn: str = ...,
         FirewallName: str = ...,
         LoggingConfiguration: LoggingConfigurationTypeDef = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Sets the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_logging_configuration)
         """
-
     def update_rule_group(
         self,
         *,
         UpdateToken: str,
         RuleGroupArn: str = ...,
         RuleGroupName: str = ...,
         RuleGroup: RuleGroupTypeDef = ...,
@@ -527,15 +540,14 @@
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the rule settings for the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_rule_group)
         """
-
     def update_subnet_change_protection(
         self,
         *,
         SubnetChangeProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
@@ -544,38 +556,59 @@
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/network-
         firewall-2020-11-12/UpdateSubnetChangeProtection).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_subnet_change_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_subnet_change_protection)
         """
+    def update_tls_inspection_configuration(
+        self,
+        *,
+        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
+        UpdateToken: str,
+        TLSInspectionConfigurationArn: str = ...,
+        TLSInspectionConfigurationName: str = ...,
+        Description: str = ...,
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+    ) -> UpdateTLSInspectionConfigurationResponseTypeDef:
+        """
+        Updates the TLS inspection configuration settings for the specified TLS
+        inspection configuration.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_tls_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_tls_inspection_configuration)
+        """
     @overload
     def get_paginator(
         self, operation_name: Literal["list_firewall_policies"]
     ) -> ListFirewallPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_firewalls"]) -> ListFirewallsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_rule_groups"]) -> ListRuleGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#get_paginator)
         """
-
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_tls_inspection_configurations"]
+    ) -> ListTLSInspectionConfigurationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#get_paginator)
+        """
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#get_paginator)
```

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/client.pyi` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,66 +20,76 @@
 
 from .literals import ResourceManagedStatusType, ResourceManagedTypeType, RuleGroupTypeType
 from .paginator import (
     ListFirewallPoliciesPaginator,
     ListFirewallsPaginator,
     ListRuleGroupsPaginator,
     ListTagsForResourcePaginator,
+    ListTLSInspectionConfigurationsPaginator,
 )
 from .type_defs import (
     AssociateFirewallPolicyResponseTypeDef,
     AssociateSubnetsResponseTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     CreateFirewallResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
+    CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DeleteRuleGroupResponseTypeDef,
+    DeleteTLSInspectionConfigurationResponseTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
     DescribeFirewallResponseTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     DescribeRuleGroupResponseTypeDef,
+    DescribeTLSInspectionConfigurationResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     EncryptionConfigurationTypeDef,
     FirewallPolicyTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListTLSInspectionConfigurationsResponseTypeDef,
     LoggingConfigurationTypeDef,
     RuleGroupTypeDef,
     SourceMetadataTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
+    TLSInspectionConfigurationTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
+    UpdateTLSInspectionConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("NetworkFirewallClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InsufficientCapacityException: Type[BotocoreClientError]
     InternalServerError: Type[BotocoreClientError]
     InvalidOperationException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     InvalidResourcePolicyException: Type[BotocoreClientError]
@@ -87,14 +97,15 @@
     LimitExceededException: Type[BotocoreClientError]
     LogDestinationPermissionException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceOwnerCheckException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
+
 class NetworkFirewallClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/)
     """
 
     meta: ClientMeta
@@ -103,56 +114,61 @@
     def exceptions(self) -> Exceptions:
         """
         NetworkFirewallClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#exceptions)
         """
+
     def associate_firewall_policy(
         self,
         *,
         FirewallPolicyArn: str,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> AssociateFirewallPolicyResponseTypeDef:
         """
         Associates a  FirewallPolicy to a  Firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.associate_firewall_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#associate_firewall_policy)
         """
+
     def associate_subnets(
         self,
         *,
         SubnetMappings: Sequence[SubnetMappingTypeDef],
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> AssociateSubnetsResponseTypeDef:
         """
         Associates the specified subnets in the Amazon VPC to the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.associate_subnets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#associate_subnets)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#close)
         """
+
     def create_firewall(
         self,
         *,
         FirewallName: str,
         FirewallPolicyArn: str,
         VpcId: str,
         SubnetMappings: Sequence[SubnetMappingTypeDef],
@@ -166,14 +182,15 @@
         """
         Creates an Network Firewall  Firewall and accompanying  FirewallStatus for a
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_firewall)
         """
+
     def create_firewall_policy(
         self,
         *,
         FirewallPolicyName: str,
         FirewallPolicy: FirewallPolicyTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
@@ -182,14 +199,15 @@
     ) -> CreateFirewallPolicyResponseTypeDef:
         """
         Creates the firewall policy for the firewall according to the specifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_firewall_policy)
         """
+
     def create_rule_group(
         self,
         *,
         RuleGroupName: str,
         Type: RuleGroupTypeType,
         Capacity: int,
         RuleGroup: RuleGroupTypeDef = ...,
@@ -203,148 +221,199 @@
         """
         Creates the specified stateless or stateful rule group, which includes the rules
         for network traffic inspection, a capacity setting, and tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_rule_group)
         """
+
+    def create_tls_inspection_configuration(
+        self,
+        *,
+        TLSInspectionConfigurationName: str,
+        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
+        Description: str = ...,
+        Tags: Sequence[TagTypeDef] = ...,
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+    ) -> CreateTLSInspectionConfigurationResponseTypeDef:
+        """
+        Creates an Network Firewall TLS inspection configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_tls_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_tls_inspection_configuration)
+        """
+
     def delete_firewall(
         self, *, FirewallName: str = ..., FirewallArn: str = ...
     ) -> DeleteFirewallResponseTypeDef:
         """
         Deletes the specified  Firewall and its  FirewallStatus.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#delete_firewall)
         """
+
     def delete_firewall_policy(
         self, *, FirewallPolicyName: str = ..., FirewallPolicyArn: str = ...
     ) -> DeleteFirewallPolicyResponseTypeDef:
         """
         Deletes the specified  FirewallPolicy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_firewall_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#delete_firewall_policy)
         """
+
     def delete_resource_policy(self, *, ResourceArn: str) -> Dict[str, Any]:
         """
         Deletes a resource policy that you created in a  PutResourcePolicy request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#delete_resource_policy)
         """
+
     def delete_rule_group(
         self, *, RuleGroupName: str = ..., RuleGroupArn: str = ..., Type: RuleGroupTypeType = ...
     ) -> DeleteRuleGroupResponseTypeDef:
         """
         Deletes the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#delete_rule_group)
         """
+
+    def delete_tls_inspection_configuration(
+        self, *, TLSInspectionConfigurationArn: str = ..., TLSInspectionConfigurationName: str = ...
+    ) -> DeleteTLSInspectionConfigurationResponseTypeDef:
+        """
+        Deletes the specified  TLSInspectionConfiguration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_tls_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#delete_tls_inspection_configuration)
+        """
+
     def describe_firewall(
         self, *, FirewallName: str = ..., FirewallArn: str = ...
     ) -> DescribeFirewallResponseTypeDef:
         """
         Returns the data objects for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_firewall)
         """
+
     def describe_firewall_policy(
         self, *, FirewallPolicyName: str = ..., FirewallPolicyArn: str = ...
     ) -> DescribeFirewallPolicyResponseTypeDef:
         """
         Returns the data objects for the specified firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_firewall_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_firewall_policy)
         """
+
     def describe_logging_configuration(
         self, *, FirewallArn: str = ..., FirewallName: str = ...
     ) -> DescribeLoggingConfigurationResponseTypeDef:
         """
         Returns the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_logging_configuration)
         """
+
     def describe_resource_policy(
         self, *, ResourceArn: str
     ) -> DescribeResourcePolicyResponseTypeDef:
         """
         Retrieves a resource policy that you created in a  PutResourcePolicy request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_resource_policy)
         """
+
     def describe_rule_group(
         self, *, RuleGroupName: str = ..., RuleGroupArn: str = ..., Type: RuleGroupTypeType = ...
     ) -> DescribeRuleGroupResponseTypeDef:
         """
         Returns the data objects for the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_rule_group)
         """
+
     def describe_rule_group_metadata(
         self, *, RuleGroupName: str = ..., RuleGroupArn: str = ..., Type: RuleGroupTypeType = ...
     ) -> DescribeRuleGroupMetadataResponseTypeDef:
         """
         High-level information about a rule group, returned by operations like create
         and describe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_rule_group_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_rule_group_metadata)
         """
+
+    def describe_tls_inspection_configuration(
+        self, *, TLSInspectionConfigurationArn: str = ..., TLSInspectionConfigurationName: str = ...
+    ) -> DescribeTLSInspectionConfigurationResponseTypeDef:
+        """
+        Returns the data objects for the specified TLS inspection configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_tls_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#describe_tls_inspection_configuration)
+        """
+
     def disassociate_subnets(
         self,
         *,
         SubnetIds: Sequence[str],
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> DisassociateSubnetsResponseTypeDef:
         """
         Removes the specified subnet associations from the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.disassociate_subnets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#disassociate_subnets)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#generate_presigned_url)
         """
+
     def list_firewall_policies(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListFirewallPoliciesResponseTypeDef:
         """
         Retrieves the metadata for the firewall policies that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_firewall_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#list_firewall_policies)
         """
+
     def list_firewalls(
         self, *, NextToken: str = ..., VpcIds: Sequence[str] = ..., MaxResults: int = ...
     ) -> ListFirewallsResponseTypeDef:
         """
         Retrieves the metadata for the firewalls that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_firewalls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#list_firewalls)
         """
+
     def list_rule_groups(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
@@ -352,87 +421,106 @@
     ) -> ListRuleGroupsResponseTypeDef:
         """
         Retrieves the metadata for the rule groups that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_rule_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#list_rule_groups)
         """
+
     def list_tags_for_resource(
         self, *, ResourceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves the tags associated with the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#list_tags_for_resource)
         """
+
+    def list_tls_inspection_configurations(
+        self, *, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListTLSInspectionConfigurationsResponseTypeDef:
+        """
+        Retrieves the metadata for the TLS inspection configurations that you have
+        defined.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_tls_inspection_configurations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#list_tls_inspection_configurations)
+        """
+
     def put_resource_policy(self, *, ResourceArn: str, Policy: str) -> Dict[str, Any]:
         """
         Creates or updates an IAM policy for your rule group or firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#put_resource_policy)
         """
+
     def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds the specified tags to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the tags with the specified keys from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#untag_resource)
         """
+
     def update_firewall_delete_protection(
         self,
         *,
         DeleteProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> UpdateFirewallDeleteProtectionResponseTypeDef:
         """
-        Modifies the flag, `DeleteProtection` , which indicates whether it is possible
-        to delete the firewall.
+        Modifies the flag, `DeleteProtection`, which indicates whether it is possible to
+        delete the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_delete_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_delete_protection)
         """
+
     def update_firewall_description(
         self,
         *,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...,
         Description: str = ...
     ) -> UpdateFirewallDescriptionResponseTypeDef:
         """
         Modifies the description for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_description)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_description)
         """
+
     def update_firewall_encryption_configuration(
         self,
         *,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateFirewallEncryptionConfigurationResponseTypeDef:
         """
         A complex type that contains settings for encryption of your firewall resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_encryption_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_encryption_configuration)
         """
+
     def update_firewall_policy(
         self,
         *,
         UpdateToken: str,
         FirewallPolicy: FirewallPolicyTypeDef,
         FirewallPolicyArn: str = ...,
         FirewallPolicyName: str = ...,
@@ -442,42 +530,45 @@
     ) -> UpdateFirewallPolicyResponseTypeDef:
         """
         Updates the properties of the specified firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_policy)
         """
+
     def update_firewall_policy_change_protection(
         self,
         *,
         FirewallPolicyChangeProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> UpdateFirewallPolicyChangeProtectionResponseTypeDef:
         """
-        Modifies the flag, `ChangeProtection` , which indicates whether it is possible
-        to change the firewall.
+        Modifies the flag, `ChangeProtection`, which indicates whether it is possible to
+        change the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_policy_change_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_policy_change_protection)
         """
+
     def update_logging_configuration(
         self,
         *,
         FirewallArn: str = ...,
         FirewallName: str = ...,
         LoggingConfiguration: LoggingConfigurationTypeDef = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Sets the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_logging_configuration)
         """
+
     def update_rule_group(
         self,
         *,
         UpdateToken: str,
         RuleGroupArn: str = ...,
         RuleGroupName: str = ...,
         RuleGroup: RuleGroupTypeDef = ...,
@@ -490,14 +581,15 @@
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the rule settings for the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_rule_group)
         """
+
     def update_subnet_change_protection(
         self,
         *,
         SubnetChangeProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
@@ -506,34 +598,65 @@
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/network-
         firewall-2020-11-12/UpdateSubnetChangeProtection).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_subnet_change_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_subnet_change_protection)
         """
+
+    def update_tls_inspection_configuration(
+        self,
+        *,
+        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
+        UpdateToken: str,
+        TLSInspectionConfigurationArn: str = ...,
+        TLSInspectionConfigurationName: str = ...,
+        Description: str = ...,
+        EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
+    ) -> UpdateTLSInspectionConfigurationResponseTypeDef:
+        """
+        Updates the TLS inspection configuration settings for the specified TLS
+        inspection configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_tls_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_tls_inspection_configuration)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_firewall_policies"]
     ) -> ListFirewallPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_firewalls"]) -> ListFirewallsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_rule_groups"]) -> ListRuleGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#get_paginator)
         """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_tls_inspection_configurations"]
+    ) -> ListTLSInspectionConfigurationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#get_paginator)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#get_paginator)
```

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/literals.py` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "EncryptionTypeType",
     "FirewallStatusValueType",
     "GeneratedRulesTypeType",
     "IPAddressTypeType",
     "ListFirewallPoliciesPaginatorName",
     "ListFirewallsPaginatorName",
     "ListRuleGroupsPaginatorName",
+    "ListTLSInspectionConfigurationsPaginatorName",
     "ListTagsForResourcePaginatorName",
     "LogDestinationTypeType",
     "LogTypeType",
     "OverrideActionType",
     "PerObjectSyncStatusType",
     "ResourceManagedStatusType",
     "ResourceManagedTypeType",
@@ -49,23 +50,24 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
-AttachmentStatusType = Literal["CREATING", "DELETING", "READY", "SCALING"]
+AttachmentStatusType = Literal["CREATING", "DELETING", "ERROR", "FAILED", "READY", "SCALING"]
 ConfigurationSyncStateType = Literal["CAPACITY_CONSTRAINED", "IN_SYNC", "PENDING"]
 EncryptionTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_KMS"]
 FirewallStatusValueType = Literal["DELETING", "PROVISIONING", "READY"]
 GeneratedRulesTypeType = Literal["ALLOWLIST", "DENYLIST"]
-IPAddressTypeType = Literal["DUALSTACK", "IPV4"]
+IPAddressTypeType = Literal["DUALSTACK", "IPV4", "IPV6"]
 ListFirewallPoliciesPaginatorName = Literal["list_firewall_policies"]
 ListFirewallsPaginatorName = Literal["list_firewalls"]
 ListRuleGroupsPaginatorName = Literal["list_rule_groups"]
+ListTLSInspectionConfigurationsPaginatorName = Literal["list_tls_inspection_configurations"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 LogDestinationTypeType = Literal["CloudWatchLogs", "KinesisDataFirehose", "S3"]
 LogTypeType = Literal["ALERT", "FLOW"]
 OverrideActionType = Literal["DROP_TO_ALERT"]
 PerObjectSyncStatusType = Literal["CAPACITY_CONSTRAINED", "IN_SYNC", "PENDING"]
 ResourceManagedStatusType = Literal["ACCOUNT", "MANAGED"]
 ResourceManagedTypeType = Literal["AWS_MANAGED_DOMAIN_LISTS", "AWS_MANAGED_THREAT_SIGNATURES"]
@@ -91,15 +93,15 @@
     "SMTP",
     "SSH",
     "TCP",
     "TFTP",
     "TLS",
     "UDP",
 ]
-StreamExceptionPolicyType = Literal["CONTINUE", "DROP"]
+StreamExceptionPolicyType = Literal["CONTINUE", "DROP", "REJECT"]
 TCPFlagType = Literal["ACK", "CWR", "ECE", "FIN", "PSH", "RST", "SYN", "URG"]
 TargetTypeType = Literal["HTTP_HOST", "TLS_SNI"]
 NetworkFirewallServiceName = Literal["network-firewall"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -110,14 +112,15 @@
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
@@ -149,21 +152,23 @@
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
@@ -242,14 +247,15 @@
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
@@ -260,14 +266,15 @@
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
@@ -303,14 +310,15 @@
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
@@ -329,16 +337,19 @@
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
@@ -418,18 +429,21 @@
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
@@ -448,15 +462,19 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "list_firewall_policies", "list_firewalls", "list_rule_groups", "list_tags_for_resource"
+    "list_firewall_policies",
+    "list_firewalls",
+    "list_rule_groups",
+    "list_tags_for_resource",
+    "list_tls_inspection_configurations",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
@@ -467,14 +485,15 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
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

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/literals.pyi` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "EncryptionTypeType",
     "FirewallStatusValueType",
     "GeneratedRulesTypeType",
     "IPAddressTypeType",
     "ListFirewallPoliciesPaginatorName",
     "ListFirewallsPaginatorName",
     "ListRuleGroupsPaginatorName",
+    "ListTLSInspectionConfigurationsPaginatorName",
     "ListTagsForResourcePaginatorName",
     "LogDestinationTypeType",
     "LogTypeType",
     "OverrideActionType",
     "PerObjectSyncStatusType",
     "ResourceManagedStatusType",
     "ResourceManagedTypeType",
@@ -47,23 +48,24 @@
     "NetworkFirewallServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-AttachmentStatusType = Literal["CREATING", "DELETING", "READY", "SCALING"]
+AttachmentStatusType = Literal["CREATING", "DELETING", "ERROR", "FAILED", "READY", "SCALING"]
 ConfigurationSyncStateType = Literal["CAPACITY_CONSTRAINED", "IN_SYNC", "PENDING"]
 EncryptionTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_KMS"]
 FirewallStatusValueType = Literal["DELETING", "PROVISIONING", "READY"]
 GeneratedRulesTypeType = Literal["ALLOWLIST", "DENYLIST"]
-IPAddressTypeType = Literal["DUALSTACK", "IPV4"]
+IPAddressTypeType = Literal["DUALSTACK", "IPV4", "IPV6"]
 ListFirewallPoliciesPaginatorName = Literal["list_firewall_policies"]
 ListFirewallsPaginatorName = Literal["list_firewalls"]
 ListRuleGroupsPaginatorName = Literal["list_rule_groups"]
+ListTLSInspectionConfigurationsPaginatorName = Literal["list_tls_inspection_configurations"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 LogDestinationTypeType = Literal["CloudWatchLogs", "KinesisDataFirehose", "S3"]
 LogTypeType = Literal["ALERT", "FLOW"]
 OverrideActionType = Literal["DROP_TO_ALERT"]
 PerObjectSyncStatusType = Literal["CAPACITY_CONSTRAINED", "IN_SYNC", "PENDING"]
 ResourceManagedStatusType = Literal["ACCOUNT", "MANAGED"]
 ResourceManagedTypeType = Literal["AWS_MANAGED_DOMAIN_LISTS", "AWS_MANAGED_THREAT_SIGNATURES"]
@@ -89,15 +91,15 @@
     "SMTP",
     "SSH",
     "TCP",
     "TFTP",
     "TLS",
     "UDP",
 ]
-StreamExceptionPolicyType = Literal["CONTINUE", "DROP"]
+StreamExceptionPolicyType = Literal["CONTINUE", "DROP", "REJECT"]
 TCPFlagType = Literal["ACK", "CWR", "ECE", "FIN", "PSH", "RST", "SYN", "URG"]
 TargetTypeType = Literal["HTTP_HOST", "TLS_SNI"]
 NetworkFirewallServiceName = Literal["network-firewall"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -108,14 +110,15 @@
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
@@ -147,21 +150,23 @@
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
@@ -240,14 +245,15 @@
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
@@ -258,14 +264,15 @@
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
@@ -301,14 +308,15 @@
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
@@ -327,16 +335,19 @@
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
@@ -416,18 +427,21 @@
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
@@ -446,15 +460,19 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "list_firewall_policies", "list_firewalls", "list_rule_groups", "list_tags_for_resource"
+    "list_firewall_policies",
+    "list_firewalls",
+    "list_rule_groups",
+    "list_tags_for_resource",
+    "list_tls_inspection_configurations",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
@@ -465,14 +483,15 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
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

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/paginator.py` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/paginator.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,43 +9,47 @@
     from boto3.session import Session
 
     from mypy_boto3_network_firewall.client import NetworkFirewallClient
     from mypy_boto3_network_firewall.paginator import (
         ListFirewallPoliciesPaginator,
         ListFirewallsPaginator,
         ListRuleGroupsPaginator,
+        ListTLSInspectionConfigurationsPaginator,
         ListTagsForResourcePaginator,
     )
 
     session = Session()
     client: NetworkFirewallClient = session.client("network-firewall")
 
     list_firewall_policies_paginator: ListFirewallPoliciesPaginator = client.get_paginator("list_firewall_policies")
     list_firewalls_paginator: ListFirewallsPaginator = client.get_paginator("list_firewalls")
     list_rule_groups_paginator: ListRuleGroupsPaginator = client.get_paginator("list_rule_groups")
+    list_tls_inspection_configurations_paginator: ListTLSInspectionConfigurationsPaginator = client.get_paginator("list_tls_inspection_configurations")
     list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ResourceManagedStatusType, ResourceManagedTypeType, RuleGroupTypeType
 from .type_defs import (
     ListFirewallPoliciesResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListTLSInspectionConfigurationsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListFirewallPoliciesPaginator",
     "ListFirewallsPaginator",
     "ListRuleGroupsPaginator",
+    "ListTLSInspectionConfigurationsPaginator",
     "ListTagsForResourcePaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
@@ -59,30 +63,30 @@
 class ListFirewallPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallpoliciespaginator)
         """
 
 
 class ListFirewallsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallspaginator)
     """
 
     def paginate(
-        self, *, VpcIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, VpcIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFirewallsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallspaginator)
         """
 
 
@@ -94,28 +98,43 @@
 
     def paginate(
         self,
         *,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
         Type: RuleGroupTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListRuleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listrulegroupspaginator)
         """
 
 
+class ListTLSInspectionConfigurationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtlsinspectionconfigurationspaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListTLSInspectionConfigurationsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtlsinspectionconfigurationspaginator)
+        """
+
+
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/paginator.pyi` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/paginator.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -9,43 +9,47 @@
     from boto3.session import Session
 
     from mypy_boto3_network_firewall.client import NetworkFirewallClient
     from mypy_boto3_network_firewall.paginator import (
         ListFirewallPoliciesPaginator,
         ListFirewallsPaginator,
         ListRuleGroupsPaginator,
+        ListTLSInspectionConfigurationsPaginator,
         ListTagsForResourcePaginator,
     )
 
     session = Session()
     client: NetworkFirewallClient = session.client("network-firewall")
 
     list_firewall_policies_paginator: ListFirewallPoliciesPaginator = client.get_paginator("list_firewall_policies")
     list_firewalls_paginator: ListFirewallsPaginator = client.get_paginator("list_firewalls")
     list_rule_groups_paginator: ListRuleGroupsPaginator = client.get_paginator("list_rule_groups")
+    list_tls_inspection_configurations_paginator: ListTLSInspectionConfigurationsPaginator = client.get_paginator("list_tls_inspection_configurations")
     list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ResourceManagedStatusType, ResourceManagedTypeType, RuleGroupTypeType
 from .type_defs import (
     ListFirewallPoliciesResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListTLSInspectionConfigurationsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListFirewallPoliciesPaginator",
     "ListFirewallsPaginator",
     "ListRuleGroupsPaginator",
+    "ListTLSInspectionConfigurationsPaginator",
     "ListTagsForResourcePaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
@@ -56,29 +60,29 @@
 class ListFirewallPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallpoliciespaginator)
         """
 
 class ListFirewallsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallspaginator)
     """
 
     def paginate(
-        self, *, VpcIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, VpcIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFirewallsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallspaginator)
         """
 
 class ListRuleGroupsPaginator(Paginator):
@@ -89,27 +93,41 @@
 
     def paginate(
         self,
         *,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
         Type: RuleGroupTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListRuleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listrulegroupspaginator)
         """
 
+class ListTLSInspectionConfigurationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtlsinspectionconfigurationspaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListTLSInspectionConfigurationsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtlsinspectionconfigurationspaginator)
+        """
+
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/type_defs.py` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,66 +47,77 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddressTypeDef",
     "AssociateFirewallPolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateFirewallPolicyResponseTypeDef",
     "SubnetMappingTypeDef",
     "AttachmentTypeDef",
     "IPSetMetadataTypeDef",
     "EncryptionConfigurationTypeDef",
     "TagTypeDef",
     "SourceMetadataTypeDef",
     "DeleteFirewallPolicyRequestRequestTypeDef",
     "DeleteFirewallRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
+    "DeleteTLSInspectionConfigurationRequestRequestTypeDef",
     "DescribeFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallRequestRequestTypeDef",
     "DescribeLoggingConfigurationRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
     "StatefulRuleOptionsTypeDef",
     "DescribeRuleGroupRequestRequestTypeDef",
+    "DescribeTLSInspectionConfigurationRequestRequestTypeDef",
     "DimensionTypeDef",
     "DisassociateSubnetsRequestRequestTypeDef",
     "FirewallMetadataTypeDef",
     "FirewallPolicyMetadataTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupReferenceTypeDef",
     "HeaderTypeDef",
     "IPSetReferenceTypeDef",
     "IPSetTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
     "ListFirewallPoliciesRequestRequestTypeDef",
+    "ListFirewallsRequestListFirewallsPaginateTypeDef",
     "ListFirewallsRequestRequestTypeDef",
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupMetadataTypeDef",
+    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
+    "ListTLSInspectionConfigurationsRequestRequestTypeDef",
+    "TLSInspectionConfigurationMetadataTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "LogDestinationConfigTypeDef",
     "PortRangeTypeDef",
     "TCPFlagFieldTypeDef",
+    "PaginatorConfigTypeDef",
     "PerObjectStatusTypeDef",
     "PortSetTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RuleOptionTypeDef",
     "RulesSourceListTypeDef",
+    "ServerCertificateTypeDef",
     "StatefulRuleGroupOverrideTypeDef",
+    "TlsCertificateDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallDeleteProtectionRequestRequestTypeDef",
-    "UpdateFirewallDescriptionRequestRequestTypeDef",
-    "UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
-    "UpdateSubnetChangeProtectionRequestRequestTypeDef",
-    "AssociateFirewallPolicyResponseTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "UpdateFirewallDeleteProtectionResponseTypeDef",
+    "UpdateFirewallDescriptionRequestRequestTypeDef",
     "UpdateFirewallDescriptionResponseTypeDef",
+    "UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
     "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
+    "UpdateSubnetChangeProtectionRequestRequestTypeDef",
     "UpdateSubnetChangeProtectionResponseTypeDef",
     "AssociateSubnetsRequestRequestTypeDef",
     "AssociateSubnetsResponseTypeDef",
     "DisassociateSubnetsResponseTypeDef",
     "CIDRSummaryTypeDef",
     "UpdateFirewallEncryptionConfigurationRequestRequestTypeDef",
     "UpdateFirewallEncryptionConfigurationResponseTypeDef",
@@ -117,44 +128,52 @@
     "TagResourceRequestRequestTypeDef",
     "RuleGroupResponseTypeDef",
     "DescribeRuleGroupMetadataResponseTypeDef",
     "PublishMetricActionTypeDef",
     "ListFirewallsResponseTypeDef",
     "ListFirewallPoliciesResponseTypeDef",
     "ReferenceSetsTypeDef",
-    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
-    "ListFirewallsRequestListFirewallsPaginateTypeDef",
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "PolicyVariablesTypeDef",
     "ListRuleGroupsResponseTypeDef",
+    "ListTLSInspectionConfigurationsResponseTypeDef",
     "LoggingConfigurationTypeDef",
+    "ServerCertificateScopeTypeDef",
     "MatchAttributesTypeDef",
     "SyncStateTypeDef",
     "RuleVariablesTypeDef",
     "StatefulRuleTypeDef",
     "StatefulRuleGroupReferenceTypeDef",
+    "TLSInspectionConfigurationResponseTypeDef",
     "CapacityUsageSummaryTypeDef",
     "CreateFirewallPolicyResponseTypeDef",
     "DeleteFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "DeleteRuleGroupResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "ActionDefinitionTypeDef",
     "DescribeLoggingConfigurationResponseTypeDef",
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
+    "ServerCertificateConfigurationTypeDef",
     "RuleDefinitionTypeDef",
+    "CreateTLSInspectionConfigurationResponseTypeDef",
+    "DeleteTLSInspectionConfigurationResponseTypeDef",
+    "UpdateTLSInspectionConfigurationResponseTypeDef",
     "FirewallStatusTypeDef",
     "CustomActionTypeDef",
+    "TLSInspectionConfigurationTypeDef",
     "StatelessRuleTypeDef",
     "CreateFirewallResponseTypeDef",
     "DeleteFirewallResponseTypeDef",
     "DescribeFirewallResponseTypeDef",
     "FirewallPolicyTypeDef",
+    "CreateTLSInspectionConfigurationRequestRequestTypeDef",
+    "DescribeTLSInspectionConfigurationResponseTypeDef",
+    "UpdateTLSInspectionConfigurationRequestRequestTypeDef",
     "StatelessRulesAndCustomActionsTypeDef",
     "CreateFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyRequestRequestTypeDef",
     "RulesSourceTypeDef",
     "RuleGroupTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
@@ -189,22 +208,22 @@
 class AssociateFirewallPolicyRequestRequestTypeDef(
     _RequiredAssociateFirewallPolicyRequestRequestTypeDef,
     _OptionalAssociateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateFirewallPolicyResponseTypeDef = TypedDict(
+    "AssociateFirewallPolicyResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "FirewallArn": str,
+        "FirewallName": str,
+        "FirewallPolicyArn": str,
+        "UpdateToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSubnetMappingTypeDef = TypedDict(
     "_RequiredSubnetMappingTypeDef",
     {
         "SubnetId": str,
@@ -311,14 +330,23 @@
         "RuleGroupName": str,
         "RuleGroupArn": str,
         "Type": RuleGroupTypeType,
     },
     total=False,
 )
 
+DeleteTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "DeleteTLSInspectionConfigurationRequestRequestTypeDef",
+    {
+        "TLSInspectionConfigurationArn": str,
+        "TLSInspectionConfigurationName": str,
+    },
+    total=False,
+)
+
 DescribeFirewallPolicyRequestRequestTypeDef = TypedDict(
     "DescribeFirewallPolicyRequestRequestTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicyArn": str,
     },
     total=False,
@@ -345,14 +373,22 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeRuleGroupMetadataRequestRequestTypeDef = TypedDict(
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
     {
         "RuleGroupName": str,
         "RuleGroupArn": str,
         "Type": RuleGroupTypeType,
     },
@@ -373,14 +409,23 @@
         "RuleGroupName": str,
         "RuleGroupArn": str,
         "Type": RuleGroupTypeType,
     },
     total=False,
 )
 
+DescribeTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "DescribeTLSInspectionConfigurationRequestRequestTypeDef",
+    {
+        "TLSInspectionConfigurationArn": str,
+        "TLSInspectionConfigurationName": str,
+    },
+    total=False,
+)
+
 DimensionTypeDef = TypedDict(
     "DimensionTypeDef",
     {
         "Value": str,
     },
 )
 
@@ -466,43 +511,61 @@
 IPSetTypeDef = TypedDict(
     "IPSetTypeDef",
     {
         "Definition": Sequence[str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = TypedDict(
+    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "ListFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListFirewallsRequestListFirewallsPaginateTypeDef = TypedDict(
+    "ListFirewallsRequestListFirewallsPaginateTypeDef",
+    {
+        "VpcIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFirewallsRequestRequestTypeDef = TypedDict(
     "ListFirewallsRequestRequestTypeDef",
     {
         "NextToken": str,
         "VpcIds": Sequence[str],
         "MaxResults": int,
     },
     total=False,
 )
 
+ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    {
+        "Scope": ResourceManagedStatusType,
+        "ManagedType": ResourceManagedTypeType,
+        "Type": RuleGroupTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Scope": ResourceManagedStatusType,
         "ManagedType": ResourceManagedTypeType,
@@ -516,14 +579,62 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
+ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef = TypedDict(
+    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListTLSInspectionConfigurationsRequestRequestTypeDef = TypedDict(
+    "ListTLSInspectionConfigurationsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+TLSInspectionConfigurationMetadataTypeDef = TypedDict(
+    "TLSInspectionConfigurationMetadataTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -575,14 +686,24 @@
 )
 
 
 class TCPFlagFieldTypeDef(_RequiredTCPFlagFieldTypeDef, _OptionalTCPFlagFieldTypeDef):
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
 PerObjectStatusTypeDef = TypedDict(
     "PerObjectStatusTypeDef",
     {
         "SyncStatus": PerObjectSyncStatusType,
         "UpdateToken": str,
     },
     total=False,
@@ -600,14 +721,25 @@
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
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
 _RequiredRuleOptionTypeDef = TypedDict(
     "_RequiredRuleOptionTypeDef",
     {
         "Keyword": str,
     },
 )
 _OptionalRuleOptionTypeDef = TypedDict(
@@ -628,22 +760,41 @@
     {
         "Targets": Sequence[str],
         "TargetTypes": Sequence[TargetTypeType],
         "GeneratedRulesType": GeneratedRulesTypeType,
     },
 )
 
+ServerCertificateTypeDef = TypedDict(
+    "ServerCertificateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+    total=False,
+)
+
 StatefulRuleGroupOverrideTypeDef = TypedDict(
     "StatefulRuleGroupOverrideTypeDef",
     {
         "Action": Literal["DROP_TO_ALERT"],
     },
     total=False,
 )
 
+TlsCertificateDataTypeDef = TypedDict(
+    "TlsCertificateDataTypeDef",
+    {
+        "CertificateArn": str,
+        "CertificateSerial": str,
+        "Status": str,
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -668,25 +819,47 @@
 class UpdateFirewallDeleteProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallDeleteProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallDeleteProtectionRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateFirewallDeleteProtectionResponseTypeDef = TypedDict(
+    "UpdateFirewallDeleteProtectionResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "DeleteProtection": bool,
+        "UpdateToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateFirewallDescriptionRequestRequestTypeDef = TypedDict(
     "UpdateFirewallDescriptionRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "Description": str,
     },
     total=False,
 )
 
+UpdateFirewallDescriptionResponseTypeDef = TypedDict(
+    "UpdateFirewallDescriptionResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "Description": str,
+        "UpdateToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
     {
         "FirewallPolicyChangeProtection": bool,
     },
 )
 _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -703,14 +876,25 @@
 class UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateFirewallPolicyChangeProtectionResponseTypeDef = TypedDict(
+    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "FirewallArn": str,
+        "FirewallName": str,
+        "FirewallPolicyChangeProtection": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef",
     {
         "SubnetChangeProtection": bool,
     },
 )
 _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -727,74 +911,22 @@
 class UpdateSubnetChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateFirewallPolicyResponseTypeDef = TypedDict(
-    "AssociateFirewallPolicyResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "FirewallPolicyArn": str,
-        "UpdateToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFirewallDeleteProtectionResponseTypeDef = TypedDict(
-    "UpdateFirewallDeleteProtectionResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "DeleteProtection": bool,
-        "UpdateToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFirewallDescriptionResponseTypeDef = TypedDict(
-    "UpdateFirewallDescriptionResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "Description": str,
-        "UpdateToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFirewallPolicyChangeProtectionResponseTypeDef = TypedDict(
-    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "FirewallArn": str,
-        "FirewallName": str,
-        "FirewallPolicyChangeProtection": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateSubnetChangeProtectionResponseTypeDef = TypedDict(
     "UpdateSubnetChangeProtectionResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetChangeProtection": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAssociateSubnetsRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateSubnetsRequestRequestTypeDef",
     {
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
@@ -820,26 +952,26 @@
 AssociateSubnetsResponseTypeDef = TypedDict(
     "AssociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateSubnetsResponseTypeDef = TypedDict(
     "DisassociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CIDRSummaryTypeDef = TypedDict(
     "CIDRSummaryTypeDef",
     {
         "AvailableCIDRCount": int,
@@ -863,15 +995,15 @@
 UpdateFirewallEncryptionConfigurationResponseTypeDef = TypedDict(
     "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "UpdateToken": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFirewallRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRequestRequestTypeDef",
     {
         "FirewallName": str,
@@ -960,15 +1092,15 @@
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextToken": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1015,15 +1147,15 @@
         "RuleGroupArn": str,
         "RuleGroupName": str,
         "Description": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
         "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
         "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PublishMetricActionTypeDef = TypedDict(
     "PublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
@@ -1031,101 +1163,80 @@
 )
 
 ListFirewallsResponseTypeDef = TypedDict(
     "ListFirewallsResponseTypeDef",
     {
         "NextToken": str,
         "Firewalls": List[FirewallMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFirewallPoliciesResponseTypeDef = TypedDict(
     "ListFirewallPoliciesResponseTypeDef",
     {
         "NextToken": str,
         "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReferenceSetsTypeDef = TypedDict(
     "ReferenceSetsTypeDef",
     {
         "IPSetReferences": Mapping[str, IPSetReferenceTypeDef],
     },
     total=False,
 )
 
-ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = TypedDict(
-    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFirewallsRequestListFirewallsPaginateTypeDef = TypedDict(
-    "ListFirewallsRequestListFirewallsPaginateTypeDef",
+PolicyVariablesTypeDef = TypedDict(
+    "PolicyVariablesTypeDef",
     {
-        "VpcIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "RuleVariables": Mapping[str, IPSetTypeDef],
     },
     total=False,
 )
 
-ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
-    {
-        "Scope": ResourceManagedStatusType,
-        "ManagedType": ResourceManagedTypeType,
-        "Type": RuleGroupTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+ListRuleGroupsResponseTypeDef = TypedDict(
+    "ListRuleGroupsResponseTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "RuleGroups": List[RuleGroupMetadataTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
-ListRuleGroupsResponseTypeDef = TypedDict(
-    "ListRuleGroupsResponseTypeDef",
+ListTLSInspectionConfigurationsResponseTypeDef = TypedDict(
+    "ListTLSInspectionConfigurationsResponseTypeDef",
     {
         "NextToken": str,
-        "RuleGroups": List[RuleGroupMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TLSInspectionConfigurations": List[TLSInspectionConfigurationMetadataTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "LogDestinationConfigs": List[LogDestinationConfigTypeDef],
     },
 )
 
+ServerCertificateScopeTypeDef = TypedDict(
+    "ServerCertificateScopeTypeDef",
+    {
+        "Sources": Sequence[AddressTypeDef],
+        "Destinations": Sequence[AddressTypeDef],
+        "SourcePorts": Sequence[PortRangeTypeDef],
+        "DestinationPorts": Sequence[PortRangeTypeDef],
+        "Protocols": Sequence[int],
+    },
+    total=False,
+)
+
 MatchAttributesTypeDef = TypedDict(
     "MatchAttributesTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
@@ -1180,71 +1291,101 @@
 
 class StatefulRuleGroupReferenceTypeDef(
     _RequiredStatefulRuleGroupReferenceTypeDef, _OptionalStatefulRuleGroupReferenceTypeDef
 ):
     pass
 
 
+_RequiredTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "_RequiredTLSInspectionConfigurationResponseTypeDef",
+    {
+        "TLSInspectionConfigurationArn": str,
+        "TLSInspectionConfigurationName": str,
+        "TLSInspectionConfigurationId": str,
+    },
+)
+_OptionalTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "_OptionalTLSInspectionConfigurationResponseTypeDef",
+    {
+        "TLSInspectionConfigurationStatus": ResourceStatusType,
+        "Description": str,
+        "Tags": List[TagTypeDef],
+        "LastModifiedTime": datetime,
+        "NumberOfAssociations": int,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "Certificates": List[TlsCertificateDataTypeDef],
+    },
+    total=False,
+)
+
+
+class TLSInspectionConfigurationResponseTypeDef(
+    _RequiredTLSInspectionConfigurationResponseTypeDef,
+    _OptionalTLSInspectionConfigurationResponseTypeDef,
+):
+    pass
+
+
 CapacityUsageSummaryTypeDef = TypedDict(
     "CapacityUsageSummaryTypeDef",
     {
         "CIDRs": CIDRSummaryTypeDef,
     },
     total=False,
 )
 
 CreateFirewallPolicyResponseTypeDef = TypedDict(
     "CreateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteFirewallPolicyResponseTypeDef = TypedDict(
     "DeleteFirewallPolicyResponseTypeDef",
     {
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFirewallPolicyResponseTypeDef = TypedDict(
     "UpdateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "UpdateToken": str,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRuleGroupResponseTypeDef = TypedDict(
     "DeleteRuleGroupResponseTypeDef",
     {
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRuleGroupResponseTypeDef = TypedDict(
     "UpdateRuleGroupResponseTypeDef",
     {
         "UpdateToken": str,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActionDefinitionTypeDef = TypedDict(
     "ActionDefinitionTypeDef",
     {
         "PublishMetricAction": PublishMetricActionTypeDef,
@@ -1253,15 +1394,15 @@
 )
 
 DescribeLoggingConfigurationResponseTypeDef = TypedDict(
     "DescribeLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "FirewallArn": str,
@@ -1273,26 +1414,61 @@
 
 UpdateLoggingConfigurationResponseTypeDef = TypedDict(
     "UpdateLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ServerCertificateConfigurationTypeDef = TypedDict(
+    "ServerCertificateConfigurationTypeDef",
+    {
+        "ServerCertificates": Sequence[ServerCertificateTypeDef],
+        "Scopes": Sequence[ServerCertificateScopeTypeDef],
+    },
+    total=False,
+)
+
 RuleDefinitionTypeDef = TypedDict(
     "RuleDefinitionTypeDef",
     {
         "MatchAttributes": MatchAttributesTypeDef,
         "Actions": Sequence[str],
     },
 )
 
+CreateTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "CreateTLSInspectionConfigurationResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "DeleteTLSInspectionConfigurationResponseTypeDef",
+    {
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "UpdateTLSInspectionConfigurationResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFirewallStatusTypeDef = TypedDict(
     "_RequiredFirewallStatusTypeDef",
     {
         "Status": FirewallStatusValueType,
         "ConfigurationSyncStateSummary": ConfigurationSyncStateType,
     },
 )
@@ -1314,47 +1490,55 @@
     "CustomActionTypeDef",
     {
         "ActionName": str,
         "ActionDefinition": ActionDefinitionTypeDef,
     },
 )
 
+TLSInspectionConfigurationTypeDef = TypedDict(
+    "TLSInspectionConfigurationTypeDef",
+    {
+        "ServerCertificateConfigurations": Sequence[ServerCertificateConfigurationTypeDef],
+    },
+    total=False,
+)
+
 StatelessRuleTypeDef = TypedDict(
     "StatelessRuleTypeDef",
     {
         "RuleDefinition": RuleDefinitionTypeDef,
         "Priority": int,
     },
 )
 
 CreateFirewallResponseTypeDef = TypedDict(
     "CreateFirewallResponseTypeDef",
     {
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteFirewallResponseTypeDef = TypedDict(
     "DeleteFirewallResponseTypeDef",
     {
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFirewallResponseTypeDef = TypedDict(
     "DescribeFirewallResponseTypeDef",
     {
         "UpdateToken": str,
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFirewallPolicyTypeDef = TypedDict(
     "_RequiredFirewallPolicyTypeDef",
     {
         "StatelessDefaultActions": Sequence[str],
@@ -1365,23 +1549,86 @@
     "_OptionalFirewallPolicyTypeDef",
     {
         "StatelessRuleGroupReferences": Sequence[StatelessRuleGroupReferenceTypeDef],
         "StatelessCustomActions": Sequence[CustomActionTypeDef],
         "StatefulRuleGroupReferences": Sequence[StatefulRuleGroupReferenceTypeDef],
         "StatefulDefaultActions": Sequence[str],
         "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
+        "TLSInspectionConfigurationArn": str,
+        "PolicyVariables": PolicyVariablesTypeDef,
     },
     total=False,
 )
 
 
 class FirewallPolicyTypeDef(_RequiredFirewallPolicyTypeDef, _OptionalFirewallPolicyTypeDef):
     pass
 
 
+_RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef",
+    {
+        "TLSInspectionConfigurationName": str,
+        "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
+    },
+)
+_OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateTLSInspectionConfigurationRequestRequestTypeDef(
+    _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef,
+    _OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "DescribeTLSInspectionConfigurationResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef",
+    {
+        "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
+        "UpdateToken": str,
+    },
+)
+_OptionalUpdateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTLSInspectionConfigurationRequestRequestTypeDef",
+    {
+        "TLSInspectionConfigurationArn": str,
+        "TLSInspectionConfigurationName": str,
+        "Description": str,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateTLSInspectionConfigurationRequestRequestTypeDef(
+    _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef,
+    _OptionalUpdateTLSInspectionConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredStatelessRulesAndCustomActionsTypeDef = TypedDict(
     "_RequiredStatelessRulesAndCustomActionsTypeDef",
     {
         "StatelessRules": Sequence[StatelessRuleTypeDef],
     },
 )
 _OptionalStatelessRulesAndCustomActionsTypeDef = TypedDict(
@@ -1427,15 +1674,15 @@
 
 DescribeFirewallPolicyResponseTypeDef = TypedDict(
     "DescribeFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
         "FirewallPolicy": FirewallPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyRequestRequestTypeDef",
     {
         "UpdateToken": str,
@@ -1525,15 +1772,15 @@
 
 DescribeRuleGroupResponseTypeDef = TypedDict(
     "DescribeRuleGroupResponseTypeDef",
     {
         "UpdateToken": str,
         "RuleGroup": RuleGroupTypeDef,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "UpdateToken": str,
```

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/type_defs.pyi` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -46,66 +46,77 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddressTypeDef",
     "AssociateFirewallPolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateFirewallPolicyResponseTypeDef",
     "SubnetMappingTypeDef",
     "AttachmentTypeDef",
     "IPSetMetadataTypeDef",
     "EncryptionConfigurationTypeDef",
     "TagTypeDef",
     "SourceMetadataTypeDef",
     "DeleteFirewallPolicyRequestRequestTypeDef",
     "DeleteFirewallRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
+    "DeleteTLSInspectionConfigurationRequestRequestTypeDef",
     "DescribeFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallRequestRequestTypeDef",
     "DescribeLoggingConfigurationRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
     "StatefulRuleOptionsTypeDef",
     "DescribeRuleGroupRequestRequestTypeDef",
+    "DescribeTLSInspectionConfigurationRequestRequestTypeDef",
     "DimensionTypeDef",
     "DisassociateSubnetsRequestRequestTypeDef",
     "FirewallMetadataTypeDef",
     "FirewallPolicyMetadataTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupReferenceTypeDef",
     "HeaderTypeDef",
     "IPSetReferenceTypeDef",
     "IPSetTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
     "ListFirewallPoliciesRequestRequestTypeDef",
+    "ListFirewallsRequestListFirewallsPaginateTypeDef",
     "ListFirewallsRequestRequestTypeDef",
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupMetadataTypeDef",
+    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
+    "ListTLSInspectionConfigurationsRequestRequestTypeDef",
+    "TLSInspectionConfigurationMetadataTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "LogDestinationConfigTypeDef",
     "PortRangeTypeDef",
     "TCPFlagFieldTypeDef",
+    "PaginatorConfigTypeDef",
     "PerObjectStatusTypeDef",
     "PortSetTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RuleOptionTypeDef",
     "RulesSourceListTypeDef",
+    "ServerCertificateTypeDef",
     "StatefulRuleGroupOverrideTypeDef",
+    "TlsCertificateDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallDeleteProtectionRequestRequestTypeDef",
-    "UpdateFirewallDescriptionRequestRequestTypeDef",
-    "UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
-    "UpdateSubnetChangeProtectionRequestRequestTypeDef",
-    "AssociateFirewallPolicyResponseTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "UpdateFirewallDeleteProtectionResponseTypeDef",
+    "UpdateFirewallDescriptionRequestRequestTypeDef",
     "UpdateFirewallDescriptionResponseTypeDef",
+    "UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
     "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
+    "UpdateSubnetChangeProtectionRequestRequestTypeDef",
     "UpdateSubnetChangeProtectionResponseTypeDef",
     "AssociateSubnetsRequestRequestTypeDef",
     "AssociateSubnetsResponseTypeDef",
     "DisassociateSubnetsResponseTypeDef",
     "CIDRSummaryTypeDef",
     "UpdateFirewallEncryptionConfigurationRequestRequestTypeDef",
     "UpdateFirewallEncryptionConfigurationResponseTypeDef",
@@ -116,44 +127,52 @@
     "TagResourceRequestRequestTypeDef",
     "RuleGroupResponseTypeDef",
     "DescribeRuleGroupMetadataResponseTypeDef",
     "PublishMetricActionTypeDef",
     "ListFirewallsResponseTypeDef",
     "ListFirewallPoliciesResponseTypeDef",
     "ReferenceSetsTypeDef",
-    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
-    "ListFirewallsRequestListFirewallsPaginateTypeDef",
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "PolicyVariablesTypeDef",
     "ListRuleGroupsResponseTypeDef",
+    "ListTLSInspectionConfigurationsResponseTypeDef",
     "LoggingConfigurationTypeDef",
+    "ServerCertificateScopeTypeDef",
     "MatchAttributesTypeDef",
     "SyncStateTypeDef",
     "RuleVariablesTypeDef",
     "StatefulRuleTypeDef",
     "StatefulRuleGroupReferenceTypeDef",
+    "TLSInspectionConfigurationResponseTypeDef",
     "CapacityUsageSummaryTypeDef",
     "CreateFirewallPolicyResponseTypeDef",
     "DeleteFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "DeleteRuleGroupResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "ActionDefinitionTypeDef",
     "DescribeLoggingConfigurationResponseTypeDef",
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
+    "ServerCertificateConfigurationTypeDef",
     "RuleDefinitionTypeDef",
+    "CreateTLSInspectionConfigurationResponseTypeDef",
+    "DeleteTLSInspectionConfigurationResponseTypeDef",
+    "UpdateTLSInspectionConfigurationResponseTypeDef",
     "FirewallStatusTypeDef",
     "CustomActionTypeDef",
+    "TLSInspectionConfigurationTypeDef",
     "StatelessRuleTypeDef",
     "CreateFirewallResponseTypeDef",
     "DeleteFirewallResponseTypeDef",
     "DescribeFirewallResponseTypeDef",
     "FirewallPolicyTypeDef",
+    "CreateTLSInspectionConfigurationRequestRequestTypeDef",
+    "DescribeTLSInspectionConfigurationResponseTypeDef",
+    "UpdateTLSInspectionConfigurationRequestRequestTypeDef",
     "StatelessRulesAndCustomActionsTypeDef",
     "CreateFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyRequestRequestTypeDef",
     "RulesSourceTypeDef",
     "RuleGroupTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
@@ -186,22 +205,22 @@
 
 class AssociateFirewallPolicyRequestRequestTypeDef(
     _RequiredAssociateFirewallPolicyRequestRequestTypeDef,
     _OptionalAssociateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateFirewallPolicyResponseTypeDef = TypedDict(
+    "AssociateFirewallPolicyResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "FirewallArn": str,
+        "FirewallName": str,
+        "FirewallPolicyArn": str,
+        "UpdateToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSubnetMappingTypeDef = TypedDict(
     "_RequiredSubnetMappingTypeDef",
     {
         "SubnetId": str,
@@ -304,14 +323,23 @@
         "RuleGroupName": str,
         "RuleGroupArn": str,
         "Type": RuleGroupTypeType,
     },
     total=False,
 )
 
+DeleteTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "DeleteTLSInspectionConfigurationRequestRequestTypeDef",
+    {
+        "TLSInspectionConfigurationArn": str,
+        "TLSInspectionConfigurationName": str,
+    },
+    total=False,
+)
+
 DescribeFirewallPolicyRequestRequestTypeDef = TypedDict(
     "DescribeFirewallPolicyRequestRequestTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicyArn": str,
     },
     total=False,
@@ -338,14 +366,22 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeRuleGroupMetadataRequestRequestTypeDef = TypedDict(
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
     {
         "RuleGroupName": str,
         "RuleGroupArn": str,
         "Type": RuleGroupTypeType,
     },
@@ -366,14 +402,23 @@
         "RuleGroupName": str,
         "RuleGroupArn": str,
         "Type": RuleGroupTypeType,
     },
     total=False,
 )
 
+DescribeTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "DescribeTLSInspectionConfigurationRequestRequestTypeDef",
+    {
+        "TLSInspectionConfigurationArn": str,
+        "TLSInspectionConfigurationName": str,
+    },
+    total=False,
+)
+
 DimensionTypeDef = TypedDict(
     "DimensionTypeDef",
     {
         "Value": str,
     },
 )
 
@@ -457,43 +502,61 @@
 IPSetTypeDef = TypedDict(
     "IPSetTypeDef",
     {
         "Definition": Sequence[str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = TypedDict(
+    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "ListFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListFirewallsRequestListFirewallsPaginateTypeDef = TypedDict(
+    "ListFirewallsRequestListFirewallsPaginateTypeDef",
+    {
+        "VpcIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFirewallsRequestRequestTypeDef = TypedDict(
     "ListFirewallsRequestRequestTypeDef",
     {
         "NextToken": str,
         "VpcIds": Sequence[str],
         "MaxResults": int,
     },
     total=False,
 )
 
+ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    {
+        "Scope": ResourceManagedStatusType,
+        "ManagedType": ResourceManagedTypeType,
+        "Type": RuleGroupTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Scope": ResourceManagedStatusType,
         "ManagedType": ResourceManagedTypeType,
@@ -507,14 +570,60 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
+ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef = TypedDict(
+    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListTLSInspectionConfigurationsRequestRequestTypeDef = TypedDict(
+    "ListTLSInspectionConfigurationsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+TLSInspectionConfigurationMetadataTypeDef = TypedDict(
+    "TLSInspectionConfigurationMetadataTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -562,14 +671,24 @@
     },
     total=False,
 )
 
 class TCPFlagFieldTypeDef(_RequiredTCPFlagFieldTypeDef, _OptionalTCPFlagFieldTypeDef):
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
 PerObjectStatusTypeDef = TypedDict(
     "PerObjectStatusTypeDef",
     {
         "SyncStatus": PerObjectSyncStatusType,
         "UpdateToken": str,
     },
     total=False,
@@ -587,14 +706,25 @@
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
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
 _RequiredRuleOptionTypeDef = TypedDict(
     "_RequiredRuleOptionTypeDef",
     {
         "Keyword": str,
     },
 )
 _OptionalRuleOptionTypeDef = TypedDict(
@@ -613,22 +743,41 @@
     {
         "Targets": Sequence[str],
         "TargetTypes": Sequence[TargetTypeType],
         "GeneratedRulesType": GeneratedRulesTypeType,
     },
 )
 
+ServerCertificateTypeDef = TypedDict(
+    "ServerCertificateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+    total=False,
+)
+
 StatefulRuleGroupOverrideTypeDef = TypedDict(
     "StatefulRuleGroupOverrideTypeDef",
     {
         "Action": Literal["DROP_TO_ALERT"],
     },
     total=False,
 )
 
+TlsCertificateDataTypeDef = TypedDict(
+    "TlsCertificateDataTypeDef",
+    {
+        "CertificateArn": str,
+        "CertificateSerial": str,
+        "Status": str,
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -651,25 +800,47 @@
 
 class UpdateFirewallDeleteProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallDeleteProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallDeleteProtectionRequestRequestTypeDef,
 ):
     pass
 
+UpdateFirewallDeleteProtectionResponseTypeDef = TypedDict(
+    "UpdateFirewallDeleteProtectionResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "DeleteProtection": bool,
+        "UpdateToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateFirewallDescriptionRequestRequestTypeDef = TypedDict(
     "UpdateFirewallDescriptionRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "Description": str,
     },
     total=False,
 )
 
+UpdateFirewallDescriptionResponseTypeDef = TypedDict(
+    "UpdateFirewallDescriptionResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "Description": str,
+        "UpdateToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
     {
         "FirewallPolicyChangeProtection": bool,
     },
 )
 _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -684,14 +855,25 @@
 
 class UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
+UpdateFirewallPolicyChangeProtectionResponseTypeDef = TypedDict(
+    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "FirewallArn": str,
+        "FirewallName": str,
+        "FirewallPolicyChangeProtection": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef",
     {
         "SubnetChangeProtection": bool,
     },
 )
 _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -706,74 +888,22 @@
 
 class UpdateSubnetChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
-AssociateFirewallPolicyResponseTypeDef = TypedDict(
-    "AssociateFirewallPolicyResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "FirewallPolicyArn": str,
-        "UpdateToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFirewallDeleteProtectionResponseTypeDef = TypedDict(
-    "UpdateFirewallDeleteProtectionResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "DeleteProtection": bool,
-        "UpdateToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFirewallDescriptionResponseTypeDef = TypedDict(
-    "UpdateFirewallDescriptionResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "Description": str,
-        "UpdateToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFirewallPolicyChangeProtectionResponseTypeDef = TypedDict(
-    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "FirewallArn": str,
-        "FirewallName": str,
-        "FirewallPolicyChangeProtection": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateSubnetChangeProtectionResponseTypeDef = TypedDict(
     "UpdateSubnetChangeProtectionResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetChangeProtection": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAssociateSubnetsRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateSubnetsRequestRequestTypeDef",
     {
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
@@ -797,26 +927,26 @@
 AssociateSubnetsResponseTypeDef = TypedDict(
     "AssociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateSubnetsResponseTypeDef = TypedDict(
     "DisassociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CIDRSummaryTypeDef = TypedDict(
     "CIDRSummaryTypeDef",
     {
         "AvailableCIDRCount": int,
@@ -840,15 +970,15 @@
 UpdateFirewallEncryptionConfigurationResponseTypeDef = TypedDict(
     "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "UpdateToken": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFirewallRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRequestRequestTypeDef",
     {
         "FirewallName": str,
@@ -931,15 +1061,15 @@
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextToken": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -984,15 +1114,15 @@
         "RuleGroupArn": str,
         "RuleGroupName": str,
         "Description": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
         "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
         "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PublishMetricActionTypeDef = TypedDict(
     "PublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
@@ -1000,99 +1130,80 @@
 )
 
 ListFirewallsResponseTypeDef = TypedDict(
     "ListFirewallsResponseTypeDef",
     {
         "NextToken": str,
         "Firewalls": List[FirewallMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFirewallPoliciesResponseTypeDef = TypedDict(
     "ListFirewallPoliciesResponseTypeDef",
     {
         "NextToken": str,
         "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReferenceSetsTypeDef = TypedDict(
     "ReferenceSetsTypeDef",
     {
         "IPSetReferences": Mapping[str, IPSetReferenceTypeDef],
     },
     total=False,
 )
 
-ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = TypedDict(
-    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFirewallsRequestListFirewallsPaginateTypeDef = TypedDict(
-    "ListFirewallsRequestListFirewallsPaginateTypeDef",
+PolicyVariablesTypeDef = TypedDict(
+    "PolicyVariablesTypeDef",
     {
-        "VpcIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "RuleVariables": Mapping[str, IPSetTypeDef],
     },
     total=False,
 )
 
-ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+ListRuleGroupsResponseTypeDef = TypedDict(
+    "ListRuleGroupsResponseTypeDef",
     {
-        "Scope": ResourceManagedStatusType,
-        "ManagedType": ResourceManagedTypeType,
-        "Type": RuleGroupTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "RuleGroups": List[RuleGroupMetadataTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-ListRuleGroupsResponseTypeDef = TypedDict(
-    "ListRuleGroupsResponseTypeDef",
+ListTLSInspectionConfigurationsResponseTypeDef = TypedDict(
+    "ListTLSInspectionConfigurationsResponseTypeDef",
     {
         "NextToken": str,
-        "RuleGroups": List[RuleGroupMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TLSInspectionConfigurations": List[TLSInspectionConfigurationMetadataTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "LogDestinationConfigs": List[LogDestinationConfigTypeDef],
     },
 )
 
+ServerCertificateScopeTypeDef = TypedDict(
+    "ServerCertificateScopeTypeDef",
+    {
+        "Sources": Sequence[AddressTypeDef],
+        "Destinations": Sequence[AddressTypeDef],
+        "SourcePorts": Sequence[PortRangeTypeDef],
+        "DestinationPorts": Sequence[PortRangeTypeDef],
+        "Protocols": Sequence[int],
+    },
+    total=False,
+)
+
 MatchAttributesTypeDef = TypedDict(
     "MatchAttributesTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
@@ -1145,71 +1256,99 @@
 )
 
 class StatefulRuleGroupReferenceTypeDef(
     _RequiredStatefulRuleGroupReferenceTypeDef, _OptionalStatefulRuleGroupReferenceTypeDef
 ):
     pass
 
+_RequiredTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "_RequiredTLSInspectionConfigurationResponseTypeDef",
+    {
+        "TLSInspectionConfigurationArn": str,
+        "TLSInspectionConfigurationName": str,
+        "TLSInspectionConfigurationId": str,
+    },
+)
+_OptionalTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "_OptionalTLSInspectionConfigurationResponseTypeDef",
+    {
+        "TLSInspectionConfigurationStatus": ResourceStatusType,
+        "Description": str,
+        "Tags": List[TagTypeDef],
+        "LastModifiedTime": datetime,
+        "NumberOfAssociations": int,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "Certificates": List[TlsCertificateDataTypeDef],
+    },
+    total=False,
+)
+
+class TLSInspectionConfigurationResponseTypeDef(
+    _RequiredTLSInspectionConfigurationResponseTypeDef,
+    _OptionalTLSInspectionConfigurationResponseTypeDef,
+):
+    pass
+
 CapacityUsageSummaryTypeDef = TypedDict(
     "CapacityUsageSummaryTypeDef",
     {
         "CIDRs": CIDRSummaryTypeDef,
     },
     total=False,
 )
 
 CreateFirewallPolicyResponseTypeDef = TypedDict(
     "CreateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteFirewallPolicyResponseTypeDef = TypedDict(
     "DeleteFirewallPolicyResponseTypeDef",
     {
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFirewallPolicyResponseTypeDef = TypedDict(
     "UpdateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "UpdateToken": str,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRuleGroupResponseTypeDef = TypedDict(
     "DeleteRuleGroupResponseTypeDef",
     {
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRuleGroupResponseTypeDef = TypedDict(
     "UpdateRuleGroupResponseTypeDef",
     {
         "UpdateToken": str,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActionDefinitionTypeDef = TypedDict(
     "ActionDefinitionTypeDef",
     {
         "PublishMetricAction": PublishMetricActionTypeDef,
@@ -1218,15 +1357,15 @@
 )
 
 DescribeLoggingConfigurationResponseTypeDef = TypedDict(
     "DescribeLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "FirewallArn": str,
@@ -1238,26 +1377,61 @@
 
 UpdateLoggingConfigurationResponseTypeDef = TypedDict(
     "UpdateLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ServerCertificateConfigurationTypeDef = TypedDict(
+    "ServerCertificateConfigurationTypeDef",
+    {
+        "ServerCertificates": Sequence[ServerCertificateTypeDef],
+        "Scopes": Sequence[ServerCertificateScopeTypeDef],
     },
+    total=False,
 )
 
 RuleDefinitionTypeDef = TypedDict(
     "RuleDefinitionTypeDef",
     {
         "MatchAttributes": MatchAttributesTypeDef,
         "Actions": Sequence[str],
     },
 )
 
+CreateTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "CreateTLSInspectionConfigurationResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "DeleteTLSInspectionConfigurationResponseTypeDef",
+    {
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "UpdateTLSInspectionConfigurationResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFirewallStatusTypeDef = TypedDict(
     "_RequiredFirewallStatusTypeDef",
     {
         "Status": FirewallStatusValueType,
         "ConfigurationSyncStateSummary": ConfigurationSyncStateType,
     },
 )
@@ -1277,47 +1451,55 @@
     "CustomActionTypeDef",
     {
         "ActionName": str,
         "ActionDefinition": ActionDefinitionTypeDef,
     },
 )
 
+TLSInspectionConfigurationTypeDef = TypedDict(
+    "TLSInspectionConfigurationTypeDef",
+    {
+        "ServerCertificateConfigurations": Sequence[ServerCertificateConfigurationTypeDef],
+    },
+    total=False,
+)
+
 StatelessRuleTypeDef = TypedDict(
     "StatelessRuleTypeDef",
     {
         "RuleDefinition": RuleDefinitionTypeDef,
         "Priority": int,
     },
 )
 
 CreateFirewallResponseTypeDef = TypedDict(
     "CreateFirewallResponseTypeDef",
     {
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteFirewallResponseTypeDef = TypedDict(
     "DeleteFirewallResponseTypeDef",
     {
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFirewallResponseTypeDef = TypedDict(
     "DescribeFirewallResponseTypeDef",
     {
         "UpdateToken": str,
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFirewallPolicyTypeDef = TypedDict(
     "_RequiredFirewallPolicyTypeDef",
     {
         "StatelessDefaultActions": Sequence[str],
@@ -1328,21 +1510,80 @@
     "_OptionalFirewallPolicyTypeDef",
     {
         "StatelessRuleGroupReferences": Sequence[StatelessRuleGroupReferenceTypeDef],
         "StatelessCustomActions": Sequence[CustomActionTypeDef],
         "StatefulRuleGroupReferences": Sequence[StatefulRuleGroupReferenceTypeDef],
         "StatefulDefaultActions": Sequence[str],
         "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
+        "TLSInspectionConfigurationArn": str,
+        "PolicyVariables": PolicyVariablesTypeDef,
     },
     total=False,
 )
 
 class FirewallPolicyTypeDef(_RequiredFirewallPolicyTypeDef, _OptionalFirewallPolicyTypeDef):
     pass
 
+_RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef",
+    {
+        "TLSInspectionConfigurationName": str,
+        "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
+    },
+)
+_OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class CreateTLSInspectionConfigurationRequestRequestTypeDef(
+    _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef,
+    _OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef,
+):
+    pass
+
+DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "DescribeTLSInspectionConfigurationResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef",
+    {
+        "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
+        "UpdateToken": str,
+    },
+)
+_OptionalUpdateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTLSInspectionConfigurationRequestRequestTypeDef",
+    {
+        "TLSInspectionConfigurationArn": str,
+        "TLSInspectionConfigurationName": str,
+        "Description": str,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateTLSInspectionConfigurationRequestRequestTypeDef(
+    _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef,
+    _OptionalUpdateTLSInspectionConfigurationRequestRequestTypeDef,
+):
+    pass
+
 _RequiredStatelessRulesAndCustomActionsTypeDef = TypedDict(
     "_RequiredStatelessRulesAndCustomActionsTypeDef",
     {
         "StatelessRules": Sequence[StatelessRuleTypeDef],
     },
 )
 _OptionalStatelessRulesAndCustomActionsTypeDef = TypedDict(
@@ -1384,15 +1625,15 @@
 
 DescribeFirewallPolicyResponseTypeDef = TypedDict(
     "DescribeFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
         "FirewallPolicy": FirewallPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyRequestRequestTypeDef",
     {
         "UpdateToken": str,
@@ -1476,15 +1717,15 @@
 
 DescribeRuleGroupResponseTypeDef = TypedDict(
     "DescribeRuleGroupResponseTypeDef",
     {
         "UpdateToken": str,
         "RuleGroup": RuleGroupTypeDef,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "UpdateToken": str,
```

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/PKG-INFO` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-network-firewall
-Version: 1.26.51
-Summary: Type annotations for boto3.NetworkFirewall 1.26.51 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.NetworkFirewall 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-network-firewall"></a>
 
 # mypy-boto3-network-firewall
 
 [![PyPI - mypy-boto3-network-firewall](https://img.shields.io/pypi/v/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-network-firewall?color=blue)](https://pypistats.org/packages/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.26.51](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,26 +284,30 @@
 from boto3.session import Session
 
 from mypy_boto3_network_firewall import NetworkFirewallClient
 from mypy_boto3_network_firewall.paginator import (
     ListFirewallPoliciesPaginator,
     ListFirewallsPaginator,
     ListRuleGroupsPaginator,
+    ListTLSInspectionConfigurationsPaginator,
     ListTagsForResourcePaginator,
 )
 
 client: NetworkFirewallClient = Session().client("network-firewall")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_firewall_policies_paginator: ListFirewallPoliciesPaginator = client.get_paginator(
     "list_firewall_policies"
 )
 list_firewalls_paginator: ListFirewallsPaginator = client.get_paginator("list_firewalls")
 list_rule_groups_paginator: ListRuleGroupsPaginator = client.get_paginator("list_rule_groups")
+list_tls_inspection_configurations_paginator: ListTLSInspectionConfigurationsPaginator = (
+    client.get_paginator("list_tls_inspection_configurations")
+)
 list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator(
     "list_tags_for_resource"
 )
 ```
 
 <a id="literals"></a>
 
@@ -319,14 +323,15 @@
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
     IPAddressTypeType,
     ListFirewallPoliciesPaginatorName,
     ListFirewallsPaginatorName,
     ListRuleGroupsPaginatorName,
+    ListTLSInspectionConfigurationsPaginatorName,
     ListTagsForResourcePaginatorName,
     LogDestinationTypeType,
     LogTypeType,
     OverrideActionType,
     PerObjectSyncStatusType,
     ResourceManagedStatusType,
     ResourceManagedTypeType,
@@ -358,66 +363,77 @@
 `mypy_boto3_network_firewall.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_network_firewall.type_defs import (
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateFirewallPolicyResponseTypeDef,
     SubnetMappingTypeDef,
     AttachmentTypeDef,
     IPSetMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     TagTypeDef,
     SourceMetadataTypeDef,
     DeleteFirewallPolicyRequestRequestTypeDef,
     DeleteFirewallRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
+    DeleteTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallRequestRequestTypeDef,
     DescribeLoggingConfigurationRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataRequestRequestTypeDef,
     StatefulRuleOptionsTypeDef,
     DescribeRuleGroupRequestRequestTypeDef,
+    DescribeTLSInspectionConfigurationRequestRequestTypeDef,
     DimensionTypeDef,
     DisassociateSubnetsRequestRequestTypeDef,
     FirewallMetadataTypeDef,
     FirewallPolicyMetadataTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupReferenceTypeDef,
     HeaderTypeDef,
     IPSetReferenceTypeDef,
     IPSetTypeDef,
-    PaginatorConfigTypeDef,
+    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
     ListFirewallPoliciesRequestRequestTypeDef,
+    ListFirewallsRequestListFirewallsPaginateTypeDef,
     ListFirewallsRequestRequestTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupMetadataTypeDef,
+    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
+    ListTLSInspectionConfigurationsRequestRequestTypeDef,
+    TLSInspectionConfigurationMetadataTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     LogDestinationConfigTypeDef,
     PortRangeTypeDef,
     TCPFlagFieldTypeDef,
+    PaginatorConfigTypeDef,
     PerObjectStatusTypeDef,
     PortSetTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RuleOptionTypeDef,
     RulesSourceListTypeDef,
+    ServerCertificateTypeDef,
     StatefulRuleGroupOverrideTypeDef,
+    TlsCertificateDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionRequestRequestTypeDef,
-    UpdateFirewallDescriptionRequestRequestTypeDef,
-    UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
-    UpdateSubnetChangeProtectionRequestRequestTypeDef,
-    AssociateFirewallPolicyResponseTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
+    UpdateFirewallDescriptionRequestRequestTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
+    UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
+    UpdateSubnetChangeProtectionRequestRequestTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
     AssociateSubnetsRequestRequestTypeDef,
     AssociateSubnetsResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     CIDRSummaryTypeDef,
     UpdateFirewallEncryptionConfigurationRequestRequestTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
@@ -428,44 +444,52 @@
     TagResourceRequestRequestTypeDef,
     RuleGroupResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     PublishMetricActionTypeDef,
     ListFirewallsResponseTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ReferenceSetsTypeDef,
-    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
-    ListFirewallsRequestListFirewallsPaginateTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    PolicyVariablesTypeDef,
     ListRuleGroupsResponseTypeDef,
+    ListTLSInspectionConfigurationsResponseTypeDef,
     LoggingConfigurationTypeDef,
+    ServerCertificateScopeTypeDef,
     MatchAttributesTypeDef,
     SyncStateTypeDef,
     RuleVariablesTypeDef,
     StatefulRuleTypeDef,
     StatefulRuleGroupReferenceTypeDef,
+    TLSInspectionConfigurationResponseTypeDef,
     CapacityUsageSummaryTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     DeleteRuleGroupResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    ServerCertificateConfigurationTypeDef,
     RuleDefinitionTypeDef,
+    CreateTLSInspectionConfigurationResponseTypeDef,
+    DeleteTLSInspectionConfigurationResponseTypeDef,
+    UpdateTLSInspectionConfigurationResponseTypeDef,
     FirewallStatusTypeDef,
     CustomActionTypeDef,
+    TLSInspectionConfigurationTypeDef,
     StatelessRuleTypeDef,
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
     FirewallPolicyTypeDef,
+    CreateTLSInspectionConfigurationRequestRequestTypeDef,
+    DescribeTLSInspectionConfigurationResponseTypeDef,
+    UpdateTLSInspectionConfigurationRequestRequestTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
     CreateFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
     RulesSourceTypeDef,
     RuleGroupTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
@@ -481,42 +505,42 @@
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

### Comparing `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/SOURCES.txt` & `mypy-boto3-network-firewall-1.27.0/mypy_boto3_network_firewall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.26.51/setup.py` & `mypy-boto3-network-firewall-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-network-firewall.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-network-firewall",
-    version="1.26.51",
+    version="1.27.0",
     packages=["mypy_boto3_network_firewall"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.NetworkFirewall 1.26.51 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.NetworkFirewall 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/",
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


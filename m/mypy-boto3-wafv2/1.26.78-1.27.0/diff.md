# Comparing `tmp/mypy-boto3-wafv2-1.26.78.tar.gz` & `tmp/mypy-boto3-wafv2-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wafv2-1.26.78.tar", last modified: Thu Feb 23 20:34:58 2023, max compression
+gzip compressed data, was "mypy-boto3-wafv2-1.27.0.tar", last modified: Mon Jul  3 19:51:35 2023, max compression
```

## Comparing `mypy-boto3-wafv2-1.26.78.tar` & `mypy-boto3-wafv2-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:58.732411 mypy-boto3-wafv2-1.26.78/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-02-23 20:34:58.732411 mypy-boto3-wafv2-1.26.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:58.732411 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33744 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33690 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-02-23 20:34:46.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-02-23 20:34:46.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60400 2023-02-23 20:34:47.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60325 2023-02-23 20:34:47.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:58.732411 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-02-23 20:34:58.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-23 20:34:58.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:58.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:58.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 20:34:58.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-23 20:34:58.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 20:34:58.732411 mypy-boto3-wafv2-1.26.78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.892138 mypy-boto3-wafv2-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-07-03 19:51:35.892138 mypy-boto3-wafv2-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.880138 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36893 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68373 2023-07-03 19:49:38.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68292 2023-07-03 19:49:37.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.892138 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-07-03 19:51:35.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-03 19:51:35.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:35.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 19:51:35.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:35.892138 mypy-boto3-wafv2-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 19:49:35.000000 mypy-boto3-wafv2-1.27.0/setup.py
```

### Comparing `mypy-boto3-wafv2-1.26.78/LICENSE` & `mypy-boto3-wafv2-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-wafv2-1.26.78/PKG-INFO` & `mypy-boto3-wafv2-1.27.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.26.78
-Summary: Type annotations for boto3.WAFV2 1.26.78 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.WAFV2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-wafv2"></a>
 
 # mypy-boto3-wafv2
 
 [![PyPI - mypy-boto3-wafv2](https://img.shields.io/pypi/v/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wafv2?color=blue)](https://pypistats.org/packages/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -276,14 +276,15 @@
 
 `mypy_boto3_wafv2.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_wafv2.literals import (
     ActionValueType,
+    AssociatedResourceTypeType,
     BodyParsingFallbackBehaviorType,
     ComparisonOperatorType,
     CountryCodeType,
     FailureReasonType,
     FallbackBehaviorType,
     FilterBehaviorType,
     FilterRequirementType,
@@ -298,14 +299,15 @@
     PlatformType,
     PositionalConstraintType,
     RateBasedStatementAggregateKeyTypeType,
     ResourceTypeType,
     ResponseContentTypeType,
     ScopeType,
     SensitivityLevelType,
+    SizeInspectionLimitType,
     TextTransformationTypeType,
     WAFV2ServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
@@ -319,111 +321,132 @@
 ### Typed dictionaries
 
 `mypy_boto3_wafv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_wafv2.type_defs import (
+    APIKeySummaryTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
     ActionConditionTypeDef,
+    AddressFieldTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
+    RequestBodyAssociatedResourceTypeConfigTypeDef,
     BodyTypeDef,
     TextTransformationTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
-    ResponseMetadataTypeDef,
+    CheckCapacityResponseTypeDef,
     LabelNameConditionTypeDef,
     CookieMatchPatternTypeDef,
+    CreateAPIKeyRequestRequestTypeDef,
+    CreateAPIKeyResponseTypeDef,
     TagTypeDef,
     IPSetSummaryTypeDef,
     RegexTypeDef,
     RegexPatternSetSummaryTypeDef,
     CustomResponseBodyTypeDef,
     VisibilityConfigTypeDef,
     RuleGroupSummaryTypeDef,
     WebACLSummaryTypeDef,
     CustomHTTPHeaderTypeDef,
     DeleteFirewallManagerRuleGroupsRequestRequestTypeDef,
+    DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
+    DescribeAllManagedProductsRequestRequestTypeDef,
+    ManagedProductDescriptorTypeDef,
+    DescribeManagedProductsByVendorRequestRequestTypeDef,
     DescribeManagedRuleGroupRequestRequestTypeDef,
     LabelSummaryTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
+    EmailFieldTypeDef,
     ExcludedRuleTypeDef,
+    HeaderOrderTypeDef,
     SingleHeaderTypeDef,
     SingleQueryArgumentTypeDef,
     ForwardedIPConfigTypeDef,
     GenerateMobileSdkReleaseUrlRequestRequestTypeDef,
+    GenerateMobileSdkReleaseUrlResponseTypeDef,
+    GetDecryptedAPIKeyRequestRequestTypeDef,
+    GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetRequestRequestTypeDef,
     IPSetTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetManagedRuleSetRequestRequestTypeDef,
     GetMobileSdkReleaseRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
+    GetPermissionPolicyResponseTypeDef,
     GetRateBasedStatementManagedKeysRequestRequestTypeDef,
     RateBasedStatementManagedKeysIPSetTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     TimeWindowTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     HeaderMatchPatternTypeDef,
     IPSetForwardedIPConfigTypeDef,
     JsonMatchPatternTypeDef,
     LabelMatchStatementTypeDef,
     LabelTypeDef,
+    ListAPIKeysRequestRequestTypeDef,
     ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     ManagedRuleGroupVersionTypeDef,
     ListAvailableManagedRuleGroupsRequestRequestTypeDef,
     ManagedRuleGroupSummaryTypeDef,
     ListIPSetsRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListManagedRuleSetsRequestRequestTypeDef,
     ManagedRuleSetSummaryTypeDef,
     ListMobileSdkReleasesRequestRequestTypeDef,
     ReleaseSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
+    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     PasswordFieldTypeDef,
     UsernameFieldTypeDef,
     ManagedRuleSetVersionTypeDef,
     NotStatementTypeDef,
     OrStatementTypeDef,
+    PhoneNumberFieldTypeDef,
     VersionToPublishTypeDef,
+    PutManagedRuleSetVersionsResponseTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
+    RateLimitLabelNamespaceTypeDef,
     ResponseInspectionBodyContainsTypeDef,
     ResponseInspectionHeaderTypeDef,
     ResponseInspectionJsonTypeDef,
     ResponseInspectionStatusCodeTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
-    CaptchaConfigTypeDef,
-    ChallengeConfigTypeDef,
-    CheckCapacityResponseTypeDef,
-    DeleteFirewallManagerRuleGroupsResponseTypeDef,
-    GenerateMobileSdkReleaseUrlResponseTypeDef,
-    GetPermissionPolicyResponseTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
-    PutManagedRuleSetVersionsResponseTypeDef,
     UpdateIPSetResponseTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
+    ListAPIKeysResponseTypeDef,
+    AssociationConfigTypeDef,
+    RateLimitCookieTypeDef,
+    RateLimitHeaderTypeDef,
+    RateLimitQueryArgumentTypeDef,
+    RateLimitQueryStringTypeDef,
+    CaptchaConfigTypeDef,
+    ChallengeConfigTypeDef,
     ConditionTypeDef,
     CookiesTypeDef,
     CreateIPSetRequestRequestTypeDef,
     MobileSdkReleaseTypeDef,
     TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIPSetResponseTypeDef,
@@ -435,44 +458,49 @@
     ListRegexPatternSetsResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     CreateWebACLResponseTypeDef,
     ListWebACLsResponseTypeDef,
     CustomRequestHandlingTypeDef,
     CustomResponseTypeDef,
+    DescribeAllManagedProductsResponseTypeDef,
+    DescribeManagedProductsByVendorResponseTypeDef,
     GeoMatchStatementTypeDef,
-    RateBasedStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
     GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     HeadersTypeDef,
     IPSetReferenceStatementTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
+    RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
     ResponseInspectionTypeDef,
+    RateBasedStatementCustomKeyTypeDef,
     FilterTypeDef,
     GetMobileSdkReleaseResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     AllowActionTypeDef,
     CaptchaActionTypeDef,
     ChallengeActionTypeDef,
     CountActionTypeDef,
     BlockActionTypeDef,
     SampledHTTPRequestTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
+    AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
+    RateBasedStatementTypeDef,
     LoggingFilterTypeDef,
     OverrideActionTypeDef,
     DefaultActionTypeDef,
     RuleActionTypeDef,
     GetSampledRequestsResponseTypeDef,
     ByteMatchStatementTypeDef,
     RegexMatchStatementTypeDef,
@@ -504,53 +532,53 @@
     FirewallManagerRuleGroupTypeDef,
     WebACLTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
 )
 
 
-def get_structure() -> AWSManagedRulesBotControlRuleSetTypeDef:
+def get_structure() -> APIKeySummaryTypeDef:
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

### Comparing `mypy-boto3-wafv2-1.26.78/README.md` & `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-wafv2
+Version: 1.27.0
+Summary: Type annotations for boto3.WAFV2 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 wafv2 type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-wafv2"></a>
 
 # mypy-boto3-wafv2
 
 [![PyPI - mypy-boto3-wafv2](https://img.shields.io/pypi/v/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wafv2?color=blue)](https://pypistats.org/packages/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -244,14 +276,15 @@
 
 `mypy_boto3_wafv2.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_wafv2.literals import (
     ActionValueType,
+    AssociatedResourceTypeType,
     BodyParsingFallbackBehaviorType,
     ComparisonOperatorType,
     CountryCodeType,
     FailureReasonType,
     FallbackBehaviorType,
     FilterBehaviorType,
     FilterRequirementType,
@@ -266,14 +299,15 @@
     PlatformType,
     PositionalConstraintType,
     RateBasedStatementAggregateKeyTypeType,
     ResourceTypeType,
     ResponseContentTypeType,
     ScopeType,
     SensitivityLevelType,
+    SizeInspectionLimitType,
     TextTransformationTypeType,
     WAFV2ServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
@@ -287,111 +321,132 @@
 ### Typed dictionaries
 
 `mypy_boto3_wafv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_wafv2.type_defs import (
+    APIKeySummaryTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
     ActionConditionTypeDef,
+    AddressFieldTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
+    RequestBodyAssociatedResourceTypeConfigTypeDef,
     BodyTypeDef,
     TextTransformationTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
-    ResponseMetadataTypeDef,
+    CheckCapacityResponseTypeDef,
     LabelNameConditionTypeDef,
     CookieMatchPatternTypeDef,
+    CreateAPIKeyRequestRequestTypeDef,
+    CreateAPIKeyResponseTypeDef,
     TagTypeDef,
     IPSetSummaryTypeDef,
     RegexTypeDef,
     RegexPatternSetSummaryTypeDef,
     CustomResponseBodyTypeDef,
     VisibilityConfigTypeDef,
     RuleGroupSummaryTypeDef,
     WebACLSummaryTypeDef,
     CustomHTTPHeaderTypeDef,
     DeleteFirewallManagerRuleGroupsRequestRequestTypeDef,
+    DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
+    DescribeAllManagedProductsRequestRequestTypeDef,
+    ManagedProductDescriptorTypeDef,
+    DescribeManagedProductsByVendorRequestRequestTypeDef,
     DescribeManagedRuleGroupRequestRequestTypeDef,
     LabelSummaryTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
+    EmailFieldTypeDef,
     ExcludedRuleTypeDef,
+    HeaderOrderTypeDef,
     SingleHeaderTypeDef,
     SingleQueryArgumentTypeDef,
     ForwardedIPConfigTypeDef,
     GenerateMobileSdkReleaseUrlRequestRequestTypeDef,
+    GenerateMobileSdkReleaseUrlResponseTypeDef,
+    GetDecryptedAPIKeyRequestRequestTypeDef,
+    GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetRequestRequestTypeDef,
     IPSetTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetManagedRuleSetRequestRequestTypeDef,
     GetMobileSdkReleaseRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
+    GetPermissionPolicyResponseTypeDef,
     GetRateBasedStatementManagedKeysRequestRequestTypeDef,
     RateBasedStatementManagedKeysIPSetTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     TimeWindowTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     HeaderMatchPatternTypeDef,
     IPSetForwardedIPConfigTypeDef,
     JsonMatchPatternTypeDef,
     LabelMatchStatementTypeDef,
     LabelTypeDef,
+    ListAPIKeysRequestRequestTypeDef,
     ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     ManagedRuleGroupVersionTypeDef,
     ListAvailableManagedRuleGroupsRequestRequestTypeDef,
     ManagedRuleGroupSummaryTypeDef,
     ListIPSetsRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListManagedRuleSetsRequestRequestTypeDef,
     ManagedRuleSetSummaryTypeDef,
     ListMobileSdkReleasesRequestRequestTypeDef,
     ReleaseSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
+    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     PasswordFieldTypeDef,
     UsernameFieldTypeDef,
     ManagedRuleSetVersionTypeDef,
     NotStatementTypeDef,
     OrStatementTypeDef,
+    PhoneNumberFieldTypeDef,
     VersionToPublishTypeDef,
+    PutManagedRuleSetVersionsResponseTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
+    RateLimitLabelNamespaceTypeDef,
     ResponseInspectionBodyContainsTypeDef,
     ResponseInspectionHeaderTypeDef,
     ResponseInspectionJsonTypeDef,
     ResponseInspectionStatusCodeTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
-    CaptchaConfigTypeDef,
-    ChallengeConfigTypeDef,
-    CheckCapacityResponseTypeDef,
-    DeleteFirewallManagerRuleGroupsResponseTypeDef,
-    GenerateMobileSdkReleaseUrlResponseTypeDef,
-    GetPermissionPolicyResponseTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
-    PutManagedRuleSetVersionsResponseTypeDef,
     UpdateIPSetResponseTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
+    ListAPIKeysResponseTypeDef,
+    AssociationConfigTypeDef,
+    RateLimitCookieTypeDef,
+    RateLimitHeaderTypeDef,
+    RateLimitQueryArgumentTypeDef,
+    RateLimitQueryStringTypeDef,
+    CaptchaConfigTypeDef,
+    ChallengeConfigTypeDef,
     ConditionTypeDef,
     CookiesTypeDef,
     CreateIPSetRequestRequestTypeDef,
     MobileSdkReleaseTypeDef,
     TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIPSetResponseTypeDef,
@@ -403,44 +458,49 @@
     ListRegexPatternSetsResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     CreateWebACLResponseTypeDef,
     ListWebACLsResponseTypeDef,
     CustomRequestHandlingTypeDef,
     CustomResponseTypeDef,
+    DescribeAllManagedProductsResponseTypeDef,
+    DescribeManagedProductsByVendorResponseTypeDef,
     GeoMatchStatementTypeDef,
-    RateBasedStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
     GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     HeadersTypeDef,
     IPSetReferenceStatementTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
+    RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
     ResponseInspectionTypeDef,
+    RateBasedStatementCustomKeyTypeDef,
     FilterTypeDef,
     GetMobileSdkReleaseResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     AllowActionTypeDef,
     CaptchaActionTypeDef,
     ChallengeActionTypeDef,
     CountActionTypeDef,
     BlockActionTypeDef,
     SampledHTTPRequestTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
+    AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
+    RateBasedStatementTypeDef,
     LoggingFilterTypeDef,
     OverrideActionTypeDef,
     DefaultActionTypeDef,
     RuleActionTypeDef,
     GetSampledRequestsResponseTypeDef,
     ByteMatchStatementTypeDef,
     RegexMatchStatementTypeDef,
@@ -472,53 +532,53 @@
     FirewallManagerRuleGroupTypeDef,
     WebACLTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
 )
 
 
-def get_structure() -> AWSManagedRulesBotControlRuleSetTypeDef:
+def get_structure() -> APIKeySummaryTypeDef:
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

### Comparing `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/__main__.py` & `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFV2 1.26.78\nVersion:         1.26.78\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.WAFV2 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.78")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/client.py` & `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,37 +16,43 @@
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import IPAddressVersionType, PlatformType, ResourceTypeType, ScopeType
 from .type_defs import (
+    AssociationConfigTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
+    CreateAPIKeyResponseTypeDef,
     CreateIPSetResponseTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     CreateWebACLResponseTypeDef,
     CustomResponseBodyTypeDef,
     DefaultActionTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
+    DescribeAllManagedProductsResponseTypeDef,
+    DescribeManagedProductsByVendorResponseTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
+    GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetResponseTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     GetManagedRuleSetResponseTypeDef,
     GetMobileSdkReleaseResponseTypeDef,
     GetPermissionPolicyResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GetSampledRequestsResponseTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
+    ListAPIKeysResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListIPSetsResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
@@ -97,14 +103,15 @@
     WAFNonexistentItemException: Type[BotocoreClientError]
     WAFOptimisticLockException: Type[BotocoreClientError]
     WAFServiceLinkedRoleErrorException: Type[BotocoreClientError]
     WAFSubscriptionNotFoundException: Type[BotocoreClientError]
     WAFTagOperationException: Type[BotocoreClientError]
     WAFTagOperationInternalErrorException: Type[BotocoreClientError]
     WAFUnavailableEntityException: Type[BotocoreClientError]
+    WAFUnsupportedAggregateKeyTypeException: Type[BotocoreClientError]
 
 
 class WAFV2Client(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/)
     """
@@ -152,14 +159,24 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#close)
         """
 
+    def create_api_key(
+        self, *, Scope: ScopeType, TokenDomains: Sequence[str]
+    ) -> CreateAPIKeyResponseTypeDef:
+        """
+        Creates an API key that contains a set of token domains.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_api_key)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#create_api_key)
+        """
+
     def create_ip_set(
         self,
         *,
         Name: str,
         Scope: ScopeType,
         IPAddressVersion: IPAddressVersionType,
         Addresses: Sequence[str],
@@ -220,15 +237,16 @@
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
         Rules: Sequence[RuleTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
-        TokenDomains: Sequence[str] = ...
+        TokenDomains: Sequence[str] = ...,
+        AssociationConfig: AssociationConfigTypeDef = ...
     ) -> CreateWebACLResponseTypeDef:
         """
         Creates a  WebACL per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#create_web_acl)
         """
@@ -296,14 +314,36 @@
         """
         Deletes the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.delete_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#delete_web_acl)
         """
 
+    def describe_all_managed_products(
+        self, *, Scope: ScopeType
+    ) -> DescribeAllManagedProductsResponseTypeDef:
+        """
+        Provides high-level information for the Amazon Web Services Managed Rules rule
+        groups and Amazon Web Services Marketplace managed rule groups.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.describe_all_managed_products)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#describe_all_managed_products)
+        """
+
+    def describe_managed_products_by_vendor(
+        self, *, VendorName: str, Scope: ScopeType
+    ) -> DescribeManagedProductsByVendorResponseTypeDef:
+        """
+        Provides high-level information for the managed rule groups owned by a specific
+        vendor.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.describe_managed_products_by_vendor)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#describe_managed_products_by_vendor)
+        """
+
     def describe_managed_rule_group(
         self, *, VendorName: str, Name: str, Scope: ScopeType, VersionName: str = ...
     ) -> DescribeManagedRuleGroupResponseTypeDef:
         """
         Provides high-level information for a managed rule group, including descriptions
         of the rules.
 
@@ -340,14 +380,24 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#generate_presigned_url)
         """
 
+    def get_decrypted_api_key(
+        self, *, Scope: ScopeType, APIKey: str
+    ) -> GetDecryptedAPIKeyResponseTypeDef:
+        """
+        Returns your API key in decrypted form.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.get_decrypted_api_key)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#get_decrypted_api_key)
+        """
+
     def get_ip_set(self, *, Name: str, Scope: ScopeType, Id: str) -> GetIPSetResponseTypeDef:
         """
         Retrieves the specified  IPSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.get_ip_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#get_ip_set)
         """
@@ -397,15 +447,16 @@
         Scope: ScopeType,
         WebACLName: str,
         WebACLId: str,
         RuleName: str,
         RuleGroupRuleName: str = ...
     ) -> GetRateBasedStatementManagedKeysResponseTypeDef:
         """
-        Retrieves the keys that are currently blocked by a rate-based rule instance.
+        Retrieves the IP addresses that are currently blocked by a rate-based rule
+        instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.get_rate_based_statement_managed_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#get_rate_based_statement_managed_keys)
         """
 
     def get_regex_pattern_set(
         self, *, Name: str, Scope: ScopeType, Id: str
@@ -457,14 +508,24 @@
         """
         Retrieves the  WebACL for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.get_web_acl_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#get_web_acl_for_resource)
         """
 
+    def list_api_keys(
+        self, *, Scope: ScopeType, NextMarker: str = ..., Limit: int = ...
+    ) -> ListAPIKeysResponseTypeDef:
+        """
+        Retrieves a list of the API keys that you've defined for the specified scope.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.list_api_keys)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#list_api_keys)
+        """
+
     def list_available_managed_rule_group_versions(
         self,
         *,
         VendorName: str,
         Name: str,
         Scope: ScopeType,
         NextMarker: str = ...,
@@ -714,15 +775,16 @@
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
         Rules: Sequence[RuleTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
-        TokenDomains: Sequence[str] = ...
+        TokenDomains: Sequence[str] = ...,
+        AssociationConfig: AssociationConfigTypeDef = ...
     ) -> UpdateWebACLResponseTypeDef:
         """
         Updates the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#update_web_acl)
         """
```

### Comparing `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/client.pyi` & `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/client.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -16,37 +16,43 @@
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import IPAddressVersionType, PlatformType, ResourceTypeType, ScopeType
 from .type_defs import (
+    AssociationConfigTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
+    CreateAPIKeyResponseTypeDef,
     CreateIPSetResponseTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     CreateWebACLResponseTypeDef,
     CustomResponseBodyTypeDef,
     DefaultActionTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
+    DescribeAllManagedProductsResponseTypeDef,
+    DescribeManagedProductsByVendorResponseTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
+    GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetResponseTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     GetManagedRuleSetResponseTypeDef,
     GetMobileSdkReleaseResponseTypeDef,
     GetPermissionPolicyResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GetSampledRequestsResponseTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
+    ListAPIKeysResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListIPSetsResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
@@ -95,14 +101,15 @@
     WAFNonexistentItemException: Type[BotocoreClientError]
     WAFOptimisticLockException: Type[BotocoreClientError]
     WAFServiceLinkedRoleErrorException: Type[BotocoreClientError]
     WAFSubscriptionNotFoundException: Type[BotocoreClientError]
     WAFTagOperationException: Type[BotocoreClientError]
     WAFTagOperationInternalErrorException: Type[BotocoreClientError]
     WAFUnavailableEntityException: Type[BotocoreClientError]
+    WAFUnsupportedAggregateKeyTypeException: Type[BotocoreClientError]
 
 class WAFV2Client(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/)
     """
 
@@ -144,14 +151,23 @@
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#close)
         """
+    def create_api_key(
+        self, *, Scope: ScopeType, TokenDomains: Sequence[str]
+    ) -> CreateAPIKeyResponseTypeDef:
+        """
+        Creates an API key that contains a set of token domains.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_api_key)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#create_api_key)
+        """
     def create_ip_set(
         self,
         *,
         Name: str,
         Scope: ScopeType,
         IPAddressVersion: IPAddressVersionType,
         Addresses: Sequence[str],
@@ -209,15 +225,16 @@
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
         Rules: Sequence[RuleTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
-        TokenDomains: Sequence[str] = ...
+        TokenDomains: Sequence[str] = ...,
+        AssociationConfig: AssociationConfigTypeDef = ...
     ) -> CreateWebACLResponseTypeDef:
         """
         Creates a  WebACL per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#create_web_acl)
         """
@@ -277,14 +294,34 @@
     ) -> Dict[str, Any]:
         """
         Deletes the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.delete_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#delete_web_acl)
         """
+    def describe_all_managed_products(
+        self, *, Scope: ScopeType
+    ) -> DescribeAllManagedProductsResponseTypeDef:
+        """
+        Provides high-level information for the Amazon Web Services Managed Rules rule
+        groups and Amazon Web Services Marketplace managed rule groups.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.describe_all_managed_products)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#describe_all_managed_products)
+        """
+    def describe_managed_products_by_vendor(
+        self, *, VendorName: str, Scope: ScopeType
+    ) -> DescribeManagedProductsByVendorResponseTypeDef:
+        """
+        Provides high-level information for the managed rule groups owned by a specific
+        vendor.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.describe_managed_products_by_vendor)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#describe_managed_products_by_vendor)
+        """
     def describe_managed_rule_group(
         self, *, VendorName: str, Name: str, Scope: ScopeType, VersionName: str = ...
     ) -> DescribeManagedRuleGroupResponseTypeDef:
         """
         Provides high-level information for a managed rule group, including descriptions
         of the rules.
 
@@ -317,14 +354,23 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#generate_presigned_url)
         """
+    def get_decrypted_api_key(
+        self, *, Scope: ScopeType, APIKey: str
+    ) -> GetDecryptedAPIKeyResponseTypeDef:
+        """
+        Returns your API key in decrypted form.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.get_decrypted_api_key)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#get_decrypted_api_key)
+        """
     def get_ip_set(self, *, Name: str, Scope: ScopeType, Id: str) -> GetIPSetResponseTypeDef:
         """
         Retrieves the specified  IPSet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.get_ip_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#get_ip_set)
         """
@@ -369,15 +415,16 @@
         Scope: ScopeType,
         WebACLName: str,
         WebACLId: str,
         RuleName: str,
         RuleGroupRuleName: str = ...
     ) -> GetRateBasedStatementManagedKeysResponseTypeDef:
         """
-        Retrieves the keys that are currently blocked by a rate-based rule instance.
+        Retrieves the IP addresses that are currently blocked by a rate-based rule
+        instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.get_rate_based_statement_managed_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#get_rate_based_statement_managed_keys)
         """
     def get_regex_pattern_set(
         self, *, Name: str, Scope: ScopeType, Id: str
     ) -> GetRegexPatternSetResponseTypeDef:
@@ -423,14 +470,23 @@
     def get_web_acl_for_resource(self, *, ResourceArn: str) -> GetWebACLForResourceResponseTypeDef:
         """
         Retrieves the  WebACL for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.get_web_acl_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#get_web_acl_for_resource)
         """
+    def list_api_keys(
+        self, *, Scope: ScopeType, NextMarker: str = ..., Limit: int = ...
+    ) -> ListAPIKeysResponseTypeDef:
+        """
+        Retrieves a list of the API keys that you've defined for the specified scope.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.list_api_keys)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#list_api_keys)
+        """
     def list_available_managed_rule_group_versions(
         self,
         *,
         VendorName: str,
         Name: str,
         Scope: ScopeType,
         NextMarker: str = ...,
@@ -660,15 +716,16 @@
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
         Rules: Sequence[RuleTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
-        TokenDomains: Sequence[str] = ...
+        TokenDomains: Sequence[str] = ...,
+        AssociationConfig: AssociationConfigTypeDef = ...
     ) -> UpdateWebACLResponseTypeDef:
         """
         Updates the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#update_web_acl)
         """
```

### Comparing `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/literals.py` & `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "ActionValueType",
+    "AssociatedResourceTypeType",
     "BodyParsingFallbackBehaviorType",
     "ComparisonOperatorType",
     "CountryCodeType",
     "FailureReasonType",
     "FallbackBehaviorType",
     "FilterBehaviorType",
     "FilterRequirementType",
@@ -39,23 +40,25 @@
     "PlatformType",
     "PositionalConstraintType",
     "RateBasedStatementAggregateKeyTypeType",
     "ResourceTypeType",
     "ResponseContentTypeType",
     "ScopeType",
     "SensitivityLevelType",
+    "SizeInspectionLimitType",
     "TextTransformationTypeType",
     "WAFV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 
 ActionValueType = Literal["ALLOW", "BLOCK", "CAPTCHA", "CHALLENGE", "COUNT", "EXCLUDED_AS_COUNT"]
+AssociatedResourceTypeType = Literal["CLOUDFRONT"]
 BodyParsingFallbackBehaviorType = Literal["EVALUATE_AS_STRING", "MATCH", "NO_MATCH"]
 ComparisonOperatorType = Literal["EQ", "GE", "GT", "LE", "LT", "NE"]
 CountryCodeType = Literal[
     "AD",
     "AE",
     "AF",
     "AG",
@@ -320,21 +323,27 @@
 MapMatchScopeType = Literal["ALL", "KEY", "VALUE"]
 OversizeHandlingType = Literal["CONTINUE", "MATCH", "NO_MATCH"]
 PayloadTypeType = Literal["FORM_ENCODED", "JSON"]
 PlatformType = Literal["ANDROID", "IOS"]
 PositionalConstraintType = Literal[
     "CONTAINS", "CONTAINS_WORD", "ENDS_WITH", "EXACTLY", "STARTS_WITH"
 ]
-RateBasedStatementAggregateKeyTypeType = Literal["FORWARDED_IP", "IP"]
+RateBasedStatementAggregateKeyTypeType = Literal["CONSTANT", "CUSTOM_KEYS", "FORWARDED_IP", "IP"]
 ResourceTypeType = Literal[
-    "API_GATEWAY", "APPLICATION_LOAD_BALANCER", "APPSYNC", "APP_RUNNER_SERVICE", "COGNITO_USER_POOL"
+    "API_GATEWAY",
+    "APPLICATION_LOAD_BALANCER",
+    "APPSYNC",
+    "APP_RUNNER_SERVICE",
+    "COGNITO_USER_POOL",
+    "VERIFIED_ACCESS_INSTANCE",
 ]
 ResponseContentTypeType = Literal["APPLICATION_JSON", "TEXT_HTML", "TEXT_PLAIN"]
 ScopeType = Literal["CLOUDFRONT", "REGIONAL"]
 SensitivityLevelType = Literal["HIGH", "LOW"]
+SizeInspectionLimitType = Literal["KB_16", "KB_32", "KB_48", "KB_64"]
 TextTransformationTypeType = Literal[
     "BASE64_DECODE",
     "BASE64_DECODE_EXT",
     "CMD_LINE",
     "COMPRESS_WHITE_SPACE",
     "CSS_DECODE",
     "ESCAPE_SEQ_DECODE",
@@ -366,14 +375,15 @@
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
@@ -413,14 +423,15 @@
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
@@ -499,14 +510,15 @@
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
@@ -517,14 +529,15 @@
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
@@ -560,14 +573,15 @@
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
@@ -586,16 +600,19 @@
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
@@ -679,15 +696,17 @@
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
@@ -712,21 +731,25 @@
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
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/literals.pyi` & `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "ActionValueType",
+    "AssociatedResourceTypeType",
     "BodyParsingFallbackBehaviorType",
     "ComparisonOperatorType",
     "CountryCodeType",
     "FailureReasonType",
     "FallbackBehaviorType",
     "FilterBehaviorType",
     "FilterRequirementType",
@@ -38,22 +39,24 @@
     "PlatformType",
     "PositionalConstraintType",
     "RateBasedStatementAggregateKeyTypeType",
     "ResourceTypeType",
     "ResponseContentTypeType",
     "ScopeType",
     "SensitivityLevelType",
+    "SizeInspectionLimitType",
     "TextTransformationTypeType",
     "WAFV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 ActionValueType = Literal["ALLOW", "BLOCK", "CAPTCHA", "CHALLENGE", "COUNT", "EXCLUDED_AS_COUNT"]
+AssociatedResourceTypeType = Literal["CLOUDFRONT"]
 BodyParsingFallbackBehaviorType = Literal["EVALUATE_AS_STRING", "MATCH", "NO_MATCH"]
 ComparisonOperatorType = Literal["EQ", "GE", "GT", "LE", "LT", "NE"]
 CountryCodeType = Literal[
     "AD",
     "AE",
     "AF",
     "AG",
@@ -318,21 +321,27 @@
 MapMatchScopeType = Literal["ALL", "KEY", "VALUE"]
 OversizeHandlingType = Literal["CONTINUE", "MATCH", "NO_MATCH"]
 PayloadTypeType = Literal["FORM_ENCODED", "JSON"]
 PlatformType = Literal["ANDROID", "IOS"]
 PositionalConstraintType = Literal[
     "CONTAINS", "CONTAINS_WORD", "ENDS_WITH", "EXACTLY", "STARTS_WITH"
 ]
-RateBasedStatementAggregateKeyTypeType = Literal["FORWARDED_IP", "IP"]
+RateBasedStatementAggregateKeyTypeType = Literal["CONSTANT", "CUSTOM_KEYS", "FORWARDED_IP", "IP"]
 ResourceTypeType = Literal[
-    "API_GATEWAY", "APPLICATION_LOAD_BALANCER", "APPSYNC", "APP_RUNNER_SERVICE", "COGNITO_USER_POOL"
+    "API_GATEWAY",
+    "APPLICATION_LOAD_BALANCER",
+    "APPSYNC",
+    "APP_RUNNER_SERVICE",
+    "COGNITO_USER_POOL",
+    "VERIFIED_ACCESS_INSTANCE",
 ]
 ResponseContentTypeType = Literal["APPLICATION_JSON", "TEXT_HTML", "TEXT_PLAIN"]
 ScopeType = Literal["CLOUDFRONT", "REGIONAL"]
 SensitivityLevelType = Literal["HIGH", "LOW"]
+SizeInspectionLimitType = Literal["KB_16", "KB_32", "KB_48", "KB_64"]
 TextTransformationTypeType = Literal[
     "BASE64_DECODE",
     "BASE64_DECODE_EXT",
     "CMD_LINE",
     "COMPRESS_WHITE_SPACE",
     "CSS_DECODE",
     "ESCAPE_SEQ_DECODE",
@@ -364,14 +373,15 @@
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
@@ -411,14 +421,15 @@
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
@@ -497,14 +508,15 @@
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
@@ -515,14 +527,15 @@
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
@@ -558,14 +571,15 @@
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
@@ -584,16 +598,19 @@
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
@@ -677,15 +694,17 @@
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
@@ -710,21 +729,25 @@
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
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/type_defs.py` & `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for wafv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_wafv2.type_defs import AWSManagedRulesBotControlRuleSetTypeDef
+    from mypy_boto3_wafv2.type_defs import APIKeySummaryTypeDef
 
-    data: AWSManagedRulesBotControlRuleSetTypeDef = {...}
+    data: APIKeySummaryTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -37,121 +37,146 @@
     PlatformType,
     PositionalConstraintType,
     RateBasedStatementAggregateKeyTypeType,
     ResourceTypeType,
     ResponseContentTypeType,
     ScopeType,
     SensitivityLevelType,
+    SizeInspectionLimitType,
     TextTransformationTypeType,
 )
 
 if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "APIKeySummaryTypeDef",
     "AWSManagedRulesBotControlRuleSetTypeDef",
     "ActionConditionTypeDef",
+    "AddressFieldTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
+    "RequestBodyAssociatedResourceTypeConfigTypeDef",
     "BodyTypeDef",
     "TextTransformationTypeDef",
     "ImmunityTimePropertyTypeDef",
     "CaptchaResponseTypeDef",
     "ChallengeResponseTypeDef",
-    "ResponseMetadataTypeDef",
+    "CheckCapacityResponseTypeDef",
     "LabelNameConditionTypeDef",
     "CookieMatchPatternTypeDef",
+    "CreateAPIKeyRequestRequestTypeDef",
+    "CreateAPIKeyResponseTypeDef",
     "TagTypeDef",
     "IPSetSummaryTypeDef",
     "RegexTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "CustomResponseBodyTypeDef",
     "VisibilityConfigTypeDef",
     "RuleGroupSummaryTypeDef",
     "WebACLSummaryTypeDef",
     "CustomHTTPHeaderTypeDef",
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
+    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
+    "DescribeAllManagedProductsRequestRequestTypeDef",
+    "ManagedProductDescriptorTypeDef",
+    "DescribeManagedProductsByVendorRequestRequestTypeDef",
     "DescribeManagedRuleGroupRequestRequestTypeDef",
     "LabelSummaryTypeDef",
     "DisassociateWebACLRequestRequestTypeDef",
+    "EmailFieldTypeDef",
     "ExcludedRuleTypeDef",
+    "HeaderOrderTypeDef",
     "SingleHeaderTypeDef",
     "SingleQueryArgumentTypeDef",
     "ForwardedIPConfigTypeDef",
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
+    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+    "GetDecryptedAPIKeyRequestRequestTypeDef",
+    "GetDecryptedAPIKeyResponseTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "IPSetTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetManagedRuleSetRequestRequestTypeDef",
     "GetMobileSdkReleaseRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
+    "GetPermissionPolicyResponseTypeDef",
     "GetRateBasedStatementManagedKeysRequestRequestTypeDef",
     "RateBasedStatementManagedKeysIPSetTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "TimeWindowTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
     "HeaderMatchPatternTypeDef",
     "IPSetForwardedIPConfigTypeDef",
     "JsonMatchPatternTypeDef",
     "LabelMatchStatementTypeDef",
     "LabelTypeDef",
+    "ListAPIKeysRequestRequestTypeDef",
     "ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef",
     "ManagedRuleGroupVersionTypeDef",
     "ListAvailableManagedRuleGroupsRequestRequestTypeDef",
     "ManagedRuleGroupSummaryTypeDef",
     "ListIPSetsRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
     "ListManagedRuleSetsRequestRequestTypeDef",
     "ManagedRuleSetSummaryTypeDef",
     "ListMobileSdkReleasesRequestRequestTypeDef",
     "ReleaseSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
+    "ListResourcesForWebACLResponseTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "PasswordFieldTypeDef",
     "UsernameFieldTypeDef",
     "ManagedRuleSetVersionTypeDef",
     "NotStatementTypeDef",
     "OrStatementTypeDef",
+    "PhoneNumberFieldTypeDef",
     "VersionToPublishTypeDef",
+    "PutManagedRuleSetVersionsResponseTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
+    "RateLimitLabelNamespaceTypeDef",
     "ResponseInspectionBodyContainsTypeDef",
     "ResponseInspectionHeaderTypeDef",
     "ResponseInspectionJsonTypeDef",
     "ResponseInspectionStatusCodeTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
-    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
-    "CaptchaConfigTypeDef",
-    "ChallengeConfigTypeDef",
-    "CheckCapacityResponseTypeDef",
-    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
-    "GenerateMobileSdkReleaseUrlResponseTypeDef",
-    "GetPermissionPolicyResponseTypeDef",
-    "ListResourcesForWebACLResponseTypeDef",
-    "PutManagedRuleSetVersionsResponseTypeDef",
     "UpdateIPSetResponseTypeDef",
+    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
     "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
     "UpdateRegexPatternSetResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
+    "ListAPIKeysResponseTypeDef",
+    "AssociationConfigTypeDef",
+    "RateLimitCookieTypeDef",
+    "RateLimitHeaderTypeDef",
+    "RateLimitQueryArgumentTypeDef",
+    "RateLimitQueryStringTypeDef",
+    "CaptchaConfigTypeDef",
+    "ChallengeConfigTypeDef",
     "ConditionTypeDef",
     "CookiesTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "MobileSdkReleaseTypeDef",
     "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIPSetResponseTypeDef",
@@ -163,44 +188,49 @@
     "ListRegexPatternSetsResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "ListWebACLsResponseTypeDef",
     "CustomRequestHandlingTypeDef",
     "CustomResponseTypeDef",
+    "DescribeAllManagedProductsResponseTypeDef",
+    "DescribeManagedProductsByVendorResponseTypeDef",
     "GeoMatchStatementTypeDef",
-    "RateBasedStatementTypeDef",
     "GetIPSetResponseTypeDef",
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
     "HeadersTypeDef",
     "IPSetReferenceStatementTypeDef",
     "JsonBodyTypeDef",
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     "ListManagedRuleSetsResponseTypeDef",
     "ListMobileSdkReleasesResponseTypeDef",
     "RequestInspectionTypeDef",
     "ManagedRuleSetTypeDef",
+    "RequestInspectionACFPTypeDef",
     "PutManagedRuleSetVersionsRequestRequestTypeDef",
     "ResponseInspectionTypeDef",
+    "RateBasedStatementCustomKeyTypeDef",
     "FilterTypeDef",
     "GetMobileSdkReleaseResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
     "AllowActionTypeDef",
     "CaptchaActionTypeDef",
     "ChallengeActionTypeDef",
     "CountActionTypeDef",
     "BlockActionTypeDef",
     "SampledHTTPRequestTypeDef",
     "FieldToMatchTypeDef",
     "GetManagedRuleSetResponseTypeDef",
+    "AWSManagedRulesACFPRuleSetTypeDef",
     "AWSManagedRulesATPRuleSetTypeDef",
+    "RateBasedStatementTypeDef",
     "LoggingFilterTypeDef",
     "OverrideActionTypeDef",
     "DefaultActionTypeDef",
     "RuleActionTypeDef",
     "GetSampledRequestsResponseTypeDef",
     "ByteMatchStatementTypeDef",
     "RegexMatchStatementTypeDef",
@@ -231,28 +261,46 @@
     "GetRuleGroupResponseTypeDef",
     "FirewallManagerRuleGroupTypeDef",
     "WebACLTypeDef",
     "GetWebACLForResourceResponseTypeDef",
     "GetWebACLResponseTypeDef",
 )
 
+APIKeySummaryTypeDef = TypedDict(
+    "APIKeySummaryTypeDef",
+    {
+        "TokenDomains": List[str],
+        "APIKey": str,
+        "CreationTimestamp": datetime,
+        "Version": int,
+    },
+    total=False,
+)
+
 AWSManagedRulesBotControlRuleSetTypeDef = TypedDict(
     "AWSManagedRulesBotControlRuleSetTypeDef",
     {
         "InspectionLevel": InspectionLevelType,
     },
 )
 
 ActionConditionTypeDef = TypedDict(
     "ActionConditionTypeDef",
     {
         "Action": ActionValueType,
     },
 )
 
+AddressFieldTypeDef = TypedDict(
+    "AddressFieldTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 AndStatementTypeDef = TypedDict(
     "AndStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
     },
 )
 
@@ -260,14 +308,21 @@
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLArn": str,
         "ResourceArn": str,
     },
 )
 
+RequestBodyAssociatedResourceTypeConfigTypeDef = TypedDict(
+    "RequestBodyAssociatedResourceTypeConfigTypeDef",
+    {
+        "DefaultSizeInspectionLimit": SizeInspectionLimitType,
+    },
+)
+
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
     total=False,
 )
@@ -303,22 +358,19 @@
         "ResponseCode": int,
         "SolveTimestamp": int,
         "FailureReason": FailureReasonType,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CheckCapacityResponseTypeDef = TypedDict(
+    "CheckCapacityResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Capacity": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LabelNameConditionTypeDef = TypedDict(
     "LabelNameConditionTypeDef",
     {
         "LabelName": str,
@@ -331,14 +383,30 @@
         "All": Mapping[str, Any],
         "IncludedCookies": Sequence[str],
         "ExcludedCookies": Sequence[str],
     },
     total=False,
 )
 
+CreateAPIKeyRequestRequestTypeDef = TypedDict(
+    "CreateAPIKeyRequestRequestTypeDef",
+    {
+        "Scope": ScopeType,
+        "TokenDomains": Sequence[str],
+    },
+)
+
+CreateAPIKeyResponseTypeDef = TypedDict(
+    "CreateAPIKeyResponseTypeDef",
+    {
+        "APIKey": str,
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
 )
@@ -428,14 +496,22 @@
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
     {
         "WebACLArn": str,
         "WebACLLockToken": str,
     },
 )
 
+DeleteFirewallManagerRuleGroupsResponseTypeDef = TypedDict(
+    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+    {
+        "NextWebACLLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteIPSetRequestRequestTypeDef = TypedDict(
     "DeleteIPSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "LockToken": str,
@@ -482,14 +558,45 @@
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "LockToken": str,
     },
 )
 
+DescribeAllManagedProductsRequestRequestTypeDef = TypedDict(
+    "DescribeAllManagedProductsRequestRequestTypeDef",
+    {
+        "Scope": ScopeType,
+    },
+)
+
+ManagedProductDescriptorTypeDef = TypedDict(
+    "ManagedProductDescriptorTypeDef",
+    {
+        "VendorName": str,
+        "ManagedRuleSetName": str,
+        "ProductId": str,
+        "ProductLink": str,
+        "ProductTitle": str,
+        "ProductDescription": str,
+        "SnsTopicArn": str,
+        "IsVersioningSupported": bool,
+        "IsAdvancedManagedRuleSet": bool,
+    },
+    total=False,
+)
+
+DescribeManagedProductsByVendorRequestRequestTypeDef = TypedDict(
+    "DescribeManagedProductsByVendorRequestRequestTypeDef",
+    {
+        "VendorName": str,
+        "Scope": ScopeType,
+    },
+)
+
 _RequiredDescribeManagedRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeManagedRuleGroupRequestRequestTypeDef",
     {
         "VendorName": str,
         "Name": str,
         "Scope": ScopeType,
     },
@@ -498,22 +605,20 @@
     "_OptionalDescribeManagedRuleGroupRequestRequestTypeDef",
     {
         "VersionName": str,
     },
     total=False,
 )
 
-
 class DescribeManagedRuleGroupRequestRequestTypeDef(
     _RequiredDescribeManagedRuleGroupRequestRequestTypeDef,
     _OptionalDescribeManagedRuleGroupRequestRequestTypeDef,
 ):
     pass
 
-
 LabelSummaryTypeDef = TypedDict(
     "LabelSummaryTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -521,21 +626,35 @@
 DisassociateWebACLRequestRequestTypeDef = TypedDict(
     "DisassociateWebACLRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+EmailFieldTypeDef = TypedDict(
+    "EmailFieldTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 ExcludedRuleTypeDef = TypedDict(
     "ExcludedRuleTypeDef",
     {
         "Name": str,
     },
 )
 
+HeaderOrderTypeDef = TypedDict(
+    "HeaderOrderTypeDef",
+    {
+        "OversizeHandling": OversizeHandlingType,
+    },
+)
+
 SingleHeaderTypeDef = TypedDict(
     "SingleHeaderTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -558,14 +677,39 @@
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
     {
         "Platform": PlatformType,
         "ReleaseVersion": str,
     },
 )
 
+GenerateMobileSdkReleaseUrlResponseTypeDef = TypedDict(
+    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDecryptedAPIKeyRequestRequestTypeDef = TypedDict(
+    "GetDecryptedAPIKeyRequestRequestTypeDef",
+    {
+        "Scope": ScopeType,
+        "APIKey": str,
+    },
+)
+
+GetDecryptedAPIKeyResponseTypeDef = TypedDict(
+    "GetDecryptedAPIKeyResponseTypeDef",
+    {
+        "TokenDomains": List[str],
+        "CreationTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetIPSetRequestRequestTypeDef = TypedDict(
     "GetIPSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
     },
@@ -585,19 +729,17 @@
     "_OptionalIPSetTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class IPSetTypeDef(_RequiredIPSetTypeDef, _OptionalIPSetTypeDef):
     pass
 
-
 GetLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetLoggingConfigurationRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -621,14 +763,22 @@
 GetPermissionPolicyRequestRequestTypeDef = TypedDict(
     "GetPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+GetPermissionPolicyResponseTypeDef = TypedDict(
+    "GetPermissionPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "WebACLName": str,
         "WebACLId": str,
         "RuleName": str,
@@ -638,22 +788,20 @@
     "_OptionalGetRateBasedStatementManagedKeysRequestRequestTypeDef",
     {
         "RuleGroupRuleName": str,
     },
     total=False,
 )
 
-
 class GetRateBasedStatementManagedKeysRequestRequestTypeDef(
     _RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef,
     _OptionalGetRateBasedStatementManagedKeysRequestRequestTypeDef,
 ):
     pass
 
-
 RateBasedStatementManagedKeysIPSetTypeDef = TypedDict(
     "RateBasedStatementManagedKeysIPSetTypeDef",
     {
         "IPAddressVersion": IPAddressVersionType,
         "Addresses": List[str],
     },
     total=False,
@@ -751,14 +899,34 @@
 LabelTypeDef = TypedDict(
     "LabelTypeDef",
     {
         "Name": str,
     },
 )
 
+_RequiredListAPIKeysRequestRequestTypeDef = TypedDict(
+    "_RequiredListAPIKeysRequestRequestTypeDef",
+    {
+        "Scope": ScopeType,
+    },
+)
+_OptionalListAPIKeysRequestRequestTypeDef = TypedDict(
+    "_OptionalListAPIKeysRequestRequestTypeDef",
+    {
+        "NextMarker": str,
+        "Limit": int,
+    },
+    total=False,
+)
+
+class ListAPIKeysRequestRequestTypeDef(
+    _RequiredListAPIKeysRequestRequestTypeDef, _OptionalListAPIKeysRequestRequestTypeDef
+):
+    pass
+
 _RequiredListAvailableManagedRuleGroupVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableManagedRuleGroupVersionsRequestRequestTypeDef",
     {
         "VendorName": str,
         "Name": str,
         "Scope": ScopeType,
     },
@@ -768,22 +936,20 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef(
     _RequiredListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     _OptionalListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ManagedRuleGroupVersionTypeDef = TypedDict(
     "ManagedRuleGroupVersionTypeDef",
     {
         "Name": str,
         "LastUpdateTimestamp": datetime,
     },
     total=False,
@@ -800,22 +966,20 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListAvailableManagedRuleGroupsRequestRequestTypeDef(
     _RequiredListAvailableManagedRuleGroupsRequestRequestTypeDef,
     _OptionalListAvailableManagedRuleGroupsRequestRequestTypeDef,
 ):
     pass
 
-
 ManagedRuleGroupSummaryTypeDef = TypedDict(
     "ManagedRuleGroupSummaryTypeDef",
     {
         "VendorName": str,
         "Name": str,
         "VersioningSupported": bool,
         "Description": str,
@@ -834,21 +998,19 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListIPSetsRequestRequestTypeDef(
     _RequiredListIPSetsRequestRequestTypeDef, _OptionalListIPSetsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListLoggingConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListLoggingConfigurationsRequestRequestTypeDef",
     {
         "Scope": ScopeType,
     },
 )
 _OptionalListLoggingConfigurationsRequestRequestTypeDef = TypedDict(
@@ -856,22 +1018,20 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListLoggingConfigurationsRequestRequestTypeDef(
     _RequiredListLoggingConfigurationsRequestRequestTypeDef,
     _OptionalListLoggingConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListManagedRuleSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedRuleSetsRequestRequestTypeDef",
     {
         "Scope": ScopeType,
     },
 )
 _OptionalListManagedRuleSetsRequestRequestTypeDef = TypedDict(
@@ -879,22 +1039,20 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListManagedRuleSetsRequestRequestTypeDef(
     _RequiredListManagedRuleSetsRequestRequestTypeDef,
     _OptionalListManagedRuleSetsRequestRequestTypeDef,
 ):
     pass
 
-
 ManagedRuleSetSummaryTypeDef = TypedDict(
     "ManagedRuleSetSummaryTypeDef",
     {
         "Name": str,
         "Id": str,
         "Description": str,
         "LockToken": str,
@@ -915,22 +1073,20 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListMobileSdkReleasesRequestRequestTypeDef(
     _RequiredListMobileSdkReleasesRequestRequestTypeDef,
     _OptionalListMobileSdkReleasesRequestRequestTypeDef,
 ):
     pass
 
-
 ReleaseSummaryTypeDef = TypedDict(
     "ReleaseSummaryTypeDef",
     {
         "ReleaseVersion": str,
         "Timestamp": datetime,
     },
     total=False,
@@ -947,43 +1103,47 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListRegexPatternSetsRequestRequestTypeDef(
     _RequiredListRegexPatternSetsRequestRequestTypeDef,
     _OptionalListRegexPatternSetsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListResourcesForWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesForWebACLRequestRequestTypeDef",
     {
         "WebACLArn": str,
     },
 )
 _OptionalListResourcesForWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalListResourcesForWebACLRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeType,
     },
     total=False,
 )
 
-
 class ListResourcesForWebACLRequestRequestTypeDef(
     _RequiredListResourcesForWebACLRequestRequestTypeDef,
     _OptionalListResourcesForWebACLRequestRequestTypeDef,
 ):
     pass
 
+ListResourcesForWebACLResponseTypeDef = TypedDict(
+    "ListResourcesForWebACLResponseTypeDef",
+    {
+        "ResourceArns": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredListRuleGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListRuleGroupsRequestRequestTypeDef",
     {
         "Scope": ScopeType,
     },
 )
@@ -992,21 +1152,19 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListRuleGroupsRequestRequestTypeDef(
     _RequiredListRuleGroupsRequestRequestTypeDef, _OptionalListRuleGroupsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1014,22 +1172,20 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListWebACLsRequestRequestTypeDef = TypedDict(
     "_RequiredListWebACLsRequestRequestTypeDef",
     {
         "Scope": ScopeType,
     },
 )
 _OptionalListWebACLsRequestRequestTypeDef = TypedDict(
@@ -1037,21 +1193,19 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListWebACLsRequestRequestTypeDef(
     _RequiredListWebACLsRequestRequestTypeDef, _OptionalListWebACLsRequestRequestTypeDef
 ):
     pass
 
-
 PasswordFieldTypeDef = TypedDict(
     "PasswordFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -1085,31 +1239,53 @@
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
     },
 )
 
+PhoneNumberFieldTypeDef = TypedDict(
+    "PhoneNumberFieldTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 VersionToPublishTypeDef = TypedDict(
     "VersionToPublishTypeDef",
     {
         "AssociatedRuleGroupArn": str,
         "ForecastedLifetime": int,
     },
     total=False,
 )
 
+PutManagedRuleSetVersionsResponseTypeDef = TypedDict(
+    "PutManagedRuleSetVersionsResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutPermissionPolicyRequestRequestTypeDef = TypedDict(
     "PutPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
 
+RateLimitLabelNamespaceTypeDef = TypedDict(
+    "RateLimitLabelNamespaceTypeDef",
+    {
+        "Namespace": str,
+    },
+)
+
 ResponseInspectionBodyContainsTypeDef = TypedDict(
     "ResponseInspectionBodyContainsTypeDef",
     {
         "SuccessStrings": Sequence[str],
         "FailureStrings": Sequence[str],
     },
 )
@@ -1136,14 +1312,25 @@
     "ResponseInspectionStatusCodeTypeDef",
     {
         "SuccessCodes": Sequence[int],
         "FailureCodes": Sequence[int],
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1162,137 +1349,138 @@
     "_OptionalUpdateIPSetRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateIPSetRequestRequestTypeDef(
     _RequiredUpdateIPSetRequestRequestTypeDef, _OptionalUpdateIPSetRequestRequestTypeDef
 ):
     pass
 
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = TypedDict(
     "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "LockToken": str,
         "VersionToExpire": str,
         "ExpiryTimestamp": Union[datetime, str],
     },
 )
 
-CaptchaConfigTypeDef = TypedDict(
-    "CaptchaConfigTypeDef",
-    {
-        "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
-    },
-    total=False,
-)
-
-ChallengeConfigTypeDef = TypedDict(
-    "ChallengeConfigTypeDef",
+UpdateManagedRuleSetVersionExpiryDateResponseTypeDef = TypedDict(
+    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
     {
-        "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
+        "ExpiringVersion": str,
+        "ExpiryTimestamp": datetime,
+        "NextLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-CheckCapacityResponseTypeDef = TypedDict(
-    "CheckCapacityResponseTypeDef",
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
     {
-        "Capacity": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteFirewallManagerRuleGroupsResponseTypeDef = TypedDict(
-    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
     {
-        "NextWebACLLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GenerateMobileSdkReleaseUrlResponseTypeDef = TypedDict(
-    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+UpdateWebACLResponseTypeDef = TypedDict(
+    "UpdateWebACLResponseTypeDef",
     {
-        "Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPermissionPolicyResponseTypeDef = TypedDict(
-    "GetPermissionPolicyResponseTypeDef",
+ListAPIKeysResponseTypeDef = TypedDict(
+    "ListAPIKeysResponseTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextMarker": str,
+        "APIKeySummaries": List[APIKeySummaryTypeDef],
+        "ApplicationIntegrationURL": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListResourcesForWebACLResponseTypeDef = TypedDict(
-    "ListResourcesForWebACLResponseTypeDef",
+AssociationConfigTypeDef = TypedDict(
+    "AssociationConfigTypeDef",
     {
-        "ResourceArns": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestBody": Mapping[
+            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef
+        ],
     },
+    total=False,
 )
 
-PutManagedRuleSetVersionsResponseTypeDef = TypedDict(
-    "PutManagedRuleSetVersionsResponseTypeDef",
+RateLimitCookieTypeDef = TypedDict(
+    "RateLimitCookieTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-UpdateIPSetResponseTypeDef = TypedDict(
-    "UpdateIPSetResponseTypeDef",
+RateLimitHeaderTypeDef = TypedDict(
+    "RateLimitHeaderTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-UpdateManagedRuleSetVersionExpiryDateResponseTypeDef = TypedDict(
-    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+RateLimitQueryArgumentTypeDef = TypedDict(
+    "RateLimitQueryArgumentTypeDef",
     {
-        "ExpiringVersion": str,
-        "ExpiryTimestamp": datetime,
-        "NextLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-UpdateRegexPatternSetResponseTypeDef = TypedDict(
-    "UpdateRegexPatternSetResponseTypeDef",
+RateLimitQueryStringTypeDef = TypedDict(
+    "RateLimitQueryStringTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+CaptchaConfigTypeDef = TypedDict(
+    "CaptchaConfigTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
     },
+    total=False,
 )
 
-UpdateWebACLResponseTypeDef = TypedDict(
-    "UpdateWebACLResponseTypeDef",
+ChallengeConfigTypeDef = TypedDict(
+    "ChallengeConfigTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
     },
+    total=False,
 )
 
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "ActionCondition": ActionConditionTypeDef,
         "LabelNameCondition": LabelNameConditionTypeDef,
@@ -1323,21 +1511,19 @@
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateIPSetRequestRequestTypeDef(
     _RequiredCreateIPSetRequestRequestTypeDef, _OptionalCreateIPSetRequestRequestTypeDef
 ):
     pass
 
-
 MobileSdkReleaseTypeDef = TypedDict(
     "MobileSdkReleaseTypeDef",
     {
         "ReleaseVersion": str,
         "Timestamp": datetime,
         "ReleaseNotes": str,
         "Tags": List[TagTypeDef],
@@ -1362,24 +1548,24 @@
     },
 )
 
 CreateIPSetResponseTypeDef = TypedDict(
     "CreateIPSetResponseTypeDef",
     {
         "Summary": IPSetSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIPSetsResponseTypeDef = TypedDict(
     "ListIPSetsResponseTypeDef",
     {
         "NextMarker": str,
         "IPSets": List[IPSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateRegexPatternSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRegexPatternSetRequestRequestTypeDef",
     {
         "Name": str,
@@ -1392,22 +1578,20 @@
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRegexPatternSetRequestRequestTypeDef(
     _RequiredCreateRegexPatternSetRequestRequestTypeDef,
     _OptionalCreateRegexPatternSetRequestRequestTypeDef,
 ):
     pass
 
-
 RegexPatternSetTypeDef = TypedDict(
     "RegexPatternSetTypeDef",
     {
         "Name": str,
         "Id": str,
         "ARN": str,
         "Description": str,
@@ -1430,70 +1614,68 @@
     "_OptionalUpdateRegexPatternSetRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateRegexPatternSetRequestRequestTypeDef(
     _RequiredUpdateRegexPatternSetRequestRequestTypeDef,
     _OptionalUpdateRegexPatternSetRequestRequestTypeDef,
 ):
     pass
 
-
 CreateRegexPatternSetResponseTypeDef = TypedDict(
     "CreateRegexPatternSetResponseTypeDef",
     {
         "Summary": RegexPatternSetSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRegexPatternSetsResponseTypeDef = TypedDict(
     "ListRegexPatternSetsResponseTypeDef",
     {
         "NextMarker": str,
         "RegexPatternSets": List[RegexPatternSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "Summary": RuleGroupSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[RuleGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "Summary": WebACLSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWebACLsResponseTypeDef = TypedDict(
     "ListWebACLsResponseTypeDef",
     {
         "NextMarker": str,
         "WebACLs": List[WebACLSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CustomRequestHandlingTypeDef = TypedDict(
     "CustomRequestHandlingTypeDef",
     {
         "InsertHeaders": Sequence[CustomHTTPHeaderTypeDef],
@@ -1511,66 +1693,57 @@
     {
         "CustomResponseBodyKey": str,
         "ResponseHeaders": Sequence[CustomHTTPHeaderTypeDef],
     },
     total=False,
 )
 
-
 class CustomResponseTypeDef(_RequiredCustomResponseTypeDef, _OptionalCustomResponseTypeDef):
     pass
 
-
-GeoMatchStatementTypeDef = TypedDict(
-    "GeoMatchStatementTypeDef",
+DescribeAllManagedProductsResponseTypeDef = TypedDict(
+    "DescribeAllManagedProductsResponseTypeDef",
     {
-        "CountryCodes": Sequence[CountryCodeType],
-        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
+        "ManagedProducts": List[ManagedProductDescriptorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredRateBasedStatementTypeDef = TypedDict(
-    "_RequiredRateBasedStatementTypeDef",
+DescribeManagedProductsByVendorResponseTypeDef = TypedDict(
+    "DescribeManagedProductsByVendorResponseTypeDef",
     {
-        "Limit": int,
-        "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
+        "ManagedProducts": List[ManagedProductDescriptorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalRateBasedStatementTypeDef = TypedDict(
-    "_OptionalRateBasedStatementTypeDef",
+
+GeoMatchStatementTypeDef = TypedDict(
+    "GeoMatchStatementTypeDef",
     {
-        "ScopeDownStatement": "StatementTypeDef",
+        "CountryCodes": Sequence[CountryCodeType],
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
     },
     total=False,
 )
 
-
-class RateBasedStatementTypeDef(
-    _RequiredRateBasedStatementTypeDef, _OptionalRateBasedStatementTypeDef
-):
-    pass
-
-
 GetIPSetResponseTypeDef = TypedDict(
     "GetIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRateBasedStatementManagedKeysResponseTypeDef = TypedDict(
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     {
         "ManagedKeysIPV4": RateBasedStatementManagedKeysIPSetTypeDef,
         "ManagedKeysIPV6": RateBasedStatementManagedKeysIPSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSampledRequestsRequestRequestTypeDef = TypedDict(
     "GetSampledRequestsRequestRequestTypeDef",
     {
         "WebAclArn": str,
@@ -1613,21 +1786,19 @@
     "_OptionalIPSetReferenceStatementTypeDef",
     {
         "IPSetForwardedIPConfig": IPSetForwardedIPConfigTypeDef,
     },
     total=False,
 )
 
-
 class IPSetReferenceStatementTypeDef(
     _RequiredIPSetReferenceStatementTypeDef, _OptionalIPSetReferenceStatementTypeDef
 ):
     pass
 
-
 _RequiredJsonBodyTypeDef = TypedDict(
     "_RequiredJsonBodyTypeDef",
     {
         "MatchPattern": JsonMatchPatternTypeDef,
         "MatchScope": JsonMatchScopeType,
     },
 )
@@ -1636,53 +1807,51 @@
     {
         "InvalidFallbackBehavior": BodyParsingFallbackBehaviorType,
         "OversizeHandling": OversizeHandlingType,
     },
     total=False,
 )
 
-
 class JsonBodyTypeDef(_RequiredJsonBodyTypeDef, _OptionalJsonBodyTypeDef):
     pass
 
-
 ListAvailableManagedRuleGroupVersionsResponseTypeDef = TypedDict(
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     {
         "NextMarker": str,
         "Versions": List[ManagedRuleGroupVersionTypeDef],
         "CurrentDefaultVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAvailableManagedRuleGroupsResponseTypeDef = TypedDict(
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "ManagedRuleGroups": List[ManagedRuleGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListManagedRuleSetsResponseTypeDef = TypedDict(
     "ListManagedRuleSetsResponseTypeDef",
     {
         "NextMarker": str,
         "ManagedRuleSets": List[ManagedRuleSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMobileSdkReleasesResponseTypeDef = TypedDict(
     "ListMobileSdkReleasesResponseTypeDef",
     {
         "ReleaseSummaries": List[ReleaseSummaryTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RequestInspectionTypeDef = TypedDict(
     "RequestInspectionTypeDef",
     {
         "PayloadType": PayloadTypeType,
@@ -1706,18 +1875,39 @@
         "PublishedVersions": Dict[str, ManagedRuleSetVersionTypeDef],
         "RecommendedVersion": str,
         "LabelNamespace": str,
     },
     total=False,
 )
 
-
 class ManagedRuleSetTypeDef(_RequiredManagedRuleSetTypeDef, _OptionalManagedRuleSetTypeDef):
     pass
 
+_RequiredRequestInspectionACFPTypeDef = TypedDict(
+    "_RequiredRequestInspectionACFPTypeDef",
+    {
+        "PayloadType": PayloadTypeType,
+    },
+)
+_OptionalRequestInspectionACFPTypeDef = TypedDict(
+    "_OptionalRequestInspectionACFPTypeDef",
+    {
+        "UsernameField": UsernameFieldTypeDef,
+        "PasswordField": PasswordFieldTypeDef,
+        "EmailField": EmailFieldTypeDef,
+        "PhoneNumberFields": Sequence[PhoneNumberFieldTypeDef],
+        "AddressFields": Sequence[AddressFieldTypeDef],
+    },
+    total=False,
+)
+
+class RequestInspectionACFPTypeDef(
+    _RequiredRequestInspectionACFPTypeDef, _OptionalRequestInspectionACFPTypeDef
+):
+    pass
 
 _RequiredPutManagedRuleSetVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutManagedRuleSetVersionsRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
@@ -1729,65 +1919,78 @@
     {
         "RecommendedVersion": str,
         "VersionsToPublish": Mapping[str, VersionToPublishTypeDef],
     },
     total=False,
 )
 
-
 class PutManagedRuleSetVersionsRequestRequestTypeDef(
     _RequiredPutManagedRuleSetVersionsRequestRequestTypeDef,
     _OptionalPutManagedRuleSetVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ResponseInspectionTypeDef = TypedDict(
     "ResponseInspectionTypeDef",
     {
         "StatusCode": ResponseInspectionStatusCodeTypeDef,
         "Header": ResponseInspectionHeaderTypeDef,
         "BodyContains": ResponseInspectionBodyContainsTypeDef,
         "Json": ResponseInspectionJsonTypeDef,
     },
     total=False,
 )
 
+RateBasedStatementCustomKeyTypeDef = TypedDict(
+    "RateBasedStatementCustomKeyTypeDef",
+    {
+        "Header": RateLimitHeaderTypeDef,
+        "Cookie": RateLimitCookieTypeDef,
+        "QueryArgument": RateLimitQueryArgumentTypeDef,
+        "QueryString": RateLimitQueryStringTypeDef,
+        "HTTPMethod": Mapping[str, Any],
+        "ForwardedIP": Mapping[str, Any],
+        "IP": Mapping[str, Any],
+        "LabelNamespace": RateLimitLabelNamespaceTypeDef,
+    },
+    total=False,
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Behavior": FilterBehaviorType,
         "Requirement": FilterRequirementType,
         "Conditions": List[ConditionTypeDef],
     },
 )
 
 GetMobileSdkReleaseResponseTypeDef = TypedDict(
     "GetMobileSdkReleaseResponseTypeDef",
     {
         "MobileSdkRelease": MobileSdkReleaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextMarker": str,
         "TagInfoForResource": TagInfoForResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRegexPatternSetResponseTypeDef = TypedDict(
     "GetRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AllowActionTypeDef = TypedDict(
     "AllowActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
@@ -1846,68 +2049,110 @@
         "CaptchaResponse": CaptchaResponseTypeDef,
         "ChallengeResponse": ChallengeResponseTypeDef,
         "OverriddenAction": str,
     },
     total=False,
 )
 
-
 class SampledHTTPRequestTypeDef(
     _RequiredSampledHTTPRequestTypeDef, _OptionalSampledHTTPRequestTypeDef
 ):
     pass
 
-
 FieldToMatchTypeDef = TypedDict(
     "FieldToMatchTypeDef",
     {
         "SingleHeader": SingleHeaderTypeDef,
         "SingleQueryArgument": SingleQueryArgumentTypeDef,
         "AllQueryArguments": Mapping[str, Any],
         "UriPath": Mapping[str, Any],
         "QueryString": Mapping[str, Any],
         "Body": BodyTypeDef,
         "Method": Mapping[str, Any],
         "JsonBody": JsonBodyTypeDef,
         "Headers": HeadersTypeDef,
         "Cookies": CookiesTypeDef,
+        "HeaderOrder": HeaderOrderTypeDef,
     },
     total=False,
 )
 
 GetManagedRuleSetResponseTypeDef = TypedDict(
     "GetManagedRuleSetResponseTypeDef",
     {
         "ManagedRuleSet": ManagedRuleSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredAWSManagedRulesACFPRuleSetTypeDef = TypedDict(
+    "_RequiredAWSManagedRulesACFPRuleSetTypeDef",
+    {
+        "CreationPath": str,
+        "RegistrationPagePath": str,
+        "RequestInspection": RequestInspectionACFPTypeDef,
+    },
+)
+_OptionalAWSManagedRulesACFPRuleSetTypeDef = TypedDict(
+    "_OptionalAWSManagedRulesACFPRuleSetTypeDef",
+    {
+        "ResponseInspection": ResponseInspectionTypeDef,
+        "EnableRegexInPath": bool,
     },
+    total=False,
 )
 
+class AWSManagedRulesACFPRuleSetTypeDef(
+    _RequiredAWSManagedRulesACFPRuleSetTypeDef, _OptionalAWSManagedRulesACFPRuleSetTypeDef
+):
+    pass
+
 _RequiredAWSManagedRulesATPRuleSetTypeDef = TypedDict(
     "_RequiredAWSManagedRulesATPRuleSetTypeDef",
     {
         "LoginPath": str,
     },
 )
 _OptionalAWSManagedRulesATPRuleSetTypeDef = TypedDict(
     "_OptionalAWSManagedRulesATPRuleSetTypeDef",
     {
         "RequestInspection": RequestInspectionTypeDef,
         "ResponseInspection": ResponseInspectionTypeDef,
+        "EnableRegexInPath": bool,
     },
     total=False,
 )
 
-
 class AWSManagedRulesATPRuleSetTypeDef(
     _RequiredAWSManagedRulesATPRuleSetTypeDef, _OptionalAWSManagedRulesATPRuleSetTypeDef
 ):
     pass
 
+_RequiredRateBasedStatementTypeDef = TypedDict(
+    "_RequiredRateBasedStatementTypeDef",
+    {
+        "Limit": int,
+        "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
+    },
+)
+_OptionalRateBasedStatementTypeDef = TypedDict(
+    "_OptionalRateBasedStatementTypeDef",
+    {
+        "ScopeDownStatement": "StatementTypeDef",
+        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
+        "CustomKeys": Sequence[RateBasedStatementCustomKeyTypeDef],
+    },
+    total=False,
+)
+
+class RateBasedStatementTypeDef(
+    _RequiredRateBasedStatementTypeDef, _OptionalRateBasedStatementTypeDef
+):
+    pass
 
 LoggingFilterTypeDef = TypedDict(
     "LoggingFilterTypeDef",
     {
         "Filters": List[FilterTypeDef],
         "DefaultBehavior": FilterBehaviorType,
     },
@@ -1945,15 +2190,15 @@
 
 GetSampledRequestsResponseTypeDef = TypedDict(
     "GetSampledRequestsResponseTypeDef",
     {
         "SampledRequests": List[SampledHTTPRequestTypeDef],
         "PopulationSize": int,
         "TimeWindow": TimeWindowTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ByteMatchStatementTypeDef = TypedDict(
     "ByteMatchStatementTypeDef",
     {
         "SearchString": Union[str, bytes, IO[Any], StreamingBody],
@@ -2002,21 +2247,19 @@
     "_OptionalSqliMatchStatementTypeDef",
     {
         "SensitivityLevel": SensitivityLevelType,
     },
     total=False,
 )
 
-
 class SqliMatchStatementTypeDef(
     _RequiredSqliMatchStatementTypeDef, _OptionalSqliMatchStatementTypeDef
 ):
     pass
 
-
 XssMatchStatementTypeDef = TypedDict(
     "XssMatchStatementTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
@@ -2026,14 +2269,15 @@
     {
         "LoginPath": str,
         "PayloadType": PayloadTypeType,
         "UsernameField": UsernameFieldTypeDef,
         "PasswordField": PasswordFieldTypeDef,
         "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
         "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetTypeDef,
+        "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetTypeDef,
     },
     total=False,
 )
 
 _RequiredLoggingConfigurationTypeDef = TypedDict(
     "_RequiredLoggingConfigurationTypeDef",
     {
@@ -2047,21 +2291,19 @@
         "RedactedFields": List[FieldToMatchTypeDef],
         "ManagedByFirewallManager": bool,
         "LoggingFilter": LoggingFilterTypeDef,
     },
     total=False,
 )
 
-
 class LoggingConfigurationTypeDef(
     _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
 ):
     pass
 
-
 RuleActionOverrideTypeDef = TypedDict(
     "RuleActionOverrideTypeDef",
     {
         "Name": str,
         "ActionToUse": RuleActionTypeDef,
     },
 )
@@ -2092,48 +2334,46 @@
         "RuleLabels": Sequence[LabelTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
     },
     total=False,
 )
 
-
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
-
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
         "LoggingConfigurations": List[LoggingConfigurationTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutLoggingConfigurationRequestRequestTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
 PutLoggingConfigurationResponseTypeDef = TypedDict(
     "PutLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredManagedRuleGroupStatementTypeDef = TypedDict(
     "_RequiredManagedRuleGroupStatementTypeDef",
     {
         "VendorName": str,
@@ -2148,21 +2388,19 @@
         "ScopeDownStatement": "StatementTypeDef",
         "ManagedRuleGroupConfigs": Sequence[ManagedRuleGroupConfigTypeDef],
         "RuleActionOverrides": Sequence[RuleActionOverrideTypeDef],
     },
     total=False,
 )
 
-
 class ManagedRuleGroupStatementTypeDef(
     _RequiredManagedRuleGroupStatementTypeDef, _OptionalManagedRuleGroupStatementTypeDef
 ):
     pass
 
-
 _RequiredRuleGroupReferenceStatementTypeDef = TypedDict(
     "_RequiredRuleGroupReferenceStatementTypeDef",
     {
         "ARN": str,
     },
 )
 _OptionalRuleGroupReferenceStatementTypeDef = TypedDict(
@@ -2170,32 +2408,30 @@
     {
         "ExcludedRules": Sequence[ExcludedRuleTypeDef],
         "RuleActionOverrides": Sequence[RuleActionOverrideTypeDef],
     },
     total=False,
 )
 
-
 class RuleGroupReferenceStatementTypeDef(
     _RequiredRuleGroupReferenceStatementTypeDef, _OptionalRuleGroupReferenceStatementTypeDef
 ):
     pass
 
-
 DescribeManagedRuleGroupResponseTypeDef = TypedDict(
     "DescribeManagedRuleGroupResponseTypeDef",
     {
         "VersionName": str,
         "SnsTopicArn": str,
         "Capacity": int,
         "Rules": List[RuleSummaryTypeDef],
         "LabelNamespace": str,
         "AvailableLabels": List[LabelSummaryTypeDef],
         "ConsumedLabels": List[LabelSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CheckCapacityRequestRequestTypeDef = TypedDict(
     "CheckCapacityRequestRequestTypeDef",
     {
         "Scope": ScopeType,
@@ -2219,21 +2455,19 @@
         "Rules": Sequence[RuleTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
-
 class CreateRuleGroupRequestRequestTypeDef(
     _RequiredCreateRuleGroupRequestRequestTypeDef, _OptionalCreateRuleGroupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWebACLRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "DefaultAction": DefaultActionTypeDef,
         "VisibilityConfig": VisibilityConfigTypeDef,
@@ -2245,25 +2479,24 @@
         "Description": str,
         "Rules": Sequence[RuleTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
+        "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
 )
 
-
 class CreateWebACLRequestRequestTypeDef(
     _RequiredCreateWebACLRequestRequestTypeDef, _OptionalCreateWebACLRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredRuleGroupTypeDef = TypedDict(
     "_RequiredRuleGroupTypeDef",
     {
         "Name": str,
         "Id": str,
         "Capacity": int,
         "ARN": str,
@@ -2279,19 +2512,17 @@
         "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
         "AvailableLabels": List[LabelSummaryTypeDef],
         "ConsumedLabels": List[LabelSummaryTypeDef],
     },
     total=False,
 )
 
-
 class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
     pass
 
-
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "VisibilityConfig": VisibilityConfigTypeDef,
@@ -2304,21 +2535,19 @@
         "Description": str,
         "Rules": Sequence[RuleTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
-
 class UpdateRuleGroupRequestRequestTypeDef(
     _RequiredUpdateRuleGroupRequestRequestTypeDef, _OptionalUpdateRuleGroupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWebACLRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "DefaultAction": DefaultActionTypeDef,
@@ -2331,25 +2560,24 @@
     {
         "Description": str,
         "Rules": Sequence[RuleTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
+        "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateWebACLRequestRequestTypeDef(
     _RequiredUpdateWebACLRequestRequestTypeDef, _OptionalUpdateWebACLRequestRequestTypeDef
 ):
     pass
 
-
 FirewallManagerStatementTypeDef = TypedDict(
     "FirewallManagerStatementTypeDef",
     {
         "ManagedRuleGroupStatement": ManagedRuleGroupStatementTypeDef,
         "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
     },
     total=False,
@@ -2378,15 +2606,15 @@
 )
 
 GetRuleGroupResponseTypeDef = TypedDict(
     "GetRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
         "LockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FirewallManagerRuleGroupTypeDef = TypedDict(
     "FirewallManagerRuleGroupTypeDef",
     {
         "Name": str,
@@ -2417,33 +2645,32 @@
         "PostProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "ManagedByFirewallManager": bool,
         "LabelNamespace": str,
         "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": List[str],
+        "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
 )
 
-
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
 
-
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWebACLResponseTypeDef = TypedDict(
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "LockToken": str,
         "ApplicationIntegrationURL": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/type_defs.pyi` & `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/type_defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for wafv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_wafv2.type_defs import AWSManagedRulesBotControlRuleSetTypeDef
+    from mypy_boto3_wafv2.type_defs import APIKeySummaryTypeDef
 
-    data: AWSManagedRulesBotControlRuleSetTypeDef = {...}
+    data: APIKeySummaryTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -37,120 +37,147 @@
     PlatformType,
     PositionalConstraintType,
     RateBasedStatementAggregateKeyTypeType,
     ResourceTypeType,
     ResponseContentTypeType,
     ScopeType,
     SensitivityLevelType,
+    SizeInspectionLimitType,
     TextTransformationTypeType,
 )
 
 if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "APIKeySummaryTypeDef",
     "AWSManagedRulesBotControlRuleSetTypeDef",
     "ActionConditionTypeDef",
+    "AddressFieldTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
+    "RequestBodyAssociatedResourceTypeConfigTypeDef",
     "BodyTypeDef",
     "TextTransformationTypeDef",
     "ImmunityTimePropertyTypeDef",
     "CaptchaResponseTypeDef",
     "ChallengeResponseTypeDef",
-    "ResponseMetadataTypeDef",
+    "CheckCapacityResponseTypeDef",
     "LabelNameConditionTypeDef",
     "CookieMatchPatternTypeDef",
+    "CreateAPIKeyRequestRequestTypeDef",
+    "CreateAPIKeyResponseTypeDef",
     "TagTypeDef",
     "IPSetSummaryTypeDef",
     "RegexTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "CustomResponseBodyTypeDef",
     "VisibilityConfigTypeDef",
     "RuleGroupSummaryTypeDef",
     "WebACLSummaryTypeDef",
     "CustomHTTPHeaderTypeDef",
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
+    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
+    "DescribeAllManagedProductsRequestRequestTypeDef",
+    "ManagedProductDescriptorTypeDef",
+    "DescribeManagedProductsByVendorRequestRequestTypeDef",
     "DescribeManagedRuleGroupRequestRequestTypeDef",
     "LabelSummaryTypeDef",
     "DisassociateWebACLRequestRequestTypeDef",
+    "EmailFieldTypeDef",
     "ExcludedRuleTypeDef",
+    "HeaderOrderTypeDef",
     "SingleHeaderTypeDef",
     "SingleQueryArgumentTypeDef",
     "ForwardedIPConfigTypeDef",
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
+    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+    "GetDecryptedAPIKeyRequestRequestTypeDef",
+    "GetDecryptedAPIKeyResponseTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "IPSetTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetManagedRuleSetRequestRequestTypeDef",
     "GetMobileSdkReleaseRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
+    "GetPermissionPolicyResponseTypeDef",
     "GetRateBasedStatementManagedKeysRequestRequestTypeDef",
     "RateBasedStatementManagedKeysIPSetTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "TimeWindowTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
     "HeaderMatchPatternTypeDef",
     "IPSetForwardedIPConfigTypeDef",
     "JsonMatchPatternTypeDef",
     "LabelMatchStatementTypeDef",
     "LabelTypeDef",
+    "ListAPIKeysRequestRequestTypeDef",
     "ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef",
     "ManagedRuleGroupVersionTypeDef",
     "ListAvailableManagedRuleGroupsRequestRequestTypeDef",
     "ManagedRuleGroupSummaryTypeDef",
     "ListIPSetsRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
     "ListManagedRuleSetsRequestRequestTypeDef",
     "ManagedRuleSetSummaryTypeDef",
     "ListMobileSdkReleasesRequestRequestTypeDef",
     "ReleaseSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
+    "ListResourcesForWebACLResponseTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "PasswordFieldTypeDef",
     "UsernameFieldTypeDef",
     "ManagedRuleSetVersionTypeDef",
     "NotStatementTypeDef",
     "OrStatementTypeDef",
+    "PhoneNumberFieldTypeDef",
     "VersionToPublishTypeDef",
+    "PutManagedRuleSetVersionsResponseTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
+    "RateLimitLabelNamespaceTypeDef",
     "ResponseInspectionBodyContainsTypeDef",
     "ResponseInspectionHeaderTypeDef",
     "ResponseInspectionJsonTypeDef",
     "ResponseInspectionStatusCodeTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
-    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
-    "CaptchaConfigTypeDef",
-    "ChallengeConfigTypeDef",
-    "CheckCapacityResponseTypeDef",
-    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
-    "GenerateMobileSdkReleaseUrlResponseTypeDef",
-    "GetPermissionPolicyResponseTypeDef",
-    "ListResourcesForWebACLResponseTypeDef",
-    "PutManagedRuleSetVersionsResponseTypeDef",
     "UpdateIPSetResponseTypeDef",
+    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
     "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
     "UpdateRegexPatternSetResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
+    "ListAPIKeysResponseTypeDef",
+    "AssociationConfigTypeDef",
+    "RateLimitCookieTypeDef",
+    "RateLimitHeaderTypeDef",
+    "RateLimitQueryArgumentTypeDef",
+    "RateLimitQueryStringTypeDef",
+    "CaptchaConfigTypeDef",
+    "ChallengeConfigTypeDef",
     "ConditionTypeDef",
     "CookiesTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "MobileSdkReleaseTypeDef",
     "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIPSetResponseTypeDef",
@@ -162,44 +189,49 @@
     "ListRegexPatternSetsResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "ListWebACLsResponseTypeDef",
     "CustomRequestHandlingTypeDef",
     "CustomResponseTypeDef",
+    "DescribeAllManagedProductsResponseTypeDef",
+    "DescribeManagedProductsByVendorResponseTypeDef",
     "GeoMatchStatementTypeDef",
-    "RateBasedStatementTypeDef",
     "GetIPSetResponseTypeDef",
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
     "HeadersTypeDef",
     "IPSetReferenceStatementTypeDef",
     "JsonBodyTypeDef",
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     "ListManagedRuleSetsResponseTypeDef",
     "ListMobileSdkReleasesResponseTypeDef",
     "RequestInspectionTypeDef",
     "ManagedRuleSetTypeDef",
+    "RequestInspectionACFPTypeDef",
     "PutManagedRuleSetVersionsRequestRequestTypeDef",
     "ResponseInspectionTypeDef",
+    "RateBasedStatementCustomKeyTypeDef",
     "FilterTypeDef",
     "GetMobileSdkReleaseResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
     "AllowActionTypeDef",
     "CaptchaActionTypeDef",
     "ChallengeActionTypeDef",
     "CountActionTypeDef",
     "BlockActionTypeDef",
     "SampledHTTPRequestTypeDef",
     "FieldToMatchTypeDef",
     "GetManagedRuleSetResponseTypeDef",
+    "AWSManagedRulesACFPRuleSetTypeDef",
     "AWSManagedRulesATPRuleSetTypeDef",
+    "RateBasedStatementTypeDef",
     "LoggingFilterTypeDef",
     "OverrideActionTypeDef",
     "DefaultActionTypeDef",
     "RuleActionTypeDef",
     "GetSampledRequestsResponseTypeDef",
     "ByteMatchStatementTypeDef",
     "RegexMatchStatementTypeDef",
@@ -230,28 +262,46 @@
     "GetRuleGroupResponseTypeDef",
     "FirewallManagerRuleGroupTypeDef",
     "WebACLTypeDef",
     "GetWebACLForResourceResponseTypeDef",
     "GetWebACLResponseTypeDef",
 )
 
+APIKeySummaryTypeDef = TypedDict(
+    "APIKeySummaryTypeDef",
+    {
+        "TokenDomains": List[str],
+        "APIKey": str,
+        "CreationTimestamp": datetime,
+        "Version": int,
+    },
+    total=False,
+)
+
 AWSManagedRulesBotControlRuleSetTypeDef = TypedDict(
     "AWSManagedRulesBotControlRuleSetTypeDef",
     {
         "InspectionLevel": InspectionLevelType,
     },
 )
 
 ActionConditionTypeDef = TypedDict(
     "ActionConditionTypeDef",
     {
         "Action": ActionValueType,
     },
 )
 
+AddressFieldTypeDef = TypedDict(
+    "AddressFieldTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 AndStatementTypeDef = TypedDict(
     "AndStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
     },
 )
 
@@ -259,14 +309,21 @@
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLArn": str,
         "ResourceArn": str,
     },
 )
 
+RequestBodyAssociatedResourceTypeConfigTypeDef = TypedDict(
+    "RequestBodyAssociatedResourceTypeConfigTypeDef",
+    {
+        "DefaultSizeInspectionLimit": SizeInspectionLimitType,
+    },
+)
+
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
     total=False,
 )
@@ -302,22 +359,19 @@
         "ResponseCode": int,
         "SolveTimestamp": int,
         "FailureReason": FailureReasonType,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CheckCapacityResponseTypeDef = TypedDict(
+    "CheckCapacityResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Capacity": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LabelNameConditionTypeDef = TypedDict(
     "LabelNameConditionTypeDef",
     {
         "LabelName": str,
@@ -330,14 +384,30 @@
         "All": Mapping[str, Any],
         "IncludedCookies": Sequence[str],
         "ExcludedCookies": Sequence[str],
     },
     total=False,
 )
 
+CreateAPIKeyRequestRequestTypeDef = TypedDict(
+    "CreateAPIKeyRequestRequestTypeDef",
+    {
+        "Scope": ScopeType,
+        "TokenDomains": Sequence[str],
+    },
+)
+
+CreateAPIKeyResponseTypeDef = TypedDict(
+    "CreateAPIKeyResponseTypeDef",
+    {
+        "APIKey": str,
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
 )
@@ -427,14 +497,22 @@
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
     {
         "WebACLArn": str,
         "WebACLLockToken": str,
     },
 )
 
+DeleteFirewallManagerRuleGroupsResponseTypeDef = TypedDict(
+    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+    {
+        "NextWebACLLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteIPSetRequestRequestTypeDef = TypedDict(
     "DeleteIPSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "LockToken": str,
@@ -481,14 +559,45 @@
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "LockToken": str,
     },
 )
 
+DescribeAllManagedProductsRequestRequestTypeDef = TypedDict(
+    "DescribeAllManagedProductsRequestRequestTypeDef",
+    {
+        "Scope": ScopeType,
+    },
+)
+
+ManagedProductDescriptorTypeDef = TypedDict(
+    "ManagedProductDescriptorTypeDef",
+    {
+        "VendorName": str,
+        "ManagedRuleSetName": str,
+        "ProductId": str,
+        "ProductLink": str,
+        "ProductTitle": str,
+        "ProductDescription": str,
+        "SnsTopicArn": str,
+        "IsVersioningSupported": bool,
+        "IsAdvancedManagedRuleSet": bool,
+    },
+    total=False,
+)
+
+DescribeManagedProductsByVendorRequestRequestTypeDef = TypedDict(
+    "DescribeManagedProductsByVendorRequestRequestTypeDef",
+    {
+        "VendorName": str,
+        "Scope": ScopeType,
+    },
+)
+
 _RequiredDescribeManagedRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeManagedRuleGroupRequestRequestTypeDef",
     {
         "VendorName": str,
         "Name": str,
         "Scope": ScopeType,
     },
@@ -497,20 +606,22 @@
     "_OptionalDescribeManagedRuleGroupRequestRequestTypeDef",
     {
         "VersionName": str,
     },
     total=False,
 )
 
+
 class DescribeManagedRuleGroupRequestRequestTypeDef(
     _RequiredDescribeManagedRuleGroupRequestRequestTypeDef,
     _OptionalDescribeManagedRuleGroupRequestRequestTypeDef,
 ):
     pass
 
+
 LabelSummaryTypeDef = TypedDict(
     "LabelSummaryTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -518,21 +629,35 @@
 DisassociateWebACLRequestRequestTypeDef = TypedDict(
     "DisassociateWebACLRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+EmailFieldTypeDef = TypedDict(
+    "EmailFieldTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 ExcludedRuleTypeDef = TypedDict(
     "ExcludedRuleTypeDef",
     {
         "Name": str,
     },
 )
 
+HeaderOrderTypeDef = TypedDict(
+    "HeaderOrderTypeDef",
+    {
+        "OversizeHandling": OversizeHandlingType,
+    },
+)
+
 SingleHeaderTypeDef = TypedDict(
     "SingleHeaderTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -555,14 +680,39 @@
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
     {
         "Platform": PlatformType,
         "ReleaseVersion": str,
     },
 )
 
+GenerateMobileSdkReleaseUrlResponseTypeDef = TypedDict(
+    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDecryptedAPIKeyRequestRequestTypeDef = TypedDict(
+    "GetDecryptedAPIKeyRequestRequestTypeDef",
+    {
+        "Scope": ScopeType,
+        "APIKey": str,
+    },
+)
+
+GetDecryptedAPIKeyResponseTypeDef = TypedDict(
+    "GetDecryptedAPIKeyResponseTypeDef",
+    {
+        "TokenDomains": List[str],
+        "CreationTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetIPSetRequestRequestTypeDef = TypedDict(
     "GetIPSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
     },
@@ -582,17 +732,19 @@
     "_OptionalIPSetTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class IPSetTypeDef(_RequiredIPSetTypeDef, _OptionalIPSetTypeDef):
     pass
 
+
 GetLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetLoggingConfigurationRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -616,14 +768,22 @@
 GetPermissionPolicyRequestRequestTypeDef = TypedDict(
     "GetPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+GetPermissionPolicyResponseTypeDef = TypedDict(
+    "GetPermissionPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "WebACLName": str,
         "WebACLId": str,
         "RuleName": str,
@@ -633,20 +793,22 @@
     "_OptionalGetRateBasedStatementManagedKeysRequestRequestTypeDef",
     {
         "RuleGroupRuleName": str,
     },
     total=False,
 )
 
+
 class GetRateBasedStatementManagedKeysRequestRequestTypeDef(
     _RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef,
     _OptionalGetRateBasedStatementManagedKeysRequestRequestTypeDef,
 ):
     pass
 
+
 RateBasedStatementManagedKeysIPSetTypeDef = TypedDict(
     "RateBasedStatementManagedKeysIPSetTypeDef",
     {
         "IPAddressVersion": IPAddressVersionType,
         "Addresses": List[str],
     },
     total=False,
@@ -744,14 +906,36 @@
 LabelTypeDef = TypedDict(
     "LabelTypeDef",
     {
         "Name": str,
     },
 )
 
+_RequiredListAPIKeysRequestRequestTypeDef = TypedDict(
+    "_RequiredListAPIKeysRequestRequestTypeDef",
+    {
+        "Scope": ScopeType,
+    },
+)
+_OptionalListAPIKeysRequestRequestTypeDef = TypedDict(
+    "_OptionalListAPIKeysRequestRequestTypeDef",
+    {
+        "NextMarker": str,
+        "Limit": int,
+    },
+    total=False,
+)
+
+
+class ListAPIKeysRequestRequestTypeDef(
+    _RequiredListAPIKeysRequestRequestTypeDef, _OptionalListAPIKeysRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredListAvailableManagedRuleGroupVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableManagedRuleGroupVersionsRequestRequestTypeDef",
     {
         "VendorName": str,
         "Name": str,
         "Scope": ScopeType,
     },
@@ -761,20 +945,22 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef(
     _RequiredListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     _OptionalListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ManagedRuleGroupVersionTypeDef = TypedDict(
     "ManagedRuleGroupVersionTypeDef",
     {
         "Name": str,
         "LastUpdateTimestamp": datetime,
     },
     total=False,
@@ -791,20 +977,22 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListAvailableManagedRuleGroupsRequestRequestTypeDef(
     _RequiredListAvailableManagedRuleGroupsRequestRequestTypeDef,
     _OptionalListAvailableManagedRuleGroupsRequestRequestTypeDef,
 ):
     pass
 
+
 ManagedRuleGroupSummaryTypeDef = TypedDict(
     "ManagedRuleGroupSummaryTypeDef",
     {
         "VendorName": str,
         "Name": str,
         "VersioningSupported": bool,
         "Description": str,
@@ -823,19 +1011,21 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListIPSetsRequestRequestTypeDef(
     _RequiredListIPSetsRequestRequestTypeDef, _OptionalListIPSetsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListLoggingConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListLoggingConfigurationsRequestRequestTypeDef",
     {
         "Scope": ScopeType,
     },
 )
 _OptionalListLoggingConfigurationsRequestRequestTypeDef = TypedDict(
@@ -843,20 +1033,22 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListLoggingConfigurationsRequestRequestTypeDef(
     _RequiredListLoggingConfigurationsRequestRequestTypeDef,
     _OptionalListLoggingConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListManagedRuleSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedRuleSetsRequestRequestTypeDef",
     {
         "Scope": ScopeType,
     },
 )
 _OptionalListManagedRuleSetsRequestRequestTypeDef = TypedDict(
@@ -864,20 +1056,22 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListManagedRuleSetsRequestRequestTypeDef(
     _RequiredListManagedRuleSetsRequestRequestTypeDef,
     _OptionalListManagedRuleSetsRequestRequestTypeDef,
 ):
     pass
 
+
 ManagedRuleSetSummaryTypeDef = TypedDict(
     "ManagedRuleSetSummaryTypeDef",
     {
         "Name": str,
         "Id": str,
         "Description": str,
         "LockToken": str,
@@ -898,20 +1092,22 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListMobileSdkReleasesRequestRequestTypeDef(
     _RequiredListMobileSdkReleasesRequestRequestTypeDef,
     _OptionalListMobileSdkReleasesRequestRequestTypeDef,
 ):
     pass
 
+
 ReleaseSummaryTypeDef = TypedDict(
     "ReleaseSummaryTypeDef",
     {
         "ReleaseVersion": str,
         "Timestamp": datetime,
     },
     total=False,
@@ -928,40 +1124,52 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListRegexPatternSetsRequestRequestTypeDef(
     _RequiredListRegexPatternSetsRequestRequestTypeDef,
     _OptionalListRegexPatternSetsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListResourcesForWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesForWebACLRequestRequestTypeDef",
     {
         "WebACLArn": str,
     },
 )
 _OptionalListResourcesForWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalListResourcesForWebACLRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeType,
     },
     total=False,
 )
 
+
 class ListResourcesForWebACLRequestRequestTypeDef(
     _RequiredListResourcesForWebACLRequestRequestTypeDef,
     _OptionalListResourcesForWebACLRequestRequestTypeDef,
 ):
     pass
 
+
+ListResourcesForWebACLResponseTypeDef = TypedDict(
+    "ListResourcesForWebACLResponseTypeDef",
+    {
+        "ResourceArns": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListRuleGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListRuleGroupsRequestRequestTypeDef",
     {
         "Scope": ScopeType,
     },
 )
 _OptionalListRuleGroupsRequestRequestTypeDef = TypedDict(
@@ -969,19 +1177,21 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListRuleGroupsRequestRequestTypeDef(
     _RequiredListRuleGroupsRequestRequestTypeDef, _OptionalListRuleGroupsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -989,20 +1199,22 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListWebACLsRequestRequestTypeDef = TypedDict(
     "_RequiredListWebACLsRequestRequestTypeDef",
     {
         "Scope": ScopeType,
     },
 )
 _OptionalListWebACLsRequestRequestTypeDef = TypedDict(
@@ -1010,19 +1222,21 @@
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListWebACLsRequestRequestTypeDef(
     _RequiredListWebACLsRequestRequestTypeDef, _OptionalListWebACLsRequestRequestTypeDef
 ):
     pass
 
+
 PasswordFieldTypeDef = TypedDict(
     "PasswordFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -1056,31 +1270,53 @@
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
     },
 )
 
+PhoneNumberFieldTypeDef = TypedDict(
+    "PhoneNumberFieldTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 VersionToPublishTypeDef = TypedDict(
     "VersionToPublishTypeDef",
     {
         "AssociatedRuleGroupArn": str,
         "ForecastedLifetime": int,
     },
     total=False,
 )
 
+PutManagedRuleSetVersionsResponseTypeDef = TypedDict(
+    "PutManagedRuleSetVersionsResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutPermissionPolicyRequestRequestTypeDef = TypedDict(
     "PutPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
 
+RateLimitLabelNamespaceTypeDef = TypedDict(
+    "RateLimitLabelNamespaceTypeDef",
+    {
+        "Namespace": str,
+    },
+)
+
 ResponseInspectionBodyContainsTypeDef = TypedDict(
     "ResponseInspectionBodyContainsTypeDef",
     {
         "SuccessStrings": Sequence[str],
         "FailureStrings": Sequence[str],
     },
 )
@@ -1107,14 +1343,25 @@
     "ResponseInspectionStatusCodeTypeDef",
     {
         "SuccessCodes": Sequence[int],
         "FailureCodes": Sequence[int],
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1133,135 +1380,140 @@
     "_OptionalUpdateIPSetRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateIPSetRequestRequestTypeDef(
     _RequiredUpdateIPSetRequestRequestTypeDef, _OptionalUpdateIPSetRequestRequestTypeDef
 ):
     pass
 
+
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = TypedDict(
     "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "LockToken": str,
         "VersionToExpire": str,
         "ExpiryTimestamp": Union[datetime, str],
     },
 )
 
-CaptchaConfigTypeDef = TypedDict(
-    "CaptchaConfigTypeDef",
-    {
-        "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
-    },
-    total=False,
-)
-
-ChallengeConfigTypeDef = TypedDict(
-    "ChallengeConfigTypeDef",
+UpdateManagedRuleSetVersionExpiryDateResponseTypeDef = TypedDict(
+    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
     {
-        "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
+        "ExpiringVersion": str,
+        "ExpiryTimestamp": datetime,
+        "NextLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-CheckCapacityResponseTypeDef = TypedDict(
-    "CheckCapacityResponseTypeDef",
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
     {
-        "Capacity": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteFirewallManagerRuleGroupsResponseTypeDef = TypedDict(
-    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
     {
-        "NextWebACLLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GenerateMobileSdkReleaseUrlResponseTypeDef = TypedDict(
-    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+UpdateWebACLResponseTypeDef = TypedDict(
+    "UpdateWebACLResponseTypeDef",
     {
-        "Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextLockToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPermissionPolicyResponseTypeDef = TypedDict(
-    "GetPermissionPolicyResponseTypeDef",
+ListAPIKeysResponseTypeDef = TypedDict(
+    "ListAPIKeysResponseTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextMarker": str,
+        "APIKeySummaries": List[APIKeySummaryTypeDef],
+        "ApplicationIntegrationURL": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListResourcesForWebACLResponseTypeDef = TypedDict(
-    "ListResourcesForWebACLResponseTypeDef",
+AssociationConfigTypeDef = TypedDict(
+    "AssociationConfigTypeDef",
     {
-        "ResourceArns": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestBody": Mapping[
+            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef
+        ],
     },
+    total=False,
 )
 
-PutManagedRuleSetVersionsResponseTypeDef = TypedDict(
-    "PutManagedRuleSetVersionsResponseTypeDef",
+RateLimitCookieTypeDef = TypedDict(
+    "RateLimitCookieTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-UpdateIPSetResponseTypeDef = TypedDict(
-    "UpdateIPSetResponseTypeDef",
+RateLimitHeaderTypeDef = TypedDict(
+    "RateLimitHeaderTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-UpdateManagedRuleSetVersionExpiryDateResponseTypeDef = TypedDict(
-    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+RateLimitQueryArgumentTypeDef = TypedDict(
+    "RateLimitQueryArgumentTypeDef",
     {
-        "ExpiringVersion": str,
-        "ExpiryTimestamp": datetime,
-        "NextLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-UpdateRegexPatternSetResponseTypeDef = TypedDict(
-    "UpdateRegexPatternSetResponseTypeDef",
+RateLimitQueryStringTypeDef = TypedDict(
+    "RateLimitQueryStringTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+CaptchaConfigTypeDef = TypedDict(
+    "CaptchaConfigTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
     },
+    total=False,
 )
 
-UpdateWebACLResponseTypeDef = TypedDict(
-    "UpdateWebACLResponseTypeDef",
+ChallengeConfigTypeDef = TypedDict(
+    "ChallengeConfigTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
     },
+    total=False,
 )
 
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "ActionCondition": ActionConditionTypeDef,
         "LabelNameCondition": LabelNameConditionTypeDef,
@@ -1292,19 +1544,21 @@
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateIPSetRequestRequestTypeDef(
     _RequiredCreateIPSetRequestRequestTypeDef, _OptionalCreateIPSetRequestRequestTypeDef
 ):
     pass
 
+
 MobileSdkReleaseTypeDef = TypedDict(
     "MobileSdkReleaseTypeDef",
     {
         "ReleaseVersion": str,
         "Timestamp": datetime,
         "ReleaseNotes": str,
         "Tags": List[TagTypeDef],
@@ -1329,24 +1583,24 @@
     },
 )
 
 CreateIPSetResponseTypeDef = TypedDict(
     "CreateIPSetResponseTypeDef",
     {
         "Summary": IPSetSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIPSetsResponseTypeDef = TypedDict(
     "ListIPSetsResponseTypeDef",
     {
         "NextMarker": str,
         "IPSets": List[IPSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateRegexPatternSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRegexPatternSetRequestRequestTypeDef",
     {
         "Name": str,
@@ -1359,20 +1613,22 @@
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRegexPatternSetRequestRequestTypeDef(
     _RequiredCreateRegexPatternSetRequestRequestTypeDef,
     _OptionalCreateRegexPatternSetRequestRequestTypeDef,
 ):
     pass
 
+
 RegexPatternSetTypeDef = TypedDict(
     "RegexPatternSetTypeDef",
     {
         "Name": str,
         "Id": str,
         "ARN": str,
         "Description": str,
@@ -1395,68 +1651,70 @@
     "_OptionalUpdateRegexPatternSetRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateRegexPatternSetRequestRequestTypeDef(
     _RequiredUpdateRegexPatternSetRequestRequestTypeDef,
     _OptionalUpdateRegexPatternSetRequestRequestTypeDef,
 ):
     pass
 
+
 CreateRegexPatternSetResponseTypeDef = TypedDict(
     "CreateRegexPatternSetResponseTypeDef",
     {
         "Summary": RegexPatternSetSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRegexPatternSetsResponseTypeDef = TypedDict(
     "ListRegexPatternSetsResponseTypeDef",
     {
         "NextMarker": str,
         "RegexPatternSets": List[RegexPatternSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "Summary": RuleGroupSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[RuleGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "Summary": WebACLSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWebACLsResponseTypeDef = TypedDict(
     "ListWebACLsResponseTypeDef",
     {
         "NextMarker": str,
         "WebACLs": List[WebACLSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CustomRequestHandlingTypeDef = TypedDict(
     "CustomRequestHandlingTypeDef",
     {
         "InsertHeaders": Sequence[CustomHTTPHeaderTypeDef],
@@ -1474,62 +1732,59 @@
     {
         "CustomResponseBodyKey": str,
         "ResponseHeaders": Sequence[CustomHTTPHeaderTypeDef],
     },
     total=False,
 )
 
+
 class CustomResponseTypeDef(_RequiredCustomResponseTypeDef, _OptionalCustomResponseTypeDef):
     pass
 
-GeoMatchStatementTypeDef = TypedDict(
-    "GeoMatchStatementTypeDef",
+
+DescribeAllManagedProductsResponseTypeDef = TypedDict(
+    "DescribeAllManagedProductsResponseTypeDef",
     {
-        "CountryCodes": Sequence[CountryCodeType],
-        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
+        "ManagedProducts": List[ManagedProductDescriptorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredRateBasedStatementTypeDef = TypedDict(
-    "_RequiredRateBasedStatementTypeDef",
+DescribeManagedProductsByVendorResponseTypeDef = TypedDict(
+    "DescribeManagedProductsByVendorResponseTypeDef",
     {
-        "Limit": int,
-        "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
+        "ManagedProducts": List[ManagedProductDescriptorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalRateBasedStatementTypeDef = TypedDict(
-    "_OptionalRateBasedStatementTypeDef",
+
+GeoMatchStatementTypeDef = TypedDict(
+    "GeoMatchStatementTypeDef",
     {
-        "ScopeDownStatement": "StatementTypeDef",
+        "CountryCodes": Sequence[CountryCodeType],
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
     },
     total=False,
 )
 
-class RateBasedStatementTypeDef(
-    _RequiredRateBasedStatementTypeDef, _OptionalRateBasedStatementTypeDef
-):
-    pass
-
 GetIPSetResponseTypeDef = TypedDict(
     "GetIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRateBasedStatementManagedKeysResponseTypeDef = TypedDict(
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     {
         "ManagedKeysIPV4": RateBasedStatementManagedKeysIPSetTypeDef,
         "ManagedKeysIPV6": RateBasedStatementManagedKeysIPSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSampledRequestsRequestRequestTypeDef = TypedDict(
     "GetSampledRequestsRequestRequestTypeDef",
     {
         "WebAclArn": str,
@@ -1572,19 +1827,21 @@
     "_OptionalIPSetReferenceStatementTypeDef",
     {
         "IPSetForwardedIPConfig": IPSetForwardedIPConfigTypeDef,
     },
     total=False,
 )
 
+
 class IPSetReferenceStatementTypeDef(
     _RequiredIPSetReferenceStatementTypeDef, _OptionalIPSetReferenceStatementTypeDef
 ):
     pass
 
+
 _RequiredJsonBodyTypeDef = TypedDict(
     "_RequiredJsonBodyTypeDef",
     {
         "MatchPattern": JsonMatchPatternTypeDef,
         "MatchScope": JsonMatchScopeType,
     },
 )
@@ -1593,51 +1850,53 @@
     {
         "InvalidFallbackBehavior": BodyParsingFallbackBehaviorType,
         "OversizeHandling": OversizeHandlingType,
     },
     total=False,
 )
 
+
 class JsonBodyTypeDef(_RequiredJsonBodyTypeDef, _OptionalJsonBodyTypeDef):
     pass
 
+
 ListAvailableManagedRuleGroupVersionsResponseTypeDef = TypedDict(
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     {
         "NextMarker": str,
         "Versions": List[ManagedRuleGroupVersionTypeDef],
         "CurrentDefaultVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAvailableManagedRuleGroupsResponseTypeDef = TypedDict(
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "ManagedRuleGroups": List[ManagedRuleGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListManagedRuleSetsResponseTypeDef = TypedDict(
     "ListManagedRuleSetsResponseTypeDef",
     {
         "NextMarker": str,
         "ManagedRuleSets": List[ManagedRuleSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMobileSdkReleasesResponseTypeDef = TypedDict(
     "ListMobileSdkReleasesResponseTypeDef",
     {
         "ReleaseSummaries": List[ReleaseSummaryTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RequestInspectionTypeDef = TypedDict(
     "RequestInspectionTypeDef",
     {
         "PayloadType": PayloadTypeType,
@@ -1661,17 +1920,44 @@
         "PublishedVersions": Dict[str, ManagedRuleSetVersionTypeDef],
         "RecommendedVersion": str,
         "LabelNamespace": str,
     },
     total=False,
 )
 
+
 class ManagedRuleSetTypeDef(_RequiredManagedRuleSetTypeDef, _OptionalManagedRuleSetTypeDef):
     pass
 
+
+_RequiredRequestInspectionACFPTypeDef = TypedDict(
+    "_RequiredRequestInspectionACFPTypeDef",
+    {
+        "PayloadType": PayloadTypeType,
+    },
+)
+_OptionalRequestInspectionACFPTypeDef = TypedDict(
+    "_OptionalRequestInspectionACFPTypeDef",
+    {
+        "UsernameField": UsernameFieldTypeDef,
+        "PasswordField": PasswordFieldTypeDef,
+        "EmailField": EmailFieldTypeDef,
+        "PhoneNumberFields": Sequence[PhoneNumberFieldTypeDef],
+        "AddressFields": Sequence[AddressFieldTypeDef],
+    },
+    total=False,
+)
+
+
+class RequestInspectionACFPTypeDef(
+    _RequiredRequestInspectionACFPTypeDef, _OptionalRequestInspectionACFPTypeDef
+):
+    pass
+
+
 _RequiredPutManagedRuleSetVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutManagedRuleSetVersionsRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "LockToken": str,
@@ -1682,63 +1968,80 @@
     {
         "RecommendedVersion": str,
         "VersionsToPublish": Mapping[str, VersionToPublishTypeDef],
     },
     total=False,
 )
 
+
 class PutManagedRuleSetVersionsRequestRequestTypeDef(
     _RequiredPutManagedRuleSetVersionsRequestRequestTypeDef,
     _OptionalPutManagedRuleSetVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ResponseInspectionTypeDef = TypedDict(
     "ResponseInspectionTypeDef",
     {
         "StatusCode": ResponseInspectionStatusCodeTypeDef,
         "Header": ResponseInspectionHeaderTypeDef,
         "BodyContains": ResponseInspectionBodyContainsTypeDef,
         "Json": ResponseInspectionJsonTypeDef,
     },
     total=False,
 )
 
+RateBasedStatementCustomKeyTypeDef = TypedDict(
+    "RateBasedStatementCustomKeyTypeDef",
+    {
+        "Header": RateLimitHeaderTypeDef,
+        "Cookie": RateLimitCookieTypeDef,
+        "QueryArgument": RateLimitQueryArgumentTypeDef,
+        "QueryString": RateLimitQueryStringTypeDef,
+        "HTTPMethod": Mapping[str, Any],
+        "ForwardedIP": Mapping[str, Any],
+        "IP": Mapping[str, Any],
+        "LabelNamespace": RateLimitLabelNamespaceTypeDef,
+    },
+    total=False,
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Behavior": FilterBehaviorType,
         "Requirement": FilterRequirementType,
         "Conditions": List[ConditionTypeDef],
     },
 )
 
 GetMobileSdkReleaseResponseTypeDef = TypedDict(
     "GetMobileSdkReleaseResponseTypeDef",
     {
         "MobileSdkRelease": MobileSdkReleaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextMarker": str,
         "TagInfoForResource": TagInfoForResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRegexPatternSetResponseTypeDef = TypedDict(
     "GetRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AllowActionTypeDef = TypedDict(
     "AllowActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
@@ -1797,65 +2100,119 @@
         "CaptchaResponse": CaptchaResponseTypeDef,
         "ChallengeResponse": ChallengeResponseTypeDef,
         "OverriddenAction": str,
     },
     total=False,
 )
 
+
 class SampledHTTPRequestTypeDef(
     _RequiredSampledHTTPRequestTypeDef, _OptionalSampledHTTPRequestTypeDef
 ):
     pass
 
+
 FieldToMatchTypeDef = TypedDict(
     "FieldToMatchTypeDef",
     {
         "SingleHeader": SingleHeaderTypeDef,
         "SingleQueryArgument": SingleQueryArgumentTypeDef,
         "AllQueryArguments": Mapping[str, Any],
         "UriPath": Mapping[str, Any],
         "QueryString": Mapping[str, Any],
         "Body": BodyTypeDef,
         "Method": Mapping[str, Any],
         "JsonBody": JsonBodyTypeDef,
         "Headers": HeadersTypeDef,
         "Cookies": CookiesTypeDef,
+        "HeaderOrder": HeaderOrderTypeDef,
     },
     total=False,
 )
 
 GetManagedRuleSetResponseTypeDef = TypedDict(
     "GetManagedRuleSetResponseTypeDef",
     {
         "ManagedRuleSet": ManagedRuleSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredAWSManagedRulesACFPRuleSetTypeDef = TypedDict(
+    "_RequiredAWSManagedRulesACFPRuleSetTypeDef",
+    {
+        "CreationPath": str,
+        "RegistrationPagePath": str,
+        "RequestInspection": RequestInspectionACFPTypeDef,
+    },
+)
+_OptionalAWSManagedRulesACFPRuleSetTypeDef = TypedDict(
+    "_OptionalAWSManagedRulesACFPRuleSetTypeDef",
+    {
+        "ResponseInspection": ResponseInspectionTypeDef,
+        "EnableRegexInPath": bool,
     },
+    total=False,
 )
 
+
+class AWSManagedRulesACFPRuleSetTypeDef(
+    _RequiredAWSManagedRulesACFPRuleSetTypeDef, _OptionalAWSManagedRulesACFPRuleSetTypeDef
+):
+    pass
+
+
 _RequiredAWSManagedRulesATPRuleSetTypeDef = TypedDict(
     "_RequiredAWSManagedRulesATPRuleSetTypeDef",
     {
         "LoginPath": str,
     },
 )
 _OptionalAWSManagedRulesATPRuleSetTypeDef = TypedDict(
     "_OptionalAWSManagedRulesATPRuleSetTypeDef",
     {
         "RequestInspection": RequestInspectionTypeDef,
         "ResponseInspection": ResponseInspectionTypeDef,
+        "EnableRegexInPath": bool,
     },
     total=False,
 )
 
+
 class AWSManagedRulesATPRuleSetTypeDef(
     _RequiredAWSManagedRulesATPRuleSetTypeDef, _OptionalAWSManagedRulesATPRuleSetTypeDef
 ):
     pass
 
+
+_RequiredRateBasedStatementTypeDef = TypedDict(
+    "_RequiredRateBasedStatementTypeDef",
+    {
+        "Limit": int,
+        "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
+    },
+)
+_OptionalRateBasedStatementTypeDef = TypedDict(
+    "_OptionalRateBasedStatementTypeDef",
+    {
+        "ScopeDownStatement": "StatementTypeDef",
+        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
+        "CustomKeys": Sequence[RateBasedStatementCustomKeyTypeDef],
+    },
+    total=False,
+)
+
+
+class RateBasedStatementTypeDef(
+    _RequiredRateBasedStatementTypeDef, _OptionalRateBasedStatementTypeDef
+):
+    pass
+
+
 LoggingFilterTypeDef = TypedDict(
     "LoggingFilterTypeDef",
     {
         "Filters": List[FilterTypeDef],
         "DefaultBehavior": FilterBehaviorType,
     },
 )
@@ -1892,15 +2249,15 @@
 
 GetSampledRequestsResponseTypeDef = TypedDict(
     "GetSampledRequestsResponseTypeDef",
     {
         "SampledRequests": List[SampledHTTPRequestTypeDef],
         "PopulationSize": int,
         "TimeWindow": TimeWindowTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ByteMatchStatementTypeDef = TypedDict(
     "ByteMatchStatementTypeDef",
     {
         "SearchString": Union[str, bytes, IO[Any], StreamingBody],
@@ -1949,19 +2306,21 @@
     "_OptionalSqliMatchStatementTypeDef",
     {
         "SensitivityLevel": SensitivityLevelType,
     },
     total=False,
 )
 
+
 class SqliMatchStatementTypeDef(
     _RequiredSqliMatchStatementTypeDef, _OptionalSqliMatchStatementTypeDef
 ):
     pass
 
+
 XssMatchStatementTypeDef = TypedDict(
     "XssMatchStatementTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
@@ -1971,14 +2330,15 @@
     {
         "LoginPath": str,
         "PayloadType": PayloadTypeType,
         "UsernameField": UsernameFieldTypeDef,
         "PasswordField": PasswordFieldTypeDef,
         "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
         "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetTypeDef,
+        "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetTypeDef,
     },
     total=False,
 )
 
 _RequiredLoggingConfigurationTypeDef = TypedDict(
     "_RequiredLoggingConfigurationTypeDef",
     {
@@ -1992,19 +2352,21 @@
         "RedactedFields": List[FieldToMatchTypeDef],
         "ManagedByFirewallManager": bool,
         "LoggingFilter": LoggingFilterTypeDef,
     },
     total=False,
 )
 
+
 class LoggingConfigurationTypeDef(
     _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
 ):
     pass
 
+
 RuleActionOverrideTypeDef = TypedDict(
     "RuleActionOverrideTypeDef",
     {
         "Name": str,
         "ActionToUse": RuleActionTypeDef,
     },
 )
@@ -2035,46 +2397,48 @@
         "RuleLabels": Sequence[LabelTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
     },
     total=False,
 )
 
+
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
+
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
         "LoggingConfigurations": List[LoggingConfigurationTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutLoggingConfigurationRequestRequestTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
 PutLoggingConfigurationResponseTypeDef = TypedDict(
     "PutLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredManagedRuleGroupStatementTypeDef = TypedDict(
     "_RequiredManagedRuleGroupStatementTypeDef",
     {
         "VendorName": str,
@@ -2089,19 +2453,21 @@
         "ScopeDownStatement": "StatementTypeDef",
         "ManagedRuleGroupConfigs": Sequence[ManagedRuleGroupConfigTypeDef],
         "RuleActionOverrides": Sequence[RuleActionOverrideTypeDef],
     },
     total=False,
 )
 
+
 class ManagedRuleGroupStatementTypeDef(
     _RequiredManagedRuleGroupStatementTypeDef, _OptionalManagedRuleGroupStatementTypeDef
 ):
     pass
 
+
 _RequiredRuleGroupReferenceStatementTypeDef = TypedDict(
     "_RequiredRuleGroupReferenceStatementTypeDef",
     {
         "ARN": str,
     },
 )
 _OptionalRuleGroupReferenceStatementTypeDef = TypedDict(
@@ -2109,30 +2475,32 @@
     {
         "ExcludedRules": Sequence[ExcludedRuleTypeDef],
         "RuleActionOverrides": Sequence[RuleActionOverrideTypeDef],
     },
     total=False,
 )
 
+
 class RuleGroupReferenceStatementTypeDef(
     _RequiredRuleGroupReferenceStatementTypeDef, _OptionalRuleGroupReferenceStatementTypeDef
 ):
     pass
 
+
 DescribeManagedRuleGroupResponseTypeDef = TypedDict(
     "DescribeManagedRuleGroupResponseTypeDef",
     {
         "VersionName": str,
         "SnsTopicArn": str,
         "Capacity": int,
         "Rules": List[RuleSummaryTypeDef],
         "LabelNamespace": str,
         "AvailableLabels": List[LabelSummaryTypeDef],
         "ConsumedLabels": List[LabelSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CheckCapacityRequestRequestTypeDef = TypedDict(
     "CheckCapacityRequestRequestTypeDef",
     {
         "Scope": ScopeType,
@@ -2156,19 +2524,21 @@
         "Rules": Sequence[RuleTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
+
 class CreateRuleGroupRequestRequestTypeDef(
     _RequiredCreateRuleGroupRequestRequestTypeDef, _OptionalCreateRuleGroupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWebACLRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "DefaultAction": DefaultActionTypeDef,
         "VisibilityConfig": VisibilityConfigTypeDef,
@@ -2180,23 +2550,26 @@
         "Description": str,
         "Rules": Sequence[RuleTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
+        "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
 )
 
+
 class CreateWebACLRequestRequestTypeDef(
     _RequiredCreateWebACLRequestRequestTypeDef, _OptionalCreateWebACLRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredRuleGroupTypeDef = TypedDict(
     "_RequiredRuleGroupTypeDef",
     {
         "Name": str,
         "Id": str,
         "Capacity": int,
         "ARN": str,
@@ -2212,17 +2585,19 @@
         "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
         "AvailableLabels": List[LabelSummaryTypeDef],
         "ConsumedLabels": List[LabelSummaryTypeDef],
     },
     total=False,
 )
 
+
 class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
     pass
 
+
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "VisibilityConfig": VisibilityConfigTypeDef,
@@ -2235,19 +2610,21 @@
         "Description": str,
         "Rules": Sequence[RuleTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
+
 class UpdateRuleGroupRequestRequestTypeDef(
     _RequiredUpdateRuleGroupRequestRequestTypeDef, _OptionalUpdateRuleGroupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWebACLRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "DefaultAction": DefaultActionTypeDef,
@@ -2260,23 +2637,26 @@
     {
         "Description": str,
         "Rules": Sequence[RuleTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
+        "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateWebACLRequestRequestTypeDef(
     _RequiredUpdateWebACLRequestRequestTypeDef, _OptionalUpdateWebACLRequestRequestTypeDef
 ):
     pass
 
+
 FirewallManagerStatementTypeDef = TypedDict(
     "FirewallManagerStatementTypeDef",
     {
         "ManagedRuleGroupStatement": ManagedRuleGroupStatementTypeDef,
         "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
     },
     total=False,
@@ -2305,15 +2685,15 @@
 )
 
 GetRuleGroupResponseTypeDef = TypedDict(
     "GetRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
         "LockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FirewallManagerRuleGroupTypeDef = TypedDict(
     "FirewallManagerRuleGroupTypeDef",
     {
         "Name": str,
@@ -2344,31 +2724,34 @@
         "PostProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "ManagedByFirewallManager": bool,
         "LabelNamespace": str,
         "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": List[str],
+        "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
 )
 
+
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
 
+
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWebACLResponseTypeDef = TypedDict(
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "LockToken": str,
         "ApplicationIntegrationURL": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/SOURCES.txt` & `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.26.78/setup.py` & `mypy-boto3-wafv2-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-wafv2.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wafv2",
-    version="1.26.78",
+    version="1.27.0",
     packages=["mypy_boto3_wafv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAFV2 1.26.78 service generated with mypy-boto3-builder 7.12.4"
+        "Type annotations for boto3.WAFV2 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -44,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/",
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


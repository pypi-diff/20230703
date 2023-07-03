# Comparing `tmp/mypy-boto3-waf-regional-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-waf-regional-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-waf-regional-1.26.0.post1.tar", last modified: Tue Nov  1 21:44:06 2022, max compression
+gzip compressed data, was "mypy-boto3-waf-regional-1.27.0.tar", last modified: Mon Jul  3 19:51:35 2023, max compression
```

## Comparing `mypy-boto3-waf-regional-1.26.0.post1.tar` & `mypy-boto3-waf-regional-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:06.868855 mypy-boto3-waf-regional-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:42:22.000000 mypy-boto3-waf-regional-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    20392 2022-11-01 21:44:06.860855 mypy-boto3-waf-regional-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18932 2022-11-01 21:42:22.000000 mypy-boto3-waf-regional-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:06.856855 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-11-01 21:42:22.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-11-01 21:42:22.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-11-01 21:42:22.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    46208 2022-11-01 21:42:22.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    46120 2022-11-01 21:42:22.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11315 2022-11-01 21:42:23.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    11313 2022-11-01 21:42:22.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:42:22.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    55338 2022-11-01 21:42:24.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    55291 2022-11-01 21:42:23.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:42:22.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:06.860855 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    20392 2022-11-01 21:44:06.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-11-01 21:44:06.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:06.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:06.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:44:06.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-01 21:44:06.000000 mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:44:06.868855 mypy-boto3-waf-regional-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-11-01 21:42:22.000000 mypy-boto3-waf-regional-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.732135 mypy-boto3-waf-regional-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-07-03 19:51:35.732135 mypy-boto3-waf-regional-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.728135 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55486 2023-07-03 19:49:30.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55439 2023-07-03 19:49:29.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.732135 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-07-03 19:51:35.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 19:51:35.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:35.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:51:35.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:35.732135 mypy-boto3-waf-regional-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/setup.py
```

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/LICENSE` & `mypy-boto3-waf-regional-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/PKG-INFO` & `mypy-boto3-waf-regional-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf-regional
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.WAFRegional 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.WAFRegional 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/
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
 
 <a id="mypy-boto3-waf-regional"></a>
 
 # mypy-boto3-waf-regional
 
 [![PyPI - mypy-boto3-waf-regional](https://img.shields.io/pypi/v/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-waf-regional?color=blue)](https://pypistats.org/packages/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,50 +318,66 @@
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
     ByteMatchSetSummaryTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
     RegexPatternSetTypeDef,
     RuleGroupTypeDef,
     CreateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateWebACLMigrationStackRequestRequestTypeDef,
+    CreateWebACLMigrationStackResponseTypeDef,
     CreateXssMatchSetRequestRequestTypeDef,
     DeleteByteMatchSetRequestRequestTypeDef,
+    DeleteByteMatchSetResponseTypeDef,
     DeleteGeoMatchSetRequestRequestTypeDef,
+    DeleteGeoMatchSetResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
+    DeleteIPSetResponseTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRateBasedRuleRequestRequestTypeDef,
+    DeleteRateBasedRuleResponseTypeDef,
     DeleteRegexMatchSetRequestRequestTypeDef,
+    DeleteRegexMatchSetResponseTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
+    DeleteRegexPatternSetResponseTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
+    DeleteRuleGroupResponseTypeDef,
     DeleteRuleRequestRequestTypeDef,
+    DeleteRuleResponseTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
+    DeleteSizeConstraintSetResponseTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
+    DeleteSqlInjectionMatchSetResponseTypeDef,
     DeleteWebACLRequestRequestTypeDef,
+    DeleteWebACLResponseTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
+    DeleteXssMatchSetResponseTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
+    GetChangeTokenResponseTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
+    GetChangeTokenStatusResponseTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
+    GetPermissionPolicyResponseTypeDef,
     GetRateBasedRuleManagedKeysRequestRequestTypeDef,
+    GetRateBasedRuleManagedKeysResponseTypeDef,
     GetRateBasedRuleRequestRequestTypeDef,
     GetRegexMatchSetRequestRequestTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
     TimeWindowTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
@@ -380,14 +397,15 @@
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
+    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
     ListRulesRequestRequestTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
@@ -396,53 +414,36 @@
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ActivatedRuleTypeDef,
-    ByteMatchTupleTypeDef,
-    LoggingConfigurationTypeDef,
-    RegexMatchTupleTypeDef,
-    SizeConstraintTypeDef,
-    SqlInjectionMatchTupleTypeDef,
-    XssMatchTupleTypeDef,
-    CreateWebACLMigrationStackResponseTypeDef,
-    DeleteByteMatchSetResponseTypeDef,
-    DeleteGeoMatchSetResponseTypeDef,
-    DeleteIPSetResponseTypeDef,
-    DeleteRateBasedRuleResponseTypeDef,
-    DeleteRegexMatchSetResponseTypeDef,
-    DeleteRegexPatternSetResponseTypeDef,
-    DeleteRuleGroupResponseTypeDef,
-    DeleteRuleResponseTypeDef,
-    DeleteSizeConstraintSetResponseTypeDef,
-    DeleteSqlInjectionMatchSetResponseTypeDef,
-    DeleteWebACLResponseTypeDef,
-    DeleteXssMatchSetResponseTypeDef,
-    GetChangeTokenResponseTypeDef,
-    GetChangeTokenStatusResponseTypeDef,
-    GetPermissionPolicyResponseTypeDef,
-    GetRateBasedRuleManagedKeysResponseTypeDef,
-    ListByteMatchSetsResponseTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateSizeConstraintSetResponseTypeDef,
     UpdateSqlInjectionMatchSetResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     UpdateXssMatchSetResponseTypeDef,
+    ActivatedRuleTypeDef,
+    ListByteMatchSetsResponseTypeDef,
+    ByteMatchTupleTypeDef,
+    LoggingConfigurationTypeDef,
+    RegexMatchTupleTypeDef,
+    SizeConstraintTypeDef,
+    SqlInjectionMatchTupleTypeDef,
+    XssMatchTupleTypeDef,
     CreateRateBasedRuleRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
     TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
@@ -534,42 +535,42 @@
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

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/README.md` & `mypy-boto3-waf-regional-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-waf-regional"></a>
 
 # mypy-boto3-waf-regional
 
 [![PyPI - mypy-boto3-waf-regional](https://img.shields.io/pypi/v/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-waf-regional?color=blue)](https://pypistats.org/packages/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,50 +286,66 @@
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
     ByteMatchSetSummaryTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
     RegexPatternSetTypeDef,
     RuleGroupTypeDef,
     CreateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateWebACLMigrationStackRequestRequestTypeDef,
+    CreateWebACLMigrationStackResponseTypeDef,
     CreateXssMatchSetRequestRequestTypeDef,
     DeleteByteMatchSetRequestRequestTypeDef,
+    DeleteByteMatchSetResponseTypeDef,
     DeleteGeoMatchSetRequestRequestTypeDef,
+    DeleteGeoMatchSetResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
+    DeleteIPSetResponseTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRateBasedRuleRequestRequestTypeDef,
+    DeleteRateBasedRuleResponseTypeDef,
     DeleteRegexMatchSetRequestRequestTypeDef,
+    DeleteRegexMatchSetResponseTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
+    DeleteRegexPatternSetResponseTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
+    DeleteRuleGroupResponseTypeDef,
     DeleteRuleRequestRequestTypeDef,
+    DeleteRuleResponseTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
+    DeleteSizeConstraintSetResponseTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
+    DeleteSqlInjectionMatchSetResponseTypeDef,
     DeleteWebACLRequestRequestTypeDef,
+    DeleteWebACLResponseTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
+    DeleteXssMatchSetResponseTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
+    GetChangeTokenResponseTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
+    GetChangeTokenStatusResponseTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
+    GetPermissionPolicyResponseTypeDef,
     GetRateBasedRuleManagedKeysRequestRequestTypeDef,
+    GetRateBasedRuleManagedKeysResponseTypeDef,
     GetRateBasedRuleRequestRequestTypeDef,
     GetRegexMatchSetRequestRequestTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
     TimeWindowTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
@@ -349,14 +365,15 @@
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
+    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
     ListRulesRequestRequestTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
@@ -365,53 +382,36 @@
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ActivatedRuleTypeDef,
-    ByteMatchTupleTypeDef,
-    LoggingConfigurationTypeDef,
-    RegexMatchTupleTypeDef,
-    SizeConstraintTypeDef,
-    SqlInjectionMatchTupleTypeDef,
-    XssMatchTupleTypeDef,
-    CreateWebACLMigrationStackResponseTypeDef,
-    DeleteByteMatchSetResponseTypeDef,
-    DeleteGeoMatchSetResponseTypeDef,
-    DeleteIPSetResponseTypeDef,
-    DeleteRateBasedRuleResponseTypeDef,
-    DeleteRegexMatchSetResponseTypeDef,
-    DeleteRegexPatternSetResponseTypeDef,
-    DeleteRuleGroupResponseTypeDef,
-    DeleteRuleResponseTypeDef,
-    DeleteSizeConstraintSetResponseTypeDef,
-    DeleteSqlInjectionMatchSetResponseTypeDef,
-    DeleteWebACLResponseTypeDef,
-    DeleteXssMatchSetResponseTypeDef,
-    GetChangeTokenResponseTypeDef,
-    GetChangeTokenStatusResponseTypeDef,
-    GetPermissionPolicyResponseTypeDef,
-    GetRateBasedRuleManagedKeysResponseTypeDef,
-    ListByteMatchSetsResponseTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateSizeConstraintSetResponseTypeDef,
     UpdateSqlInjectionMatchSetResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     UpdateXssMatchSetResponseTypeDef,
+    ActivatedRuleTypeDef,
+    ListByteMatchSetsResponseTypeDef,
+    ByteMatchTupleTypeDef,
+    LoggingConfigurationTypeDef,
+    RegexMatchTupleTypeDef,
+    SizeConstraintTypeDef,
+    SqlInjectionMatchTupleTypeDef,
+    XssMatchTupleTypeDef,
     CreateRateBasedRuleRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
     TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
@@ -503,42 +503,42 @@
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

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/__main__.py` & `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFRegional 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.WAFRegional 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/client.py` & `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/client.pyi` & `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/literals.py` & `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -333,23 +333,25 @@
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
@@ -359,30 +361,35 @@
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
@@ -408,14 +415,15 @@
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
@@ -460,51 +468,57 @@
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
@@ -517,14 +531,15 @@
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
@@ -536,28 +551,35 @@
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
@@ -566,14 +588,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -584,55 +607,64 @@
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
@@ -657,24 +689,29 @@
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

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/literals.pyi` & `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -331,23 +331,25 @@
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
@@ -357,30 +359,35 @@
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
@@ -406,14 +413,15 @@
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
@@ -458,51 +466,57 @@
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
@@ -515,14 +529,15 @@
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
@@ -534,28 +549,35 @@
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
@@ -564,14 +586,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -582,55 +605,64 @@
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
@@ -655,24 +687,29 @@
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

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/type_defs.py` & `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,50 +45,66 @@
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
     "CreateRegexMatchSetRequestRequestTypeDef",
     "CreateRegexPatternSetRequestRequestTypeDef",
     "RegexPatternSetTypeDef",
     "RuleGroupTypeDef",
     "CreateSizeConstraintSetRequestRequestTypeDef",
     "CreateSqlInjectionMatchSetRequestRequestTypeDef",
     "CreateWebACLMigrationStackRequestRequestTypeDef",
+    "CreateWebACLMigrationStackResponseTypeDef",
     "CreateXssMatchSetRequestRequestTypeDef",
     "DeleteByteMatchSetRequestRequestTypeDef",
+    "DeleteByteMatchSetResponseTypeDef",
     "DeleteGeoMatchSetRequestRequestTypeDef",
+    "DeleteGeoMatchSetResponseTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
+    "DeleteIPSetResponseTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRateBasedRuleRequestRequestTypeDef",
+    "DeleteRateBasedRuleResponseTypeDef",
     "DeleteRegexMatchSetRequestRequestTypeDef",
+    "DeleteRegexMatchSetResponseTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
+    "DeleteRegexPatternSetResponseTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
+    "DeleteRuleGroupResponseTypeDef",
     "DeleteRuleRequestRequestTypeDef",
+    "DeleteRuleResponseTypeDef",
     "DeleteSizeConstraintSetRequestRequestTypeDef",
+    "DeleteSizeConstraintSetResponseTypeDef",
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
+    "DeleteSqlInjectionMatchSetResponseTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
+    "DeleteWebACLResponseTypeDef",
     "DeleteXssMatchSetRequestRequestTypeDef",
+    "DeleteXssMatchSetResponseTypeDef",
     "DisassociateWebACLRequestRequestTypeDef",
     "GeoMatchConstraintTypeDef",
     "GeoMatchSetSummaryTypeDef",
     "GetByteMatchSetRequestRequestTypeDef",
+    "GetChangeTokenResponseTypeDef",
     "GetChangeTokenStatusRequestRequestTypeDef",
+    "GetChangeTokenStatusResponseTypeDef",
     "GetGeoMatchSetRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
+    "GetPermissionPolicyResponseTypeDef",
     "GetRateBasedRuleManagedKeysRequestRequestTypeDef",
+    "GetRateBasedRuleManagedKeysResponseTypeDef",
     "GetRateBasedRuleRequestRequestTypeDef",
     "GetRegexMatchSetRequestRequestTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
     "TimeWindowTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
@@ -108,14 +124,15 @@
     "ListRateBasedRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
     "ListRegexMatchSetsRequestRequestTypeDef",
     "RegexMatchSetSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
+    "ListResourcesForWebACLResponseTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupSummaryTypeDef",
     "ListRulesRequestRequestTypeDef",
     "ListSizeConstraintSetsRequestRequestTypeDef",
     "SizeConstraintSetSummaryTypeDef",
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     "SqlInjectionMatchSetSummaryTypeDef",
@@ -124,53 +141,36 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
     "PredicateTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RegexPatternSetUpdateTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ActivatedRuleTypeDef",
-    "ByteMatchTupleTypeDef",
-    "LoggingConfigurationTypeDef",
-    "RegexMatchTupleTypeDef",
-    "SizeConstraintTypeDef",
-    "SqlInjectionMatchTupleTypeDef",
-    "XssMatchTupleTypeDef",
-    "CreateWebACLMigrationStackResponseTypeDef",
-    "DeleteByteMatchSetResponseTypeDef",
-    "DeleteGeoMatchSetResponseTypeDef",
-    "DeleteIPSetResponseTypeDef",
-    "DeleteRateBasedRuleResponseTypeDef",
-    "DeleteRegexMatchSetResponseTypeDef",
-    "DeleteRegexPatternSetResponseTypeDef",
-    "DeleteRuleGroupResponseTypeDef",
-    "DeleteRuleResponseTypeDef",
-    "DeleteSizeConstraintSetResponseTypeDef",
-    "DeleteSqlInjectionMatchSetResponseTypeDef",
-    "DeleteWebACLResponseTypeDef",
-    "DeleteXssMatchSetResponseTypeDef",
-    "GetChangeTokenResponseTypeDef",
-    "GetChangeTokenStatusResponseTypeDef",
-    "GetPermissionPolicyResponseTypeDef",
-    "GetRateBasedRuleManagedKeysResponseTypeDef",
-    "ListByteMatchSetsResponseTypeDef",
-    "ListResourcesForWebACLResponseTypeDef",
     "UpdateByteMatchSetResponseTypeDef",
     "UpdateGeoMatchSetResponseTypeDef",
     "UpdateIPSetResponseTypeDef",
     "UpdateRateBasedRuleResponseTypeDef",
     "UpdateRegexMatchSetResponseTypeDef",
     "UpdateRegexPatternSetResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "UpdateRuleResponseTypeDef",
     "UpdateSizeConstraintSetResponseTypeDef",
     "UpdateSqlInjectionMatchSetResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
     "UpdateXssMatchSetResponseTypeDef",
+    "ActivatedRuleTypeDef",
+    "ListByteMatchSetsResponseTypeDef",
+    "ByteMatchTupleTypeDef",
+    "LoggingConfigurationTypeDef",
+    "RegexMatchTupleTypeDef",
+    "SizeConstraintTypeDef",
+    "SqlInjectionMatchTupleTypeDef",
+    "XssMatchTupleTypeDef",
     "CreateRateBasedRuleRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
     "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
@@ -314,25 +314,14 @@
     "CreateByteMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
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
 CreateGeoMatchSetRequestRequestTypeDef = TypedDict(
     "CreateGeoMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
@@ -430,14 +419,22 @@
     {
         "WebACLId": str,
         "S3BucketName": str,
         "IgnoreUnsupportedType": bool,
     },
 )
 
+CreateWebACLMigrationStackResponseTypeDef = TypedDict(
+    "CreateWebACLMigrationStackResponseTypeDef",
+    {
+        "S3ObjectUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateXssMatchSetRequestRequestTypeDef = TypedDict(
     "CreateXssMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
@@ -446,30 +443,54 @@
     "DeleteByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteByteMatchSetResponseTypeDef = TypedDict(
+    "DeleteByteMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteGeoMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteGeoMatchSetResponseTypeDef = TypedDict(
+    "DeleteGeoMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteIPSetRequestRequestTypeDef = TypedDict(
     "DeleteIPSetRequestRequestTypeDef",
     {
         "IPSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteIPSetResponseTypeDef = TypedDict(
+    "DeleteIPSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -484,78 +505,150 @@
     "DeleteRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteRateBasedRuleResponseTypeDef = TypedDict(
+    "DeleteRateBasedRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRegexMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteRegexMatchSetRequestRequestTypeDef",
     {
         "RegexMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteRegexMatchSetResponseTypeDef = TypedDict(
+    "DeleteRegexMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRegexPatternSetRequestRequestTypeDef = TypedDict(
     "DeleteRegexPatternSetRequestRequestTypeDef",
     {
         "RegexPatternSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteRegexPatternSetResponseTypeDef = TypedDict(
+    "DeleteRegexPatternSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRuleGroupRequestRequestTypeDef = TypedDict(
     "DeleteRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteRuleGroupResponseTypeDef = TypedDict(
+    "DeleteRuleGroupResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "RuleId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteRuleResponseTypeDef = TypedDict(
+    "DeleteRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "DeleteSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteSizeConstraintSetResponseTypeDef = TypedDict(
+    "DeleteSizeConstraintSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
     {
         "SqlInjectionMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteSqlInjectionMatchSetResponseTypeDef = TypedDict(
+    "DeleteSqlInjectionMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteWebACLRequestRequestTypeDef = TypedDict(
     "DeleteWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteWebACLResponseTypeDef = TypedDict(
+    "DeleteWebACLResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteXssMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteXssMatchSetResponseTypeDef = TypedDict(
+    "DeleteXssMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateWebACLRequestRequestTypeDef = TypedDict(
     "DisassociateWebACLRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -578,21 +671,37 @@
 GetByteMatchSetRequestRequestTypeDef = TypedDict(
     "GetByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
     },
 )
 
+GetChangeTokenResponseTypeDef = TypedDict(
+    "GetChangeTokenResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetChangeTokenStatusRequestRequestTypeDef = TypedDict(
     "GetChangeTokenStatusRequestRequestTypeDef",
     {
         "ChangeToken": str,
     },
 )
 
+GetChangeTokenStatusResponseTypeDef = TypedDict(
+    "GetChangeTokenStatusResponseTypeDef",
+    {
+        "ChangeTokenStatus": ChangeTokenStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetGeoMatchSetRequestRequestTypeDef = TypedDict(
     "GetGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
     },
 )
 
@@ -613,14 +722,22 @@
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
 _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
@@ -635,14 +752,23 @@
 class GetRateBasedRuleManagedKeysRequestRequestTypeDef(
     _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef,
     _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef,
 ):
     pass
 
 
+GetRateBasedRuleManagedKeysResponseTypeDef = TypedDict(
+    "GetRateBasedRuleManagedKeysResponseTypeDef",
+    {
+        "ManagedKeys": List[str],
+        "NextMarker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRateBasedRuleRequestRequestTypeDef = TypedDict(
     "GetRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 
@@ -865,14 +991,22 @@
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
+
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1017,359 +1151,225 @@
     "RegexPatternSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "RegexPatternString": str,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
-    },
-)
-
-_RequiredActivatedRuleTypeDef = TypedDict(
-    "_RequiredActivatedRuleTypeDef",
-    {
-        "Priority": int,
-        "RuleId": str,
-    },
-)
-_OptionalActivatedRuleTypeDef = TypedDict(
-    "_OptionalActivatedRuleTypeDef",
-    {
-        "Action": WafActionTypeDef,
-        "OverrideAction": WafOverrideActionTypeDef,
-        "Type": WafRuleTypeType,
-        "ExcludedRules": List[ExcludedRuleTypeDef],
-    },
-    total=False,
-)
-
-
-class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
-    pass
-
-
-ByteMatchTupleTypeDef = TypedDict(
-    "ByteMatchTupleTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": bytes,
-        "TextTransformation": TextTransformationType,
-        "PositionalConstraint": PositionalConstraintType,
-    },
-)
-
-_RequiredLoggingConfigurationTypeDef = TypedDict(
-    "_RequiredLoggingConfigurationTypeDef",
-    {
-        "ResourceArn": str,
-        "LogDestinationConfigs": List[str],
-    },
-)
-_OptionalLoggingConfigurationTypeDef = TypedDict(
-    "_OptionalLoggingConfigurationTypeDef",
-    {
-        "RedactedFields": List[FieldToMatchTypeDef],
-    },
-    total=False,
-)
-
-
-class LoggingConfigurationTypeDef(
-    _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
-):
-    pass
-
-
-RegexMatchTupleTypeDef = TypedDict(
-    "RegexMatchTupleTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
-        "RegexPatternSetId": str,
-    },
-)
-
-SizeConstraintTypeDef = TypedDict(
-    "SizeConstraintTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
-        "ComparisonOperator": ComparisonOperatorType,
-        "Size": int,
-    },
-)
-
-SqlInjectionMatchTupleTypeDef = TypedDict(
-    "SqlInjectionMatchTupleTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
-    },
-)
-
-XssMatchTupleTypeDef = TypedDict(
-    "XssMatchTupleTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-CreateWebACLMigrationStackResponseTypeDef = TypedDict(
-    "CreateWebACLMigrationStackResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "S3ObjectUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-DeleteByteMatchSetResponseTypeDef = TypedDict(
-    "DeleteByteMatchSetResponseTypeDef",
+UpdateByteMatchSetResponseTypeDef = TypedDict(
+    "UpdateByteMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteGeoMatchSetResponseTypeDef = TypedDict(
-    "DeleteGeoMatchSetResponseTypeDef",
+UpdateGeoMatchSetResponseTypeDef = TypedDict(
+    "UpdateGeoMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteIPSetResponseTypeDef = TypedDict(
-    "DeleteIPSetResponseTypeDef",
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRateBasedRuleResponseTypeDef = TypedDict(
-    "DeleteRateBasedRuleResponseTypeDef",
+UpdateRateBasedRuleResponseTypeDef = TypedDict(
+    "UpdateRateBasedRuleResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRegexMatchSetResponseTypeDef = TypedDict(
-    "DeleteRegexMatchSetResponseTypeDef",
+UpdateRegexMatchSetResponseTypeDef = TypedDict(
+    "UpdateRegexMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRegexPatternSetResponseTypeDef = TypedDict(
-    "DeleteRegexPatternSetResponseTypeDef",
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRuleGroupResponseTypeDef = TypedDict(
-    "DeleteRuleGroupResponseTypeDef",
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRuleResponseTypeDef = TypedDict(
-    "DeleteRuleResponseTypeDef",
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteSizeConstraintSetResponseTypeDef = TypedDict(
-    "DeleteSizeConstraintSetResponseTypeDef",
+UpdateSizeConstraintSetResponseTypeDef = TypedDict(
+    "UpdateSizeConstraintSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteSqlInjectionMatchSetResponseTypeDef = TypedDict(
-    "DeleteSqlInjectionMatchSetResponseTypeDef",
+UpdateSqlInjectionMatchSetResponseTypeDef = TypedDict(
+    "UpdateSqlInjectionMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteWebACLResponseTypeDef = TypedDict(
-    "DeleteWebACLResponseTypeDef",
+UpdateWebACLResponseTypeDef = TypedDict(
+    "UpdateWebACLResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteXssMatchSetResponseTypeDef = TypedDict(
-    "DeleteXssMatchSetResponseTypeDef",
+UpdateXssMatchSetResponseTypeDef = TypedDict(
+    "UpdateXssMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetChangeTokenResponseTypeDef = TypedDict(
-    "GetChangeTokenResponseTypeDef",
+_RequiredActivatedRuleTypeDef = TypedDict(
+    "_RequiredActivatedRuleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Priority": int,
+        "RuleId": str,
     },
 )
-
-GetChangeTokenStatusResponseTypeDef = TypedDict(
-    "GetChangeTokenStatusResponseTypeDef",
+_OptionalActivatedRuleTypeDef = TypedDict(
+    "_OptionalActivatedRuleTypeDef",
     {
-        "ChangeTokenStatus": ChangeTokenStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Action": WafActionTypeDef,
+        "OverrideAction": WafOverrideActionTypeDef,
+        "Type": WafRuleTypeType,
+        "ExcludedRules": List[ExcludedRuleTypeDef],
     },
+    total=False,
 )
 
-GetPermissionPolicyResponseTypeDef = TypedDict(
-    "GetPermissionPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-GetRateBasedRuleManagedKeysResponseTypeDef = TypedDict(
-    "GetRateBasedRuleManagedKeysResponseTypeDef",
-    {
-        "ManagedKeys": List[str],
-        "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
+    pass
+
 
 ListByteMatchSetsResponseTypeDef = TypedDict(
     "ListByteMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "ByteMatchSets": List[ByteMatchSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListResourcesForWebACLResponseTypeDef = TypedDict(
-    "ListResourcesForWebACLResponseTypeDef",
-    {
-        "ResourceArns": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateByteMatchSetResponseTypeDef = TypedDict(
-    "UpdateByteMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateGeoMatchSetResponseTypeDef = TypedDict(
-    "UpdateGeoMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateIPSetResponseTypeDef = TypedDict(
-    "UpdateIPSetResponseTypeDef",
+ByteMatchTupleTypeDef = TypedDict(
+    "ByteMatchTupleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TargetString": bytes,
+        "TextTransformation": TextTransformationType,
+        "PositionalConstraint": PositionalConstraintType,
     },
 )
 
-UpdateRateBasedRuleResponseTypeDef = TypedDict(
-    "UpdateRateBasedRuleResponseTypeDef",
+_RequiredLoggingConfigurationTypeDef = TypedDict(
+    "_RequiredLoggingConfigurationTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "LogDestinationConfigs": List[str],
     },
 )
-
-UpdateRegexMatchSetResponseTypeDef = TypedDict(
-    "UpdateRegexMatchSetResponseTypeDef",
+_OptionalLoggingConfigurationTypeDef = TypedDict(
+    "_OptionalLoggingConfigurationTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RedactedFields": List[FieldToMatchTypeDef],
     },
+    total=False,
 )
 
-UpdateRegexPatternSetResponseTypeDef = TypedDict(
-    "UpdateRegexPatternSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class LoggingConfigurationTypeDef(
+    _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
+):
+    pass
 
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateSizeConstraintSetResponseTypeDef = TypedDict(
-    "UpdateSizeConstraintSetResponseTypeDef",
+RegexMatchTupleTypeDef = TypedDict(
+    "RegexMatchTupleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
+        "RegexPatternSetId": str,
     },
 )
 
-UpdateSqlInjectionMatchSetResponseTypeDef = TypedDict(
-    "UpdateSqlInjectionMatchSetResponseTypeDef",
+SizeConstraintTypeDef = TypedDict(
+    "SizeConstraintTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Size": int,
     },
 )
 
-UpdateWebACLResponseTypeDef = TypedDict(
-    "UpdateWebACLResponseTypeDef",
+SqlInjectionMatchTupleTypeDef = TypedDict(
+    "SqlInjectionMatchTupleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
     },
 )
 
-UpdateXssMatchSetResponseTypeDef = TypedDict(
-    "UpdateXssMatchSetResponseTypeDef",
+XssMatchTupleTypeDef = TypedDict(
+    "XssMatchTupleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
     },
 )
 
 _RequiredCreateRateBasedRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRateBasedRuleRequestRequestTypeDef",
     {
         "Name": str,
@@ -1483,40 +1483,40 @@
 )
 
 CreateRegexPatternSetResponseTypeDef = TypedDict(
     "CreateRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRegexPatternSetResponseTypeDef = TypedDict(
     "GetRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRuleGroupResponseTypeDef = TypedDict(
     "GetRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGeoMatchSetTypeDef = TypedDict(
     "_RequiredGeoMatchSetTypeDef",
     {
         "GeoMatchSetId": str,
@@ -1545,15 +1545,15 @@
 )
 
 ListGeoMatchSetsResponseTypeDef = TypedDict(
     "ListGeoMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "GeoMatchSets": List[GeoMatchSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSampledRequestsRequestRequestTypeDef = TypedDict(
     "GetSampledRequestsRequestRequestTypeDef",
     {
         "WebAclId": str,
@@ -1563,24 +1563,24 @@
     },
 )
 
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACLSummary": WebACLSummaryTypeDef,
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
 
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
@@ -1622,96 +1622,96 @@
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
 
 ListRateBasedRulesResponseTypeDef = TypedDict(
     "ListRateBasedRulesResponseTypeDef",
     {
         "NextMarker": str,
         "Rules": List[RuleSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "NextMarker": str,
         "Rules": List[RuleSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRegexMatchSetsResponseTypeDef = TypedDict(
     "ListRegexMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "RegexMatchSets": List[RegexMatchSetSummaryTypeDef],
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
 
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[RuleGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSizeConstraintSetsResponseTypeDef = TypedDict(
     "ListSizeConstraintSetsResponseTypeDef",
     {
         "NextMarker": str,
         "SizeConstraintSets": List[SizeConstraintSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSqlInjectionMatchSetsResponseTypeDef = TypedDict(
     "ListSqlInjectionMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "SqlInjectionMatchSets": List[SqlInjectionMatchSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSubscribedRuleGroupsResponseTypeDef = TypedDict(
     "ListSubscribedRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[SubscribedRuleGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListXssMatchSetsResponseTypeDef = TypedDict(
     "ListXssMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "XssMatchSets": List[XssMatchSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRateBasedRuleTypeDef = TypedDict(
     "_RequiredRateBasedRuleTypeDef",
     {
         "RuleId": str,
@@ -1773,15 +1773,15 @@
 )
 
 ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
     "ListActivatedRulesInRuleGroupResponseTypeDef",
     {
         "NextMarker": str,
         "ActivatedRules": List[ActivatedRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleGroupUpdateTypeDef = TypedDict(
     "RuleGroupUpdateTypeDef",
     {
         "Action": ChangeActionType,
@@ -1848,39 +1848,39 @@
     },
 )
 
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
 
 RegexMatchSetTypeDef = TypedDict(
     "RegexMatchSetTypeDef",
     {
         "RegexMatchSetId": str,
@@ -1987,32 +1987,32 @@
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
 
 CreateGeoMatchSetResponseTypeDef = TypedDict(
     "CreateGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGeoMatchSetResponseTypeDef = TypedDict(
     "GetGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGeoMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
@@ -2046,23 +2046,23 @@
 
 
 CreateIPSetResponseTypeDef = TypedDict(
     "CreateIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIPSetResponseTypeDef = TypedDict(
     "GetIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateIPSetRequestRequestTypeDef = TypedDict(
     "UpdateIPSetRequestRequestTypeDef",
     {
         "IPSetId": str,
@@ -2072,40 +2072,40 @@
 )
 
 CreateRateBasedRuleResponseTypeDef = TypedDict(
     "CreateRateBasedRuleResponseTypeDef",
     {
         "Rule": RateBasedRuleTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRateBasedRuleResponseTypeDef = TypedDict(
     "GetRateBasedRuleResponseTypeDef",
     {
         "Rule": RateBasedRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRateBasedRuleRequestRequestTypeDef = TypedDict(
     "UpdateRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
@@ -2134,23 +2134,23 @@
 )
 
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWebACLResponseTypeDef = TypedDict(
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
@@ -2174,23 +2174,23 @@
 
 
 CreateByteMatchSetResponseTypeDef = TypedDict(
     "CreateByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetByteMatchSetResponseTypeDef = TypedDict(
     "GetByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateByteMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
@@ -2200,23 +2200,23 @@
 )
 
 CreateRegexMatchSetResponseTypeDef = TypedDict(
     "CreateRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRegexMatchSetResponseTypeDef = TypedDict(
     "GetRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRegexMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateRegexMatchSetRequestRequestTypeDef",
     {
         "RegexMatchSetId": str,
@@ -2226,23 +2226,23 @@
 )
 
 CreateSizeConstraintSetResponseTypeDef = TypedDict(
     "CreateSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSizeConstraintSetResponseTypeDef = TypedDict(
     "GetSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "UpdateSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
@@ -2252,23 +2252,23 @@
 )
 
 CreateSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "CreateSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "GetSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
     {
         "SqlInjectionMatchSetId": str,
@@ -2278,23 +2278,23 @@
 )
 
 CreateXssMatchSetResponseTypeDef = TypedDict(
     "CreateXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetXssMatchSetResponseTypeDef = TypedDict(
     "GetXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateXssMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
@@ -2305,10 +2305,10 @@
 
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
```

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional/type_defs.pyi` & `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,50 +44,66 @@
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
     "CreateRegexMatchSetRequestRequestTypeDef",
     "CreateRegexPatternSetRequestRequestTypeDef",
     "RegexPatternSetTypeDef",
     "RuleGroupTypeDef",
     "CreateSizeConstraintSetRequestRequestTypeDef",
     "CreateSqlInjectionMatchSetRequestRequestTypeDef",
     "CreateWebACLMigrationStackRequestRequestTypeDef",
+    "CreateWebACLMigrationStackResponseTypeDef",
     "CreateXssMatchSetRequestRequestTypeDef",
     "DeleteByteMatchSetRequestRequestTypeDef",
+    "DeleteByteMatchSetResponseTypeDef",
     "DeleteGeoMatchSetRequestRequestTypeDef",
+    "DeleteGeoMatchSetResponseTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
+    "DeleteIPSetResponseTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRateBasedRuleRequestRequestTypeDef",
+    "DeleteRateBasedRuleResponseTypeDef",
     "DeleteRegexMatchSetRequestRequestTypeDef",
+    "DeleteRegexMatchSetResponseTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
+    "DeleteRegexPatternSetResponseTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
+    "DeleteRuleGroupResponseTypeDef",
     "DeleteRuleRequestRequestTypeDef",
+    "DeleteRuleResponseTypeDef",
     "DeleteSizeConstraintSetRequestRequestTypeDef",
+    "DeleteSizeConstraintSetResponseTypeDef",
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
+    "DeleteSqlInjectionMatchSetResponseTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
+    "DeleteWebACLResponseTypeDef",
     "DeleteXssMatchSetRequestRequestTypeDef",
+    "DeleteXssMatchSetResponseTypeDef",
     "DisassociateWebACLRequestRequestTypeDef",
     "GeoMatchConstraintTypeDef",
     "GeoMatchSetSummaryTypeDef",
     "GetByteMatchSetRequestRequestTypeDef",
+    "GetChangeTokenResponseTypeDef",
     "GetChangeTokenStatusRequestRequestTypeDef",
+    "GetChangeTokenStatusResponseTypeDef",
     "GetGeoMatchSetRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
+    "GetPermissionPolicyResponseTypeDef",
     "GetRateBasedRuleManagedKeysRequestRequestTypeDef",
+    "GetRateBasedRuleManagedKeysResponseTypeDef",
     "GetRateBasedRuleRequestRequestTypeDef",
     "GetRegexMatchSetRequestRequestTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
     "TimeWindowTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
@@ -107,14 +123,15 @@
     "ListRateBasedRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
     "ListRegexMatchSetsRequestRequestTypeDef",
     "RegexMatchSetSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
+    "ListResourcesForWebACLResponseTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupSummaryTypeDef",
     "ListRulesRequestRequestTypeDef",
     "ListSizeConstraintSetsRequestRequestTypeDef",
     "SizeConstraintSetSummaryTypeDef",
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     "SqlInjectionMatchSetSummaryTypeDef",
@@ -123,53 +140,36 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
     "PredicateTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RegexPatternSetUpdateTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ActivatedRuleTypeDef",
-    "ByteMatchTupleTypeDef",
-    "LoggingConfigurationTypeDef",
-    "RegexMatchTupleTypeDef",
-    "SizeConstraintTypeDef",
-    "SqlInjectionMatchTupleTypeDef",
-    "XssMatchTupleTypeDef",
-    "CreateWebACLMigrationStackResponseTypeDef",
-    "DeleteByteMatchSetResponseTypeDef",
-    "DeleteGeoMatchSetResponseTypeDef",
-    "DeleteIPSetResponseTypeDef",
-    "DeleteRateBasedRuleResponseTypeDef",
-    "DeleteRegexMatchSetResponseTypeDef",
-    "DeleteRegexPatternSetResponseTypeDef",
-    "DeleteRuleGroupResponseTypeDef",
-    "DeleteRuleResponseTypeDef",
-    "DeleteSizeConstraintSetResponseTypeDef",
-    "DeleteSqlInjectionMatchSetResponseTypeDef",
-    "DeleteWebACLResponseTypeDef",
-    "DeleteXssMatchSetResponseTypeDef",
-    "GetChangeTokenResponseTypeDef",
-    "GetChangeTokenStatusResponseTypeDef",
-    "GetPermissionPolicyResponseTypeDef",
-    "GetRateBasedRuleManagedKeysResponseTypeDef",
-    "ListByteMatchSetsResponseTypeDef",
-    "ListResourcesForWebACLResponseTypeDef",
     "UpdateByteMatchSetResponseTypeDef",
     "UpdateGeoMatchSetResponseTypeDef",
     "UpdateIPSetResponseTypeDef",
     "UpdateRateBasedRuleResponseTypeDef",
     "UpdateRegexMatchSetResponseTypeDef",
     "UpdateRegexPatternSetResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "UpdateRuleResponseTypeDef",
     "UpdateSizeConstraintSetResponseTypeDef",
     "UpdateSqlInjectionMatchSetResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
     "UpdateXssMatchSetResponseTypeDef",
+    "ActivatedRuleTypeDef",
+    "ListByteMatchSetsResponseTypeDef",
+    "ByteMatchTupleTypeDef",
+    "LoggingConfigurationTypeDef",
+    "RegexMatchTupleTypeDef",
+    "SizeConstraintTypeDef",
+    "SqlInjectionMatchTupleTypeDef",
+    "XssMatchTupleTypeDef",
     "CreateRateBasedRuleRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
     "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
@@ -311,25 +311,14 @@
     "CreateByteMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
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
 CreateGeoMatchSetRequestRequestTypeDef = TypedDict(
     "CreateGeoMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
@@ -423,14 +412,22 @@
     {
         "WebACLId": str,
         "S3BucketName": str,
         "IgnoreUnsupportedType": bool,
     },
 )
 
+CreateWebACLMigrationStackResponseTypeDef = TypedDict(
+    "CreateWebACLMigrationStackResponseTypeDef",
+    {
+        "S3ObjectUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateXssMatchSetRequestRequestTypeDef = TypedDict(
     "CreateXssMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
@@ -439,30 +436,54 @@
     "DeleteByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteByteMatchSetResponseTypeDef = TypedDict(
+    "DeleteByteMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteGeoMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteGeoMatchSetResponseTypeDef = TypedDict(
+    "DeleteGeoMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteIPSetRequestRequestTypeDef = TypedDict(
     "DeleteIPSetRequestRequestTypeDef",
     {
         "IPSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteIPSetResponseTypeDef = TypedDict(
+    "DeleteIPSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -477,78 +498,150 @@
     "DeleteRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteRateBasedRuleResponseTypeDef = TypedDict(
+    "DeleteRateBasedRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRegexMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteRegexMatchSetRequestRequestTypeDef",
     {
         "RegexMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteRegexMatchSetResponseTypeDef = TypedDict(
+    "DeleteRegexMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRegexPatternSetRequestRequestTypeDef = TypedDict(
     "DeleteRegexPatternSetRequestRequestTypeDef",
     {
         "RegexPatternSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteRegexPatternSetResponseTypeDef = TypedDict(
+    "DeleteRegexPatternSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRuleGroupRequestRequestTypeDef = TypedDict(
     "DeleteRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteRuleGroupResponseTypeDef = TypedDict(
+    "DeleteRuleGroupResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "RuleId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteRuleResponseTypeDef = TypedDict(
+    "DeleteRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "DeleteSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteSizeConstraintSetResponseTypeDef = TypedDict(
+    "DeleteSizeConstraintSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
     {
         "SqlInjectionMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteSqlInjectionMatchSetResponseTypeDef = TypedDict(
+    "DeleteSqlInjectionMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteWebACLRequestRequestTypeDef = TypedDict(
     "DeleteWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteWebACLResponseTypeDef = TypedDict(
+    "DeleteWebACLResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteXssMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
+DeleteXssMatchSetResponseTypeDef = TypedDict(
+    "DeleteXssMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateWebACLRequestRequestTypeDef = TypedDict(
     "DisassociateWebACLRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -571,21 +664,37 @@
 GetByteMatchSetRequestRequestTypeDef = TypedDict(
     "GetByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
     },
 )
 
+GetChangeTokenResponseTypeDef = TypedDict(
+    "GetChangeTokenResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetChangeTokenStatusRequestRequestTypeDef = TypedDict(
     "GetChangeTokenStatusRequestRequestTypeDef",
     {
         "ChangeToken": str,
     },
 )
 
+GetChangeTokenStatusResponseTypeDef = TypedDict(
+    "GetChangeTokenStatusResponseTypeDef",
+    {
+        "ChangeTokenStatus": ChangeTokenStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetGeoMatchSetRequestRequestTypeDef = TypedDict(
     "GetGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
     },
 )
 
@@ -606,14 +715,22 @@
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
 _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
@@ -626,14 +743,23 @@
 
 class GetRateBasedRuleManagedKeysRequestRequestTypeDef(
     _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef,
     _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef,
 ):
     pass
 
+GetRateBasedRuleManagedKeysResponseTypeDef = TypedDict(
+    "GetRateBasedRuleManagedKeysResponseTypeDef",
+    {
+        "ManagedKeys": List[str],
+        "NextMarker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRateBasedRuleRequestRequestTypeDef = TypedDict(
     "GetRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 
@@ -854,14 +980,22 @@
 
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
+
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1004,355 +1138,221 @@
     "RegexPatternSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "RegexPatternString": str,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
-    },
-)
-
-_RequiredActivatedRuleTypeDef = TypedDict(
-    "_RequiredActivatedRuleTypeDef",
-    {
-        "Priority": int,
-        "RuleId": str,
-    },
-)
-_OptionalActivatedRuleTypeDef = TypedDict(
-    "_OptionalActivatedRuleTypeDef",
-    {
-        "Action": WafActionTypeDef,
-        "OverrideAction": WafOverrideActionTypeDef,
-        "Type": WafRuleTypeType,
-        "ExcludedRules": List[ExcludedRuleTypeDef],
-    },
-    total=False,
-)
-
-class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
-    pass
-
-ByteMatchTupleTypeDef = TypedDict(
-    "ByteMatchTupleTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": bytes,
-        "TextTransformation": TextTransformationType,
-        "PositionalConstraint": PositionalConstraintType,
-    },
-)
-
-_RequiredLoggingConfigurationTypeDef = TypedDict(
-    "_RequiredLoggingConfigurationTypeDef",
-    {
-        "ResourceArn": str,
-        "LogDestinationConfigs": List[str],
-    },
-)
-_OptionalLoggingConfigurationTypeDef = TypedDict(
-    "_OptionalLoggingConfigurationTypeDef",
-    {
-        "RedactedFields": List[FieldToMatchTypeDef],
-    },
-    total=False,
-)
-
-class LoggingConfigurationTypeDef(
-    _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
-):
-    pass
-
-RegexMatchTupleTypeDef = TypedDict(
-    "RegexMatchTupleTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
-        "RegexPatternSetId": str,
-    },
-)
-
-SizeConstraintTypeDef = TypedDict(
-    "SizeConstraintTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
-        "ComparisonOperator": ComparisonOperatorType,
-        "Size": int,
-    },
-)
-
-SqlInjectionMatchTupleTypeDef = TypedDict(
-    "SqlInjectionMatchTupleTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
-    },
-)
-
-XssMatchTupleTypeDef = TypedDict(
-    "XssMatchTupleTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
-    },
-)
-
-CreateWebACLMigrationStackResponseTypeDef = TypedDict(
-    "CreateWebACLMigrationStackResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "S3ObjectUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-DeleteByteMatchSetResponseTypeDef = TypedDict(
-    "DeleteByteMatchSetResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-DeleteGeoMatchSetResponseTypeDef = TypedDict(
-    "DeleteGeoMatchSetResponseTypeDef",
+UpdateByteMatchSetResponseTypeDef = TypedDict(
+    "UpdateByteMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteIPSetResponseTypeDef = TypedDict(
-    "DeleteIPSetResponseTypeDef",
+UpdateGeoMatchSetResponseTypeDef = TypedDict(
+    "UpdateGeoMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRateBasedRuleResponseTypeDef = TypedDict(
-    "DeleteRateBasedRuleResponseTypeDef",
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRegexMatchSetResponseTypeDef = TypedDict(
-    "DeleteRegexMatchSetResponseTypeDef",
+UpdateRateBasedRuleResponseTypeDef = TypedDict(
+    "UpdateRateBasedRuleResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRegexPatternSetResponseTypeDef = TypedDict(
-    "DeleteRegexPatternSetResponseTypeDef",
+UpdateRegexMatchSetResponseTypeDef = TypedDict(
+    "UpdateRegexMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRuleGroupResponseTypeDef = TypedDict(
-    "DeleteRuleGroupResponseTypeDef",
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRuleResponseTypeDef = TypedDict(
-    "DeleteRuleResponseTypeDef",
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteSizeConstraintSetResponseTypeDef = TypedDict(
-    "DeleteSizeConstraintSetResponseTypeDef",
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteSqlInjectionMatchSetResponseTypeDef = TypedDict(
-    "DeleteSqlInjectionMatchSetResponseTypeDef",
+UpdateSizeConstraintSetResponseTypeDef = TypedDict(
+    "UpdateSizeConstraintSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteWebACLResponseTypeDef = TypedDict(
-    "DeleteWebACLResponseTypeDef",
+UpdateSqlInjectionMatchSetResponseTypeDef = TypedDict(
+    "UpdateSqlInjectionMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteXssMatchSetResponseTypeDef = TypedDict(
-    "DeleteXssMatchSetResponseTypeDef",
+UpdateWebACLResponseTypeDef = TypedDict(
+    "UpdateWebACLResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetChangeTokenResponseTypeDef = TypedDict(
-    "GetChangeTokenResponseTypeDef",
+UpdateXssMatchSetResponseTypeDef = TypedDict(
+    "UpdateXssMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetChangeTokenStatusResponseTypeDef = TypedDict(
-    "GetChangeTokenStatusResponseTypeDef",
+_RequiredActivatedRuleTypeDef = TypedDict(
+    "_RequiredActivatedRuleTypeDef",
     {
-        "ChangeTokenStatus": ChangeTokenStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Priority": int,
+        "RuleId": str,
     },
 )
-
-GetPermissionPolicyResponseTypeDef = TypedDict(
-    "GetPermissionPolicyResponseTypeDef",
+_OptionalActivatedRuleTypeDef = TypedDict(
+    "_OptionalActivatedRuleTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Action": WafActionTypeDef,
+        "OverrideAction": WafOverrideActionTypeDef,
+        "Type": WafRuleTypeType,
+        "ExcludedRules": List[ExcludedRuleTypeDef],
     },
+    total=False,
 )
 
-GetRateBasedRuleManagedKeysResponseTypeDef = TypedDict(
-    "GetRateBasedRuleManagedKeysResponseTypeDef",
-    {
-        "ManagedKeys": List[str],
-        "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
+    pass
 
 ListByteMatchSetsResponseTypeDef = TypedDict(
     "ListByteMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "ByteMatchSets": List[ByteMatchSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListResourcesForWebACLResponseTypeDef = TypedDict(
-    "ListResourcesForWebACLResponseTypeDef",
-    {
-        "ResourceArns": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateByteMatchSetResponseTypeDef = TypedDict(
-    "UpdateByteMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGeoMatchSetResponseTypeDef = TypedDict(
-    "UpdateGeoMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateIPSetResponseTypeDef = TypedDict(
-    "UpdateIPSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRateBasedRuleResponseTypeDef = TypedDict(
-    "UpdateRateBasedRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRegexMatchSetResponseTypeDef = TypedDict(
-    "UpdateRegexMatchSetResponseTypeDef",
+ByteMatchTupleTypeDef = TypedDict(
+    "ByteMatchTupleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TargetString": bytes,
+        "TextTransformation": TextTransformationType,
+        "PositionalConstraint": PositionalConstraintType,
     },
 )
 
-UpdateRegexPatternSetResponseTypeDef = TypedDict(
-    "UpdateRegexPatternSetResponseTypeDef",
+_RequiredLoggingConfigurationTypeDef = TypedDict(
+    "_RequiredLoggingConfigurationTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "LogDestinationConfigs": List[str],
     },
 )
-
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+_OptionalLoggingConfigurationTypeDef = TypedDict(
+    "_OptionalLoggingConfigurationTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RedactedFields": List[FieldToMatchTypeDef],
     },
+    total=False,
 )
 
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class LoggingConfigurationTypeDef(
+    _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
+):
+    pass
 
-UpdateSizeConstraintSetResponseTypeDef = TypedDict(
-    "UpdateSizeConstraintSetResponseTypeDef",
+RegexMatchTupleTypeDef = TypedDict(
+    "RegexMatchTupleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
+        "RegexPatternSetId": str,
     },
 )
 
-UpdateSqlInjectionMatchSetResponseTypeDef = TypedDict(
-    "UpdateSqlInjectionMatchSetResponseTypeDef",
+SizeConstraintTypeDef = TypedDict(
+    "SizeConstraintTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Size": int,
     },
 )
 
-UpdateWebACLResponseTypeDef = TypedDict(
-    "UpdateWebACLResponseTypeDef",
+SqlInjectionMatchTupleTypeDef = TypedDict(
+    "SqlInjectionMatchTupleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
     },
 )
 
-UpdateXssMatchSetResponseTypeDef = TypedDict(
-    "UpdateXssMatchSetResponseTypeDef",
+XssMatchTupleTypeDef = TypedDict(
+    "XssMatchTupleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
     },
 )
 
 _RequiredCreateRateBasedRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRateBasedRuleRequestRequestTypeDef",
     {
         "Name": str,
@@ -1458,40 +1458,40 @@
 )
 
 CreateRegexPatternSetResponseTypeDef = TypedDict(
     "CreateRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRegexPatternSetResponseTypeDef = TypedDict(
     "GetRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRuleGroupResponseTypeDef = TypedDict(
     "GetRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGeoMatchSetTypeDef = TypedDict(
     "_RequiredGeoMatchSetTypeDef",
     {
         "GeoMatchSetId": str,
@@ -1518,15 +1518,15 @@
 )
 
 ListGeoMatchSetsResponseTypeDef = TypedDict(
     "ListGeoMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "GeoMatchSets": List[GeoMatchSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSampledRequestsRequestRequestTypeDef = TypedDict(
     "GetSampledRequestsRequestRequestTypeDef",
     {
         "WebAclId": str,
@@ -1536,24 +1536,24 @@
     },
 )
 
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACLSummary": WebACLSummaryTypeDef,
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
 
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
@@ -1593,96 +1593,96 @@
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
 
 ListRateBasedRulesResponseTypeDef = TypedDict(
     "ListRateBasedRulesResponseTypeDef",
     {
         "NextMarker": str,
         "Rules": List[RuleSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "NextMarker": str,
         "Rules": List[RuleSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRegexMatchSetsResponseTypeDef = TypedDict(
     "ListRegexMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "RegexMatchSets": List[RegexMatchSetSummaryTypeDef],
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
 
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[RuleGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSizeConstraintSetsResponseTypeDef = TypedDict(
     "ListSizeConstraintSetsResponseTypeDef",
     {
         "NextMarker": str,
         "SizeConstraintSets": List[SizeConstraintSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSqlInjectionMatchSetsResponseTypeDef = TypedDict(
     "ListSqlInjectionMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "SqlInjectionMatchSets": List[SqlInjectionMatchSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSubscribedRuleGroupsResponseTypeDef = TypedDict(
     "ListSubscribedRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[SubscribedRuleGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListXssMatchSetsResponseTypeDef = TypedDict(
     "ListXssMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "XssMatchSets": List[XssMatchSetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRateBasedRuleTypeDef = TypedDict(
     "_RequiredRateBasedRuleTypeDef",
     {
         "RuleId": str,
@@ -1740,15 +1740,15 @@
 )
 
 ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
     "ListActivatedRulesInRuleGroupResponseTypeDef",
     {
         "NextMarker": str,
         "ActivatedRules": List[ActivatedRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleGroupUpdateTypeDef = TypedDict(
     "RuleGroupUpdateTypeDef",
     {
         "Action": ChangeActionType,
@@ -1811,39 +1811,39 @@
     },
 )
 
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
 
 RegexMatchSetTypeDef = TypedDict(
     "RegexMatchSetTypeDef",
     {
         "RegexMatchSetId": str,
@@ -1944,32 +1944,32 @@
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
 
 CreateGeoMatchSetResponseTypeDef = TypedDict(
     "CreateGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGeoMatchSetResponseTypeDef = TypedDict(
     "GetGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGeoMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
@@ -2001,23 +2001,23 @@
     pass
 
 CreateIPSetResponseTypeDef = TypedDict(
     "CreateIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIPSetResponseTypeDef = TypedDict(
     "GetIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateIPSetRequestRequestTypeDef = TypedDict(
     "UpdateIPSetRequestRequestTypeDef",
     {
         "IPSetId": str,
@@ -2027,40 +2027,40 @@
 )
 
 CreateRateBasedRuleResponseTypeDef = TypedDict(
     "CreateRateBasedRuleResponseTypeDef",
     {
         "Rule": RateBasedRuleTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRateBasedRuleResponseTypeDef = TypedDict(
     "GetRateBasedRuleResponseTypeDef",
     {
         "Rule": RateBasedRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRateBasedRuleRequestRequestTypeDef = TypedDict(
     "UpdateRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
@@ -2089,23 +2089,23 @@
 )
 
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWebACLResponseTypeDef = TypedDict(
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
@@ -2127,23 +2127,23 @@
     pass
 
 CreateByteMatchSetResponseTypeDef = TypedDict(
     "CreateByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetByteMatchSetResponseTypeDef = TypedDict(
     "GetByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateByteMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
@@ -2153,23 +2153,23 @@
 )
 
 CreateRegexMatchSetResponseTypeDef = TypedDict(
     "CreateRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRegexMatchSetResponseTypeDef = TypedDict(
     "GetRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRegexMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateRegexMatchSetRequestRequestTypeDef",
     {
         "RegexMatchSetId": str,
@@ -2179,23 +2179,23 @@
 )
 
 CreateSizeConstraintSetResponseTypeDef = TypedDict(
     "CreateSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSizeConstraintSetResponseTypeDef = TypedDict(
     "GetSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "UpdateSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
@@ -2205,23 +2205,23 @@
 )
 
 CreateSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "CreateSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "GetSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
     {
         "SqlInjectionMatchSetId": str,
@@ -2231,23 +2231,23 @@
 )
 
 CreateXssMatchSetResponseTypeDef = TypedDict(
     "CreateXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetXssMatchSetResponseTypeDef = TypedDict(
     "GetXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateXssMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
@@ -2258,10 +2258,10 @@
 
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
```

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional.egg-info/PKG-INFO` & `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf-regional
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.WAFRegional 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.WAFRegional 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/
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
 
 <a id="mypy-boto3-waf-regional"></a>
 
 # mypy-boto3-waf-regional
 
 [![PyPI - mypy-boto3-waf-regional](https://img.shields.io/pypi/v/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-waf-regional?color=blue)](https://pypistats.org/packages/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,50 +318,66 @@
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
     ByteMatchSetSummaryTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
     RegexPatternSetTypeDef,
     RuleGroupTypeDef,
     CreateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateWebACLMigrationStackRequestRequestTypeDef,
+    CreateWebACLMigrationStackResponseTypeDef,
     CreateXssMatchSetRequestRequestTypeDef,
     DeleteByteMatchSetRequestRequestTypeDef,
+    DeleteByteMatchSetResponseTypeDef,
     DeleteGeoMatchSetRequestRequestTypeDef,
+    DeleteGeoMatchSetResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
+    DeleteIPSetResponseTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRateBasedRuleRequestRequestTypeDef,
+    DeleteRateBasedRuleResponseTypeDef,
     DeleteRegexMatchSetRequestRequestTypeDef,
+    DeleteRegexMatchSetResponseTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
+    DeleteRegexPatternSetResponseTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
+    DeleteRuleGroupResponseTypeDef,
     DeleteRuleRequestRequestTypeDef,
+    DeleteRuleResponseTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
+    DeleteSizeConstraintSetResponseTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
+    DeleteSqlInjectionMatchSetResponseTypeDef,
     DeleteWebACLRequestRequestTypeDef,
+    DeleteWebACLResponseTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
+    DeleteXssMatchSetResponseTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
+    GetChangeTokenResponseTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
+    GetChangeTokenStatusResponseTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
+    GetPermissionPolicyResponseTypeDef,
     GetRateBasedRuleManagedKeysRequestRequestTypeDef,
+    GetRateBasedRuleManagedKeysResponseTypeDef,
     GetRateBasedRuleRequestRequestTypeDef,
     GetRegexMatchSetRequestRequestTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
     TimeWindowTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
@@ -380,14 +397,15 @@
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
+    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
     ListRulesRequestRequestTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
@@ -396,53 +414,36 @@
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ActivatedRuleTypeDef,
-    ByteMatchTupleTypeDef,
-    LoggingConfigurationTypeDef,
-    RegexMatchTupleTypeDef,
-    SizeConstraintTypeDef,
-    SqlInjectionMatchTupleTypeDef,
-    XssMatchTupleTypeDef,
-    CreateWebACLMigrationStackResponseTypeDef,
-    DeleteByteMatchSetResponseTypeDef,
-    DeleteGeoMatchSetResponseTypeDef,
-    DeleteIPSetResponseTypeDef,
-    DeleteRateBasedRuleResponseTypeDef,
-    DeleteRegexMatchSetResponseTypeDef,
-    DeleteRegexPatternSetResponseTypeDef,
-    DeleteRuleGroupResponseTypeDef,
-    DeleteRuleResponseTypeDef,
-    DeleteSizeConstraintSetResponseTypeDef,
-    DeleteSqlInjectionMatchSetResponseTypeDef,
-    DeleteWebACLResponseTypeDef,
-    DeleteXssMatchSetResponseTypeDef,
-    GetChangeTokenResponseTypeDef,
-    GetChangeTokenStatusResponseTypeDef,
-    GetPermissionPolicyResponseTypeDef,
-    GetRateBasedRuleManagedKeysResponseTypeDef,
-    ListByteMatchSetsResponseTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateSizeConstraintSetResponseTypeDef,
     UpdateSqlInjectionMatchSetResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     UpdateXssMatchSetResponseTypeDef,
+    ActivatedRuleTypeDef,
+    ListByteMatchSetsResponseTypeDef,
+    ByteMatchTupleTypeDef,
+    LoggingConfigurationTypeDef,
+    RegexMatchTupleTypeDef,
+    SizeConstraintTypeDef,
+    SqlInjectionMatchTupleTypeDef,
+    XssMatchTupleTypeDef,
     CreateRateBasedRuleRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
     TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
@@ -534,42 +535,42 @@
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

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/mypy_boto3_waf_regional.egg-info/SOURCES.txt` & `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.26.0.post1/setup.py` & `mypy-boto3-waf-regional-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-waf-regional.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-waf-regional",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_waf_regional"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAFRegional 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.WAFRegional 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 waf-regional type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_waf_regional": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_waf_regional": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/",
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


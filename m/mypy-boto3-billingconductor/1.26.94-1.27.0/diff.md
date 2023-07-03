# Comparing `tmp/mypy-boto3-billingconductor-1.26.94.tar.gz` & `tmp/mypy-boto3-billingconductor-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-billingconductor-1.26.94.tar", last modified: Fri Mar 17 19:32:19 2023, max compression
+gzip compressed data, was "mypy-boto3-billingconductor-1.27.0.tar", last modified: Mon Jul  3 19:50:26 2023, max compression
```

## Comparing `mypy-boto3-billingconductor-1.26.94.tar` & `mypy-boto3-billingconductor-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:32:19.873377 mypy-boto3-billingconductor-1.26.94/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-17 19:31:55.000000 mypy-boto3-billingconductor-1.26.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20438 2023-03-17 19:32:19.873377 mypy-boto3-billingconductor-1.26.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-03-17 19:31:55.000000 mypy-boto3-billingconductor-1.26.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:32:19.865377 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-03-17 19:31:55.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-03-17 19:31:55.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-17 19:31:55.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31565 2023-03-17 19:31:56.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31517 2023-03-17 19:31:56.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-03-17 19:31:56.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-03-17 19:31:56.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-03-17 19:31:56.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-03-17 19:31:56.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:31:55.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42714 2023-03-17 19:31:57.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42667 2023-03-17 19:31:57.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-17 19:31:55.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:32:19.873377 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20438 2023-03-17 19:32:19.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-17 19:32:19.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 19:32:19.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 19:32:19.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-17 19:32:19.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-17 19:32:19.000000 mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 19:32:19.873377 mypy-boto3-billingconductor-1.26.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-17 19:31:55.000000 mypy-boto3-billingconductor-1.26.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:26.922900 mypy-boto3-billingconductor-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-07-03 19:50:26.922900 mypy-boto3-billingconductor-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18902 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:26.914899 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31565 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31517 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14433 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42792 2023-07-03 19:33:10.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42745 2023-07-03 19:33:10.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:26.922900 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-07-03 19:50:26.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-03 19:50:26.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:26.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:26.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:26.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 19:50:26.000000 mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:26.922900 mypy-boto3-billingconductor-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-03 19:33:08.000000 mypy-boto3-billingconductor-1.27.0/setup.py
```

### Comparing `mypy-boto3-billingconductor-1.26.94/LICENSE` & `mypy-boto3-billingconductor-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-billingconductor-1.26.94/PKG-INFO` & `mypy-boto3-billingconductor-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-billingconductor
-Version: 1.26.94
-Summary: Type annotations for boto3.BillingConductor 1.26.94 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.BillingConductor 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-billingconductor"></a>
 
 # mypy-boto3-billingconductor
 
 [![PyPI - mypy-boto3-billingconductor](https://img.shields.io/pypi/v/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-billingconductor?color=blue)](https://pypistats.org/packages/mypy-boto3-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BillingConductor 1.26.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[boto3.BillingConductor 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-billingconductor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,86 +374,86 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_billingconductor.type_defs import (
     AccountAssociationsListElementTypeDef,
     AccountGroupingTypeDef,
     AssociateAccountsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateAccountsOutputTypeDef,
     AssociatePricingRulesInputRequestTypeDef,
+    AssociatePricingRulesOutputTypeDef,
     AssociateResourceErrorTypeDef,
     CustomLineItemBillingPeriodRangeTypeDef,
     BillingGroupCostReportElementTypeDef,
     ComputationPreferenceTypeDef,
+    CreateBillingGroupOutputTypeDef,
+    CreateCustomLineItemOutputTypeDef,
     CreateFreeTierConfigTypeDef,
     CreatePricingPlanInputRequestTypeDef,
+    CreatePricingPlanOutputTypeDef,
+    CreatePricingRuleOutputTypeDef,
     CustomLineItemFlatChargeDetailsTypeDef,
     CustomLineItemPercentageChargeDetailsTypeDef,
     DeleteBillingGroupInputRequestTypeDef,
+    DeleteBillingGroupOutputTypeDef,
+    DeleteCustomLineItemOutputTypeDef,
     DeletePricingPlanInputRequestTypeDef,
+    DeletePricingPlanOutputTypeDef,
     DeletePricingRuleInputRequestTypeDef,
+    DeletePricingRuleOutputTypeDef,
     DisassociateAccountsInputRequestTypeDef,
+    DisassociateAccountsOutputTypeDef,
     DisassociatePricingRulesInputRequestTypeDef,
+    DisassociatePricingRulesOutputTypeDef,
     FreeTierConfigTypeDef,
     ListAccountAssociationsFilterTypeDef,
-    PaginatorConfigTypeDef,
     ListBillingGroupCostReportsFilterTypeDef,
     ListBillingGroupsFilterTypeDef,
     ListCustomLineItemFlatChargeDetailsTypeDef,
     ListCustomLineItemPercentageChargeDetailsTypeDef,
     ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef,
     ListCustomLineItemsFilterTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
     ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
     ListPricingPlansFilterTypeDef,
     PricingPlanListElementTypeDef,
+    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
     ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
+    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
     ListPricingRulesFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemResponseElementTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateBillingGroupOutputTypeDef,
     UpdateCustomLineItemFlatChargeDetailsTypeDef,
     UpdateCustomLineItemPercentageChargeDetailsTypeDef,
     UpdateFreeTierConfigTypeDef,
     UpdatePricingPlanInputRequestTypeDef,
-    AssociateAccountsOutputTypeDef,
-    AssociatePricingRulesOutputTypeDef,
-    CreateBillingGroupOutputTypeDef,
-    CreateCustomLineItemOutputTypeDef,
-    CreatePricingPlanOutputTypeDef,
-    CreatePricingRuleOutputTypeDef,
-    DeleteBillingGroupOutputTypeDef,
-    DeleteCustomLineItemOutputTypeDef,
-    DeletePricingPlanOutputTypeDef,
-    DeletePricingRuleOutputTypeDef,
-    DisassociateAccountsOutputTypeDef,
-    DisassociatePricingRulesOutputTypeDef,
-    ListAccountAssociationsOutputTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
-    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateBillingGroupOutputTypeDef,
     UpdatePricingPlanOutputTypeDef,
+    ListAccountAssociationsOutputTypeDef,
     AssociateResourceResponseElementTypeDef,
     DisassociateResourceResponseElementTypeDef,
     BatchAssociateResourcesToCustomLineItemInputRequestTypeDef,
     BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef,
     DeleteCustomLineItemInputRequestTypeDef,
     ListBillingGroupCostReportsOutputTypeDef,
     BillingGroupListElementTypeDef,
     CreateBillingGroupInputRequestTypeDef,
     UpdateBillingGroupInputRequestTypeDef,
     CreateTieringInputTypeDef,
     CustomLineItemChargeDetailsTypeDef,
     TieringTypeDef,
-    ListAccountAssociationsInputRequestTypeDef,
     ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+    ListAccountAssociationsInputRequestTypeDef,
     ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef,
     ListBillingGroupCostReportsInputRequestTypeDef,
     ListBillingGroupsInputListBillingGroupsPaginateTypeDef,
     ListBillingGroupsInputRequestTypeDef,
     ListCustomLineItemChargeDetailsTypeDef,
     ListCustomLineItemVersionsFilterTypeDef,
     ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef,
@@ -495,42 +495,42 @@
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

### Comparing `mypy-boto3-billingconductor-1.26.94/README.md` & `mypy-boto3-billingconductor-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-billingconductor"></a>
 
 # mypy-boto3-billingconductor
 
 [![PyPI - mypy-boto3-billingconductor](https://img.shields.io/pypi/v/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-billingconductor?color=blue)](https://pypistats.org/packages/mypy-boto3-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BillingConductor 1.26.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[boto3.BillingConductor 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-billingconductor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,86 +342,86 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_billingconductor.type_defs import (
     AccountAssociationsListElementTypeDef,
     AccountGroupingTypeDef,
     AssociateAccountsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateAccountsOutputTypeDef,
     AssociatePricingRulesInputRequestTypeDef,
+    AssociatePricingRulesOutputTypeDef,
     AssociateResourceErrorTypeDef,
     CustomLineItemBillingPeriodRangeTypeDef,
     BillingGroupCostReportElementTypeDef,
     ComputationPreferenceTypeDef,
+    CreateBillingGroupOutputTypeDef,
+    CreateCustomLineItemOutputTypeDef,
     CreateFreeTierConfigTypeDef,
     CreatePricingPlanInputRequestTypeDef,
+    CreatePricingPlanOutputTypeDef,
+    CreatePricingRuleOutputTypeDef,
     CustomLineItemFlatChargeDetailsTypeDef,
     CustomLineItemPercentageChargeDetailsTypeDef,
     DeleteBillingGroupInputRequestTypeDef,
+    DeleteBillingGroupOutputTypeDef,
+    DeleteCustomLineItemOutputTypeDef,
     DeletePricingPlanInputRequestTypeDef,
+    DeletePricingPlanOutputTypeDef,
     DeletePricingRuleInputRequestTypeDef,
+    DeletePricingRuleOutputTypeDef,
     DisassociateAccountsInputRequestTypeDef,
+    DisassociateAccountsOutputTypeDef,
     DisassociatePricingRulesInputRequestTypeDef,
+    DisassociatePricingRulesOutputTypeDef,
     FreeTierConfigTypeDef,
     ListAccountAssociationsFilterTypeDef,
-    PaginatorConfigTypeDef,
     ListBillingGroupCostReportsFilterTypeDef,
     ListBillingGroupsFilterTypeDef,
     ListCustomLineItemFlatChargeDetailsTypeDef,
     ListCustomLineItemPercentageChargeDetailsTypeDef,
     ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef,
     ListCustomLineItemsFilterTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
     ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
     ListPricingPlansFilterTypeDef,
     PricingPlanListElementTypeDef,
+    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
     ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
+    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
     ListPricingRulesFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemResponseElementTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateBillingGroupOutputTypeDef,
     UpdateCustomLineItemFlatChargeDetailsTypeDef,
     UpdateCustomLineItemPercentageChargeDetailsTypeDef,
     UpdateFreeTierConfigTypeDef,
     UpdatePricingPlanInputRequestTypeDef,
-    AssociateAccountsOutputTypeDef,
-    AssociatePricingRulesOutputTypeDef,
-    CreateBillingGroupOutputTypeDef,
-    CreateCustomLineItemOutputTypeDef,
-    CreatePricingPlanOutputTypeDef,
-    CreatePricingRuleOutputTypeDef,
-    DeleteBillingGroupOutputTypeDef,
-    DeleteCustomLineItemOutputTypeDef,
-    DeletePricingPlanOutputTypeDef,
-    DeletePricingRuleOutputTypeDef,
-    DisassociateAccountsOutputTypeDef,
-    DisassociatePricingRulesOutputTypeDef,
-    ListAccountAssociationsOutputTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
-    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateBillingGroupOutputTypeDef,
     UpdatePricingPlanOutputTypeDef,
+    ListAccountAssociationsOutputTypeDef,
     AssociateResourceResponseElementTypeDef,
     DisassociateResourceResponseElementTypeDef,
     BatchAssociateResourcesToCustomLineItemInputRequestTypeDef,
     BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef,
     DeleteCustomLineItemInputRequestTypeDef,
     ListBillingGroupCostReportsOutputTypeDef,
     BillingGroupListElementTypeDef,
     CreateBillingGroupInputRequestTypeDef,
     UpdateBillingGroupInputRequestTypeDef,
     CreateTieringInputTypeDef,
     CustomLineItemChargeDetailsTypeDef,
     TieringTypeDef,
-    ListAccountAssociationsInputRequestTypeDef,
     ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+    ListAccountAssociationsInputRequestTypeDef,
     ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef,
     ListBillingGroupCostReportsInputRequestTypeDef,
     ListBillingGroupsInputListBillingGroupsPaginateTypeDef,
     ListBillingGroupsInputRequestTypeDef,
     ListCustomLineItemChargeDetailsTypeDef,
     ListCustomLineItemVersionsFilterTypeDef,
     ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef,
@@ -463,42 +463,42 @@
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

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/__init__.py` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/__init__.pyi` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/__main__.py` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.BillingConductor 1.26.94\nVersion:         1.26.94\nBuilder"
-        " version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.BillingConductor 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.94")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/client.py` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/client.pyi` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/literals.py` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
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
@@ -132,14 +133,15 @@
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
@@ -237,14 +239,15 @@
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
@@ -280,14 +283,15 @@
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
@@ -306,16 +310,19 @@
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
@@ -399,15 +406,17 @@
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

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/literals.pyi` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
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
@@ -130,14 +131,15 @@
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
@@ -235,14 +237,15 @@
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
@@ -278,14 +281,15 @@
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
@@ -304,16 +308,19 @@
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
@@ -397,15 +404,17 @@
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

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/paginator.py` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListAccountAssociationsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListAccountAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listaccountassociationspaginator)
         """
 
 
@@ -113,15 +113,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupCostReportsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBillingGroupCostReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroupCostReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listbillinggroupcostreportspaginator)
         """
 
 
@@ -132,15 +132,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBillingGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listbillinggroupspaginator)
         """
 
 
@@ -151,15 +151,15 @@
     """
 
     def paginate(
         self,
         *,
         Arn: str,
         Filters: ListCustomLineItemVersionsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomLineItemVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItemVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listcustomlineitemversionspaginator)
         """
 
 
@@ -170,15 +170,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListCustomLineItemsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomLineItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listcustomlineitemspaginator)
         """
 
 
@@ -189,15 +189,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingPlansFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingplanspaginator)
         """
 
 
@@ -208,15 +208,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingRuleArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingPlansAssociatedWithPricingRuleOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlansAssociatedWithPricingRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingplansassociatedwithpricingrulepaginator)
         """
 
 
@@ -227,15 +227,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingRulesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingrulespaginator)
         """
 
 
@@ -246,15 +246,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingPlanArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingRulesAssociatedToPricingPlanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRulesAssociatedToPricingPlan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingrulesassociatedtopricingplanpaginator)
         """
 
 
@@ -266,13 +266,13 @@
 
     def paginate(
         self,
         *,
         Arn: str,
         BillingPeriod: str = ...,
         Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourcesAssociatedToCustomLineItemOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListResourcesAssociatedToCustomLineItem.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listresourcesassociatedtocustomlineitempaginator)
         """
```

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/paginator.pyi` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListAccountAssociationsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListAccountAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listaccountassociationspaginator)
         """
 
 class ListBillingGroupCostReportsPaginator(Paginator):
@@ -109,15 +109,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupCostReportsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBillingGroupCostReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroupCostReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listbillinggroupcostreportspaginator)
         """
 
 class ListBillingGroupsPaginator(Paginator):
@@ -127,15 +127,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBillingGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listbillinggroupspaginator)
         """
 
 class ListCustomLineItemVersionsPaginator(Paginator):
@@ -145,15 +145,15 @@
     """
 
     def paginate(
         self,
         *,
         Arn: str,
         Filters: ListCustomLineItemVersionsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomLineItemVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItemVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listcustomlineitemversionspaginator)
         """
 
 class ListCustomLineItemsPaginator(Paginator):
@@ -163,15 +163,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListCustomLineItemsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomLineItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listcustomlineitemspaginator)
         """
 
 class ListPricingPlansPaginator(Paginator):
@@ -181,15 +181,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingPlansFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingplanspaginator)
         """
 
 class ListPricingPlansAssociatedWithPricingRulePaginator(Paginator):
@@ -199,15 +199,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingRuleArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingPlansAssociatedWithPricingRuleOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlansAssociatedWithPricingRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingplansassociatedwithpricingrulepaginator)
         """
 
 class ListPricingRulesPaginator(Paginator):
@@ -217,15 +217,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingRulesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingrulespaginator)
         """
 
 class ListPricingRulesAssociatedToPricingPlanPaginator(Paginator):
@@ -235,15 +235,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingPlanArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingRulesAssociatedToPricingPlanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRulesAssociatedToPricingPlan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingrulesassociatedtopricingplanpaginator)
         """
 
 class ListResourcesAssociatedToCustomLineItemPaginator(Paginator):
@@ -254,13 +254,13 @@
 
     def paginate(
         self,
         *,
         Arn: str,
         BillingPeriod: str = ...,
         Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourcesAssociatedToCustomLineItemOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListResourcesAssociatedToCustomLineItem.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listresourcesassociatedtocustomlineitempaginator)
         """
```

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/type_defs.py` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,86 +30,86 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountAssociationsListElementTypeDef",
     "AccountGroupingTypeDef",
     "AssociateAccountsInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateAccountsOutputTypeDef",
     "AssociatePricingRulesInputRequestTypeDef",
+    "AssociatePricingRulesOutputTypeDef",
     "AssociateResourceErrorTypeDef",
     "CustomLineItemBillingPeriodRangeTypeDef",
     "BillingGroupCostReportElementTypeDef",
     "ComputationPreferenceTypeDef",
+    "CreateBillingGroupOutputTypeDef",
+    "CreateCustomLineItemOutputTypeDef",
     "CreateFreeTierConfigTypeDef",
     "CreatePricingPlanInputRequestTypeDef",
+    "CreatePricingPlanOutputTypeDef",
+    "CreatePricingRuleOutputTypeDef",
     "CustomLineItemFlatChargeDetailsTypeDef",
     "CustomLineItemPercentageChargeDetailsTypeDef",
     "DeleteBillingGroupInputRequestTypeDef",
+    "DeleteBillingGroupOutputTypeDef",
+    "DeleteCustomLineItemOutputTypeDef",
     "DeletePricingPlanInputRequestTypeDef",
+    "DeletePricingPlanOutputTypeDef",
     "DeletePricingRuleInputRequestTypeDef",
+    "DeletePricingRuleOutputTypeDef",
     "DisassociateAccountsInputRequestTypeDef",
+    "DisassociateAccountsOutputTypeDef",
     "DisassociatePricingRulesInputRequestTypeDef",
+    "DisassociatePricingRulesOutputTypeDef",
     "FreeTierConfigTypeDef",
     "ListAccountAssociationsFilterTypeDef",
-    "PaginatorConfigTypeDef",
     "ListBillingGroupCostReportsFilterTypeDef",
     "ListBillingGroupsFilterTypeDef",
     "ListCustomLineItemFlatChargeDetailsTypeDef",
     "ListCustomLineItemPercentageChargeDetailsTypeDef",
     "ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef",
     "ListCustomLineItemsFilterTypeDef",
+    "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
     "ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef",
+    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
     "ListPricingPlansFilterTypeDef",
     "PricingPlanListElementTypeDef",
+    "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
     "ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
+    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
     "ListPricingRulesFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemResponseElementTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateBillingGroupOutputTypeDef",
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     "UpdateCustomLineItemPercentageChargeDetailsTypeDef",
     "UpdateFreeTierConfigTypeDef",
     "UpdatePricingPlanInputRequestTypeDef",
-    "AssociateAccountsOutputTypeDef",
-    "AssociatePricingRulesOutputTypeDef",
-    "CreateBillingGroupOutputTypeDef",
-    "CreateCustomLineItemOutputTypeDef",
-    "CreatePricingPlanOutputTypeDef",
-    "CreatePricingRuleOutputTypeDef",
-    "DeleteBillingGroupOutputTypeDef",
-    "DeleteCustomLineItemOutputTypeDef",
-    "DeletePricingPlanOutputTypeDef",
-    "DeletePricingRuleOutputTypeDef",
-    "DisassociateAccountsOutputTypeDef",
-    "DisassociatePricingRulesOutputTypeDef",
-    "ListAccountAssociationsOutputTypeDef",
-    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
-    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateBillingGroupOutputTypeDef",
     "UpdatePricingPlanOutputTypeDef",
+    "ListAccountAssociationsOutputTypeDef",
     "AssociateResourceResponseElementTypeDef",
     "DisassociateResourceResponseElementTypeDef",
     "BatchAssociateResourcesToCustomLineItemInputRequestTypeDef",
     "BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef",
     "DeleteCustomLineItemInputRequestTypeDef",
     "ListBillingGroupCostReportsOutputTypeDef",
     "BillingGroupListElementTypeDef",
     "CreateBillingGroupInputRequestTypeDef",
     "UpdateBillingGroupInputRequestTypeDef",
     "CreateTieringInputTypeDef",
     "CustomLineItemChargeDetailsTypeDef",
     "TieringTypeDef",
-    "ListAccountAssociationsInputRequestTypeDef",
     "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
-    "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    "ListAccountAssociationsInputRequestTypeDef",
     "ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef",
     "ListBillingGroupCostReportsInputRequestTypeDef",
     "ListBillingGroupsInputListBillingGroupsPaginateTypeDef",
     "ListBillingGroupsInputRequestTypeDef",
     "ListCustomLineItemChargeDetailsTypeDef",
     "ListCustomLineItemVersionsFilterTypeDef",
     "ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef",
@@ -165,33 +165,38 @@
     "AssociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateAccountsOutputTypeDef = TypedDict(
+    "AssociateAccountsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociatePricingRulesInputRequestTypeDef = TypedDict(
     "AssociatePricingRulesInputRequestTypeDef",
     {
         "Arn": str,
         "PricingRuleArns": Sequence[str],
     },
 )
 
+AssociatePricingRulesOutputTypeDef = TypedDict(
+    "AssociatePricingRulesOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateResourceErrorTypeDef = TypedDict(
     "AssociateResourceErrorTypeDef",
     {
         "Message": str,
         "Reason": AssociateResourceErrorReasonType,
     },
     total=False,
@@ -235,14 +240,30 @@
 ComputationPreferenceTypeDef = TypedDict(
     "ComputationPreferenceTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 
+CreateBillingGroupOutputTypeDef = TypedDict(
+    "CreateBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCustomLineItemOutputTypeDef = TypedDict(
+    "CreateCustomLineItemOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateFreeTierConfigTypeDef = TypedDict(
     "CreateFreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -266,14 +287,30 @@
 
 class CreatePricingPlanInputRequestTypeDef(
     _RequiredCreatePricingPlanInputRequestTypeDef, _OptionalCreatePricingPlanInputRequestTypeDef
 ):
     pass
 
 
+CreatePricingPlanOutputTypeDef = TypedDict(
+    "CreatePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePricingRuleOutputTypeDef = TypedDict(
+    "CreatePricingRuleOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "CustomLineItemFlatChargeDetailsTypeDef",
     {
         "ChargeValue": float,
     },
 )
 
@@ -302,44 +339,92 @@
 DeleteBillingGroupInputRequestTypeDef = TypedDict(
     "DeleteBillingGroupInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeleteBillingGroupOutputTypeDef = TypedDict(
+    "DeleteBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteCustomLineItemOutputTypeDef = TypedDict(
+    "DeleteCustomLineItemOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePricingPlanInputRequestTypeDef = TypedDict(
     "DeletePricingPlanInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeletePricingPlanOutputTypeDef = TypedDict(
+    "DeletePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePricingRuleInputRequestTypeDef = TypedDict(
     "DeletePricingRuleInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeletePricingRuleOutputTypeDef = TypedDict(
+    "DeletePricingRuleOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateAccountsInputRequestTypeDef = TypedDict(
     "DisassociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
 )
 
+DisassociateAccountsOutputTypeDef = TypedDict(
+    "DisassociateAccountsOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociatePricingRulesInputRequestTypeDef = TypedDict(
     "DisassociatePricingRulesInputRequestTypeDef",
     {
         "Arn": str,
         "PricingRuleArns": Sequence[str],
     },
 )
 
+DisassociatePricingRulesOutputTypeDef = TypedDict(
+    "DisassociatePricingRulesOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FreeTierConfigTypeDef = TypedDict(
     "FreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -349,24 +434,14 @@
         "Association": str,
         "AccountId": str,
         "AccountIds": Sequence[str],
     },
     total=False,
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
 ListBillingGroupCostReportsFilterTypeDef = TypedDict(
     "ListBillingGroupCostReportsFilterTypeDef",
     {
         "BillingGroupArns": Sequence[str],
     },
     total=False,
 )
@@ -410,14 +485,37 @@
         "Names": Sequence[str],
         "BillingGroups": Sequence[str],
         "Arns": Sequence[str],
     },
     total=False,
 )
 
+_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
+    "_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
+    {
+        "PricingRuleArn": str,
+    },
+)
+_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
+    "_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
+    {
+        "BillingPeriod": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef(
+    _RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+    _OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef",
     {
         "PricingRuleArn": str,
     },
 )
 _OptionalListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = TypedDict(
@@ -434,14 +532,25 @@
 class ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef(
     _RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
     _OptionalListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
 ):
     pass
 
 
+ListPricingPlansAssociatedWithPricingRuleOutputTypeDef = TypedDict(
+    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
+    {
+        "BillingPeriod": str,
+        "PricingRuleArn": str,
+        "PricingPlanArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListPricingPlansFilterTypeDef = TypedDict(
     "ListPricingPlansFilterTypeDef",
     {
         "Arns": Sequence[str],
     },
     total=False,
 )
@@ -455,14 +564,37 @@
         "Size": int,
         "CreationTime": int,
         "LastModifiedTime": int,
     },
     total=False,
 )
 
+_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
+    "_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    {
+        "PricingPlanArn": str,
+    },
+)
+_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
+    "_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    {
+        "BillingPeriod": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef(
+    _RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+    _OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = TypedDict(
     "_RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 _OptionalListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = TypedDict(
@@ -479,14 +611,25 @@
 class ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef(
     _RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
     _OptionalListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
 ):
     pass
 
 
+ListPricingRulesAssociatedToPricingPlanOutputTypeDef = TypedDict(
+    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
+    {
+        "BillingPeriod": str,
+        "PricingPlanArn": str,
+        "PricingRuleArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListPricingRulesFilterTypeDef = TypedDict(
     "ListPricingRulesFilterTypeDef",
     {
         "Arns": Sequence[str],
     },
     total=False,
 )
@@ -512,14 +655,43 @@
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
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -528,14 +700,30 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateBillingGroupOutputTypeDef = TypedDict(
+    "UpdateBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "PrimaryAccountId": str,
+        "PricingPlanArn": str,
+        "Size": int,
+        "LastModifiedTime": int,
+        "Status": BillingGroupStatusType,
+        "StatusReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateCustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     {
         "ChargeValue": float,
     },
 )
 
@@ -571,174 +759,32 @@
 
 class UpdatePricingPlanInputRequestTypeDef(
     _RequiredUpdatePricingPlanInputRequestTypeDef, _OptionalUpdatePricingPlanInputRequestTypeDef
 ):
     pass
 
 
-AssociateAccountsOutputTypeDef = TypedDict(
-    "AssociateAccountsOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociatePricingRulesOutputTypeDef = TypedDict(
-    "AssociatePricingRulesOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBillingGroupOutputTypeDef = TypedDict(
-    "CreateBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCustomLineItemOutputTypeDef = TypedDict(
-    "CreateCustomLineItemOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePricingPlanOutputTypeDef = TypedDict(
-    "CreatePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePricingRuleOutputTypeDef = TypedDict(
-    "CreatePricingRuleOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBillingGroupOutputTypeDef = TypedDict(
-    "DeleteBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteCustomLineItemOutputTypeDef = TypedDict(
-    "DeleteCustomLineItemOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePricingPlanOutputTypeDef = TypedDict(
-    "DeletePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePricingRuleOutputTypeDef = TypedDict(
-    "DeletePricingRuleOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateAccountsOutputTypeDef = TypedDict(
-    "DisassociateAccountsOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociatePricingRulesOutputTypeDef = TypedDict(
-    "DisassociatePricingRulesOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAccountAssociationsOutputTypeDef = TypedDict(
-    "ListAccountAssociationsOutputTypeDef",
-    {
-        "LinkedAccounts": List[AccountAssociationsListElementTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPricingPlansAssociatedWithPricingRuleOutputTypeDef = TypedDict(
-    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
-    {
-        "BillingPeriod": str,
-        "PricingRuleArn": str,
-        "PricingPlanArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPricingRulesAssociatedToPricingPlanOutputTypeDef = TypedDict(
-    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
-    {
-        "BillingPeriod": str,
-        "PricingPlanArn": str,
-        "PricingRuleArns": List[str],
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
-UpdateBillingGroupOutputTypeDef = TypedDict(
-    "UpdateBillingGroupOutputTypeDef",
+UpdatePricingPlanOutputTypeDef = TypedDict(
+    "UpdatePricingPlanOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Description": str,
-        "PrimaryAccountId": str,
-        "PricingPlanArn": str,
         "Size": int,
         "LastModifiedTime": int,
-        "Status": BillingGroupStatusType,
-        "StatusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdatePricingPlanOutputTypeDef = TypedDict(
-    "UpdatePricingPlanOutputTypeDef",
+ListAccountAssociationsOutputTypeDef = TypedDict(
+    "ListAccountAssociationsOutputTypeDef",
     {
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "Size": int,
-        "LastModifiedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LinkedAccounts": List[AccountAssociationsListElementTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateResourceResponseElementTypeDef = TypedDict(
     "AssociateResourceResponseElementTypeDef",
     {
         "Arn": str,
@@ -825,15 +871,15 @@
 
 
 ListBillingGroupCostReportsOutputTypeDef = TypedDict(
     "ListBillingGroupCostReportsOutputTypeDef",
     {
         "BillingGroupCostReports": List[BillingGroupCostReportElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BillingGroupListElementTypeDef = TypedDict(
     "BillingGroupListElementTypeDef",
     {
         "Name": str,
@@ -932,86 +978,40 @@
 TieringTypeDef = TypedDict(
     "TieringTypeDef",
     {
         "FreeTier": FreeTierConfigTypeDef,
     },
 )
 
-ListAccountAssociationsInputRequestTypeDef = TypedDict(
-    "ListAccountAssociationsInputRequestTypeDef",
-    {
-        "BillingPeriod": str,
-        "Filters": ListAccountAssociationsFilterTypeDef,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef = TypedDict(
     "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListAccountAssociationsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
-    "_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    {
-        "PricingRuleArn": str,
-    },
-)
-_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
-    "_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    {
-        "BillingPeriod": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef(
-    _RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-    _OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-):
-    pass
-
-
-_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
-    "_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
-    {
-        "PricingPlanArn": str,
-    },
-)
-_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
-    "_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+ListAccountAssociationsInputRequestTypeDef = TypedDict(
+    "ListAccountAssociationsInputRequestTypeDef",
     {
         "BillingPeriod": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Filters": ListAccountAssociationsFilterTypeDef,
+        "NextToken": str,
     },
     total=False,
 )
 
-
-class ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef(
-    _RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
-    _OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
-):
-    pass
-
-
 ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef = TypedDict(
     "ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListBillingGroupCostReportsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBillingGroupCostReportsInputRequestTypeDef = TypedDict(
     "ListBillingGroupCostReportsInputRequestTypeDef",
     {
@@ -1024,15 +1024,15 @@
 )
 
 ListBillingGroupsInputListBillingGroupsPaginateTypeDef = TypedDict(
     "ListBillingGroupsInputListBillingGroupsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListBillingGroupsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBillingGroupsInputRequestTypeDef = TypedDict(
     "ListBillingGroupsInputRequestTypeDef",
     {
@@ -1075,15 +1075,15 @@
 )
 
 ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef = TypedDict(
     "ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListCustomLineItemsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCustomLineItemsInputRequestTypeDef = TypedDict(
     "ListCustomLineItemsInputRequestTypeDef",
     {
@@ -1096,15 +1096,15 @@
 )
 
 ListPricingPlansInputListPricingPlansPaginateTypeDef = TypedDict(
     "ListPricingPlansInputListPricingPlansPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListPricingPlansFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPricingPlansInputRequestTypeDef = TypedDict(
     "ListPricingPlansInputRequestTypeDef",
     {
@@ -1118,24 +1118,24 @@
 
 ListPricingPlansOutputTypeDef = TypedDict(
     "ListPricingPlansOutputTypeDef",
     {
         "BillingPeriod": str,
         "PricingPlans": List[PricingPlanListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPricingRulesInputListPricingRulesPaginateTypeDef = TypedDict(
     "ListPricingRulesInputListPricingRulesPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListPricingRulesFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPricingRulesInputRequestTypeDef = TypedDict(
     "ListPricingRulesInputRequestTypeDef",
     {
@@ -1154,15 +1154,15 @@
     },
 )
 _OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef = TypedDict(
     "_OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListResourcesAssociatedToCustomLineItemFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef(
     _RequiredListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef,
@@ -1198,15 +1198,15 @@
 
 ListResourcesAssociatedToCustomLineItemOutputTypeDef = TypedDict(
     "ListResourcesAssociatedToCustomLineItemOutputTypeDef",
     {
         "Arn": str,
         "AssociatedResources": List[ListResourcesAssociatedToCustomLineItemResponseElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCustomLineItemChargeDetailsTypeDef = TypedDict(
     "UpdateCustomLineItemChargeDetailsTypeDef",
     {
         "Flat": UpdateCustomLineItemFlatChargeDetailsTypeDef,
@@ -1223,33 +1223,33 @@
 )
 
 BatchAssociateResourcesToCustomLineItemOutputTypeDef = TypedDict(
     "BatchAssociateResourcesToCustomLineItemOutputTypeDef",
     {
         "SuccessfullyAssociatedResources": List[AssociateResourceResponseElementTypeDef],
         "FailedAssociatedResources": List[AssociateResourceResponseElementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisassociateResourcesFromCustomLineItemOutputTypeDef = TypedDict(
     "BatchDisassociateResourcesFromCustomLineItemOutputTypeDef",
     {
         "SuccessfullyDisassociatedResources": List[DisassociateResourceResponseElementTypeDef],
         "FailedDisassociatedResources": List[DisassociateResourceResponseElementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBillingGroupsOutputTypeDef = TypedDict(
     "ListBillingGroupsOutputTypeDef",
     {
         "BillingGroups": List[BillingGroupListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreatePricingRuleInputRequestTypeDef",
     {
         "Name": str,
@@ -1371,29 +1371,29 @@
         "Arn": str,
         "BillingGroupArn": str,
         "Name": str,
         "Description": str,
         "ChargeDetails": ListCustomLineItemChargeDetailsTypeDef,
         "LastModifiedTime": int,
         "AssociationSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef = TypedDict(
     "_RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef = TypedDict(
     "_OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef",
     {
         "Filters": ListCustomLineItemVersionsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef(
     _RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef,
@@ -1488,38 +1488,38 @@
         "Service": str,
         "AssociatedPricingPlanCount": int,
         "LastModifiedTime": int,
         "BillingEntity": str,
         "Tiering": UpdateTieringInputTypeDef,
         "UsageType": str,
         "Operation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPricingRulesOutputTypeDef = TypedDict(
     "ListPricingRulesOutputTypeDef",
     {
         "BillingPeriod": str,
         "PricingRules": List[PricingRuleListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomLineItemsOutputTypeDef = TypedDict(
     "ListCustomLineItemsOutputTypeDef",
     {
         "CustomLineItems": List[CustomLineItemListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomLineItemVersionsOutputTypeDef = TypedDict(
     "ListCustomLineItemVersionsOutputTypeDef",
     {
         "CustomLineItemVersions": List[CustomLineItemVersionListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor/type_defs.pyi` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,86 +29,86 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountAssociationsListElementTypeDef",
     "AccountGroupingTypeDef",
     "AssociateAccountsInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateAccountsOutputTypeDef",
     "AssociatePricingRulesInputRequestTypeDef",
+    "AssociatePricingRulesOutputTypeDef",
     "AssociateResourceErrorTypeDef",
     "CustomLineItemBillingPeriodRangeTypeDef",
     "BillingGroupCostReportElementTypeDef",
     "ComputationPreferenceTypeDef",
+    "CreateBillingGroupOutputTypeDef",
+    "CreateCustomLineItemOutputTypeDef",
     "CreateFreeTierConfigTypeDef",
     "CreatePricingPlanInputRequestTypeDef",
+    "CreatePricingPlanOutputTypeDef",
+    "CreatePricingRuleOutputTypeDef",
     "CustomLineItemFlatChargeDetailsTypeDef",
     "CustomLineItemPercentageChargeDetailsTypeDef",
     "DeleteBillingGroupInputRequestTypeDef",
+    "DeleteBillingGroupOutputTypeDef",
+    "DeleteCustomLineItemOutputTypeDef",
     "DeletePricingPlanInputRequestTypeDef",
+    "DeletePricingPlanOutputTypeDef",
     "DeletePricingRuleInputRequestTypeDef",
+    "DeletePricingRuleOutputTypeDef",
     "DisassociateAccountsInputRequestTypeDef",
+    "DisassociateAccountsOutputTypeDef",
     "DisassociatePricingRulesInputRequestTypeDef",
+    "DisassociatePricingRulesOutputTypeDef",
     "FreeTierConfigTypeDef",
     "ListAccountAssociationsFilterTypeDef",
-    "PaginatorConfigTypeDef",
     "ListBillingGroupCostReportsFilterTypeDef",
     "ListBillingGroupsFilterTypeDef",
     "ListCustomLineItemFlatChargeDetailsTypeDef",
     "ListCustomLineItemPercentageChargeDetailsTypeDef",
     "ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef",
     "ListCustomLineItemsFilterTypeDef",
+    "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
     "ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef",
+    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
     "ListPricingPlansFilterTypeDef",
     "PricingPlanListElementTypeDef",
+    "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
     "ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
+    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
     "ListPricingRulesFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemResponseElementTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateBillingGroupOutputTypeDef",
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     "UpdateCustomLineItemPercentageChargeDetailsTypeDef",
     "UpdateFreeTierConfigTypeDef",
     "UpdatePricingPlanInputRequestTypeDef",
-    "AssociateAccountsOutputTypeDef",
-    "AssociatePricingRulesOutputTypeDef",
-    "CreateBillingGroupOutputTypeDef",
-    "CreateCustomLineItemOutputTypeDef",
-    "CreatePricingPlanOutputTypeDef",
-    "CreatePricingRuleOutputTypeDef",
-    "DeleteBillingGroupOutputTypeDef",
-    "DeleteCustomLineItemOutputTypeDef",
-    "DeletePricingPlanOutputTypeDef",
-    "DeletePricingRuleOutputTypeDef",
-    "DisassociateAccountsOutputTypeDef",
-    "DisassociatePricingRulesOutputTypeDef",
-    "ListAccountAssociationsOutputTypeDef",
-    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
-    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateBillingGroupOutputTypeDef",
     "UpdatePricingPlanOutputTypeDef",
+    "ListAccountAssociationsOutputTypeDef",
     "AssociateResourceResponseElementTypeDef",
     "DisassociateResourceResponseElementTypeDef",
     "BatchAssociateResourcesToCustomLineItemInputRequestTypeDef",
     "BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef",
     "DeleteCustomLineItemInputRequestTypeDef",
     "ListBillingGroupCostReportsOutputTypeDef",
     "BillingGroupListElementTypeDef",
     "CreateBillingGroupInputRequestTypeDef",
     "UpdateBillingGroupInputRequestTypeDef",
     "CreateTieringInputTypeDef",
     "CustomLineItemChargeDetailsTypeDef",
     "TieringTypeDef",
-    "ListAccountAssociationsInputRequestTypeDef",
     "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
-    "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    "ListAccountAssociationsInputRequestTypeDef",
     "ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef",
     "ListBillingGroupCostReportsInputRequestTypeDef",
     "ListBillingGroupsInputListBillingGroupsPaginateTypeDef",
     "ListBillingGroupsInputRequestTypeDef",
     "ListCustomLineItemChargeDetailsTypeDef",
     "ListCustomLineItemVersionsFilterTypeDef",
     "ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef",
@@ -164,33 +164,38 @@
     "AssociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateAccountsOutputTypeDef = TypedDict(
+    "AssociateAccountsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociatePricingRulesInputRequestTypeDef = TypedDict(
     "AssociatePricingRulesInputRequestTypeDef",
     {
         "Arn": str,
         "PricingRuleArns": Sequence[str],
     },
 )
 
+AssociatePricingRulesOutputTypeDef = TypedDict(
+    "AssociatePricingRulesOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateResourceErrorTypeDef = TypedDict(
     "AssociateResourceErrorTypeDef",
     {
         "Message": str,
         "Reason": AssociateResourceErrorReasonType,
     },
     total=False,
@@ -232,14 +237,30 @@
 ComputationPreferenceTypeDef = TypedDict(
     "ComputationPreferenceTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 
+CreateBillingGroupOutputTypeDef = TypedDict(
+    "CreateBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCustomLineItemOutputTypeDef = TypedDict(
+    "CreateCustomLineItemOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateFreeTierConfigTypeDef = TypedDict(
     "CreateFreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -261,14 +282,30 @@
 )
 
 class CreatePricingPlanInputRequestTypeDef(
     _RequiredCreatePricingPlanInputRequestTypeDef, _OptionalCreatePricingPlanInputRequestTypeDef
 ):
     pass
 
+CreatePricingPlanOutputTypeDef = TypedDict(
+    "CreatePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePricingRuleOutputTypeDef = TypedDict(
+    "CreatePricingRuleOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "CustomLineItemFlatChargeDetailsTypeDef",
     {
         "ChargeValue": float,
     },
 )
 
@@ -295,44 +332,92 @@
 DeleteBillingGroupInputRequestTypeDef = TypedDict(
     "DeleteBillingGroupInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeleteBillingGroupOutputTypeDef = TypedDict(
+    "DeleteBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteCustomLineItemOutputTypeDef = TypedDict(
+    "DeleteCustomLineItemOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePricingPlanInputRequestTypeDef = TypedDict(
     "DeletePricingPlanInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeletePricingPlanOutputTypeDef = TypedDict(
+    "DeletePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePricingRuleInputRequestTypeDef = TypedDict(
     "DeletePricingRuleInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeletePricingRuleOutputTypeDef = TypedDict(
+    "DeletePricingRuleOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateAccountsInputRequestTypeDef = TypedDict(
     "DisassociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
 )
 
+DisassociateAccountsOutputTypeDef = TypedDict(
+    "DisassociateAccountsOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociatePricingRulesInputRequestTypeDef = TypedDict(
     "DisassociatePricingRulesInputRequestTypeDef",
     {
         "Arn": str,
         "PricingRuleArns": Sequence[str],
     },
 )
 
+DisassociatePricingRulesOutputTypeDef = TypedDict(
+    "DisassociatePricingRulesOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FreeTierConfigTypeDef = TypedDict(
     "FreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -342,24 +427,14 @@
         "Association": str,
         "AccountId": str,
         "AccountIds": Sequence[str],
     },
     total=False,
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
 ListBillingGroupCostReportsFilterTypeDef = TypedDict(
     "ListBillingGroupCostReportsFilterTypeDef",
     {
         "BillingGroupArns": Sequence[str],
     },
     total=False,
 )
@@ -403,14 +478,35 @@
         "Names": Sequence[str],
         "BillingGroups": Sequence[str],
         "Arns": Sequence[str],
     },
     total=False,
 )
 
+_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
+    "_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
+    {
+        "PricingRuleArn": str,
+    },
+)
+_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
+    "_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
+    {
+        "BillingPeriod": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef(
+    _RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+    _OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+):
+    pass
+
 _RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef",
     {
         "PricingRuleArn": str,
     },
 )
 _OptionalListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = TypedDict(
@@ -425,14 +521,25 @@
 
 class ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef(
     _RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
     _OptionalListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
 ):
     pass
 
+ListPricingPlansAssociatedWithPricingRuleOutputTypeDef = TypedDict(
+    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
+    {
+        "BillingPeriod": str,
+        "PricingRuleArn": str,
+        "PricingPlanArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListPricingPlansFilterTypeDef = TypedDict(
     "ListPricingPlansFilterTypeDef",
     {
         "Arns": Sequence[str],
     },
     total=False,
 )
@@ -446,14 +553,35 @@
         "Size": int,
         "CreationTime": int,
         "LastModifiedTime": int,
     },
     total=False,
 )
 
+_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
+    "_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    {
+        "PricingPlanArn": str,
+    },
+)
+_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
+    "_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    {
+        "BillingPeriod": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef(
+    _RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+    _OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+):
+    pass
+
 _RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = TypedDict(
     "_RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 _OptionalListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = TypedDict(
@@ -468,14 +596,25 @@
 
 class ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef(
     _RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
     _OptionalListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
 ):
     pass
 
+ListPricingRulesAssociatedToPricingPlanOutputTypeDef = TypedDict(
+    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
+    {
+        "BillingPeriod": str,
+        "PricingPlanArn": str,
+        "PricingRuleArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListPricingRulesFilterTypeDef = TypedDict(
     "ListPricingRulesFilterTypeDef",
     {
         "Arns": Sequence[str],
     },
     total=False,
 )
@@ -501,14 +640,43 @@
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
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -517,14 +685,30 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateBillingGroupOutputTypeDef = TypedDict(
+    "UpdateBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "PrimaryAccountId": str,
+        "PricingPlanArn": str,
+        "Size": int,
+        "LastModifiedTime": int,
+        "Status": BillingGroupStatusType,
+        "StatusReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateCustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     {
         "ChargeValue": float,
     },
 )
 
@@ -558,174 +742,32 @@
 )
 
 class UpdatePricingPlanInputRequestTypeDef(
     _RequiredUpdatePricingPlanInputRequestTypeDef, _OptionalUpdatePricingPlanInputRequestTypeDef
 ):
     pass
 
-AssociateAccountsOutputTypeDef = TypedDict(
-    "AssociateAccountsOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociatePricingRulesOutputTypeDef = TypedDict(
-    "AssociatePricingRulesOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBillingGroupOutputTypeDef = TypedDict(
-    "CreateBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCustomLineItemOutputTypeDef = TypedDict(
-    "CreateCustomLineItemOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePricingPlanOutputTypeDef = TypedDict(
-    "CreatePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePricingRuleOutputTypeDef = TypedDict(
-    "CreatePricingRuleOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBillingGroupOutputTypeDef = TypedDict(
-    "DeleteBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteCustomLineItemOutputTypeDef = TypedDict(
-    "DeleteCustomLineItemOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePricingPlanOutputTypeDef = TypedDict(
-    "DeletePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePricingRuleOutputTypeDef = TypedDict(
-    "DeletePricingRuleOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateAccountsOutputTypeDef = TypedDict(
-    "DisassociateAccountsOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociatePricingRulesOutputTypeDef = TypedDict(
-    "DisassociatePricingRulesOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAccountAssociationsOutputTypeDef = TypedDict(
-    "ListAccountAssociationsOutputTypeDef",
-    {
-        "LinkedAccounts": List[AccountAssociationsListElementTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPricingPlansAssociatedWithPricingRuleOutputTypeDef = TypedDict(
-    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
-    {
-        "BillingPeriod": str,
-        "PricingRuleArn": str,
-        "PricingPlanArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPricingRulesAssociatedToPricingPlanOutputTypeDef = TypedDict(
-    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
-    {
-        "BillingPeriod": str,
-        "PricingPlanArn": str,
-        "PricingRuleArns": List[str],
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
-UpdateBillingGroupOutputTypeDef = TypedDict(
-    "UpdateBillingGroupOutputTypeDef",
+UpdatePricingPlanOutputTypeDef = TypedDict(
+    "UpdatePricingPlanOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Description": str,
-        "PrimaryAccountId": str,
-        "PricingPlanArn": str,
         "Size": int,
         "LastModifiedTime": int,
-        "Status": BillingGroupStatusType,
-        "StatusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdatePricingPlanOutputTypeDef = TypedDict(
-    "UpdatePricingPlanOutputTypeDef",
+ListAccountAssociationsOutputTypeDef = TypedDict(
+    "ListAccountAssociationsOutputTypeDef",
     {
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "Size": int,
-        "LastModifiedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LinkedAccounts": List[AccountAssociationsListElementTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateResourceResponseElementTypeDef = TypedDict(
     "AssociateResourceResponseElementTypeDef",
     {
         "Arn": str,
@@ -806,15 +848,15 @@
     pass
 
 ListBillingGroupCostReportsOutputTypeDef = TypedDict(
     "ListBillingGroupCostReportsOutputTypeDef",
     {
         "BillingGroupCostReports": List[BillingGroupCostReportElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BillingGroupListElementTypeDef = TypedDict(
     "BillingGroupListElementTypeDef",
     {
         "Name": str,
@@ -907,82 +949,40 @@
 TieringTypeDef = TypedDict(
     "TieringTypeDef",
     {
         "FreeTier": FreeTierConfigTypeDef,
     },
 )
 
-ListAccountAssociationsInputRequestTypeDef = TypedDict(
-    "ListAccountAssociationsInputRequestTypeDef",
-    {
-        "BillingPeriod": str,
-        "Filters": ListAccountAssociationsFilterTypeDef,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef = TypedDict(
     "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListAccountAssociationsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
-    "_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    {
-        "PricingRuleArn": str,
-    },
-)
-_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
-    "_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    {
-        "BillingPeriod": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef(
-    _RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-    _OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-):
-    pass
-
-_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
-    "_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
-    {
-        "PricingPlanArn": str,
-    },
-)
-_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
-    "_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+ListAccountAssociationsInputRequestTypeDef = TypedDict(
+    "ListAccountAssociationsInputRequestTypeDef",
     {
         "BillingPeriod": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Filters": ListAccountAssociationsFilterTypeDef,
+        "NextToken": str,
     },
     total=False,
 )
 
-class ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef(
-    _RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
-    _OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
-):
-    pass
-
 ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef = TypedDict(
     "ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListBillingGroupCostReportsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBillingGroupCostReportsInputRequestTypeDef = TypedDict(
     "ListBillingGroupCostReportsInputRequestTypeDef",
     {
@@ -995,15 +995,15 @@
 )
 
 ListBillingGroupsInputListBillingGroupsPaginateTypeDef = TypedDict(
     "ListBillingGroupsInputListBillingGroupsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListBillingGroupsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBillingGroupsInputRequestTypeDef = TypedDict(
     "ListBillingGroupsInputRequestTypeDef",
     {
@@ -1044,15 +1044,15 @@
 )
 
 ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef = TypedDict(
     "ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListCustomLineItemsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCustomLineItemsInputRequestTypeDef = TypedDict(
     "ListCustomLineItemsInputRequestTypeDef",
     {
@@ -1065,15 +1065,15 @@
 )
 
 ListPricingPlansInputListPricingPlansPaginateTypeDef = TypedDict(
     "ListPricingPlansInputListPricingPlansPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListPricingPlansFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPricingPlansInputRequestTypeDef = TypedDict(
     "ListPricingPlansInputRequestTypeDef",
     {
@@ -1087,24 +1087,24 @@
 
 ListPricingPlansOutputTypeDef = TypedDict(
     "ListPricingPlansOutputTypeDef",
     {
         "BillingPeriod": str,
         "PricingPlans": List[PricingPlanListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPricingRulesInputListPricingRulesPaginateTypeDef = TypedDict(
     "ListPricingRulesInputListPricingRulesPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListPricingRulesFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPricingRulesInputRequestTypeDef = TypedDict(
     "ListPricingRulesInputRequestTypeDef",
     {
@@ -1123,15 +1123,15 @@
     },
 )
 _OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef = TypedDict(
     "_OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListResourcesAssociatedToCustomLineItemFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef(
     _RequiredListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef,
     _OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef,
@@ -1163,15 +1163,15 @@
 
 ListResourcesAssociatedToCustomLineItemOutputTypeDef = TypedDict(
     "ListResourcesAssociatedToCustomLineItemOutputTypeDef",
     {
         "Arn": str,
         "AssociatedResources": List[ListResourcesAssociatedToCustomLineItemResponseElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCustomLineItemChargeDetailsTypeDef = TypedDict(
     "UpdateCustomLineItemChargeDetailsTypeDef",
     {
         "Flat": UpdateCustomLineItemFlatChargeDetailsTypeDef,
@@ -1188,33 +1188,33 @@
 )
 
 BatchAssociateResourcesToCustomLineItemOutputTypeDef = TypedDict(
     "BatchAssociateResourcesToCustomLineItemOutputTypeDef",
     {
         "SuccessfullyAssociatedResources": List[AssociateResourceResponseElementTypeDef],
         "FailedAssociatedResources": List[AssociateResourceResponseElementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisassociateResourcesFromCustomLineItemOutputTypeDef = TypedDict(
     "BatchDisassociateResourcesFromCustomLineItemOutputTypeDef",
     {
         "SuccessfullyDisassociatedResources": List[DisassociateResourceResponseElementTypeDef],
         "FailedDisassociatedResources": List[DisassociateResourceResponseElementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBillingGroupsOutputTypeDef = TypedDict(
     "ListBillingGroupsOutputTypeDef",
     {
         "BillingGroups": List[BillingGroupListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreatePricingRuleInputRequestTypeDef",
     {
         "Name": str,
@@ -1332,29 +1332,29 @@
         "Arn": str,
         "BillingGroupArn": str,
         "Name": str,
         "Description": str,
         "ChargeDetails": ListCustomLineItemChargeDetailsTypeDef,
         "LastModifiedTime": int,
         "AssociationSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef = TypedDict(
     "_RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef = TypedDict(
     "_OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef",
     {
         "Filters": ListCustomLineItemVersionsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef(
     _RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef,
     _OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef,
@@ -1441,38 +1441,38 @@
         "Service": str,
         "AssociatedPricingPlanCount": int,
         "LastModifiedTime": int,
         "BillingEntity": str,
         "Tiering": UpdateTieringInputTypeDef,
         "UsageType": str,
         "Operation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPricingRulesOutputTypeDef = TypedDict(
     "ListPricingRulesOutputTypeDef",
     {
         "BillingPeriod": str,
         "PricingRules": List[PricingRuleListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomLineItemsOutputTypeDef = TypedDict(
     "ListCustomLineItemsOutputTypeDef",
     {
         "CustomLineItems": List[CustomLineItemListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomLineItemVersionsOutputTypeDef = TypedDict(
     "ListCustomLineItemVersionsOutputTypeDef",
     {
         "CustomLineItemVersions": List[CustomLineItemVersionListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor.egg-info/PKG-INFO` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-billingconductor
-Version: 1.26.94
-Summary: Type annotations for boto3.BillingConductor 1.26.94 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.BillingConductor 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-billingconductor"></a>
 
 # mypy-boto3-billingconductor
 
 [![PyPI - mypy-boto3-billingconductor](https://img.shields.io/pypi/v/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-billingconductor?color=blue)](https://pypistats.org/packages/mypy-boto3-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BillingConductor 1.26.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[boto3.BillingConductor 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-billingconductor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,86 +374,86 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_billingconductor.type_defs import (
     AccountAssociationsListElementTypeDef,
     AccountGroupingTypeDef,
     AssociateAccountsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateAccountsOutputTypeDef,
     AssociatePricingRulesInputRequestTypeDef,
+    AssociatePricingRulesOutputTypeDef,
     AssociateResourceErrorTypeDef,
     CustomLineItemBillingPeriodRangeTypeDef,
     BillingGroupCostReportElementTypeDef,
     ComputationPreferenceTypeDef,
+    CreateBillingGroupOutputTypeDef,
+    CreateCustomLineItemOutputTypeDef,
     CreateFreeTierConfigTypeDef,
     CreatePricingPlanInputRequestTypeDef,
+    CreatePricingPlanOutputTypeDef,
+    CreatePricingRuleOutputTypeDef,
     CustomLineItemFlatChargeDetailsTypeDef,
     CustomLineItemPercentageChargeDetailsTypeDef,
     DeleteBillingGroupInputRequestTypeDef,
+    DeleteBillingGroupOutputTypeDef,
+    DeleteCustomLineItemOutputTypeDef,
     DeletePricingPlanInputRequestTypeDef,
+    DeletePricingPlanOutputTypeDef,
     DeletePricingRuleInputRequestTypeDef,
+    DeletePricingRuleOutputTypeDef,
     DisassociateAccountsInputRequestTypeDef,
+    DisassociateAccountsOutputTypeDef,
     DisassociatePricingRulesInputRequestTypeDef,
+    DisassociatePricingRulesOutputTypeDef,
     FreeTierConfigTypeDef,
     ListAccountAssociationsFilterTypeDef,
-    PaginatorConfigTypeDef,
     ListBillingGroupCostReportsFilterTypeDef,
     ListBillingGroupsFilterTypeDef,
     ListCustomLineItemFlatChargeDetailsTypeDef,
     ListCustomLineItemPercentageChargeDetailsTypeDef,
     ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef,
     ListCustomLineItemsFilterTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
     ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
     ListPricingPlansFilterTypeDef,
     PricingPlanListElementTypeDef,
+    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
     ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
+    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
     ListPricingRulesFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemResponseElementTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateBillingGroupOutputTypeDef,
     UpdateCustomLineItemFlatChargeDetailsTypeDef,
     UpdateCustomLineItemPercentageChargeDetailsTypeDef,
     UpdateFreeTierConfigTypeDef,
     UpdatePricingPlanInputRequestTypeDef,
-    AssociateAccountsOutputTypeDef,
-    AssociatePricingRulesOutputTypeDef,
-    CreateBillingGroupOutputTypeDef,
-    CreateCustomLineItemOutputTypeDef,
-    CreatePricingPlanOutputTypeDef,
-    CreatePricingRuleOutputTypeDef,
-    DeleteBillingGroupOutputTypeDef,
-    DeleteCustomLineItemOutputTypeDef,
-    DeletePricingPlanOutputTypeDef,
-    DeletePricingRuleOutputTypeDef,
-    DisassociateAccountsOutputTypeDef,
-    DisassociatePricingRulesOutputTypeDef,
-    ListAccountAssociationsOutputTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
-    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateBillingGroupOutputTypeDef,
     UpdatePricingPlanOutputTypeDef,
+    ListAccountAssociationsOutputTypeDef,
     AssociateResourceResponseElementTypeDef,
     DisassociateResourceResponseElementTypeDef,
     BatchAssociateResourcesToCustomLineItemInputRequestTypeDef,
     BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef,
     DeleteCustomLineItemInputRequestTypeDef,
     ListBillingGroupCostReportsOutputTypeDef,
     BillingGroupListElementTypeDef,
     CreateBillingGroupInputRequestTypeDef,
     UpdateBillingGroupInputRequestTypeDef,
     CreateTieringInputTypeDef,
     CustomLineItemChargeDetailsTypeDef,
     TieringTypeDef,
-    ListAccountAssociationsInputRequestTypeDef,
     ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+    ListAccountAssociationsInputRequestTypeDef,
     ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef,
     ListBillingGroupCostReportsInputRequestTypeDef,
     ListBillingGroupsInputListBillingGroupsPaginateTypeDef,
     ListBillingGroupsInputRequestTypeDef,
     ListCustomLineItemChargeDetailsTypeDef,
     ListCustomLineItemVersionsFilterTypeDef,
     ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef,
@@ -495,42 +495,42 @@
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

### Comparing `mypy-boto3-billingconductor-1.26.94/mypy_boto3_billingconductor.egg-info/SOURCES.txt` & `mypy-boto3-billingconductor-1.27.0/mypy_boto3_billingconductor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.26.94/setup.py` & `mypy-boto3-billingconductor-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-billingconductor.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-billingconductor",
-    version="1.26.94",
+    version="1.27.0",
     packages=["mypy_boto3_billingconductor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.BillingConductor 1.26.94 service generated with"
-        " mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.BillingConductor 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/",
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


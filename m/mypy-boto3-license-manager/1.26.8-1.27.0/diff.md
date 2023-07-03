# Comparing `tmp/mypy-boto3-license-manager-1.26.8.tar.gz` & `tmp/mypy-boto3-license-manager-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-1.26.8.tar", last modified: Fri Nov 11 21:07:54 2022, max compression
+gzip compressed data, was "mypy-boto3-license-manager-1.27.0.tar", last modified: Mon Jul  3 19:51:01 2023, max compression
```

## Comparing `mypy-boto3-license-manager-1.26.8.tar` & `mypy-boto3-license-manager-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.050122 mypy-boto3-license-manager-1.26.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    20161 2022-11-11 21:07:54.050122 mypy-boto3-license-manager-1.26.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18695 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.050122 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40665 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    40603 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11544 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    11542 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7586 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7579 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    54780 2022-11-11 21:07:30.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    54709 2022-11-11 21:07:29.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.050122 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    20161 2022-11-11 21:07:53.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-11-11 21:07:53.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 21:07:53.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-11 21:07:53.000000 mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 21:07:54.050122 mypy-boto3-license-manager-1.26.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-11-11 21:07:28.000000 mypy-boto3-license-manager-1.26.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.783563 mypy-boto3-license-manager-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20263 2023-07-03 19:51:01.783563 mypy-boto3-license-manager-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18747 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.771562 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40707 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55151 2023-07-03 19:41:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55080 2023-07-03 19:41:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.783563 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20263 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:01.783563 mypy-boto3-license-manager-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/setup.py
```

### Comparing `mypy-boto3-license-manager-1.26.8/LICENSE` & `mypy-boto3-license-manager-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-license-manager-1.26.8/PKG-INFO` & `mypy-boto3-license-manager-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,60 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-license-manager
-Version: 1.26.8
-Summary: Type annotations for boto3.LicenseManager 1.26.8 service generated with mypy-boto3-builder 7.11.10
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 license-manager type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-license-manager"></a>
 
 # mypy-boto3-license-manager
 
 [![PyPI - mypy-boto3-license-manager](https://img.shields.io/pypi/v/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,14 +286,15 @@
 ### Literals
 
 `mypy_boto3_license_manager.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_license_manager.literals import (
+    ActivationOverrideBehaviorType,
     AllowedOperationType,
     CheckoutTypeType,
     DigitalSignatureMethodType,
     EntitlementDataUnitType,
     EntitlementUnitType,
     GrantStatusType,
     InventoryFilterConditionType,
@@ -348,146 +318,147 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: AllowedOperationType) -> bool:
+def check_value(value: ActivationOverrideBehaviorType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_license_manager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AcceptGrantResponseTypeDef,
     AutomatedDiscoveryInformationTypeDef,
     BorrowConfigurationTypeDef,
     CheckInLicenseRequestRequestTypeDef,
     EntitlementDataTypeDef,
     MetadataTypeDef,
     ConsumedLicenseSummaryTypeDef,
     ProvisionalConfigurationTypeDef,
     CreateGrantRequestRequestTypeDef,
-    CreateGrantVersionRequestRequestTypeDef,
+    CreateGrantResponseTypeDef,
+    OptionsTypeDef,
+    CreateGrantVersionResponseTypeDef,
     TagTypeDef,
+    CreateLicenseConfigurationResponseTypeDef,
     LicenseConversionContextTypeDef,
+    CreateLicenseConversionTaskForResourceResponseTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
+    CreateLicenseManagerReportGeneratorResponseTypeDef,
     DatetimeRangeTypeDef,
     EntitlementTypeDef,
     IssuerTypeDef,
+    CreateLicenseResponseTypeDef,
+    CreateLicenseVersionResponseTypeDef,
     CreateTokenRequestRequestTypeDef,
+    CreateTokenResponseTypeDef,
     DeleteGrantRequestRequestTypeDef,
+    DeleteGrantResponseTypeDef,
     DeleteLicenseConfigurationRequestRequestTypeDef,
     DeleteLicenseManagerReportGeneratorRequestRequestTypeDef,
     DeleteLicenseRequestRequestTypeDef,
+    DeleteLicenseResponseTypeDef,
     DeleteTokenRequestRequestTypeDef,
     EntitlementUsageTypeDef,
     ExtendLicenseConsumptionRequestRequestTypeDef,
+    ExtendLicenseConsumptionResponseTypeDef,
     FilterTypeDef,
     GetAccessTokenRequestRequestTypeDef,
+    GetAccessTokenResponseTypeDef,
     GetGrantRequestRequestTypeDef,
-    GrantTypeDef,
     GetLicenseConfigurationRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
     GetLicenseConversionTaskRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorRequestRequestTypeDef,
     GetLicenseRequestRequestTypeDef,
     GetLicenseUsageRequestRequestTypeDef,
     OrganizationConfigurationTypeDef,
     IssuerDetailsTypeDef,
     ReceivedMetadataTypeDef,
     InventoryFilterTypeDef,
     LicenseConfigurationAssociationTypeDef,
     LicenseConfigurationUsageTypeDef,
     LicenseSpecificationTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
     ListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
+    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListLicenseVersionsRequestRequestTypeDef,
     ResourceInventoryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TokenDataTypeDef,
+    PaginatorConfigTypeDef,
     ProductInformationFilterTypeDef,
     RejectGrantRequestRequestTypeDef,
+    RejectGrantResponseTypeDef,
     S3LocationTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AcceptGrantResponseTypeDef,
-    CreateGrantResponseTypeDef,
-    CreateGrantVersionResponseTypeDef,
-    CreateLicenseConfigurationResponseTypeDef,
-    CreateLicenseConversionTaskForResourceResponseTypeDef,
-    CreateLicenseManagerReportGeneratorResponseTypeDef,
-    CreateLicenseResponseTypeDef,
-    CreateLicenseVersionResponseTypeDef,
-    CreateTokenResponseTypeDef,
-    DeleteGrantResponseTypeDef,
-    DeleteLicenseResponseTypeDef,
-    ExtendLicenseConsumptionResponseTypeDef,
-    GetAccessTokenResponseTypeDef,
-    RejectGrantResponseTypeDef,
     CheckoutLicenseRequestRequestTypeDef,
     CheckoutLicenseResponseTypeDef,
     CheckoutBorrowLicenseRequestRequestTypeDef,
     CheckoutBorrowLicenseResponseTypeDef,
     LicenseOperationFailureTypeDef,
     ConsumptionConfigurationTypeDef,
+    CreateGrantVersionRequestRequestTypeDef,
+    GrantTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLicenseConversionTaskForResourceRequestRequestTypeDef,
     GetLicenseConversionTaskResponseTypeDef,
     LicenseConversionTaskTypeDef,
     CreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     UpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     LicenseUsageTypeDef,
     ListDistributedGrantsRequestRequestTypeDef,
+    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
     ListLicenseConfigurationsRequestRequestTypeDef,
     ListLicenseConversionTasksRequestRequestTypeDef,
     ListLicenseManagerReportGeneratorsRequestRequestTypeDef,
     ListLicensesRequestRequestTypeDef,
     ListReceivedGrantsForOrganizationRequestRequestTypeDef,
     ListReceivedGrantsRequestRequestTypeDef,
     ListReceivedLicensesForOrganizationRequestRequestTypeDef,
     ListReceivedLicensesRequestRequestTypeDef,
     ListTokensRequestRequestTypeDef,
+    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestRequestTypeDef,
-    GetGrantResponseTypeDef,
-    ListDistributedGrantsResponseTypeDef,
-    ListReceivedGrantsForOrganizationResponseTypeDef,
-    ListReceivedGrantsResponseTypeDef,
     GetServiceSettingsResponseTypeDef,
     UpdateServiceSettingsRequestRequestTypeDef,
+    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
     ListResourceInventoryRequestRequestTypeDef,
     ListAssociationsForLicenseConfigurationResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     ListLicenseSpecificationsForResourceResponseTypeDef,
     UpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
-    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
-    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
-    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
     ProductInformationTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
     CreateLicenseRequestRequestTypeDef,
     CreateLicenseVersionRequestRequestTypeDef,
     GrantedLicenseTypeDef,
     LicenseTypeDef,
+    GetGrantResponseTypeDef,
+    ListDistributedGrantsResponseTypeDef,
+    ListReceivedGrantsForOrganizationResponseTypeDef,
+    ListReceivedGrantsResponseTypeDef,
     ListLicenseConversionTasksResponseTypeDef,
     GetLicenseUsageResponseTypeDef,
     CreateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
     UpdateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
@@ -508,42 +479,42 @@
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

### Comparing `mypy-boto3-license-manager-1.26.8/README.md` & `mypy-boto3-license-manager-1.27.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-license-manager
+Version: 1.27.0
+Summary: Type annotations for boto3.LicenseManager 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 license-manager type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-license-manager"></a>
 
 # mypy-boto3-license-manager
 
 [![PyPI - mypy-boto3-license-manager](https://img.shields.io/pypi/v/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,14 +318,15 @@
 ### Literals
 
 `mypy_boto3_license_manager.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_license_manager.literals import (
+    ActivationOverrideBehaviorType,
     AllowedOperationType,
     CheckoutTypeType,
     DigitalSignatureMethodType,
     EntitlementDataUnitType,
     EntitlementUnitType,
     GrantStatusType,
     InventoryFilterConditionType,
@@ -317,146 +350,147 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: AllowedOperationType) -> bool:
+def check_value(value: ActivationOverrideBehaviorType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_license_manager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AcceptGrantResponseTypeDef,
     AutomatedDiscoveryInformationTypeDef,
     BorrowConfigurationTypeDef,
     CheckInLicenseRequestRequestTypeDef,
     EntitlementDataTypeDef,
     MetadataTypeDef,
     ConsumedLicenseSummaryTypeDef,
     ProvisionalConfigurationTypeDef,
     CreateGrantRequestRequestTypeDef,
-    CreateGrantVersionRequestRequestTypeDef,
+    CreateGrantResponseTypeDef,
+    OptionsTypeDef,
+    CreateGrantVersionResponseTypeDef,
     TagTypeDef,
+    CreateLicenseConfigurationResponseTypeDef,
     LicenseConversionContextTypeDef,
+    CreateLicenseConversionTaskForResourceResponseTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
+    CreateLicenseManagerReportGeneratorResponseTypeDef,
     DatetimeRangeTypeDef,
     EntitlementTypeDef,
     IssuerTypeDef,
+    CreateLicenseResponseTypeDef,
+    CreateLicenseVersionResponseTypeDef,
     CreateTokenRequestRequestTypeDef,
+    CreateTokenResponseTypeDef,
     DeleteGrantRequestRequestTypeDef,
+    DeleteGrantResponseTypeDef,
     DeleteLicenseConfigurationRequestRequestTypeDef,
     DeleteLicenseManagerReportGeneratorRequestRequestTypeDef,
     DeleteLicenseRequestRequestTypeDef,
+    DeleteLicenseResponseTypeDef,
     DeleteTokenRequestRequestTypeDef,
     EntitlementUsageTypeDef,
     ExtendLicenseConsumptionRequestRequestTypeDef,
+    ExtendLicenseConsumptionResponseTypeDef,
     FilterTypeDef,
     GetAccessTokenRequestRequestTypeDef,
+    GetAccessTokenResponseTypeDef,
     GetGrantRequestRequestTypeDef,
-    GrantTypeDef,
     GetLicenseConfigurationRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
     GetLicenseConversionTaskRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorRequestRequestTypeDef,
     GetLicenseRequestRequestTypeDef,
     GetLicenseUsageRequestRequestTypeDef,
     OrganizationConfigurationTypeDef,
     IssuerDetailsTypeDef,
     ReceivedMetadataTypeDef,
     InventoryFilterTypeDef,
     LicenseConfigurationAssociationTypeDef,
     LicenseConfigurationUsageTypeDef,
     LicenseSpecificationTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
     ListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
+    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListLicenseVersionsRequestRequestTypeDef,
     ResourceInventoryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TokenDataTypeDef,
+    PaginatorConfigTypeDef,
     ProductInformationFilterTypeDef,
     RejectGrantRequestRequestTypeDef,
+    RejectGrantResponseTypeDef,
     S3LocationTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AcceptGrantResponseTypeDef,
-    CreateGrantResponseTypeDef,
-    CreateGrantVersionResponseTypeDef,
-    CreateLicenseConfigurationResponseTypeDef,
-    CreateLicenseConversionTaskForResourceResponseTypeDef,
-    CreateLicenseManagerReportGeneratorResponseTypeDef,
-    CreateLicenseResponseTypeDef,
-    CreateLicenseVersionResponseTypeDef,
-    CreateTokenResponseTypeDef,
-    DeleteGrantResponseTypeDef,
-    DeleteLicenseResponseTypeDef,
-    ExtendLicenseConsumptionResponseTypeDef,
-    GetAccessTokenResponseTypeDef,
-    RejectGrantResponseTypeDef,
     CheckoutLicenseRequestRequestTypeDef,
     CheckoutLicenseResponseTypeDef,
     CheckoutBorrowLicenseRequestRequestTypeDef,
     CheckoutBorrowLicenseResponseTypeDef,
     LicenseOperationFailureTypeDef,
     ConsumptionConfigurationTypeDef,
+    CreateGrantVersionRequestRequestTypeDef,
+    GrantTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLicenseConversionTaskForResourceRequestRequestTypeDef,
     GetLicenseConversionTaskResponseTypeDef,
     LicenseConversionTaskTypeDef,
     CreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     UpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     LicenseUsageTypeDef,
     ListDistributedGrantsRequestRequestTypeDef,
+    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
     ListLicenseConfigurationsRequestRequestTypeDef,
     ListLicenseConversionTasksRequestRequestTypeDef,
     ListLicenseManagerReportGeneratorsRequestRequestTypeDef,
     ListLicensesRequestRequestTypeDef,
     ListReceivedGrantsForOrganizationRequestRequestTypeDef,
     ListReceivedGrantsRequestRequestTypeDef,
     ListReceivedLicensesForOrganizationRequestRequestTypeDef,
     ListReceivedLicensesRequestRequestTypeDef,
     ListTokensRequestRequestTypeDef,
+    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestRequestTypeDef,
-    GetGrantResponseTypeDef,
-    ListDistributedGrantsResponseTypeDef,
-    ListReceivedGrantsForOrganizationResponseTypeDef,
-    ListReceivedGrantsResponseTypeDef,
     GetServiceSettingsResponseTypeDef,
     UpdateServiceSettingsRequestRequestTypeDef,
+    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
     ListResourceInventoryRequestRequestTypeDef,
     ListAssociationsForLicenseConfigurationResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     ListLicenseSpecificationsForResourceResponseTypeDef,
     UpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
-    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
-    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
-    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
     ProductInformationTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
     CreateLicenseRequestRequestTypeDef,
     CreateLicenseVersionRequestRequestTypeDef,
     GrantedLicenseTypeDef,
     LicenseTypeDef,
+    GetGrantResponseTypeDef,
+    ListDistributedGrantsResponseTypeDef,
+    ListReceivedGrantsForOrganizationResponseTypeDef,
+    ListReceivedGrantsResponseTypeDef,
     ListLicenseConversionTasksResponseTypeDef,
     GetLicenseUsageResponseTypeDef,
     CreateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
     UpdateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
@@ -477,42 +511,42 @@
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

### Comparing `mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/__init__.py` & `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/__init__.pyi` & `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/client.py` & `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     ListReceivedLicensesForOrganizationResponseTypeDef,
     ListReceivedLicensesResponseTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTokensResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     MetadataTypeDef,
+    OptionsTypeDef,
     OrganizationConfigurationTypeDef,
     ProductInformationTypeDef,
     RejectGrantResponseTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
     TagTypeDef,
 )
@@ -238,15 +239,16 @@
         *,
         ClientToken: str,
         GrantArn: str,
         GrantName: str = ...,
         AllowedOperations: Sequence[AllowedOperationType] = ...,
         Status: GrantStatusType = ...,
         StatusReason: str = ...,
-        SourceVersion: str = ...
+        SourceVersion: str = ...,
+        Options: OptionsTypeDef = ...
     ) -> CreateGrantVersionResponseTypeDef:
         """
         Creates a new version of the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_grant_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#create_grant_version)
         """
@@ -616,15 +618,15 @@
         *,
         GrantArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListReceivedGrantsResponseTypeDef:
         """
-        Lists grants that are received but not accepted.
+        Lists grants that are received.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_grants)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#list_received_grants)
         """
 
     def list_received_grants_for_organization(
         self,
```

### Comparing `mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/client.pyi` & `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     ListReceivedLicensesForOrganizationResponseTypeDef,
     ListReceivedLicensesResponseTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTokensResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     MetadataTypeDef,
+    OptionsTypeDef,
     OrganizationConfigurationTypeDef,
     ProductInformationTypeDef,
     RejectGrantResponseTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
     TagTypeDef,
 )
@@ -226,15 +227,16 @@
         *,
         ClientToken: str,
         GrantArn: str,
         GrantName: str = ...,
         AllowedOperations: Sequence[AllowedOperationType] = ...,
         Status: GrantStatusType = ...,
         StatusReason: str = ...,
-        SourceVersion: str = ...
+        SourceVersion: str = ...,
+        Options: OptionsTypeDef = ...
     ) -> CreateGrantVersionResponseTypeDef:
         """
         Creates a new version of the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_grant_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#create_grant_version)
         """
@@ -573,15 +575,15 @@
         *,
         GrantArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListReceivedGrantsResponseTypeDef:
         """
-        Lists grants that are received but not accepted.
+        Lists grants that are received.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_grants)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#list_received_grants)
         """
     def list_received_grants_for_organization(
         self,
         *,
```

### Comparing `mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/literals.py` & `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 Type annotations for license-manager service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_license_manager.literals import AllowedOperationType
+    from mypy_boto3_license_manager.literals import ActivationOverrideBehaviorType
 
-    data: AllowedOperationType = "CheckInLicense"
+    data: ActivationOverrideBehaviorType = "ALL_GRANTS_PERMITTED_BY_ISSUER"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "ActivationOverrideBehaviorType",
     "AllowedOperationType",
     "CheckoutTypeType",
     "DigitalSignatureMethodType",
     "EntitlementDataUnitType",
     "EntitlementUnitType",
     "GrantStatusType",
     "InventoryFilterConditionType",
@@ -47,14 +48,17 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
+ActivationOverrideBehaviorType = Literal[
+    "ALL_GRANTS_PERMITTED_BY_ISSUER", "DISTRIBUTED_GRANTS_ONLY"
+]
 AllowedOperationType = Literal[
     "CheckInLicense",
     "CheckoutBorrowLicense",
     "CheckoutLicense",
     "CreateGrant",
     "CreateToken",
     "ExtendConsumptionLicense",
@@ -183,23 +187,25 @@
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
@@ -209,30 +215,35 @@
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
@@ -258,14 +269,15 @@
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
@@ -310,51 +322,57 @@
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
@@ -367,14 +385,15 @@
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
@@ -386,28 +405,35 @@
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
@@ -435,56 +461,64 @@
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
```

### Comparing `mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/literals.pyi` & `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 Type annotations for license-manager service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_license_manager.literals import AllowedOperationType
+    from mypy_boto3_license_manager.literals import ActivationOverrideBehaviorType
 
-    data: AllowedOperationType = "CheckInLicense"
+    data: ActivationOverrideBehaviorType = "ALL_GRANTS_PERMITTED_BY_ISSUER"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "ActivationOverrideBehaviorType",
     "AllowedOperationType",
     "CheckoutTypeType",
     "DigitalSignatureMethodType",
     "EntitlementDataUnitType",
     "EntitlementUnitType",
     "GrantStatusType",
     "InventoryFilterConditionType",
@@ -45,14 +46,17 @@
     "LicenseManagerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+ActivationOverrideBehaviorType = Literal[
+    "ALL_GRANTS_PERMITTED_BY_ISSUER", "DISTRIBUTED_GRANTS_ONLY"
+]
 AllowedOperationType = Literal[
     "CheckInLicense",
     "CheckoutBorrowLicense",
     "CheckoutLicense",
     "CreateGrant",
     "CreateToken",
     "ExtendConsumptionLicense",
@@ -181,23 +185,25 @@
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
@@ -207,30 +213,35 @@
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
@@ -256,14 +267,15 @@
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
@@ -308,51 +320,57 @@
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
@@ -365,14 +383,15 @@
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
@@ -384,28 +403,35 @@
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
@@ -433,56 +459,64 @@
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
```

### Comparing `mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/paginator.py` & `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class ListAssociationsForLicenseConfigurationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listassociationsforlicenseconfigurationpaginator)
     """
 
     def paginate(
-        self, *, LicenseConfigurationArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, LicenseConfigurationArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociationsForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listassociationsforlicenseconfigurationpaginator)
         """
 
 
@@ -83,30 +83,30 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLicenseConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listlicenseconfigurationspaginator)
         """
 
 
 class ListLicenseSpecificationsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listlicensespecificationsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLicenseSpecificationsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listlicensespecificationsforresourcepaginator)
         """
 
 
@@ -116,15 +116,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listresourceinventorypaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceInventoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListResourceInventory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listresourceinventorypaginator)
         """
 
 
@@ -135,13 +135,13 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsageForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListUsageForLicenseConfiguration.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listusageforlicenseconfigurationpaginator)
         """
```

### Comparing `mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/paginator.pyi` & `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 class ListAssociationsForLicenseConfigurationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listassociationsforlicenseconfigurationpaginator)
     """
 
     def paginate(
-        self, *, LicenseConfigurationArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, LicenseConfigurationArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociationsForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listassociationsforlicenseconfigurationpaginator)
         """
 
 class ListLicenseConfigurationsPaginator(Paginator):
@@ -79,29 +79,29 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLicenseConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listlicenseconfigurationspaginator)
         """
 
 class ListLicenseSpecificationsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listlicensespecificationsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLicenseSpecificationsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listlicensespecificationsforresourcepaginator)
         """
 
 class ListResourceInventoryPaginator(Paginator):
@@ -110,15 +110,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listresourceinventorypaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceInventoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListResourceInventory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listresourceinventorypaginator)
         """
 
 class ListUsageForLicenseConfigurationPaginator(Paginator):
@@ -128,13 +128,13 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsageForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListUsageForLicenseConfiguration.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/paginators/#listusageforlicenseconfigurationpaginator)
         """
```

### Comparing `mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/type_defs.py` & `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
+    ActivationOverrideBehaviorType,
     AllowedOperationType,
     CheckoutTypeType,
     EntitlementDataUnitType,
     EntitlementUnitType,
     GrantStatusType,
     InventoryFilterConditionType,
     LicenseConfigurationStatusType,
@@ -39,135 +40,135 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptGrantRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AcceptGrantResponseTypeDef",
     "AutomatedDiscoveryInformationTypeDef",
     "BorrowConfigurationTypeDef",
     "CheckInLicenseRequestRequestTypeDef",
     "EntitlementDataTypeDef",
     "MetadataTypeDef",
     "ConsumedLicenseSummaryTypeDef",
     "ProvisionalConfigurationTypeDef",
     "CreateGrantRequestRequestTypeDef",
-    "CreateGrantVersionRequestRequestTypeDef",
+    "CreateGrantResponseTypeDef",
+    "OptionsTypeDef",
+    "CreateGrantVersionResponseTypeDef",
     "TagTypeDef",
+    "CreateLicenseConfigurationResponseTypeDef",
     "LicenseConversionContextTypeDef",
+    "CreateLicenseConversionTaskForResourceResponseTypeDef",
     "ReportContextTypeDef",
     "ReportFrequencyTypeDef",
+    "CreateLicenseManagerReportGeneratorResponseTypeDef",
     "DatetimeRangeTypeDef",
     "EntitlementTypeDef",
     "IssuerTypeDef",
+    "CreateLicenseResponseTypeDef",
+    "CreateLicenseVersionResponseTypeDef",
     "CreateTokenRequestRequestTypeDef",
+    "CreateTokenResponseTypeDef",
     "DeleteGrantRequestRequestTypeDef",
+    "DeleteGrantResponseTypeDef",
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     "DeleteLicenseManagerReportGeneratorRequestRequestTypeDef",
     "DeleteLicenseRequestRequestTypeDef",
+    "DeleteLicenseResponseTypeDef",
     "DeleteTokenRequestRequestTypeDef",
     "EntitlementUsageTypeDef",
     "ExtendLicenseConsumptionRequestRequestTypeDef",
+    "ExtendLicenseConsumptionResponseTypeDef",
     "FilterTypeDef",
     "GetAccessTokenRequestRequestTypeDef",
+    "GetAccessTokenResponseTypeDef",
     "GetGrantRequestRequestTypeDef",
-    "GrantTypeDef",
     "GetLicenseConfigurationRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
     "GetLicenseConversionTaskRequestRequestTypeDef",
     "GetLicenseManagerReportGeneratorRequestRequestTypeDef",
     "GetLicenseRequestRequestTypeDef",
     "GetLicenseUsageRequestRequestTypeDef",
     "OrganizationConfigurationTypeDef",
     "IssuerDetailsTypeDef",
     "ReceivedMetadataTypeDef",
     "InventoryFilterTypeDef",
     "LicenseConfigurationAssociationTypeDef",
     "LicenseConfigurationUsageTypeDef",
     "LicenseSpecificationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
     "ListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     "ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
+    "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     "ListLicenseSpecificationsForResourceRequestRequestTypeDef",
     "ListLicenseVersionsRequestRequestTypeDef",
     "ResourceInventoryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TokenDataTypeDef",
+    "PaginatorConfigTypeDef",
     "ProductInformationFilterTypeDef",
     "RejectGrantRequestRequestTypeDef",
+    "RejectGrantResponseTypeDef",
     "S3LocationTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AcceptGrantResponseTypeDef",
-    "CreateGrantResponseTypeDef",
-    "CreateGrantVersionResponseTypeDef",
-    "CreateLicenseConfigurationResponseTypeDef",
-    "CreateLicenseConversionTaskForResourceResponseTypeDef",
-    "CreateLicenseManagerReportGeneratorResponseTypeDef",
-    "CreateLicenseResponseTypeDef",
-    "CreateLicenseVersionResponseTypeDef",
-    "CreateTokenResponseTypeDef",
-    "DeleteGrantResponseTypeDef",
-    "DeleteLicenseResponseTypeDef",
-    "ExtendLicenseConsumptionResponseTypeDef",
-    "GetAccessTokenResponseTypeDef",
-    "RejectGrantResponseTypeDef",
     "CheckoutLicenseRequestRequestTypeDef",
     "CheckoutLicenseResponseTypeDef",
     "CheckoutBorrowLicenseRequestRequestTypeDef",
     "CheckoutBorrowLicenseResponseTypeDef",
     "LicenseOperationFailureTypeDef",
     "ConsumptionConfigurationTypeDef",
+    "CreateGrantVersionRequestRequestTypeDef",
+    "GrantTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateLicenseConversionTaskForResourceRequestRequestTypeDef",
     "GetLicenseConversionTaskResponseTypeDef",
     "LicenseConversionTaskTypeDef",
     "CreateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "UpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "LicenseUsageTypeDef",
     "ListDistributedGrantsRequestRequestTypeDef",
+    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
     "ListLicenseConfigurationsRequestRequestTypeDef",
     "ListLicenseConversionTasksRequestRequestTypeDef",
     "ListLicenseManagerReportGeneratorsRequestRequestTypeDef",
     "ListLicensesRequestRequestTypeDef",
     "ListReceivedGrantsForOrganizationRequestRequestTypeDef",
     "ListReceivedGrantsRequestRequestTypeDef",
     "ListReceivedLicensesForOrganizationRequestRequestTypeDef",
     "ListReceivedLicensesRequestRequestTypeDef",
     "ListTokensRequestRequestTypeDef",
+    "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListUsageForLicenseConfigurationRequestRequestTypeDef",
-    "GetGrantResponseTypeDef",
-    "ListDistributedGrantsResponseTypeDef",
-    "ListReceivedGrantsForOrganizationResponseTypeDef",
-    "ListReceivedGrantsResponseTypeDef",
     "GetServiceSettingsResponseTypeDef",
     "UpdateServiceSettingsRequestRequestTypeDef",
+    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     "ListResourceInventoryRequestRequestTypeDef",
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     "ListUsageForLicenseConfigurationResponseTypeDef",
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     "UpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
-    "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
-    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
-    "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
-    "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListResourceInventoryResponseTypeDef",
     "ListTokensResponseTypeDef",
     "ProductInformationTypeDef",
     "ReportGeneratorTypeDef",
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     "CreateLicenseRequestRequestTypeDef",
     "CreateLicenseVersionRequestRequestTypeDef",
     "GrantedLicenseTypeDef",
     "LicenseTypeDef",
+    "GetGrantResponseTypeDef",
+    "ListDistributedGrantsResponseTypeDef",
+    "ListReceivedGrantsForOrganizationResponseTypeDef",
+    "ListReceivedGrantsResponseTypeDef",
     "ListLicenseConversionTasksResponseTypeDef",
     "GetLicenseUsageResponseTypeDef",
     "CreateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseConfigurationResponseTypeDef",
     "LicenseConfigurationTypeDef",
     "UpdateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseManagerReportGeneratorResponseTypeDef",
@@ -183,22 +184,21 @@
 AcceptGrantRequestRequestTypeDef = TypedDict(
     "AcceptGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AcceptGrantResponseTypeDef = TypedDict(
+    "AcceptGrantResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutomatedDiscoveryInformationTypeDef = TypedDict(
     "AutomatedDiscoveryInformationTypeDef",
     {
         "LastRunTime": datetime,
@@ -224,21 +224,19 @@
     "_OptionalCheckInLicenseRequestRequestTypeDef",
     {
         "Beneficiary": str,
     },
     total=False,
 )
 
-
 class CheckInLicenseRequestRequestTypeDef(
     _RequiredCheckInLicenseRequestRequestTypeDef, _OptionalCheckInLicenseRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredEntitlementDataTypeDef = TypedDict(
     "_RequiredEntitlementDataTypeDef",
     {
         "Name": str,
         "Unit": EntitlementDataUnitType,
     },
 )
@@ -246,19 +244,17 @@
     "_OptionalEntitlementDataTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class EntitlementDataTypeDef(_RequiredEntitlementDataTypeDef, _OptionalEntitlementDataTypeDef):
     pass
 
-
 MetadataTypeDef = TypedDict(
     "MetadataTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -288,58 +284,75 @@
         "LicenseArn": str,
         "Principals": Sequence[str],
         "HomeRegion": str,
         "AllowedOperations": Sequence[AllowedOperationType],
     },
 )
 
-_RequiredCreateGrantVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateGrantVersionRequestRequestTypeDef",
+CreateGrantResponseTypeDef = TypedDict(
+    "CreateGrantResponseTypeDef",
     {
-        "ClientToken": str,
         "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateGrantVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateGrantVersionRequestRequestTypeDef",
+
+OptionsTypeDef = TypedDict(
+    "OptionsTypeDef",
     {
-        "GrantName": str,
-        "AllowedOperations": Sequence[AllowedOperationType],
-        "Status": GrantStatusType,
-        "StatusReason": str,
-        "SourceVersion": str,
+        "ActivationOverrideBehavior": ActivationOverrideBehaviorType,
     },
     total=False,
 )
 
-
-class CreateGrantVersionRequestRequestTypeDef(
-    _RequiredCreateGrantVersionRequestRequestTypeDef,
-    _OptionalCreateGrantVersionRequestRequestTypeDef,
-):
-    pass
-
+CreateGrantVersionResponseTypeDef = TypedDict(
+    "CreateGrantVersionResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+CreateLicenseConfigurationResponseTypeDef = TypedDict(
+    "CreateLicenseConfigurationResponseTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LicenseConversionContextTypeDef = TypedDict(
     "LicenseConversionContextTypeDef",
     {
         "UsageOperation": str,
     },
     total=False,
 )
 
+CreateLicenseConversionTaskForResourceResponseTypeDef = TypedDict(
+    "CreateLicenseConversionTaskForResourceResponseTypeDef",
+    {
+        "LicenseConversionTaskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReportContextTypeDef = TypedDict(
     "ReportContextTypeDef",
     {
         "licenseConfigurationArns": Sequence[str],
     },
 )
 
@@ -348,33 +361,39 @@
     {
         "value": int,
         "period": ReportFrequencyTypeType,
     },
     total=False,
 )
 
+CreateLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
+    "CreateLicenseManagerReportGeneratorResponseTypeDef",
+    {
+        "LicenseManagerReportGeneratorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDatetimeRangeTypeDef = TypedDict(
     "_RequiredDatetimeRangeTypeDef",
     {
         "Begin": str,
     },
 )
 _OptionalDatetimeRangeTypeDef = TypedDict(
     "_OptionalDatetimeRangeTypeDef",
     {
         "End": str,
     },
     total=False,
 )
 
-
 class DatetimeRangeTypeDef(_RequiredDatetimeRangeTypeDef, _OptionalDatetimeRangeTypeDef):
     pass
 
-
 _RequiredEntitlementTypeDef = TypedDict(
     "_RequiredEntitlementTypeDef",
     {
         "Name": str,
         "Unit": EntitlementUnitType,
     },
 )
@@ -385,37 +404,53 @@
         "MaxCount": int,
         "Overage": bool,
         "AllowCheckIn": bool,
     },
     total=False,
 )
 
-
 class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
     pass
 
-
 _RequiredIssuerTypeDef = TypedDict(
     "_RequiredIssuerTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalIssuerTypeDef = TypedDict(
     "_OptionalIssuerTypeDef",
     {
         "SignKey": str,
     },
     total=False,
 )
 
-
 class IssuerTypeDef(_RequiredIssuerTypeDef, _OptionalIssuerTypeDef):
     pass
 
+CreateLicenseResponseTypeDef = TypedDict(
+    "CreateLicenseResponseTypeDef",
+    {
+        "LicenseArn": str,
+        "Status": LicenseStatusType,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLicenseVersionResponseTypeDef = TypedDict(
+    "CreateLicenseVersionResponseTypeDef",
+    {
+        "LicenseArn": str,
+        "Version": str,
+        "Status": LicenseStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "ClientToken": str,
     },
@@ -426,20 +461,28 @@
         "RoleArns": Sequence[str],
         "ExpirationInDays": int,
         "TokenProperties": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
+CreateTokenResponseTypeDef = TypedDict(
+    "CreateTokenResponseTypeDef",
+    {
+        "TokenId": str,
+        "TokenType": Literal["REFRESH_TOKEN"],
+        "Token": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredDeleteGrantRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
         "Version": str,
     },
@@ -448,20 +491,28 @@
     "_OptionalDeleteGrantRequestRequestTypeDef",
     {
         "StatusReason": str,
     },
     total=False,
 )
 
-
 class DeleteGrantRequestRequestTypeDef(
     _RequiredDeleteGrantRequestRequestTypeDef, _OptionalDeleteGrantRequestRequestTypeDef
 ):
     pass
 
+DeleteGrantResponseTypeDef = TypedDict(
+    "DeleteGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DeleteLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
@@ -477,14 +528,23 @@
     "DeleteLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "SourceVersion": str,
     },
 )
 
+DeleteLicenseResponseTypeDef = TypedDict(
+    "DeleteLicenseResponseTypeDef",
+    {
+        "Status": LicenseDeletionStatusType,
+        "DeletionDate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTokenRequestRequestTypeDef = TypedDict(
     "DeleteTokenRequestRequestTypeDef",
     {
         "TokenId": str,
     },
 )
 
@@ -500,40 +560,45 @@
     "_OptionalEntitlementUsageTypeDef",
     {
         "MaxCount": str,
     },
     total=False,
 )
 
-
 class EntitlementUsageTypeDef(_RequiredEntitlementUsageTypeDef, _OptionalEntitlementUsageTypeDef):
     pass
 
-
 _RequiredExtendLicenseConsumptionRequestRequestTypeDef = TypedDict(
     "_RequiredExtendLicenseConsumptionRequestRequestTypeDef",
     {
         "LicenseConsumptionToken": str,
     },
 )
 _OptionalExtendLicenseConsumptionRequestRequestTypeDef = TypedDict(
     "_OptionalExtendLicenseConsumptionRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class ExtendLicenseConsumptionRequestRequestTypeDef(
     _RequiredExtendLicenseConsumptionRequestRequestTypeDef,
     _OptionalExtendLicenseConsumptionRequestRequestTypeDef,
 ):
     pass
 
+ExtendLicenseConsumptionResponseTypeDef = TypedDict(
+    "ExtendLicenseConsumptionResponseTypeDef",
+    {
+        "LicenseConsumptionToken": str,
+        "Expiration": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
@@ -550,20 +615,26 @@
     "_OptionalGetAccessTokenRequestRequestTypeDef",
     {
         "TokenProperties": Sequence[str],
     },
     total=False,
 )
 
-
 class GetAccessTokenRequestRequestTypeDef(
     _RequiredGetAccessTokenRequestRequestTypeDef, _OptionalGetAccessTokenRequestRequestTypeDef
 ):
     pass
 
+GetAccessTokenResponseTypeDef = TypedDict(
+    "GetAccessTokenResponseTypeDef",
+    {
+        "AccessToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredGetGrantRequestRequestTypeDef = TypedDict(
     "_RequiredGetGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
@@ -571,48 +642,19 @@
     "_OptionalGetGrantRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetGrantRequestRequestTypeDef(
     _RequiredGetGrantRequestRequestTypeDef, _OptionalGetGrantRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredGrantTypeDef = TypedDict(
-    "_RequiredGrantTypeDef",
-    {
-        "GrantArn": str,
-        "GrantName": str,
-        "ParentArn": str,
-        "LicenseArn": str,
-        "GranteePrincipalArn": str,
-        "HomeRegion": str,
-        "GrantStatus": GrantStatusType,
-        "Version": str,
-        "GrantedOperations": List[AllowedOperationType],
-    },
-)
-_OptionalGrantTypeDef = TypedDict(
-    "_OptionalGrantTypeDef",
-    {
-        "StatusReason": str,
-    },
-    total=False,
-)
-
-
-class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
-    pass
-
-
 GetLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "GetLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 
@@ -649,21 +691,19 @@
     "_OptionalGetLicenseRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetLicenseRequestRequestTypeDef(
     _RequiredGetLicenseRequestRequestTypeDef, _OptionalGetLicenseRequestRequestTypeDef
 ):
     pass
 
-
 GetLicenseUsageRequestRequestTypeDef = TypedDict(
     "GetLicenseUsageRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 
@@ -705,19 +745,17 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
-
 LicenseConfigurationAssociationTypeDef = TypedDict(
     "LicenseConfigurationAssociationTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": ResourceTypeType,
         "ResourceOwnerId": str,
         "AssociationTime": datetime,
@@ -749,31 +787,39 @@
     "_OptionalLicenseSpecificationTypeDef",
     {
         "AmiAssociationScope": str,
     },
     total=False,
 )
 
-
 class LicenseSpecificationTypeDef(
     _RequiredLicenseSpecificationTypeDef, _OptionalLicenseSpecificationTypeDef
 ):
     pass
 
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
+    _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+):
+    pass
+
 _RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListAssociationsForLicenseConfigurationRequestRequestTypeDef = TypedDict(
@@ -781,22 +827,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAssociationsForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListAssociationsForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef = TypedDict(
@@ -804,21 +848,39 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef(
     _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
     _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
+    _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+    _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+):
+    pass
 
 _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
@@ -827,22 +889,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalListLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListLicenseVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseVersionsRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 _OptionalListLicenseVersionsRequestRequestTypeDef = TypedDict(
@@ -850,22 +910,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListLicenseVersionsRequestRequestTypeDef(
     _RequiredListLicenseVersionsRequestRequestTypeDef,
     _OptionalListLicenseVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ResourceInventoryTypeDef = TypedDict(
     "ResourceInventoryTypeDef",
     {
         "ResourceId": str,
         "ResourceType": ResourceTypeType,
         "ResourceArn": str,
         "Platform": str,
@@ -892,14 +950,24 @@
         "TokenProperties": List[str],
         "RoleArns": List[str],
         "Status": str,
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
 _RequiredProductInformationFilterTypeDef = TypedDict(
     "_RequiredProductInformationFilterTypeDef",
     {
         "ProductInformationFilterName": str,
         "ProductInformationFilterComparator": str,
     },
 )
@@ -907,172 +975,61 @@
     "_OptionalProductInformationFilterTypeDef",
     {
         "ProductInformationFilterValue": Sequence[str],
     },
     total=False,
 )
 
-
 class ProductInformationFilterTypeDef(
     _RequiredProductInformationFilterTypeDef, _OptionalProductInformationFilterTypeDef
 ):
     pass
 
-
 RejectGrantRequestRequestTypeDef = TypedDict(
     "RejectGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
-    {
-        "bucket": str,
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
-    },
-)
-
-AcceptGrantResponseTypeDef = TypedDict(
-    "AcceptGrantResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGrantResponseTypeDef = TypedDict(
-    "CreateGrantResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGrantVersionResponseTypeDef = TypedDict(
-    "CreateGrantVersionResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLicenseConfigurationResponseTypeDef = TypedDict(
-    "CreateLicenseConfigurationResponseTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLicenseConversionTaskForResourceResponseTypeDef = TypedDict(
-    "CreateLicenseConversionTaskForResourceResponseTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
-    "CreateLicenseManagerReportGeneratorResponseTypeDef",
-    {
-        "LicenseManagerReportGeneratorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLicenseResponseTypeDef = TypedDict(
-    "CreateLicenseResponseTypeDef",
-    {
-        "LicenseArn": str,
-        "Status": LicenseStatusType,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLicenseVersionResponseTypeDef = TypedDict(
-    "CreateLicenseVersionResponseTypeDef",
-    {
-        "LicenseArn": str,
-        "Version": str,
-        "Status": LicenseStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTokenResponseTypeDef = TypedDict(
-    "CreateTokenResponseTypeDef",
-    {
-        "TokenId": str,
-        "TokenType": Literal["REFRESH_TOKEN"],
-        "Token": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteGrantResponseTypeDef = TypedDict(
-    "DeleteGrantResponseTypeDef",
+RejectGrantResponseTypeDef = TypedDict(
+    "RejectGrantResponseTypeDef",
     {
         "GrantArn": str,
         "Status": GrantStatusType,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteLicenseResponseTypeDef = TypedDict(
-    "DeleteLicenseResponseTypeDef",
-    {
-        "Status": LicenseDeletionStatusType,
-        "DeletionDate": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExtendLicenseConsumptionResponseTypeDef = TypedDict(
-    "ExtendLicenseConsumptionResponseTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
-        "LicenseConsumptionToken": str,
-        "Expiration": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "bucket": str,
+        "keyPrefix": str,
     },
+    total=False,
 )
 
-GetAccessTokenResponseTypeDef = TypedDict(
-    "GetAccessTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AccessToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-RejectGrantResponseTypeDef = TypedDict(
-    "RejectGrantResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
 _RequiredCheckoutLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutLicenseRequestRequestTypeDef",
     {
         "ProductSKU": str,
@@ -1087,33 +1044,31 @@
     {
         "Beneficiary": str,
         "NodeId": str,
     },
     total=False,
 )
 
-
 class CheckoutLicenseRequestRequestTypeDef(
     _RequiredCheckoutLicenseRequestRequestTypeDef, _OptionalCheckoutLicenseRequestRequestTypeDef
 ):
     pass
 
-
 CheckoutLicenseResponseTypeDef = TypedDict(
     "CheckoutLicenseResponseTypeDef",
     {
         "CheckoutType": CheckoutTypeType,
         "LicenseConsumptionToken": str,
         "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "SignedToken": str,
         "NodeId": str,
         "IssuedAt": str,
         "Expiration": str,
         "LicenseArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCheckoutBorrowLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutBorrowLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
@@ -1127,34 +1082,32 @@
     {
         "NodeId": str,
         "CheckoutMetadata": Sequence[MetadataTypeDef],
     },
     total=False,
 )
 
-
 class CheckoutBorrowLicenseRequestRequestTypeDef(
     _RequiredCheckoutBorrowLicenseRequestRequestTypeDef,
     _OptionalCheckoutBorrowLicenseRequestRequestTypeDef,
 ):
     pass
 
-
 CheckoutBorrowLicenseResponseTypeDef = TypedDict(
     "CheckoutBorrowLicenseResponseTypeDef",
     {
         "LicenseArn": str,
         "LicenseConsumptionToken": str,
         "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "NodeId": str,
         "SignedToken": str,
         "IssuedAt": str,
         "Expiration": str,
         "CheckoutMetadata": List[MetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LicenseOperationFailureTypeDef = TypedDict(
     "LicenseOperationFailureTypeDef",
     {
         "ResourceArn": str,
@@ -1175,19 +1128,71 @@
         "RenewType": RenewTypeType,
         "ProvisionalConfiguration": ProvisionalConfigurationTypeDef,
         "BorrowConfiguration": BorrowConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateGrantVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateGrantVersionRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "GrantArn": str,
+    },
+)
+_OptionalCreateGrantVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateGrantVersionRequestRequestTypeDef",
+    {
+        "GrantName": str,
+        "AllowedOperations": Sequence[AllowedOperationType],
+        "Status": GrantStatusType,
+        "StatusReason": str,
+        "SourceVersion": str,
+        "Options": OptionsTypeDef,
+    },
+    total=False,
+)
+
+class CreateGrantVersionRequestRequestTypeDef(
+    _RequiredCreateGrantVersionRequestRequestTypeDef,
+    _OptionalCreateGrantVersionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredGrantTypeDef = TypedDict(
+    "_RequiredGrantTypeDef",
+    {
+        "GrantArn": str,
+        "GrantName": str,
+        "ParentArn": str,
+        "LicenseArn": str,
+        "GranteePrincipalArn": str,
+        "HomeRegion": str,
+        "GrantStatus": GrantStatusType,
+        "Version": str,
+        "GrantedOperations": List[AllowedOperationType],
+    },
+)
+_OptionalGrantTypeDef = TypedDict(
+    "_OptionalGrantTypeDef",
+    {
+        "StatusReason": str,
+        "Options": OptionsTypeDef,
+    },
+    total=False,
+)
+
+class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
+    pass
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1212,15 +1217,15 @@
         "SourceLicenseContext": LicenseConversionContextTypeDef,
         "DestinationLicenseContext": LicenseConversionContextTypeDef,
         "StatusMessage": str,
         "Status": LicenseConversionTaskStatusType,
         "StartTime": datetime,
         "LicenseConversionTime": datetime,
         "EndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LicenseConversionTaskTypeDef = TypedDict(
     "LicenseConversionTaskTypeDef",
     {
         "LicenseConversionTaskId": str,
@@ -1251,22 +1256,20 @@
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateLicenseManagerReportGeneratorRequestRequestTypeDef(
     _RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     _OptionalCreateLicenseManagerReportGeneratorRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "LicenseManagerReportGeneratorArn": str,
         "ReportGeneratorName": str,
         "Type": Sequence[ReportTypeType],
         "ReportContext": ReportContextTypeDef,
@@ -1278,22 +1281,20 @@
     "_OptionalUpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateLicenseManagerReportGeneratorRequestRequestTypeDef(
     _RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     _OptionalUpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
 ):
     pass
 
-
 LicenseUsageTypeDef = TypedDict(
     "LicenseUsageTypeDef",
     {
         "EntitlementUsages": List[EntitlementUsageTypeDef],
     },
     total=False,
 )
@@ -1305,14 +1306,24 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
+    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
+    {
+        "LicenseConfigurationArns": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLicenseConfigurationsRequestRequestTypeDef = TypedDict(
     "ListLicenseConfigurationsRequestRequestTypeDef",
     {
         "LicenseConfigurationArns": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1363,22 +1374,20 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListReceivedGrantsForOrganizationRequestRequestTypeDef(
     _RequiredListReceivedGrantsForOrganizationRequestRequestTypeDef,
     _OptionalListReceivedGrantsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
-
 ListReceivedGrantsRequestRequestTypeDef = TypedDict(
     "ListReceivedGrantsRequestRequestTypeDef",
     {
         "GrantArns": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
@@ -1414,96 +1423,89 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredListUsageForLicenseConfigurationRequestRequestTypeDef",
+_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
-_OptionalListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalListUsageForLicenseConfigurationRequestRequestTypeDef",
+_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
-class ListUsageForLicenseConfigurationRequestRequestTypeDef(
-    _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef,
-    _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef,
+class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
+    _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
+    _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
 ):
     pass
 
-
-GetGrantResponseTypeDef = TypedDict(
-    "GetGrantResponseTypeDef",
-    {
-        "Grant": GrantTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDistributedGrantsResponseTypeDef = TypedDict(
-    "ListDistributedGrantsResponseTypeDef",
+_RequiredListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredListUsageForLicenseConfigurationRequestRequestTypeDef",
     {
-        "Grants": List[GrantTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LicenseConfigurationArn": str,
     },
 )
-
-ListReceivedGrantsForOrganizationResponseTypeDef = TypedDict(
-    "ListReceivedGrantsForOrganizationResponseTypeDef",
+_OptionalListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalListUsageForLicenseConfigurationRequestRequestTypeDef",
     {
-        "Grants": List[GrantTypeDef],
+        "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Filters": Sequence[FilterTypeDef],
     },
+    total=False,
 )
 
-ListReceivedGrantsResponseTypeDef = TypedDict(
-    "ListReceivedGrantsResponseTypeDef",
-    {
-        "Grants": List[GrantTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class ListUsageForLicenseConfigurationRequestRequestTypeDef(
+    _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef,
+    _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
 
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
         "OrganizationConfiguration": OrganizationConfigurationTypeDef,
         "EnableCrossAccountsDiscovery": bool,
         "LicenseManagerResourceShareArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceSettingsRequestRequestTypeDef = TypedDict(
     "UpdateServiceSettingsRequestRequestTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
         "OrganizationConfiguration": OrganizationConfigurationTypeDef,
         "EnableCrossAccountsDiscovery": bool,
     },
     total=False,
 )
 
+ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
+    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+    {
+        "Filters": Sequence[InventoryFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListResourceInventoryRequestRequestTypeDef = TypedDict(
     "ListResourceInventoryRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[InventoryFilterTypeDef],
     },
@@ -1511,33 +1513,33 @@
 )
 
 ListAssociationsForLicenseConfigurationResponseTypeDef = TypedDict(
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationAssociations": List[LicenseConfigurationAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUsageForLicenseConfigurationResponseTypeDef = TypedDict(
     "ListUsageForLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationUsageList": List[LicenseConfigurationUsageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLicenseSpecificationsForResourceResponseTypeDef = TypedDict(
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     {
         "LicenseSpecifications": List[LicenseSpecificationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1548,123 +1550,35 @@
     {
         "AddLicenseSpecifications": Sequence[LicenseSpecificationTypeDef],
         "RemoveLicenseSpecifications": Sequence[LicenseSpecificationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
-    _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-    _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-):
-    pass
-
-
-ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
-    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
-    {
-        "LicenseConfigurationArns": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
-    _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-    _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-):
-    pass
-
-
-ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
-    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
-    {
-        "Filters": Sequence[InventoryFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
-    _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
-    _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
-):
-    pass
-
-
 ListResourceInventoryResponseTypeDef = TypedDict(
     "ListResourceInventoryResponseTypeDef",
     {
         "ResourceInventoryList": List[ResourceInventoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTokensResponseTypeDef = TypedDict(
     "ListTokensResponseTypeDef",
     {
         "Tokens": List[TokenDataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProductInformationTypeDef = TypedDict(
     "ProductInformationTypeDef",
     {
         "ResourceType": str,
@@ -1693,15 +1607,15 @@
 )
 
 ListFailuresForLicenseConfigurationOperationsResponseTypeDef = TypedDict(
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     {
         "LicenseOperationFailureList": List[LicenseOperationFailureTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseRequestRequestTypeDef",
     {
         "LicenseName": str,
@@ -1720,21 +1634,19 @@
     "_OptionalCreateLicenseRequestRequestTypeDef",
     {
         "LicenseMetadata": Sequence[MetadataTypeDef],
     },
     total=False,
 )
 
-
 class CreateLicenseRequestRequestTypeDef(
     _RequiredCreateLicenseRequestRequestTypeDef, _OptionalCreateLicenseRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateLicenseVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseVersionRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "LicenseName": str,
         "ProductName": str,
         "Issuer": IssuerTypeDef,
@@ -1751,22 +1663,20 @@
     {
         "LicenseMetadata": Sequence[MetadataTypeDef],
         "SourceVersion": str,
     },
     total=False,
 )
 
-
 class CreateLicenseVersionRequestRequestTypeDef(
     _RequiredCreateLicenseVersionRequestRequestTypeDef,
     _OptionalCreateLicenseVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GrantedLicenseTypeDef = TypedDict(
     "GrantedLicenseTypeDef",
     {
         "LicenseArn": str,
         "LicenseName": str,
         "ProductName": str,
         "ProductSKU": str,
@@ -1802,28 +1712,63 @@
         "LicenseMetadata": List[MetadataTypeDef],
         "CreateTime": str,
         "Version": str,
     },
     total=False,
 )
 
+GetGrantResponseTypeDef = TypedDict(
+    "GetGrantResponseTypeDef",
+    {
+        "Grant": GrantTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDistributedGrantsResponseTypeDef = TypedDict(
+    "ListDistributedGrantsResponseTypeDef",
+    {
+        "Grants": List[GrantTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListReceivedGrantsForOrganizationResponseTypeDef = TypedDict(
+    "ListReceivedGrantsForOrganizationResponseTypeDef",
+    {
+        "Grants": List[GrantTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListReceivedGrantsResponseTypeDef = TypedDict(
+    "ListReceivedGrantsResponseTypeDef",
+    {
+        "Grants": List[GrantTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListLicenseConversionTasksResponseTypeDef = TypedDict(
     "ListLicenseConversionTasksResponseTypeDef",
     {
         "LicenseConversionTasks": List[LicenseConversionTaskTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLicenseUsageResponseTypeDef = TypedDict(
     "GetLicenseUsageResponseTypeDef",
     {
         "LicenseUsage": LicenseUsageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
     {
         "Name": str,
@@ -1840,22 +1785,20 @@
         "Tags": Sequence[TagTypeDef],
         "DisassociateWhenNotFound": bool,
         "ProductInformationList": Sequence[ProductInformationTypeDef],
     },
     total=False,
 )
 
-
 class CreateLicenseConfigurationRequestRequestTypeDef(
     _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
     _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetLicenseConfigurationResponseTypeDef = TypedDict(
     "GetLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationId": str,
         "LicenseConfigurationArn": str,
         "Name": str,
         "Description": str,
@@ -1868,15 +1811,15 @@
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
         "Tags": List[TagTypeDef],
         "ProductInformationList": List[ProductInformationTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
         "DisassociateWhenNotFound": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LicenseConfigurationTypeDef = TypedDict(
     "LicenseConfigurationTypeDef",
     {
         "LicenseConfigurationId": str,
@@ -1916,84 +1859,82 @@
         "Description": str,
         "ProductInformationList": Sequence[ProductInformationTypeDef],
         "DisassociateWhenNotFound": bool,
     },
     total=False,
 )
 
-
 class UpdateLicenseConfigurationRequestRequestTypeDef(
     _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
     _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     {
         "ReportGenerator": ReportGeneratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLicenseManagerReportGeneratorsResponseTypeDef = TypedDict(
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     {
         "ReportGenerators": List[ReportGeneratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReceivedLicensesForOrganizationResponseTypeDef = TypedDict(
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     {
         "Licenses": List[GrantedLicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReceivedLicensesResponseTypeDef = TypedDict(
     "ListReceivedLicensesResponseTypeDef",
     {
         "Licenses": List[GrantedLicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLicenseResponseTypeDef = TypedDict(
     "GetLicenseResponseTypeDef",
     {
         "License": LicenseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLicenseVersionsResponseTypeDef = TypedDict(
     "ListLicenseVersionsResponseTypeDef",
     {
         "Licenses": List[LicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLicensesResponseTypeDef = TypedDict(
     "ListLicensesResponseTypeDef",
     {
         "Licenses": List[LicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLicenseConfigurationsResponseTypeDef = TypedDict(
     "ListLicenseConfigurationsResponseTypeDef",
     {
         "LicenseConfigurations": List[LicenseConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager/type_defs.pyi` & `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
+    ActivationOverrideBehaviorType,
     AllowedOperationType,
     CheckoutTypeType,
     EntitlementDataUnitType,
     EntitlementUnitType,
     GrantStatusType,
     InventoryFilterConditionType,
     LicenseConfigurationStatusType,
@@ -39,134 +40,136 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptGrantRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AcceptGrantResponseTypeDef",
     "AutomatedDiscoveryInformationTypeDef",
     "BorrowConfigurationTypeDef",
     "CheckInLicenseRequestRequestTypeDef",
     "EntitlementDataTypeDef",
     "MetadataTypeDef",
     "ConsumedLicenseSummaryTypeDef",
     "ProvisionalConfigurationTypeDef",
     "CreateGrantRequestRequestTypeDef",
-    "CreateGrantVersionRequestRequestTypeDef",
+    "CreateGrantResponseTypeDef",
+    "OptionsTypeDef",
+    "CreateGrantVersionResponseTypeDef",
     "TagTypeDef",
+    "CreateLicenseConfigurationResponseTypeDef",
     "LicenseConversionContextTypeDef",
+    "CreateLicenseConversionTaskForResourceResponseTypeDef",
     "ReportContextTypeDef",
     "ReportFrequencyTypeDef",
+    "CreateLicenseManagerReportGeneratorResponseTypeDef",
     "DatetimeRangeTypeDef",
     "EntitlementTypeDef",
     "IssuerTypeDef",
+    "CreateLicenseResponseTypeDef",
+    "CreateLicenseVersionResponseTypeDef",
     "CreateTokenRequestRequestTypeDef",
+    "CreateTokenResponseTypeDef",
     "DeleteGrantRequestRequestTypeDef",
+    "DeleteGrantResponseTypeDef",
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     "DeleteLicenseManagerReportGeneratorRequestRequestTypeDef",
     "DeleteLicenseRequestRequestTypeDef",
+    "DeleteLicenseResponseTypeDef",
     "DeleteTokenRequestRequestTypeDef",
     "EntitlementUsageTypeDef",
     "ExtendLicenseConsumptionRequestRequestTypeDef",
+    "ExtendLicenseConsumptionResponseTypeDef",
     "FilterTypeDef",
     "GetAccessTokenRequestRequestTypeDef",
+    "GetAccessTokenResponseTypeDef",
     "GetGrantRequestRequestTypeDef",
-    "GrantTypeDef",
     "GetLicenseConfigurationRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
     "GetLicenseConversionTaskRequestRequestTypeDef",
     "GetLicenseManagerReportGeneratorRequestRequestTypeDef",
     "GetLicenseRequestRequestTypeDef",
     "GetLicenseUsageRequestRequestTypeDef",
     "OrganizationConfigurationTypeDef",
     "IssuerDetailsTypeDef",
     "ReceivedMetadataTypeDef",
     "InventoryFilterTypeDef",
     "LicenseConfigurationAssociationTypeDef",
     "LicenseConfigurationUsageTypeDef",
     "LicenseSpecificationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
     "ListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     "ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
+    "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     "ListLicenseSpecificationsForResourceRequestRequestTypeDef",
     "ListLicenseVersionsRequestRequestTypeDef",
     "ResourceInventoryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TokenDataTypeDef",
+    "PaginatorConfigTypeDef",
     "ProductInformationFilterTypeDef",
     "RejectGrantRequestRequestTypeDef",
+    "RejectGrantResponseTypeDef",
     "S3LocationTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AcceptGrantResponseTypeDef",
-    "CreateGrantResponseTypeDef",
-    "CreateGrantVersionResponseTypeDef",
-    "CreateLicenseConfigurationResponseTypeDef",
-    "CreateLicenseConversionTaskForResourceResponseTypeDef",
-    "CreateLicenseManagerReportGeneratorResponseTypeDef",
-    "CreateLicenseResponseTypeDef",
-    "CreateLicenseVersionResponseTypeDef",
-    "CreateTokenResponseTypeDef",
-    "DeleteGrantResponseTypeDef",
-    "DeleteLicenseResponseTypeDef",
-    "ExtendLicenseConsumptionResponseTypeDef",
-    "GetAccessTokenResponseTypeDef",
-    "RejectGrantResponseTypeDef",
     "CheckoutLicenseRequestRequestTypeDef",
     "CheckoutLicenseResponseTypeDef",
     "CheckoutBorrowLicenseRequestRequestTypeDef",
     "CheckoutBorrowLicenseResponseTypeDef",
     "LicenseOperationFailureTypeDef",
     "ConsumptionConfigurationTypeDef",
+    "CreateGrantVersionRequestRequestTypeDef",
+    "GrantTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateLicenseConversionTaskForResourceRequestRequestTypeDef",
     "GetLicenseConversionTaskResponseTypeDef",
     "LicenseConversionTaskTypeDef",
     "CreateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "UpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "LicenseUsageTypeDef",
     "ListDistributedGrantsRequestRequestTypeDef",
+    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
     "ListLicenseConfigurationsRequestRequestTypeDef",
     "ListLicenseConversionTasksRequestRequestTypeDef",
     "ListLicenseManagerReportGeneratorsRequestRequestTypeDef",
     "ListLicensesRequestRequestTypeDef",
     "ListReceivedGrantsForOrganizationRequestRequestTypeDef",
     "ListReceivedGrantsRequestRequestTypeDef",
     "ListReceivedLicensesForOrganizationRequestRequestTypeDef",
     "ListReceivedLicensesRequestRequestTypeDef",
     "ListTokensRequestRequestTypeDef",
+    "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListUsageForLicenseConfigurationRequestRequestTypeDef",
-    "GetGrantResponseTypeDef",
-    "ListDistributedGrantsResponseTypeDef",
-    "ListReceivedGrantsForOrganizationResponseTypeDef",
-    "ListReceivedGrantsResponseTypeDef",
     "GetServiceSettingsResponseTypeDef",
     "UpdateServiceSettingsRequestRequestTypeDef",
+    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     "ListResourceInventoryRequestRequestTypeDef",
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     "ListUsageForLicenseConfigurationResponseTypeDef",
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     "UpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
-    "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
-    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
-    "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
-    "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListResourceInventoryResponseTypeDef",
     "ListTokensResponseTypeDef",
     "ProductInformationTypeDef",
     "ReportGeneratorTypeDef",
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     "CreateLicenseRequestRequestTypeDef",
     "CreateLicenseVersionRequestRequestTypeDef",
     "GrantedLicenseTypeDef",
     "LicenseTypeDef",
+    "GetGrantResponseTypeDef",
+    "ListDistributedGrantsResponseTypeDef",
+    "ListReceivedGrantsForOrganizationResponseTypeDef",
+    "ListReceivedGrantsResponseTypeDef",
     "ListLicenseConversionTasksResponseTypeDef",
     "GetLicenseUsageResponseTypeDef",
     "CreateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseConfigurationResponseTypeDef",
     "LicenseConfigurationTypeDef",
     "UpdateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseManagerReportGeneratorResponseTypeDef",
@@ -182,22 +185,21 @@
 AcceptGrantRequestRequestTypeDef = TypedDict(
     "AcceptGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AcceptGrantResponseTypeDef = TypedDict(
+    "AcceptGrantResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutomatedDiscoveryInformationTypeDef = TypedDict(
     "AutomatedDiscoveryInformationTypeDef",
     {
         "LastRunTime": datetime,
@@ -223,19 +225,21 @@
     "_OptionalCheckInLicenseRequestRequestTypeDef",
     {
         "Beneficiary": str,
     },
     total=False,
 )
 
+
 class CheckInLicenseRequestRequestTypeDef(
     _RequiredCheckInLicenseRequestRequestTypeDef, _OptionalCheckInLicenseRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredEntitlementDataTypeDef = TypedDict(
     "_RequiredEntitlementDataTypeDef",
     {
         "Name": str,
         "Unit": EntitlementDataUnitType,
     },
 )
@@ -243,17 +247,19 @@
     "_OptionalEntitlementDataTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class EntitlementDataTypeDef(_RequiredEntitlementDataTypeDef, _OptionalEntitlementDataTypeDef):
     pass
 
+
 MetadataTypeDef = TypedDict(
     "MetadataTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -283,56 +289,75 @@
         "LicenseArn": str,
         "Principals": Sequence[str],
         "HomeRegion": str,
         "AllowedOperations": Sequence[AllowedOperationType],
     },
 )
 
-_RequiredCreateGrantVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateGrantVersionRequestRequestTypeDef",
+CreateGrantResponseTypeDef = TypedDict(
+    "CreateGrantResponseTypeDef",
     {
-        "ClientToken": str,
         "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateGrantVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateGrantVersionRequestRequestTypeDef",
+
+OptionsTypeDef = TypedDict(
+    "OptionsTypeDef",
     {
-        "GrantName": str,
-        "AllowedOperations": Sequence[AllowedOperationType],
-        "Status": GrantStatusType,
-        "StatusReason": str,
-        "SourceVersion": str,
+        "ActivationOverrideBehavior": ActivationOverrideBehaviorType,
     },
     total=False,
 )
 
-class CreateGrantVersionRequestRequestTypeDef(
-    _RequiredCreateGrantVersionRequestRequestTypeDef,
-    _OptionalCreateGrantVersionRequestRequestTypeDef,
-):
-    pass
+CreateGrantVersionResponseTypeDef = TypedDict(
+    "CreateGrantVersionResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+CreateLicenseConfigurationResponseTypeDef = TypedDict(
+    "CreateLicenseConfigurationResponseTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LicenseConversionContextTypeDef = TypedDict(
     "LicenseConversionContextTypeDef",
     {
         "UsageOperation": str,
     },
     total=False,
 )
 
+CreateLicenseConversionTaskForResourceResponseTypeDef = TypedDict(
+    "CreateLicenseConversionTaskForResourceResponseTypeDef",
+    {
+        "LicenseConversionTaskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReportContextTypeDef = TypedDict(
     "ReportContextTypeDef",
     {
         "licenseConfigurationArns": Sequence[str],
     },
 )
 
@@ -341,31 +366,41 @@
     {
         "value": int,
         "period": ReportFrequencyTypeType,
     },
     total=False,
 )
 
+CreateLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
+    "CreateLicenseManagerReportGeneratorResponseTypeDef",
+    {
+        "LicenseManagerReportGeneratorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDatetimeRangeTypeDef = TypedDict(
     "_RequiredDatetimeRangeTypeDef",
     {
         "Begin": str,
     },
 )
 _OptionalDatetimeRangeTypeDef = TypedDict(
     "_OptionalDatetimeRangeTypeDef",
     {
         "End": str,
     },
     total=False,
 )
 
+
 class DatetimeRangeTypeDef(_RequiredDatetimeRangeTypeDef, _OptionalDatetimeRangeTypeDef):
     pass
 
+
 _RequiredEntitlementTypeDef = TypedDict(
     "_RequiredEntitlementTypeDef",
     {
         "Name": str,
         "Unit": EntitlementUnitType,
     },
 )
@@ -376,34 +411,58 @@
         "MaxCount": int,
         "Overage": bool,
         "AllowCheckIn": bool,
     },
     total=False,
 )
 
+
 class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
     pass
 
+
 _RequiredIssuerTypeDef = TypedDict(
     "_RequiredIssuerTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalIssuerTypeDef = TypedDict(
     "_OptionalIssuerTypeDef",
     {
         "SignKey": str,
     },
     total=False,
 )
 
+
 class IssuerTypeDef(_RequiredIssuerTypeDef, _OptionalIssuerTypeDef):
     pass
 
+
+CreateLicenseResponseTypeDef = TypedDict(
+    "CreateLicenseResponseTypeDef",
+    {
+        "LicenseArn": str,
+        "Status": LicenseStatusType,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLicenseVersionResponseTypeDef = TypedDict(
+    "CreateLicenseVersionResponseTypeDef",
+    {
+        "LicenseArn": str,
+        "Version": str,
+        "Status": LicenseStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "ClientToken": str,
     },
 )
@@ -413,19 +472,31 @@
         "RoleArns": Sequence[str],
         "ExpirationInDays": int,
         "TokenProperties": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
+
+CreateTokenResponseTypeDef = TypedDict(
+    "CreateTokenResponseTypeDef",
+    {
+        "TokenId": str,
+        "TokenType": Literal["REFRESH_TOKEN"],
+        "Token": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteGrantRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
         "Version": str,
     },
 )
@@ -433,19 +504,31 @@
     "_OptionalDeleteGrantRequestRequestTypeDef",
     {
         "StatusReason": str,
     },
     total=False,
 )
 
+
 class DeleteGrantRequestRequestTypeDef(
     _RequiredDeleteGrantRequestRequestTypeDef, _OptionalDeleteGrantRequestRequestTypeDef
 ):
     pass
 
+
+DeleteGrantResponseTypeDef = TypedDict(
+    "DeleteGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 
@@ -460,14 +543,23 @@
     "DeleteLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "SourceVersion": str,
     },
 )
 
+DeleteLicenseResponseTypeDef = TypedDict(
+    "DeleteLicenseResponseTypeDef",
+    {
+        "Status": LicenseDeletionStatusType,
+        "DeletionDate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTokenRequestRequestTypeDef = TypedDict(
     "DeleteTokenRequestRequestTypeDef",
     {
         "TokenId": str,
     },
 )
 
@@ -483,37 +575,50 @@
     "_OptionalEntitlementUsageTypeDef",
     {
         "MaxCount": str,
     },
     total=False,
 )
 
+
 class EntitlementUsageTypeDef(_RequiredEntitlementUsageTypeDef, _OptionalEntitlementUsageTypeDef):
     pass
 
+
 _RequiredExtendLicenseConsumptionRequestRequestTypeDef = TypedDict(
     "_RequiredExtendLicenseConsumptionRequestRequestTypeDef",
     {
         "LicenseConsumptionToken": str,
     },
 )
 _OptionalExtendLicenseConsumptionRequestRequestTypeDef = TypedDict(
     "_OptionalExtendLicenseConsumptionRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class ExtendLicenseConsumptionRequestRequestTypeDef(
     _RequiredExtendLicenseConsumptionRequestRequestTypeDef,
     _OptionalExtendLicenseConsumptionRequestRequestTypeDef,
 ):
     pass
 
+
+ExtendLicenseConsumptionResponseTypeDef = TypedDict(
+    "ExtendLicenseConsumptionResponseTypeDef",
+    {
+        "LicenseConsumptionToken": str,
+        "Expiration": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -529,62 +634,49 @@
     "_OptionalGetAccessTokenRequestRequestTypeDef",
     {
         "TokenProperties": Sequence[str],
     },
     total=False,
 )
 
+
 class GetAccessTokenRequestRequestTypeDef(
     _RequiredGetAccessTokenRequestRequestTypeDef, _OptionalGetAccessTokenRequestRequestTypeDef
 ):
     pass
 
+
+GetAccessTokenResponseTypeDef = TypedDict(
+    "GetAccessTokenResponseTypeDef",
+    {
+        "AccessToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetGrantRequestRequestTypeDef = TypedDict(
     "_RequiredGetGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 _OptionalGetGrantRequestRequestTypeDef = TypedDict(
     "_OptionalGetGrantRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetGrantRequestRequestTypeDef(
     _RequiredGetGrantRequestRequestTypeDef, _OptionalGetGrantRequestRequestTypeDef
 ):
     pass
 
-_RequiredGrantTypeDef = TypedDict(
-    "_RequiredGrantTypeDef",
-    {
-        "GrantArn": str,
-        "GrantName": str,
-        "ParentArn": str,
-        "LicenseArn": str,
-        "GranteePrincipalArn": str,
-        "HomeRegion": str,
-        "GrantStatus": GrantStatusType,
-        "Version": str,
-        "GrantedOperations": List[AllowedOperationType],
-    },
-)
-_OptionalGrantTypeDef = TypedDict(
-    "_OptionalGrantTypeDef",
-    {
-        "StatusReason": str,
-    },
-    total=False,
-)
-
-class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
-    pass
 
 GetLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "GetLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
@@ -622,19 +714,21 @@
     "_OptionalGetLicenseRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetLicenseRequestRequestTypeDef(
     _RequiredGetLicenseRequestRequestTypeDef, _OptionalGetLicenseRequestRequestTypeDef
 ):
     pass
 
+
 GetLicenseUsageRequestRequestTypeDef = TypedDict(
     "GetLicenseUsageRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 
@@ -676,17 +770,19 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
+
 LicenseConfigurationAssociationTypeDef = TypedDict(
     "LicenseConfigurationAssociationTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": ResourceTypeType,
         "ResourceOwnerId": str,
         "AssociationTime": datetime,
@@ -718,29 +814,43 @@
     "_OptionalLicenseSpecificationTypeDef",
     {
         "AmiAssociationScope": str,
     },
     total=False,
 )
 
+
 class LicenseSpecificationTypeDef(
     _RequiredLicenseSpecificationTypeDef, _OptionalLicenseSpecificationTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
+    _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListAssociationsForLicenseConfigurationRequestRequestTypeDef = TypedDict(
@@ -748,20 +858,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAssociationsForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListAssociationsForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef = TypedDict(
@@ -769,20 +881,44 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef(
     _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
     _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
+    _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+    _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
@@ -790,20 +926,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalListLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListLicenseVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseVersionsRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 _OptionalListLicenseVersionsRequestRequestTypeDef = TypedDict(
@@ -811,20 +949,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListLicenseVersionsRequestRequestTypeDef(
     _RequiredListLicenseVersionsRequestRequestTypeDef,
     _OptionalListLicenseVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ResourceInventoryTypeDef = TypedDict(
     "ResourceInventoryTypeDef",
     {
         "ResourceId": str,
         "ResourceType": ResourceTypeType,
         "ResourceArn": str,
         "Platform": str,
@@ -851,14 +991,24 @@
         "TokenProperties": List[str],
         "RoleArns": List[str],
         "Status": str,
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
 _RequiredProductInformationFilterTypeDef = TypedDict(
     "_RequiredProductInformationFilterTypeDef",
     {
         "ProductInformationFilterName": str,
         "ProductInformationFilterComparator": str,
     },
 )
@@ -866,170 +1016,63 @@
     "_OptionalProductInformationFilterTypeDef",
     {
         "ProductInformationFilterValue": Sequence[str],
     },
     total=False,
 )
 
+
 class ProductInformationFilterTypeDef(
     _RequiredProductInformationFilterTypeDef, _OptionalProductInformationFilterTypeDef
 ):
     pass
 
+
 RejectGrantRequestRequestTypeDef = TypedDict(
     "RejectGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
-    {
-        "bucket": str,
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
-    },
-)
-
-AcceptGrantResponseTypeDef = TypedDict(
-    "AcceptGrantResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGrantResponseTypeDef = TypedDict(
-    "CreateGrantResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGrantVersionResponseTypeDef = TypedDict(
-    "CreateGrantVersionResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLicenseConfigurationResponseTypeDef = TypedDict(
-    "CreateLicenseConfigurationResponseTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLicenseConversionTaskForResourceResponseTypeDef = TypedDict(
-    "CreateLicenseConversionTaskForResourceResponseTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
-    "CreateLicenseManagerReportGeneratorResponseTypeDef",
-    {
-        "LicenseManagerReportGeneratorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLicenseResponseTypeDef = TypedDict(
-    "CreateLicenseResponseTypeDef",
-    {
-        "LicenseArn": str,
-        "Status": LicenseStatusType,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLicenseVersionResponseTypeDef = TypedDict(
-    "CreateLicenseVersionResponseTypeDef",
-    {
-        "LicenseArn": str,
-        "Version": str,
-        "Status": LicenseStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTokenResponseTypeDef = TypedDict(
-    "CreateTokenResponseTypeDef",
-    {
-        "TokenId": str,
-        "TokenType": Literal["REFRESH_TOKEN"],
-        "Token": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteGrantResponseTypeDef = TypedDict(
-    "DeleteGrantResponseTypeDef",
+RejectGrantResponseTypeDef = TypedDict(
+    "RejectGrantResponseTypeDef",
     {
         "GrantArn": str,
         "Status": GrantStatusType,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteLicenseResponseTypeDef = TypedDict(
-    "DeleteLicenseResponseTypeDef",
-    {
-        "Status": LicenseDeletionStatusType,
-        "DeletionDate": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExtendLicenseConsumptionResponseTypeDef = TypedDict(
-    "ExtendLicenseConsumptionResponseTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
-        "LicenseConsumptionToken": str,
-        "Expiration": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "bucket": str,
+        "keyPrefix": str,
     },
+    total=False,
 )
 
-GetAccessTokenResponseTypeDef = TypedDict(
-    "GetAccessTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AccessToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-RejectGrantResponseTypeDef = TypedDict(
-    "RejectGrantResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
 _RequiredCheckoutLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutLicenseRequestRequestTypeDef",
     {
         "ProductSKU": str,
@@ -1044,31 +1087,33 @@
     {
         "Beneficiary": str,
         "NodeId": str,
     },
     total=False,
 )
 
+
 class CheckoutLicenseRequestRequestTypeDef(
     _RequiredCheckoutLicenseRequestRequestTypeDef, _OptionalCheckoutLicenseRequestRequestTypeDef
 ):
     pass
 
+
 CheckoutLicenseResponseTypeDef = TypedDict(
     "CheckoutLicenseResponseTypeDef",
     {
         "CheckoutType": CheckoutTypeType,
         "LicenseConsumptionToken": str,
         "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "SignedToken": str,
         "NodeId": str,
         "IssuedAt": str,
         "Expiration": str,
         "LicenseArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCheckoutBorrowLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutBorrowLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
@@ -1082,32 +1127,34 @@
     {
         "NodeId": str,
         "CheckoutMetadata": Sequence[MetadataTypeDef],
     },
     total=False,
 )
 
+
 class CheckoutBorrowLicenseRequestRequestTypeDef(
     _RequiredCheckoutBorrowLicenseRequestRequestTypeDef,
     _OptionalCheckoutBorrowLicenseRequestRequestTypeDef,
 ):
     pass
 
+
 CheckoutBorrowLicenseResponseTypeDef = TypedDict(
     "CheckoutBorrowLicenseResponseTypeDef",
     {
         "LicenseArn": str,
         "LicenseConsumptionToken": str,
         "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "NodeId": str,
         "SignedToken": str,
         "IssuedAt": str,
         "Expiration": str,
         "CheckoutMetadata": List[MetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LicenseOperationFailureTypeDef = TypedDict(
     "LicenseOperationFailureTypeDef",
     {
         "ResourceArn": str,
@@ -1128,19 +1175,75 @@
         "RenewType": RenewTypeType,
         "ProvisionalConfiguration": ProvisionalConfigurationTypeDef,
         "BorrowConfiguration": BorrowConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateGrantVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateGrantVersionRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "GrantArn": str,
+    },
+)
+_OptionalCreateGrantVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateGrantVersionRequestRequestTypeDef",
+    {
+        "GrantName": str,
+        "AllowedOperations": Sequence[AllowedOperationType],
+        "Status": GrantStatusType,
+        "StatusReason": str,
+        "SourceVersion": str,
+        "Options": OptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateGrantVersionRequestRequestTypeDef(
+    _RequiredCreateGrantVersionRequestRequestTypeDef,
+    _OptionalCreateGrantVersionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredGrantTypeDef = TypedDict(
+    "_RequiredGrantTypeDef",
+    {
+        "GrantArn": str,
+        "GrantName": str,
+        "ParentArn": str,
+        "LicenseArn": str,
+        "GranteePrincipalArn": str,
+        "HomeRegion": str,
+        "GrantStatus": GrantStatusType,
+        "Version": str,
+        "GrantedOperations": List[AllowedOperationType],
+    },
+)
+_OptionalGrantTypeDef = TypedDict(
+    "_OptionalGrantTypeDef",
+    {
+        "StatusReason": str,
+        "Options": OptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
+    pass
+
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1165,15 +1268,15 @@
         "SourceLicenseContext": LicenseConversionContextTypeDef,
         "DestinationLicenseContext": LicenseConversionContextTypeDef,
         "StatusMessage": str,
         "Status": LicenseConversionTaskStatusType,
         "StartTime": datetime,
         "LicenseConversionTime": datetime,
         "EndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LicenseConversionTaskTypeDef = TypedDict(
     "LicenseConversionTaskTypeDef",
     {
         "LicenseConversionTaskId": str,
@@ -1204,20 +1307,22 @@
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateLicenseManagerReportGeneratorRequestRequestTypeDef(
     _RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     _OptionalCreateLicenseManagerReportGeneratorRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "LicenseManagerReportGeneratorArn": str,
         "ReportGeneratorName": str,
         "Type": Sequence[ReportTypeType],
         "ReportContext": ReportContextTypeDef,
@@ -1229,20 +1334,22 @@
     "_OptionalUpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateLicenseManagerReportGeneratorRequestRequestTypeDef(
     _RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     _OptionalUpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
 ):
     pass
 
+
 LicenseUsageTypeDef = TypedDict(
     "LicenseUsageTypeDef",
     {
         "EntitlementUsages": List[EntitlementUsageTypeDef],
     },
     total=False,
 )
@@ -1254,14 +1361,24 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
+    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
+    {
+        "LicenseConfigurationArns": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLicenseConfigurationsRequestRequestTypeDef = TypedDict(
     "ListLicenseConfigurationsRequestRequestTypeDef",
     {
         "LicenseConfigurationArns": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1312,20 +1429,22 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListReceivedGrantsForOrganizationRequestRequestTypeDef(
     _RequiredListReceivedGrantsForOrganizationRequestRequestTypeDef,
     _OptionalListReceivedGrantsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
+
 ListReceivedGrantsRequestRequestTypeDef = TypedDict(
     "ListReceivedGrantsRequestRequestTypeDef",
     {
         "GrantArns": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
@@ -1361,94 +1480,93 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredListUsageForLicenseConfigurationRequestRequestTypeDef",
+_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
-_OptionalListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalListUsageForLicenseConfigurationRequestRequestTypeDef",
+_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class ListUsageForLicenseConfigurationRequestRequestTypeDef(
-    _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef,
-    _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef,
+
+class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
+    _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
+    _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
 ):
     pass
 
-GetGrantResponseTypeDef = TypedDict(
-    "GetGrantResponseTypeDef",
-    {
-        "Grant": GrantTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-ListDistributedGrantsResponseTypeDef = TypedDict(
-    "ListDistributedGrantsResponseTypeDef",
+_RequiredListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredListUsageForLicenseConfigurationRequestRequestTypeDef",
     {
-        "Grants": List[GrantTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LicenseConfigurationArn": str,
     },
 )
-
-ListReceivedGrantsForOrganizationResponseTypeDef = TypedDict(
-    "ListReceivedGrantsForOrganizationResponseTypeDef",
+_OptionalListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalListUsageForLicenseConfigurationRequestRequestTypeDef",
     {
-        "Grants": List[GrantTypeDef],
+        "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Filters": Sequence[FilterTypeDef],
     },
+    total=False,
 )
 
-ListReceivedGrantsResponseTypeDef = TypedDict(
-    "ListReceivedGrantsResponseTypeDef",
-    {
-        "Grants": List[GrantTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+
+class ListUsageForLicenseConfigurationRequestRequestTypeDef(
+    _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef,
+    _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
+
 
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
         "OrganizationConfiguration": OrganizationConfigurationTypeDef,
         "EnableCrossAccountsDiscovery": bool,
         "LicenseManagerResourceShareArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceSettingsRequestRequestTypeDef = TypedDict(
     "UpdateServiceSettingsRequestRequestTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
         "OrganizationConfiguration": OrganizationConfigurationTypeDef,
         "EnableCrossAccountsDiscovery": bool,
     },
     total=False,
 )
 
+ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
+    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+    {
+        "Filters": Sequence[InventoryFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListResourceInventoryRequestRequestTypeDef = TypedDict(
     "ListResourceInventoryRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[InventoryFilterTypeDef],
     },
@@ -1456,33 +1574,33 @@
 )
 
 ListAssociationsForLicenseConfigurationResponseTypeDef = TypedDict(
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationAssociations": List[LicenseConfigurationAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUsageForLicenseConfigurationResponseTypeDef = TypedDict(
     "ListUsageForLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationUsageList": List[LicenseConfigurationUsageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLicenseSpecificationsForResourceResponseTypeDef = TypedDict(
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     {
         "LicenseSpecifications": List[LicenseSpecificationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1493,115 +1611,37 @@
     {
         "AddLicenseSpecifications": Sequence[LicenseSpecificationTypeDef],
         "RemoveLicenseSpecifications": Sequence[LicenseSpecificationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
-    _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-    _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-):
-    pass
-
-ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
-    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
-    {
-        "LicenseConfigurationArns": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
-    _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-    _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-):
-    pass
-
-ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
-    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
-    {
-        "Filters": Sequence[InventoryFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
-    _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
-    _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
-):
-    pass
 
 ListResourceInventoryResponseTypeDef = TypedDict(
     "ListResourceInventoryResponseTypeDef",
     {
         "ResourceInventoryList": List[ResourceInventoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTokensResponseTypeDef = TypedDict(
     "ListTokensResponseTypeDef",
     {
         "Tokens": List[TokenDataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProductInformationTypeDef = TypedDict(
     "ProductInformationTypeDef",
     {
         "ResourceType": str,
@@ -1630,15 +1670,15 @@
 )
 
 ListFailuresForLicenseConfigurationOperationsResponseTypeDef = TypedDict(
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     {
         "LicenseOperationFailureList": List[LicenseOperationFailureTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseRequestRequestTypeDef",
     {
         "LicenseName": str,
@@ -1657,19 +1697,21 @@
     "_OptionalCreateLicenseRequestRequestTypeDef",
     {
         "LicenseMetadata": Sequence[MetadataTypeDef],
     },
     total=False,
 )
 
+
 class CreateLicenseRequestRequestTypeDef(
     _RequiredCreateLicenseRequestRequestTypeDef, _OptionalCreateLicenseRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateLicenseVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseVersionRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "LicenseName": str,
         "ProductName": str,
         "Issuer": IssuerTypeDef,
@@ -1686,20 +1728,22 @@
     {
         "LicenseMetadata": Sequence[MetadataTypeDef],
         "SourceVersion": str,
     },
     total=False,
 )
 
+
 class CreateLicenseVersionRequestRequestTypeDef(
     _RequiredCreateLicenseVersionRequestRequestTypeDef,
     _OptionalCreateLicenseVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GrantedLicenseTypeDef = TypedDict(
     "GrantedLicenseTypeDef",
     {
         "LicenseArn": str,
         "LicenseName": str,
         "ProductName": str,
         "ProductSKU": str,
@@ -1735,28 +1779,63 @@
         "LicenseMetadata": List[MetadataTypeDef],
         "CreateTime": str,
         "Version": str,
     },
     total=False,
 )
 
+GetGrantResponseTypeDef = TypedDict(
+    "GetGrantResponseTypeDef",
+    {
+        "Grant": GrantTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDistributedGrantsResponseTypeDef = TypedDict(
+    "ListDistributedGrantsResponseTypeDef",
+    {
+        "Grants": List[GrantTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListReceivedGrantsForOrganizationResponseTypeDef = TypedDict(
+    "ListReceivedGrantsForOrganizationResponseTypeDef",
+    {
+        "Grants": List[GrantTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListReceivedGrantsResponseTypeDef = TypedDict(
+    "ListReceivedGrantsResponseTypeDef",
+    {
+        "Grants": List[GrantTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListLicenseConversionTasksResponseTypeDef = TypedDict(
     "ListLicenseConversionTasksResponseTypeDef",
     {
         "LicenseConversionTasks": List[LicenseConversionTaskTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLicenseUsageResponseTypeDef = TypedDict(
     "GetLicenseUsageResponseTypeDef",
     {
         "LicenseUsage": LicenseUsageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
     {
         "Name": str,
@@ -1773,20 +1852,22 @@
         "Tags": Sequence[TagTypeDef],
         "DisassociateWhenNotFound": bool,
         "ProductInformationList": Sequence[ProductInformationTypeDef],
     },
     total=False,
 )
 
+
 class CreateLicenseConfigurationRequestRequestTypeDef(
     _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
     _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetLicenseConfigurationResponseTypeDef = TypedDict(
     "GetLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationId": str,
         "LicenseConfigurationArn": str,
         "Name": str,
         "Description": str,
@@ -1799,15 +1880,15 @@
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
         "Tags": List[TagTypeDef],
         "ProductInformationList": List[ProductInformationTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
         "DisassociateWhenNotFound": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LicenseConfigurationTypeDef = TypedDict(
     "LicenseConfigurationTypeDef",
     {
         "LicenseConfigurationId": str,
@@ -1847,82 +1928,84 @@
         "Description": str,
         "ProductInformationList": Sequence[ProductInformationTypeDef],
         "DisassociateWhenNotFound": bool,
     },
     total=False,
 )
 
+
 class UpdateLicenseConfigurationRequestRequestTypeDef(
     _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
     _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     {
         "ReportGenerator": ReportGeneratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLicenseManagerReportGeneratorsResponseTypeDef = TypedDict(
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     {
         "ReportGenerators": List[ReportGeneratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReceivedLicensesForOrganizationResponseTypeDef = TypedDict(
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     {
         "Licenses": List[GrantedLicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReceivedLicensesResponseTypeDef = TypedDict(
     "ListReceivedLicensesResponseTypeDef",
     {
         "Licenses": List[GrantedLicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLicenseResponseTypeDef = TypedDict(
     "GetLicenseResponseTypeDef",
     {
         "License": LicenseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLicenseVersionsResponseTypeDef = TypedDict(
     "ListLicenseVersionsResponseTypeDef",
     {
         "Licenses": List[LicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLicensesResponseTypeDef = TypedDict(
     "ListLicensesResponseTypeDef",
     {
         "Licenses": List[LicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLicenseConfigurationsResponseTypeDef = TypedDict(
     "ListLicenseConfigurationsResponseTypeDef",
     {
         "LicenseConfigurations": List[LicenseConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager.egg-info/PKG-INFO` & `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager
-Version: 1.26.8
-Summary: Type annotations for boto3.LicenseManager 1.26.8 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.LicenseManager 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
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
 
 <a id="mypy-boto3-license-manager"></a>
 
 # mypy-boto3-license-manager
 
 [![PyPI - mypy-boto3-license-manager](https://img.shields.io/pypi/v/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,14 +318,15 @@
 ### Literals
 
 `mypy_boto3_license_manager.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_license_manager.literals import (
+    ActivationOverrideBehaviorType,
     AllowedOperationType,
     CheckoutTypeType,
     DigitalSignatureMethodType,
     EntitlementDataUnitType,
     EntitlementUnitType,
     GrantStatusType,
     InventoryFilterConditionType,
@@ -348,146 +350,147 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: AllowedOperationType) -> bool:
+def check_value(value: ActivationOverrideBehaviorType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_license_manager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AcceptGrantResponseTypeDef,
     AutomatedDiscoveryInformationTypeDef,
     BorrowConfigurationTypeDef,
     CheckInLicenseRequestRequestTypeDef,
     EntitlementDataTypeDef,
     MetadataTypeDef,
     ConsumedLicenseSummaryTypeDef,
     ProvisionalConfigurationTypeDef,
     CreateGrantRequestRequestTypeDef,
-    CreateGrantVersionRequestRequestTypeDef,
+    CreateGrantResponseTypeDef,
+    OptionsTypeDef,
+    CreateGrantVersionResponseTypeDef,
     TagTypeDef,
+    CreateLicenseConfigurationResponseTypeDef,
     LicenseConversionContextTypeDef,
+    CreateLicenseConversionTaskForResourceResponseTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
+    CreateLicenseManagerReportGeneratorResponseTypeDef,
     DatetimeRangeTypeDef,
     EntitlementTypeDef,
     IssuerTypeDef,
+    CreateLicenseResponseTypeDef,
+    CreateLicenseVersionResponseTypeDef,
     CreateTokenRequestRequestTypeDef,
+    CreateTokenResponseTypeDef,
     DeleteGrantRequestRequestTypeDef,
+    DeleteGrantResponseTypeDef,
     DeleteLicenseConfigurationRequestRequestTypeDef,
     DeleteLicenseManagerReportGeneratorRequestRequestTypeDef,
     DeleteLicenseRequestRequestTypeDef,
+    DeleteLicenseResponseTypeDef,
     DeleteTokenRequestRequestTypeDef,
     EntitlementUsageTypeDef,
     ExtendLicenseConsumptionRequestRequestTypeDef,
+    ExtendLicenseConsumptionResponseTypeDef,
     FilterTypeDef,
     GetAccessTokenRequestRequestTypeDef,
+    GetAccessTokenResponseTypeDef,
     GetGrantRequestRequestTypeDef,
-    GrantTypeDef,
     GetLicenseConfigurationRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
     GetLicenseConversionTaskRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorRequestRequestTypeDef,
     GetLicenseRequestRequestTypeDef,
     GetLicenseUsageRequestRequestTypeDef,
     OrganizationConfigurationTypeDef,
     IssuerDetailsTypeDef,
     ReceivedMetadataTypeDef,
     InventoryFilterTypeDef,
     LicenseConfigurationAssociationTypeDef,
     LicenseConfigurationUsageTypeDef,
     LicenseSpecificationTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
     ListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
+    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListLicenseVersionsRequestRequestTypeDef,
     ResourceInventoryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TokenDataTypeDef,
+    PaginatorConfigTypeDef,
     ProductInformationFilterTypeDef,
     RejectGrantRequestRequestTypeDef,
+    RejectGrantResponseTypeDef,
     S3LocationTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AcceptGrantResponseTypeDef,
-    CreateGrantResponseTypeDef,
-    CreateGrantVersionResponseTypeDef,
-    CreateLicenseConfigurationResponseTypeDef,
-    CreateLicenseConversionTaskForResourceResponseTypeDef,
-    CreateLicenseManagerReportGeneratorResponseTypeDef,
-    CreateLicenseResponseTypeDef,
-    CreateLicenseVersionResponseTypeDef,
-    CreateTokenResponseTypeDef,
-    DeleteGrantResponseTypeDef,
-    DeleteLicenseResponseTypeDef,
-    ExtendLicenseConsumptionResponseTypeDef,
-    GetAccessTokenResponseTypeDef,
-    RejectGrantResponseTypeDef,
     CheckoutLicenseRequestRequestTypeDef,
     CheckoutLicenseResponseTypeDef,
     CheckoutBorrowLicenseRequestRequestTypeDef,
     CheckoutBorrowLicenseResponseTypeDef,
     LicenseOperationFailureTypeDef,
     ConsumptionConfigurationTypeDef,
+    CreateGrantVersionRequestRequestTypeDef,
+    GrantTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLicenseConversionTaskForResourceRequestRequestTypeDef,
     GetLicenseConversionTaskResponseTypeDef,
     LicenseConversionTaskTypeDef,
     CreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     UpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     LicenseUsageTypeDef,
     ListDistributedGrantsRequestRequestTypeDef,
+    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
     ListLicenseConfigurationsRequestRequestTypeDef,
     ListLicenseConversionTasksRequestRequestTypeDef,
     ListLicenseManagerReportGeneratorsRequestRequestTypeDef,
     ListLicensesRequestRequestTypeDef,
     ListReceivedGrantsForOrganizationRequestRequestTypeDef,
     ListReceivedGrantsRequestRequestTypeDef,
     ListReceivedLicensesForOrganizationRequestRequestTypeDef,
     ListReceivedLicensesRequestRequestTypeDef,
     ListTokensRequestRequestTypeDef,
+    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestRequestTypeDef,
-    GetGrantResponseTypeDef,
-    ListDistributedGrantsResponseTypeDef,
-    ListReceivedGrantsForOrganizationResponseTypeDef,
-    ListReceivedGrantsResponseTypeDef,
     GetServiceSettingsResponseTypeDef,
     UpdateServiceSettingsRequestRequestTypeDef,
+    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
     ListResourceInventoryRequestRequestTypeDef,
     ListAssociationsForLicenseConfigurationResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     ListLicenseSpecificationsForResourceResponseTypeDef,
     UpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
-    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
-    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
-    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
     ProductInformationTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
     CreateLicenseRequestRequestTypeDef,
     CreateLicenseVersionRequestRequestTypeDef,
     GrantedLicenseTypeDef,
     LicenseTypeDef,
+    GetGrantResponseTypeDef,
+    ListDistributedGrantsResponseTypeDef,
+    ListReceivedGrantsForOrganizationResponseTypeDef,
+    ListReceivedGrantsResponseTypeDef,
     ListLicenseConversionTasksResponseTypeDef,
     GetLicenseUsageResponseTypeDef,
     CreateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
     UpdateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
@@ -508,42 +511,42 @@
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

### Comparing `mypy-boto3-license-manager-1.26.8/mypy_boto3_license_manager.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.26.8/setup.py` & `mypy-boto3-license-manager-1.27.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-license-manager.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager",
-    version="1.26.8",
+    version="1.27.0",
     packages=["mypy_boto3_license_manager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManager 1.26.8 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.LicenseManager 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 license-manager type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_license_manager": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_license_manager": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/",
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


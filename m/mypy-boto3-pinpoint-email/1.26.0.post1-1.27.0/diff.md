# Comparing `tmp/mypy-boto3-pinpoint-email-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-pinpoint-email-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-email-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:50 2022, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-email-1.27.0.tar", last modified: Mon Jul  3 19:51:15 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-email-1.26.0.post1.tar` & `mypy-boto3-pinpoint-email-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:50.040840 mypy-boto3-pinpoint-email-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:39:13.000000 mypy-boto3-pinpoint-email-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18344 2022-11-01 21:43:50.036840 mypy-boto3-pinpoint-email-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16876 2022-11-01 21:39:13.000000 mypy-boto3-pinpoint-email-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:50.032840 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-11-01 21:39:13.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-11-01 21:39:13.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-11-01 21:39:13.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32971 2022-11-01 21:39:14.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    32917 2022-11-01 21:39:13.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9133 2022-11-01 21:39:14.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9131 2022-11-01 21:39:14.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6575 2022-11-01 21:39:14.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6568 2022-11-01 21:39:14.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:39:13.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    34935 2022-11-01 21:39:14.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    34901 2022-11-01 21:39:14.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:39:13.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:50.032840 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18344 2022-11-01 21:43:49.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-01 21:43:49.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:49.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:49.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:49.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-01 21:43:49.000000 mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:50.040840 mypy-boto3-pinpoint-email-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-11-01 21:39:13.000000 mypy-boto3-pinpoint-email-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:15.303804 mypy-boto3-pinpoint-email-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:37.000000 mypy-boto3-pinpoint-email-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-07-03 19:51:15.303804 mypy-boto3-pinpoint-email-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-07-03 19:43:37.000000 mypy-boto3-pinpoint-email-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:15.299804 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-03 19:43:37.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-03 19:43:37.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:43:37.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-07-03 19:43:37.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32917 2023-07-03 19:43:37.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-07-03 19:43:38.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-07-03 19:43:38.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-03 19:43:38.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-07-03 19:43:38.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:37.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34985 2023-07-03 19:43:38.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34951 2023-07-03 19:43:38.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:37.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:15.303804 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-07-03 19:51:15.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:51:15.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:15.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:15.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:15.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:51:15.000000 mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:15.303804 mypy-boto3-pinpoint-email-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-03 19:43:37.000000 mypy-boto3-pinpoint-email-1.27.0/setup.py
```

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/LICENSE` & `mypy-boto3-pinpoint-email-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/PKG-INFO` & `mypy-boto3-pinpoint-email-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-email
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.PinpointEmail 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.PinpointEmail 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/
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
 
 <a id="mypy-boto3-pinpoint-email"></a>
 
 # mypy-boto3-pinpoint-email
 
 [![PyPI - mypy-boto3-pinpoint-email](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint-email?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointEmail 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[boto3.PinpointEmail 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,15 +360,15 @@
     ContentTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
     DkimAttributesTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
@@ -382,70 +383,70 @@
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
     SendQuotaTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     IdentityInfoTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
+    ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
     ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MessageTagTypeDef,
+    PaginatorConfigTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
     PutConfigurationSetSendingOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    SendEmailResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    GetBlacklistReportsResponseTypeDef,
     BodyTypeDef,
     CloudWatchDestinationTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
-    GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
-    ListConfigurationSetsResponseTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SendEmailResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     GetAccountResponseTypeDef,
-    GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
-    ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
-    ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
-    ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     MessageTypeDef,
     EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
@@ -468,42 +469,42 @@
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

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/README.md` & `mypy-boto3-pinpoint-email-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-pinpoint-email"></a>
 
 # mypy-boto3-pinpoint-email
 
 [![PyPI - mypy-boto3-pinpoint-email](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint-email?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointEmail 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[boto3.PinpointEmail 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,15 +328,15 @@
     ContentTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
     DkimAttributesTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
@@ -351,70 +351,70 @@
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
     SendQuotaTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     IdentityInfoTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
+    ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
     ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MessageTagTypeDef,
+    PaginatorConfigTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
     PutConfigurationSetSendingOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    SendEmailResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    GetBlacklistReportsResponseTypeDef,
     BodyTypeDef,
     CloudWatchDestinationTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
-    GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
-    ListConfigurationSetsResponseTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SendEmailResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     GetAccountResponseTypeDef,
-    GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
-    ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
-    ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
-    ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     MessageTypeDef,
     EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
@@ -437,42 +437,42 @@
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

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/__init__.py` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/__init__.pyi` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/__main__.py` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PinpointEmail 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.PinpointEmail 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail\nOther"
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

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/client.py` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/client.pyi` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/literals.py` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,23 +72,25 @@
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
@@ -98,30 +100,35 @@
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
@@ -147,14 +154,15 @@
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
@@ -199,51 +207,57 @@
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
@@ -256,14 +270,15 @@
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
@@ -275,28 +290,35 @@
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
@@ -305,14 +327,15 @@
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
@@ -323,55 +346,64 @@
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
@@ -404,14 +436,15 @@
     "af-south-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
```

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/literals.pyi` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -70,23 +70,25 @@
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
@@ -96,30 +98,35 @@
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
@@ -145,14 +152,15 @@
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
@@ -197,51 +205,57 @@
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
@@ -254,14 +268,15 @@
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
@@ -273,28 +288,35 @@
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
@@ -303,14 +325,15 @@
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
@@ -321,55 +344,64 @@
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
@@ -402,14 +434,15 @@
     "af-south-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
```

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/paginator.py` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,91 +44,84 @@
     "GetDedicatedIpsPaginator",
     "ListConfigurationSetsPaginator",
     "ListDedicatedIpPoolsPaginator",
     "ListDeliverabilityTestReportsPaginator",
     "ListEmailIdentitiesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class GetDedicatedIpsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.GetDedicatedIps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#getdedicatedipspaginator)
     """
 
     def paginate(
-        self, *, PoolName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PoolName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDedicatedIpsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.GetDedicatedIps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#getdedicatedipspaginator)
         """
 
-
 class ListConfigurationSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListConfigurationSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listconfigurationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfigurationSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listconfigurationsetspaginator)
         """
 
-
 class ListDedicatedIpPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDedicatedIpPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdedicatedippoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDedicatedIpPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDedicatedIpPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdedicatedippoolspaginator)
         """
 
-
 class ListDeliverabilityTestReportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDeliverabilityTestReports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdeliverabilitytestreportspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeliverabilityTestReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDeliverabilityTestReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdeliverabilitytestreportspaginator)
         """
 
-
 class ListEmailIdentitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListEmailIdentities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listemailidentitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEmailIdentitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListEmailIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listemailidentitiespaginator)
         """
```

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/paginator.pyi` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,84 +44,91 @@
     "GetDedicatedIpsPaginator",
     "ListConfigurationSetsPaginator",
     "ListDedicatedIpPoolsPaginator",
     "ListDeliverabilityTestReportsPaginator",
     "ListEmailIdentitiesPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class GetDedicatedIpsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.GetDedicatedIps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#getdedicatedipspaginator)
     """
 
     def paginate(
-        self, *, PoolName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PoolName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDedicatedIpsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.GetDedicatedIps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#getdedicatedipspaginator)
         """
 
+
 class ListConfigurationSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListConfigurationSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listconfigurationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfigurationSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listconfigurationsetspaginator)
         """
 
+
 class ListDedicatedIpPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDedicatedIpPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdedicatedippoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDedicatedIpPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDedicatedIpPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdedicatedippoolspaginator)
         """
 
+
 class ListDeliverabilityTestReportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDeliverabilityTestReports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdeliverabilitytestreportspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeliverabilityTestReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDeliverabilityTestReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdeliverabilitytestreportspaginator)
         """
 
+
 class ListEmailIdentitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListEmailIdentities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listemailidentitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEmailIdentitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListEmailIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listemailidentitiespaginator)
         """
```

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/type_defs.py` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "ContentTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "DeliveryOptionsTypeDef",
     "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateDeliverabilityTestReportResponseTypeDef",
     "DkimAttributesTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
     "DedicatedIpTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
@@ -64,70 +64,70 @@
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "SendQuotaTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "IdentityInfoTypeDef",
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
+    "ListDedicatedIpPoolsResponseTypeDef",
+    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MessageTagTypeDef",
+    "PaginatorConfigTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "PutConfigurationSetReputationOptionsRequestRequestTypeDef",
     "PutConfigurationSetSendingOptionsRequestRequestTypeDef",
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "SendEmailResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "GetBlacklistReportsResponseTypeDef",
     "BodyTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
     "CreateEmailIdentityRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
-    "CreateDeliverabilityTestReportResponseTypeDef",
-    "GetBlacklistReportsResponseTypeDef",
     "GetConfigurationSetResponseTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
-    "ListDedicatedIpPoolsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "SendEmailResponseTypeDef",
     "CreateEmailIdentityResponseTypeDef",
     "DailyVolumeTypeDef",
     "OverallVolumeTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "GetAccountResponseTypeDef",
-    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
-    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
-    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
-    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "MessageTypeDef",
     "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
@@ -217,22 +217,20 @@
 TrackingOptionsTypeDef = TypedDict(
     "TrackingOptionsTypeDef",
     {
         "CustomRedirectDomain": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
+    "CreateDeliverabilityTestReportResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ReportId": str,
+        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DkimAttributesTypeDef = TypedDict(
     "DkimAttributesTypeDef",
     {
         "SigningEnabled": bool,
@@ -441,20 +439,19 @@
 GetDedicatedIpRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpRequestRequestTypeDef",
     {
         "Ip": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = TypedDict(
+    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PoolName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetDedicatedIpsRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpsRequestRequestTypeDef",
     {
@@ -522,32 +519,74 @@
         "IdentityType": IdentityTypeType,
         "IdentityName": str,
         "SendingEnabled": bool,
     },
     total=False,
 )
 
+ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListConfigurationSetsRequestRequestTypeDef = TypedDict(
     "ListConfigurationSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef = TypedDict(
+    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDedicatedIpPoolsRequestRequestTypeDef = TypedDict(
     "ListDedicatedIpPoolsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+ListDedicatedIpPoolsResponseTypeDef = TypedDict(
+    "ListDedicatedIpPoolsResponseTypeDef",
+    {
+        "DedicatedIpPools": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef = TypedDict(
+    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDeliverabilityTestReportsRequestRequestTypeDef = TypedDict(
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -574,14 +613,22 @@
 class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
     _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
 ):
     pass
 
 
+ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef = TypedDict(
+    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEmailIdentitiesRequestRequestTypeDef = TypedDict(
     "ListEmailIdentitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -598,14 +645,24 @@
     "MessageTagTypeDef",
     {
         "Name": str,
         "Value": str,
     },
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
 PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     {
         "AutoWarmupEnabled": bool,
     },
     total=False,
 )
@@ -786,22 +843,49 @@
 class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
 ):
     pass
 
 
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
+SendEmailResponseTypeDef = TypedDict(
+    "SendEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+GetBlacklistReportsResponseTypeDef = TypedDict(
+    "GetBlacklistReportsResponseTypeDef",
+    {
+        "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
@@ -854,14 +938,22 @@
 class CreateEmailIdentityRequestRequestTypeDef(
     _RequiredCreateEmailIdentityRequestRequestTypeDef,
     _OptionalCreateEmailIdentityRequestRequestTypeDef,
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -888,85 +980,34 @@
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
 
-CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
-    "CreateDeliverabilityTestReportResponseTypeDef",
-    {
-        "ReportId": str,
-        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBlacklistReportsResponseTypeDef = TypedDict(
-    "GetBlacklistReportsResponseTypeDef",
-    {
-        "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetConfigurationSetResponseTypeDef = TypedDict(
     "GetConfigurationSetResponseTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
-    {
-        "ConfigurationSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDedicatedIpPoolsResponseTypeDef = TypedDict(
-    "ListDedicatedIpPoolsResponseTypeDef",
-    {
-        "DedicatedIpPools": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendEmailResponseTypeDef = TypedDict(
-    "SendEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEmailIdentityResponseTypeDef = TypedDict(
     "CreateEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DailyVolumeTypeDef = TypedDict(
     "DailyVolumeTypeDef",
     {
         "StartDate": datetime,
@@ -986,50 +1027,50 @@
     total=False,
 )
 
 GetDedicatedIpResponseTypeDef = TypedDict(
     "GetDedicatedIpResponseTypeDef",
     {
         "DedicatedIp": DedicatedIpTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDedicatedIpsResponseTypeDef = TypedDict(
     "GetDedicatedIpsResponseTypeDef",
     {
         "DedicatedIps": List[DedicatedIpTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeliverabilityTestReportsResponseTypeDef = TypedDict(
     "ListDeliverabilityTestReportsResponseTypeDef",
     {
         "DeliverabilityTestReports": List[DeliverabilityTestReportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainDeliverabilityCampaignResponseTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     {
         "DomainDeliverabilityCampaign": DomainDeliverabilityCampaignTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainDeliverabilityCampaignsResponseTypeDef = TypedDict(
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     {
         "DomainDeliverabilityCampaigns": List[DomainDeliverabilityCampaignTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": str,
@@ -1043,59 +1084,18 @@
     "GetAccountResponseTypeDef",
     {
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = TypedDict(
-    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
-    {
-        "PoolName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef = TypedDict(
-    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef = TypedDict(
-    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef = TypedDict(
-    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
@@ -1106,24 +1106,24 @@
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEmailIdentitiesResponseTypeDef = TypedDict(
     "ListEmailIdentitiesResponseTypeDef",
     {
         "EmailIdentities": List[IdentityInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
@@ -1169,27 +1169,27 @@
 
 
 GetDomainStatisticsReportResponseTypeDef = TypedDict(
     "GetDomainStatisticsReportResponseTypeDef",
     {
         "OverallVolume": OverallVolumeTypeDef,
         "DailyVolumes": List[DailyVolumeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeliverabilityDashboardOptionsResponseTypeDef = TypedDict(
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     {
         "DashboardEnabled": bool,
         "SubscriptionExpiryDate": datetime,
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
         "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
         "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
     "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
         "DashboardEnabled": bool,
@@ -1215,15 +1215,15 @@
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
         "Simple": MessageTypeDef,
@@ -1251,15 +1251,15 @@
     },
 )
 
 GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     {
         "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeliverabilityTestReportRequestRequestTypeDef",
     {
         "FromEmailAddress": str,
```

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email/type_defs.pyi` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     "ContentTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "DeliveryOptionsTypeDef",
     "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateDeliverabilityTestReportResponseTypeDef",
     "DkimAttributesTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
     "DedicatedIpTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
@@ -63,70 +63,70 @@
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "SendQuotaTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "IdentityInfoTypeDef",
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
+    "ListDedicatedIpPoolsResponseTypeDef",
+    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MessageTagTypeDef",
+    "PaginatorConfigTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "PutConfigurationSetReputationOptionsRequestRequestTypeDef",
     "PutConfigurationSetSendingOptionsRequestRequestTypeDef",
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "SendEmailResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "GetBlacklistReportsResponseTypeDef",
     "BodyTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
     "CreateEmailIdentityRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
-    "CreateDeliverabilityTestReportResponseTypeDef",
-    "GetBlacklistReportsResponseTypeDef",
     "GetConfigurationSetResponseTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
-    "ListDedicatedIpPoolsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "SendEmailResponseTypeDef",
     "CreateEmailIdentityResponseTypeDef",
     "DailyVolumeTypeDef",
     "OverallVolumeTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "GetAccountResponseTypeDef",
-    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
-    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
-    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
-    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "MessageTypeDef",
     "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
@@ -214,22 +214,20 @@
 TrackingOptionsTypeDef = TypedDict(
     "TrackingOptionsTypeDef",
     {
         "CustomRedirectDomain": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
+    "CreateDeliverabilityTestReportResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ReportId": str,
+        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DkimAttributesTypeDef = TypedDict(
     "DkimAttributesTypeDef",
     {
         "SigningEnabled": bool,
@@ -436,20 +434,19 @@
 GetDedicatedIpRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpRequestRequestTypeDef",
     {
         "Ip": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = TypedDict(
+    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PoolName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetDedicatedIpsRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpsRequestRequestTypeDef",
     {
@@ -517,32 +514,74 @@
         "IdentityType": IdentityTypeType,
         "IdentityName": str,
         "SendingEnabled": bool,
     },
     total=False,
 )
 
+ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListConfigurationSetsRequestRequestTypeDef = TypedDict(
     "ListConfigurationSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef = TypedDict(
+    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDedicatedIpPoolsRequestRequestTypeDef = TypedDict(
     "ListDedicatedIpPoolsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+ListDedicatedIpPoolsResponseTypeDef = TypedDict(
+    "ListDedicatedIpPoolsResponseTypeDef",
+    {
+        "DedicatedIpPools": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef = TypedDict(
+    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDeliverabilityTestReportsRequestRequestTypeDef = TypedDict(
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -567,14 +606,22 @@
 
 class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
     _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
 ):
     pass
 
+ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef = TypedDict(
+    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEmailIdentitiesRequestRequestTypeDef = TypedDict(
     "ListEmailIdentitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -591,14 +638,24 @@
     "MessageTagTypeDef",
     {
         "Name": str,
         "Value": str,
     },
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
 PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     {
         "AutoWarmupEnabled": bool,
     },
     total=False,
 )
@@ -765,22 +822,49 @@
 
 class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
 ):
     pass
 
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
+SendEmailResponseTypeDef = TypedDict(
+    "SendEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+GetBlacklistReportsResponseTypeDef = TypedDict(
+    "GetBlacklistReportsResponseTypeDef",
+    {
+        "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
@@ -829,14 +913,22 @@
 
 class CreateEmailIdentityRequestRequestTypeDef(
     _RequiredCreateEmailIdentityRequestRequestTypeDef,
     _OptionalCreateEmailIdentityRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -861,85 +953,34 @@
 
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
-CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
-    "CreateDeliverabilityTestReportResponseTypeDef",
-    {
-        "ReportId": str,
-        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBlacklistReportsResponseTypeDef = TypedDict(
-    "GetBlacklistReportsResponseTypeDef",
-    {
-        "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetConfigurationSetResponseTypeDef = TypedDict(
     "GetConfigurationSetResponseTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
-    {
-        "ConfigurationSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDedicatedIpPoolsResponseTypeDef = TypedDict(
-    "ListDedicatedIpPoolsResponseTypeDef",
-    {
-        "DedicatedIpPools": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendEmailResponseTypeDef = TypedDict(
-    "SendEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEmailIdentityResponseTypeDef = TypedDict(
     "CreateEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DailyVolumeTypeDef = TypedDict(
     "DailyVolumeTypeDef",
     {
         "StartDate": datetime,
@@ -959,50 +1000,50 @@
     total=False,
 )
 
 GetDedicatedIpResponseTypeDef = TypedDict(
     "GetDedicatedIpResponseTypeDef",
     {
         "DedicatedIp": DedicatedIpTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDedicatedIpsResponseTypeDef = TypedDict(
     "GetDedicatedIpsResponseTypeDef",
     {
         "DedicatedIps": List[DedicatedIpTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeliverabilityTestReportsResponseTypeDef = TypedDict(
     "ListDeliverabilityTestReportsResponseTypeDef",
     {
         "DeliverabilityTestReports": List[DeliverabilityTestReportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainDeliverabilityCampaignResponseTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     {
         "DomainDeliverabilityCampaign": DomainDeliverabilityCampaignTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainDeliverabilityCampaignsResponseTypeDef = TypedDict(
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     {
         "DomainDeliverabilityCampaigns": List[DomainDeliverabilityCampaignTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": str,
@@ -1016,59 +1057,18 @@
     "GetAccountResponseTypeDef",
     {
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = TypedDict(
-    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
-    {
-        "PoolName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef = TypedDict(
-    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef = TypedDict(
-    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef = TypedDict(
-    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
@@ -1079,24 +1079,24 @@
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEmailIdentitiesResponseTypeDef = TypedDict(
     "ListEmailIdentitiesResponseTypeDef",
     {
         "EmailIdentities": List[IdentityInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
@@ -1140,27 +1140,27 @@
     pass
 
 GetDomainStatisticsReportResponseTypeDef = TypedDict(
     "GetDomainStatisticsReportResponseTypeDef",
     {
         "OverallVolume": OverallVolumeTypeDef,
         "DailyVolumes": List[DailyVolumeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeliverabilityDashboardOptionsResponseTypeDef = TypedDict(
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     {
         "DashboardEnabled": bool,
         "SubscriptionExpiryDate": datetime,
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
         "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
         "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
     "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
         "DashboardEnabled": bool,
@@ -1184,15 +1184,15 @@
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
         "Simple": MessageTypeDef,
@@ -1220,15 +1220,15 @@
     },
 )
 
 GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     {
         "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeliverabilityTestReportRequestRequestTypeDef",
     {
         "FromEmailAddress": str,
```

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-email
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.PinpointEmail 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.PinpointEmail 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/
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
 
 <a id="mypy-boto3-pinpoint-email"></a>
 
 # mypy-boto3-pinpoint-email
 
 [![PyPI - mypy-boto3-pinpoint-email](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint-email?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointEmail 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[boto3.PinpointEmail 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,15 +360,15 @@
     ContentTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
     DkimAttributesTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
@@ -382,70 +383,70 @@
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
     SendQuotaTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     IdentityInfoTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
+    ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
     ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MessageTagTypeDef,
+    PaginatorConfigTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
     PutConfigurationSetSendingOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    SendEmailResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    GetBlacklistReportsResponseTypeDef,
     BodyTypeDef,
     CloudWatchDestinationTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
-    GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
-    ListConfigurationSetsResponseTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SendEmailResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     GetAccountResponseTypeDef,
-    GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
-    ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
-    ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
-    ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     MessageTypeDef,
     EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
@@ -468,42 +469,42 @@
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

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-email-1.27.0/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.26.0.post1/setup.py` & `mypy-boto3-pinpoint-email-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-pinpoint-email.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint-email",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_pinpoint_email"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PinpointEmail 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.PinpointEmail 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 pinpoint-email type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_pinpoint_email": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_pinpoint_email": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/",
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


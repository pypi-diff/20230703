# Comparing `tmp/mypy-boto3-sesv2-1.26.88.tar.gz` & `tmp/mypy-boto3-sesv2-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sesv2-1.26.88.tar", last modified: Thu Mar  9 20:38:43 2023, max compression
+gzip compressed data, was "mypy-boto3-sesv2-1.27.0.tar", last modified: Mon Jul  3 19:51:27 2023, max compression
```

## Comparing `mypy-boto3-sesv2-1.26.88.tar` & `mypy-boto3-sesv2-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:43.962381 mypy-boto3-sesv2-1.26.88/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20945 2023-03-09 20:38:43.958381 mypy-boto3-sesv2-1.26.88/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19466 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:43.958381 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56176 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56084 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68871 2023-03-09 20:38:28.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68801 2023-03-09 20:38:27.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:43.958381 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20945 2023-03-09 20:38:43.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-09 20:38:43.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:43.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:43.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-09 20:38:43.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-09 20:38:43.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 20:38:43.962381 mypy-boto3-sesv2-1.26.88/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:27.988007 mypy-boto3-sesv2-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:07.000000 mypy-boto3-sesv2-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-03 19:51:27.984007 mypy-boto3-sesv2-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19504 2023-07-03 19:48:07.000000 mypy-boto3-sesv2-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:27.976007 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-03 19:48:07.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-03 19:48:07.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 19:48:07.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56738 2023-07-03 19:48:07.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56645 2023-07-03 19:48:07.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-03 19:48:10.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-03 19:48:07.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:07.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69232 2023-07-03 19:48:11.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69162 2023-07-03 19:48:10.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:07.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:27.984007 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-03 19:51:27.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-03 19:51:27.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:27.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:27.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:27.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 19:51:27.000000 mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:27.988007 mypy-boto3-sesv2-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 19:48:06.000000 mypy-boto3-sesv2-1.27.0/setup.py
```

### Comparing `mypy-boto3-sesv2-1.26.88/LICENSE` & `mypy-boto3-sesv2-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-sesv2-1.26.88/PKG-INFO` & `mypy-boto3-sesv2-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.26.88
-Summary: Type annotations for boto3.SESV2 1.26.88 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.SESV2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sesv2"></a>
 
 # mypy-boto3-sesv2
 
 [![PyPI - mypy-boto3-sesv2](https://img.shields.io/pypi/v/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sesv2?color=blue)](https://pypistats.org/packages/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,15 +333,14 @@
 
 ```python
 from mypy_boto3_sesv2.type_defs import (
     ReviewDetailsTypeDef,
     BatchGetMetricDataQueryTypeDef,
     MetricDataErrorTypeDef,
     MetricDataResultTypeDef,
-    ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
@@ -352,19 +351,21 @@
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
     DkimSigningAttributesTypeDef,
     DkimAttributesTypeDef,
     EmailTemplateContentTypeDef,
     ImportDataSourceTypeDef,
+    CreateImportJobResponseTypeDef,
     CustomVerificationEmailTemplateMetadataTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
     DashboardAttributesTypeDef,
     DashboardOptionsTypeDef,
     DedicatedIpPoolTypeDef,
     DedicatedIpTypeDef,
@@ -391,36 +392,40 @@
     SuppressionAttributesTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
     GetContactListRequestRequestTypeDef,
     GetContactRequestRequestTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
+    GetEmailIdentityPoliciesResponseTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
     GuardianAttributesTypeDef,
     GuardianOptionsTypeDef,
     IdentityInfoTypeDef,
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
+    ListConfigurationSetsResponseTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
     ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListEmailTemplatesRequestRequestTypeDef,
     ListImportJobsRequestRequestTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsRequestRequestTypeDef,
@@ -434,40 +439,36 @@
     PutAccountSuppressionAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
     PutConfigurationSetSendingOptionsRequestRequestTypeDef,
     PutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
+    PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
+    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     PutSuppressedDestinationRequestRequestTypeDef,
     ReplacementTemplateTypeDef,
+    ResponseMetadataTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
     SuppressedDestinationAttributesTypeDef,
     TestRenderEmailTemplateRequestRequestTypeDef,
+    TestRenderEmailTemplateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     UpdateEmailIdentityPolicyRequestRequestTypeDef,
     AccountDetailsTypeDef,
     BatchGetMetricDataRequestRequestTypeDef,
     BatchGetMetricDataResponseTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
-    CreateImportJobResponseTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
-    GetEmailIdentityPoliciesResponseTypeDef,
-    ListConfigurationSetsResponseTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
-    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
-    TestRenderEmailTemplateResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
@@ -545,42 +546,42 @@
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

### Comparing `mypy-boto3-sesv2-1.26.88/README.md` & `mypy-boto3-sesv2-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sesv2"></a>
 
 # mypy-boto3-sesv2
 
 [![PyPI - mypy-boto3-sesv2](https://img.shields.io/pypi/v/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sesv2?color=blue)](https://pypistats.org/packages/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,15 +301,14 @@
 
 ```python
 from mypy_boto3_sesv2.type_defs import (
     ReviewDetailsTypeDef,
     BatchGetMetricDataQueryTypeDef,
     MetricDataErrorTypeDef,
     MetricDataResultTypeDef,
-    ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
@@ -320,19 +319,21 @@
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
     DkimSigningAttributesTypeDef,
     DkimAttributesTypeDef,
     EmailTemplateContentTypeDef,
     ImportDataSourceTypeDef,
+    CreateImportJobResponseTypeDef,
     CustomVerificationEmailTemplateMetadataTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
     DashboardAttributesTypeDef,
     DashboardOptionsTypeDef,
     DedicatedIpPoolTypeDef,
     DedicatedIpTypeDef,
@@ -359,36 +360,40 @@
     SuppressionAttributesTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
     GetContactListRequestRequestTypeDef,
     GetContactRequestRequestTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
+    GetEmailIdentityPoliciesResponseTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
     GuardianAttributesTypeDef,
     GuardianOptionsTypeDef,
     IdentityInfoTypeDef,
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
+    ListConfigurationSetsResponseTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
     ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListEmailTemplatesRequestRequestTypeDef,
     ListImportJobsRequestRequestTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsRequestRequestTypeDef,
@@ -402,40 +407,36 @@
     PutAccountSuppressionAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
     PutConfigurationSetSendingOptionsRequestRequestTypeDef,
     PutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
+    PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
+    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     PutSuppressedDestinationRequestRequestTypeDef,
     ReplacementTemplateTypeDef,
+    ResponseMetadataTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
     SuppressedDestinationAttributesTypeDef,
     TestRenderEmailTemplateRequestRequestTypeDef,
+    TestRenderEmailTemplateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     UpdateEmailIdentityPolicyRequestRequestTypeDef,
     AccountDetailsTypeDef,
     BatchGetMetricDataRequestRequestTypeDef,
     BatchGetMetricDataResponseTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
-    CreateImportJobResponseTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
-    GetEmailIdentityPoliciesResponseTypeDef,
-    ListConfigurationSetsResponseTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
-    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
-    TestRenderEmailTemplateResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
@@ -513,42 +514,42 @@
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

### Comparing `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/__main__.py` & `mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SESV2 1.26.88\nVersion:         1.26.88\nBuilder version:"
-        " 7.12.5\nDocs:           "
+        "Type annotations for boto3.SESV2 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.88")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/client.py` & `mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -902,14 +902,24 @@
         """
         Move a dedicated IP address to an existing dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_in_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_in_pool)
         """
 
+    def put_dedicated_ip_pool_scaling_attributes(
+        self, *, PoolName: str, ScalingMode: ScalingModeType
+    ) -> Dict[str, Any]:
+        """
+        Used to convert a dedicated IP pool to a different scaling mode.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_pool_scaling_attributes)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_pool_scaling_attributes)
+        """
+
     def put_dedicated_ip_warmup_attributes(
         self, *, Ip: str, WarmupPercentage: int
     ) -> Dict[str, Any]:
         """
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/sesv2-2019-09-27/PutDedicatedIpWarmupAttributes).
```

### Comparing `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/client.pyi` & `mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -829,14 +829,23 @@
     def put_dedicated_ip_in_pool(self, *, Ip: str, DestinationPoolName: str) -> Dict[str, Any]:
         """
         Move a dedicated IP address to an existing dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_in_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_in_pool)
         """
+    def put_dedicated_ip_pool_scaling_attributes(
+        self, *, PoolName: str, ScalingMode: ScalingModeType
+    ) -> Dict[str, Any]:
+        """
+        Used to convert a dedicated IP pool to a different scaling mode.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_pool_scaling_attributes)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_pool_scaling_attributes)
+        """
     def put_dedicated_ip_warmup_attributes(
         self, *, Ip: str, WarmupPercentage: int
     ) -> Dict[str, Any]:
         """
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/sesv2-2019-09-27/PutDedicatedIpWarmupAttributes).
```

### Comparing `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/literals.py` & `mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
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
@@ -191,14 +192,15 @@
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
@@ -296,14 +298,15 @@
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
@@ -339,14 +342,15 @@
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
@@ -365,16 +369,19 @@
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
@@ -458,15 +465,17 @@
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

### Comparing `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/literals.pyi` & `mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,15 @@
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
@@ -189,14 +190,15 @@
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
@@ -294,14 +296,15 @@
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
@@ -337,14 +340,15 @@
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
@@ -363,16 +367,19 @@
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
@@ -456,15 +463,17 @@
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

### Comparing `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/type_defs.py` & `mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 
 
 __all__ = (
     "ReviewDetailsTypeDef",
     "BatchGetMetricDataQueryTypeDef",
     "MetricDataErrorTypeDef",
     "MetricDataResultTypeDef",
-    "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
     "ContentTypeDef",
     "TemplateTypeDef",
     "BulkEmailEntryResultTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
@@ -83,19 +82,21 @@
     "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "SuppressionOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "TopicTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
+    "CreateDeliverabilityTestReportResponseTypeDef",
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     "DkimSigningAttributesTypeDef",
     "DkimAttributesTypeDef",
     "EmailTemplateContentTypeDef",
     "ImportDataSourceTypeDef",
+    "CreateImportJobResponseTypeDef",
     "CustomVerificationEmailTemplateMetadataTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
     "DashboardAttributesTypeDef",
     "DashboardOptionsTypeDef",
     "DedicatedIpPoolTypeDef",
     "DedicatedIpTypeDef",
@@ -122,36 +123,40 @@
     "SuppressionAttributesTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
     "GetContactListRequestRequestTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
+    "GetEmailIdentityPoliciesResponseTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "GetEmailTemplateRequestRequestTypeDef",
     "GetImportJobRequestRequestTypeDef",
     "GetSuppressedDestinationRequestRequestTypeDef",
     "GuardianAttributesTypeDef",
     "GuardianOptionsTypeDef",
     "IdentityInfoTypeDef",
     "SuppressionListDestinationTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
     "ListContactListsRequestRequestTypeDef",
     "TopicFilterTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
+    "ListDedicatedIpPoolsResponseTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListEmailTemplatesRequestRequestTypeDef",
     "ListImportJobsRequestRequestTypeDef",
     "ListManagementOptionsTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
@@ -165,40 +170,36 @@
     "PutAccountSuppressionAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "PutConfigurationSetReputationOptionsRequestRequestTypeDef",
     "PutConfigurationSetSendingOptionsRequestRequestTypeDef",
     "PutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
+    "PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
+    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     "PutSuppressedDestinationRequestRequestTypeDef",
     "ReplacementTemplateTypeDef",
+    "ResponseMetadataTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
+    "SendCustomVerificationEmailResponseTypeDef",
+    "SendEmailResponseTypeDef",
     "SuppressedDestinationAttributesTypeDef",
     "TestRenderEmailTemplateRequestRequestTypeDef",
+    "TestRenderEmailTemplateResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "UpdateEmailIdentityPolicyRequestRequestTypeDef",
     "AccountDetailsTypeDef",
     "BatchGetMetricDataRequestRequestTypeDef",
     "BatchGetMetricDataResponseTypeDef",
-    "CreateDeliverabilityTestReportResponseTypeDef",
-    "CreateImportJobResponseTypeDef",
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
-    "GetEmailIdentityPoliciesResponseTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
-    "ListDedicatedIpPoolsResponseTypeDef",
-    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
-    "SendCustomVerificationEmailResponseTypeDef",
-    "SendEmailResponseTypeDef",
-    "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "BodyTypeDef",
     "BulkEmailContentTypeDef",
     "SendBulkEmailResponseTypeDef",
     "CloudWatchDestinationTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
@@ -318,25 +319,14 @@
         "Id": str,
         "Timestamps": List[datetime],
         "Values": List[int],
     },
     total=False,
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
 BlacklistEntryTypeDef = TypedDict(
     "BlacklistEntryTypeDef",
     {
         "RblName": str,
         "ListingTime": datetime,
         "Description": str,
     },
@@ -512,14 +502,23 @@
         "TemplateSubject": str,
         "TemplateContent": str,
         "SuccessRedirectionURL": str,
         "FailureRedirectionURL": str,
     },
 )
 
+CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    {
+        "ReportId": str,
+        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateEmailIdentityPolicyRequestRequestTypeDef = TypedDict(
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     {
         "EmailIdentity": str,
         "PolicyName": str,
         "Policy": str,
     },
@@ -563,14 +562,22 @@
     "ImportDataSourceTypeDef",
     {
         "S3Url": str,
         "DataFormat": DataFormatType,
     },
 )
 
+CreateImportJobResponseTypeDef = TypedDict(
+    "CreateImportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomVerificationEmailTemplateMetadataTypeDef = TypedDict(
     "CustomVerificationEmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "SuccessRedirectionURL": str,
@@ -868,14 +875,27 @@
 GetCustomVerificationEmailTemplateRequestRequestTypeDef = TypedDict(
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 
+GetCustomVerificationEmailTemplateResponseTypeDef = TypedDict(
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    {
+        "TemplateName": str,
+        "FromEmailAddress": str,
+        "TemplateSubject": str,
+        "TemplateContent": str,
+        "SuccessRedirectionURL": str,
+        "FailureRedirectionURL": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDedicatedIpPoolRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpPoolRequestRequestTypeDef",
     {
         "PoolName": str,
     },
 )
 
@@ -934,14 +954,22 @@
 GetEmailIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
+GetEmailIdentityPoliciesResponseTypeDef = TypedDict(
+    "GetEmailIdentityPoliciesResponseTypeDef",
+    {
+        "Policies": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetEmailIdentityRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
@@ -1014,14 +1042,23 @@
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
 ListContactListsRequestRequestTypeDef = TypedDict(
     "ListContactListsRequestRequestTypeDef",
     {
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
@@ -1050,14 +1087,23 @@
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
 ListDeliverabilityTestReportsRequestRequestTypeDef = TypedDict(
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -1353,14 +1399,22 @@
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
 
+PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef = TypedDict(
+    "PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef",
+    {
+        "PoolName": str,
+        "ScalingMode": ScalingModeType,
+    },
+)
+
 PutDedicatedIpWarmupAttributesRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     {
         "Ip": str,
         "WarmupPercentage": int,
     },
 )
@@ -1405,14 +1459,23 @@
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
 
+PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
+    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
+    {
+        "DkimStatus": DkimStatusType,
+        "DkimTokens": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
@@ -1466,14 +1529,25 @@
     "ReplacementTemplateTypeDef",
     {
         "ReplacementTemplateData": str,
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
 _RequiredSendCustomVerificationEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "EmailAddress": str,
         "TemplateName": str,
     },
 )
@@ -1489,14 +1563,30 @@
 class SendCustomVerificationEmailRequestRequestTypeDef(
     _RequiredSendCustomVerificationEmailRequestRequestTypeDef,
     _OptionalSendCustomVerificationEmailRequestRequestTypeDef,
 ):
     pass
 
 
+SendCustomVerificationEmailResponseTypeDef = TypedDict(
+    "SendCustomVerificationEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
 SuppressedDestinationAttributesTypeDef = TypedDict(
     "SuppressedDestinationAttributesTypeDef",
     {
         "MessageId": str,
         "FeedbackId": str,
     },
     total=False,
@@ -1506,14 +1596,22 @@
     "TestRenderEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
 
+TestRenderEmailTemplateResponseTypeDef = TypedDict(
+    "TestRenderEmailTemplateResponseTypeDef",
+    {
+        "RenderedTemplate": str,
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
@@ -1560,112 +1658,23 @@
 )
 
 BatchGetMetricDataResponseTypeDef = TypedDict(
     "BatchGetMetricDataResponseTypeDef",
     {
         "Results": List[MetricDataResultTypeDef],
         "Errors": List[MetricDataErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
-    "CreateDeliverabilityTestReportResponseTypeDef",
-    {
-        "ReportId": str,
-        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateImportJobResponseTypeDef = TypedDict(
-    "CreateImportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCustomVerificationEmailTemplateResponseTypeDef = TypedDict(
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
-    {
-        "TemplateName": str,
-        "FromEmailAddress": str,
-        "TemplateSubject": str,
-        "TemplateContent": str,
-        "SuccessRedirectionURL": str,
-        "FailureRedirectionURL": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetEmailIdentityPoliciesResponseTypeDef = TypedDict(
-    "GetEmailIdentityPoliciesResponseTypeDef",
-    {
-        "Policies": Dict[str, str],
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
-PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
-    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
-    {
-        "DkimStatus": DkimStatusType,
-        "DkimTokens": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendCustomVerificationEmailResponseTypeDef = TypedDict(
-    "SendCustomVerificationEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendEmailResponseTypeDef = TypedDict(
-    "SendEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestRenderEmailTemplateResponseTypeDef = TypedDict(
-    "TestRenderEmailTemplateResponseTypeDef",
-    {
-        "RenderedTemplate": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBlacklistReportsResponseTypeDef = TypedDict(
     "GetBlacklistReportsResponseTypeDef",
     {
         "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
@@ -1682,15 +1691,15 @@
     total=False,
 )
 
 SendBulkEmailResponseTypeDef = TypedDict(
     "SendBulkEmailResponseTypeDef",
     {
         "BulkEmailEntryResults": List[BulkEmailEntryResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
@@ -1698,15 +1707,15 @@
 )
 
 ListContactListsResponseTypeDef = TypedDict(
     "ListContactListsResponseTypeDef",
     {
         "ContactLists": List[ContactListTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "EmailAddress": str,
@@ -1749,15 +1758,15 @@
         "EmailAddress": str,
         "TopicPreferences": List[TopicPreferenceTypeDef],
         "TopicDefaultPreferences": List[TopicPreferenceTypeDef],
         "UnsubscribeAll": bool,
         "AttributesData": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactListName": str,
@@ -1804,15 +1813,15 @@
     pass
 
 
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
@@ -1848,15 +1857,15 @@
     {
         "ContactListName": str,
         "Topics": List[TopicTypeDef],
         "Description": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateContactListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
@@ -1927,15 +1936,15 @@
 
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
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
@@ -1944,15 +1953,15 @@
 )
 
 GetEmailTemplateResponseTypeDef = TypedDict(
     "GetEmailTemplateResponseTypeDef",
     {
         "TemplateName": str,
         "TemplateContent": EmailTemplateContentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailTemplateRequestRequestTypeDef = TypedDict(
     "UpdateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
@@ -1961,15 +1970,15 @@
 )
 
 ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     {
         "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DailyVolumeTypeDef = TypedDict(
     "DailyVolumeTypeDef",
     {
         "StartDate": datetime,
@@ -1989,58 +1998,58 @@
     total=False,
 )
 
 GetDedicatedIpPoolResponseTypeDef = TypedDict(
     "GetDedicatedIpPoolResponseTypeDef",
     {
         "DedicatedIpPool": DedicatedIpPoolTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
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
@@ -2051,15 +2060,15 @@
 )
 
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
@@ -2076,15 +2085,15 @@
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
         "Policies": Dict[str, str],
         "Tags": List[TagTypeDef],
         "ConfigurationSetName": str,
         "VerificationStatus": VerificationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredVdmAttributesTypeDef = TypedDict(
     "_RequiredVdmAttributesTypeDef",
     {
         "VdmEnabled": FeatureStatusType,
@@ -2114,15 +2123,15 @@
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
 
 ImportDestinationTypeDef = TypedDict(
     "ImportDestinationTypeDef",
     {
         "SuppressionListDestination": SuppressionListDestinationTypeDef,
@@ -2141,24 +2150,24 @@
 )
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSuppressedDestinationsResponseTypeDef = TypedDict(
     "ListSuppressedDestinationsResponseTypeDef",
     {
         "SuppressedDestinationSummaries": List[SuppressedDestinationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplacementEmailContentTypeDef = TypedDict(
     "ReplacementEmailContentTypeDef",
     {
         "ReplacementTemplate": ReplacementTemplateTypeDef,
@@ -2235,36 +2244,36 @@
 
 
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "Contacts": List[ContactTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
@@ -2290,30 +2299,30 @@
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
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "SuppressionAttributes": SuppressionAttributesTypeDef,
         "Details": AccountDetailsTypeDef,
         "VdmAttributes": VdmAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccountVdmAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountVdmAttributesRequestRequestTypeDef",
     {
         "VdmAttributes": VdmAttributesTypeDef,
@@ -2355,15 +2364,15 @@
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": List[TagTypeDef],
         "SuppressionOptions": SuppressionOptionsTypeDef,
         "VdmOptions": VdmOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
@@ -2401,15 +2410,15 @@
         "ImportDataSource": ImportDataSourceTypeDef,
         "FailureInfo": FailureInfoTypeDef,
         "JobStatus": JobStatusType,
         "CreatedTimestamp": datetime,
         "CompletedTimestamp": datetime,
         "ProcessedRecordsCount": int,
         "FailedRecordsCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportJobSummaryTypeDef = TypedDict(
     "ImportJobSummaryTypeDef",
     {
         "JobId": str,
@@ -2465,15 +2474,15 @@
     pass
 
 
 GetSuppressedDestinationResponseTypeDef = TypedDict(
     "GetSuppressedDestinationResponseTypeDef",
     {
         "SuppressedDestination": SuppressedDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
         "Simple": MessageTypeDef,
@@ -2501,24 +2510,24 @@
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
 
 ListImportJobsResponseTypeDef = TypedDict(
     "ListImportJobsResponseTypeDef",
     {
         "ImportJobs": List[ImportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSendBulkEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendBulkEmailRequestRequestTypeDef",
     {
         "DefaultContent": BulkEmailContentTypeDef,
```

### Comparing `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/type_defs.pyi` & `mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ReviewDetailsTypeDef",
     "BatchGetMetricDataQueryTypeDef",
     "MetricDataErrorTypeDef",
     "MetricDataResultTypeDef",
-    "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
     "ContentTypeDef",
     "TemplateTypeDef",
     "BulkEmailEntryResultTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
@@ -82,19 +81,21 @@
     "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "SuppressionOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "TopicTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
+    "CreateDeliverabilityTestReportResponseTypeDef",
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     "DkimSigningAttributesTypeDef",
     "DkimAttributesTypeDef",
     "EmailTemplateContentTypeDef",
     "ImportDataSourceTypeDef",
+    "CreateImportJobResponseTypeDef",
     "CustomVerificationEmailTemplateMetadataTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
     "DashboardAttributesTypeDef",
     "DashboardOptionsTypeDef",
     "DedicatedIpPoolTypeDef",
     "DedicatedIpTypeDef",
@@ -121,36 +122,40 @@
     "SuppressionAttributesTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
     "GetContactListRequestRequestTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
+    "GetEmailIdentityPoliciesResponseTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "GetEmailTemplateRequestRequestTypeDef",
     "GetImportJobRequestRequestTypeDef",
     "GetSuppressedDestinationRequestRequestTypeDef",
     "GuardianAttributesTypeDef",
     "GuardianOptionsTypeDef",
     "IdentityInfoTypeDef",
     "SuppressionListDestinationTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
     "ListContactListsRequestRequestTypeDef",
     "TopicFilterTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
+    "ListDedicatedIpPoolsResponseTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListEmailTemplatesRequestRequestTypeDef",
     "ListImportJobsRequestRequestTypeDef",
     "ListManagementOptionsTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
@@ -164,40 +169,36 @@
     "PutAccountSuppressionAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "PutConfigurationSetReputationOptionsRequestRequestTypeDef",
     "PutConfigurationSetSendingOptionsRequestRequestTypeDef",
     "PutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
+    "PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
+    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     "PutSuppressedDestinationRequestRequestTypeDef",
     "ReplacementTemplateTypeDef",
+    "ResponseMetadataTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
+    "SendCustomVerificationEmailResponseTypeDef",
+    "SendEmailResponseTypeDef",
     "SuppressedDestinationAttributesTypeDef",
     "TestRenderEmailTemplateRequestRequestTypeDef",
+    "TestRenderEmailTemplateResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "UpdateEmailIdentityPolicyRequestRequestTypeDef",
     "AccountDetailsTypeDef",
     "BatchGetMetricDataRequestRequestTypeDef",
     "BatchGetMetricDataResponseTypeDef",
-    "CreateDeliverabilityTestReportResponseTypeDef",
-    "CreateImportJobResponseTypeDef",
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
-    "GetEmailIdentityPoliciesResponseTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
-    "ListDedicatedIpPoolsResponseTypeDef",
-    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
-    "SendCustomVerificationEmailResponseTypeDef",
-    "SendEmailResponseTypeDef",
-    "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "BodyTypeDef",
     "BulkEmailContentTypeDef",
     "SendBulkEmailResponseTypeDef",
     "CloudWatchDestinationTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
@@ -315,25 +316,14 @@
         "Id": str,
         "Timestamps": List[datetime],
         "Values": List[int],
     },
     total=False,
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
 BlacklistEntryTypeDef = TypedDict(
     "BlacklistEntryTypeDef",
     {
         "RblName": str,
         "ListingTime": datetime,
         "Description": str,
     },
@@ -505,14 +495,23 @@
         "TemplateSubject": str,
         "TemplateContent": str,
         "SuccessRedirectionURL": str,
         "FailureRedirectionURL": str,
     },
 )
 
+CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    {
+        "ReportId": str,
+        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateEmailIdentityPolicyRequestRequestTypeDef = TypedDict(
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     {
         "EmailIdentity": str,
         "PolicyName": str,
         "Policy": str,
     },
@@ -556,14 +555,22 @@
     "ImportDataSourceTypeDef",
     {
         "S3Url": str,
         "DataFormat": DataFormatType,
     },
 )
 
+CreateImportJobResponseTypeDef = TypedDict(
+    "CreateImportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomVerificationEmailTemplateMetadataTypeDef = TypedDict(
     "CustomVerificationEmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "SuccessRedirectionURL": str,
@@ -859,14 +866,27 @@
 GetCustomVerificationEmailTemplateRequestRequestTypeDef = TypedDict(
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 
+GetCustomVerificationEmailTemplateResponseTypeDef = TypedDict(
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    {
+        "TemplateName": str,
+        "FromEmailAddress": str,
+        "TemplateSubject": str,
+        "TemplateContent": str,
+        "SuccessRedirectionURL": str,
+        "FailureRedirectionURL": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDedicatedIpPoolRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpPoolRequestRequestTypeDef",
     {
         "PoolName": str,
     },
 )
 
@@ -925,14 +945,22 @@
 GetEmailIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
+GetEmailIdentityPoliciesResponseTypeDef = TypedDict(
+    "GetEmailIdentityPoliciesResponseTypeDef",
+    {
+        "Policies": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetEmailIdentityRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
@@ -1005,14 +1033,23 @@
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
 ListContactListsRequestRequestTypeDef = TypedDict(
     "ListContactListsRequestRequestTypeDef",
     {
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
@@ -1041,14 +1078,23 @@
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
 ListDeliverabilityTestReportsRequestRequestTypeDef = TypedDict(
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -1328,14 +1374,22 @@
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
 
+PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef = TypedDict(
+    "PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef",
+    {
+        "PoolName": str,
+        "ScalingMode": ScalingModeType,
+    },
+)
+
 PutDedicatedIpWarmupAttributesRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     {
         "Ip": str,
         "WarmupPercentage": int,
     },
 )
@@ -1376,14 +1430,23 @@
 
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
+PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
+    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
+    {
+        "DkimStatus": DkimStatusType,
+        "DkimTokens": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
@@ -1433,14 +1496,25 @@
     "ReplacementTemplateTypeDef",
     {
         "ReplacementTemplateData": str,
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
 _RequiredSendCustomVerificationEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "EmailAddress": str,
         "TemplateName": str,
     },
 )
@@ -1454,14 +1528,30 @@
 
 class SendCustomVerificationEmailRequestRequestTypeDef(
     _RequiredSendCustomVerificationEmailRequestRequestTypeDef,
     _OptionalSendCustomVerificationEmailRequestRequestTypeDef,
 ):
     pass
 
+SendCustomVerificationEmailResponseTypeDef = TypedDict(
+    "SendCustomVerificationEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
 SuppressedDestinationAttributesTypeDef = TypedDict(
     "SuppressedDestinationAttributesTypeDef",
     {
         "MessageId": str,
         "FeedbackId": str,
     },
     total=False,
@@ -1471,14 +1561,22 @@
     "TestRenderEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
 
+TestRenderEmailTemplateResponseTypeDef = TypedDict(
+    "TestRenderEmailTemplateResponseTypeDef",
+    {
+        "RenderedTemplate": str,
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
@@ -1525,112 +1623,23 @@
 )
 
 BatchGetMetricDataResponseTypeDef = TypedDict(
     "BatchGetMetricDataResponseTypeDef",
     {
         "Results": List[MetricDataResultTypeDef],
         "Errors": List[MetricDataErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
-    "CreateDeliverabilityTestReportResponseTypeDef",
-    {
-        "ReportId": str,
-        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateImportJobResponseTypeDef = TypedDict(
-    "CreateImportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCustomVerificationEmailTemplateResponseTypeDef = TypedDict(
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
-    {
-        "TemplateName": str,
-        "FromEmailAddress": str,
-        "TemplateSubject": str,
-        "TemplateContent": str,
-        "SuccessRedirectionURL": str,
-        "FailureRedirectionURL": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetEmailIdentityPoliciesResponseTypeDef = TypedDict(
-    "GetEmailIdentityPoliciesResponseTypeDef",
-    {
-        "Policies": Dict[str, str],
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
-PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
-    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
-    {
-        "DkimStatus": DkimStatusType,
-        "DkimTokens": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendCustomVerificationEmailResponseTypeDef = TypedDict(
-    "SendCustomVerificationEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendEmailResponseTypeDef = TypedDict(
-    "SendEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestRenderEmailTemplateResponseTypeDef = TypedDict(
-    "TestRenderEmailTemplateResponseTypeDef",
-    {
-        "RenderedTemplate": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBlacklistReportsResponseTypeDef = TypedDict(
     "GetBlacklistReportsResponseTypeDef",
     {
         "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
@@ -1647,15 +1656,15 @@
     total=False,
 )
 
 SendBulkEmailResponseTypeDef = TypedDict(
     "SendBulkEmailResponseTypeDef",
     {
         "BulkEmailEntryResults": List[BulkEmailEntryResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
@@ -1663,15 +1672,15 @@
 )
 
 ListContactListsResponseTypeDef = TypedDict(
     "ListContactListsResponseTypeDef",
     {
         "ContactLists": List[ContactListTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "EmailAddress": str,
@@ -1712,15 +1721,15 @@
         "EmailAddress": str,
         "TopicPreferences": List[TopicPreferenceTypeDef],
         "TopicDefaultPreferences": List[TopicPreferenceTypeDef],
         "UnsubscribeAll": bool,
         "AttributesData": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactListName": str,
@@ -1763,15 +1772,15 @@
 ):
     pass
 
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
@@ -1805,15 +1814,15 @@
     {
         "ContactListName": str,
         "Topics": List[TopicTypeDef],
         "Description": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateContactListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
@@ -1878,15 +1887,15 @@
 
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
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
@@ -1895,15 +1904,15 @@
 )
 
 GetEmailTemplateResponseTypeDef = TypedDict(
     "GetEmailTemplateResponseTypeDef",
     {
         "TemplateName": str,
         "TemplateContent": EmailTemplateContentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailTemplateRequestRequestTypeDef = TypedDict(
     "UpdateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
@@ -1912,15 +1921,15 @@
 )
 
 ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     {
         "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DailyVolumeTypeDef = TypedDict(
     "DailyVolumeTypeDef",
     {
         "StartDate": datetime,
@@ -1940,58 +1949,58 @@
     total=False,
 )
 
 GetDedicatedIpPoolResponseTypeDef = TypedDict(
     "GetDedicatedIpPoolResponseTypeDef",
     {
         "DedicatedIpPool": DedicatedIpPoolTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
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
@@ -2002,15 +2011,15 @@
 )
 
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
@@ -2027,15 +2036,15 @@
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
         "Policies": Dict[str, str],
         "Tags": List[TagTypeDef],
         "ConfigurationSetName": str,
         "VerificationStatus": VerificationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredVdmAttributesTypeDef = TypedDict(
     "_RequiredVdmAttributesTypeDef",
     {
         "VdmEnabled": FeatureStatusType,
@@ -2063,15 +2072,15 @@
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
 
 ImportDestinationTypeDef = TypedDict(
     "ImportDestinationTypeDef",
     {
         "SuppressionListDestination": SuppressionListDestinationTypeDef,
@@ -2090,24 +2099,24 @@
 )
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSuppressedDestinationsResponseTypeDef = TypedDict(
     "ListSuppressedDestinationsResponseTypeDef",
     {
         "SuppressedDestinationSummaries": List[SuppressedDestinationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplacementEmailContentTypeDef = TypedDict(
     "ReplacementEmailContentTypeDef",
     {
         "ReplacementTemplate": ReplacementTemplateTypeDef,
@@ -2180,36 +2189,36 @@
     pass
 
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "Contacts": List[ContactTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
@@ -2233,30 +2242,30 @@
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
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "SuppressionAttributes": SuppressionAttributesTypeDef,
         "Details": AccountDetailsTypeDef,
         "VdmAttributes": VdmAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccountVdmAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountVdmAttributesRequestRequestTypeDef",
     {
         "VdmAttributes": VdmAttributesTypeDef,
@@ -2296,15 +2305,15 @@
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": List[TagTypeDef],
         "SuppressionOptions": SuppressionOptionsTypeDef,
         "VdmOptions": VdmOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
@@ -2340,15 +2349,15 @@
         "ImportDataSource": ImportDataSourceTypeDef,
         "FailureInfo": FailureInfoTypeDef,
         "JobStatus": JobStatusType,
         "CreatedTimestamp": datetime,
         "CompletedTimestamp": datetime,
         "ProcessedRecordsCount": int,
         "FailedRecordsCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportJobSummaryTypeDef = TypedDict(
     "ImportJobSummaryTypeDef",
     {
         "JobId": str,
@@ -2400,15 +2409,15 @@
 class BulkEmailEntryTypeDef(_RequiredBulkEmailEntryTypeDef, _OptionalBulkEmailEntryTypeDef):
     pass
 
 GetSuppressedDestinationResponseTypeDef = TypedDict(
     "GetSuppressedDestinationResponseTypeDef",
     {
         "SuppressedDestination": SuppressedDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
         "Simple": MessageTypeDef,
@@ -2436,24 +2445,24 @@
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
 
 ListImportJobsResponseTypeDef = TypedDict(
     "ListImportJobsResponseTypeDef",
     {
         "ImportJobs": List[ImportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSendBulkEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendBulkEmailRequestRequestTypeDef",
     {
         "DefaultContent": BulkEmailContentTypeDef,
```

### Comparing `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/PKG-INFO` & `mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.26.88
-Summary: Type annotations for boto3.SESV2 1.26.88 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.SESV2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sesv2"></a>
 
 # mypy-boto3-sesv2
 
 [![PyPI - mypy-boto3-sesv2](https://img.shields.io/pypi/v/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sesv2?color=blue)](https://pypistats.org/packages/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,15 +333,14 @@
 
 ```python
 from mypy_boto3_sesv2.type_defs import (
     ReviewDetailsTypeDef,
     BatchGetMetricDataQueryTypeDef,
     MetricDataErrorTypeDef,
     MetricDataResultTypeDef,
-    ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
@@ -352,19 +351,21 @@
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
     DkimSigningAttributesTypeDef,
     DkimAttributesTypeDef,
     EmailTemplateContentTypeDef,
     ImportDataSourceTypeDef,
+    CreateImportJobResponseTypeDef,
     CustomVerificationEmailTemplateMetadataTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
     DashboardAttributesTypeDef,
     DashboardOptionsTypeDef,
     DedicatedIpPoolTypeDef,
     DedicatedIpTypeDef,
@@ -391,36 +392,40 @@
     SuppressionAttributesTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
     GetContactListRequestRequestTypeDef,
     GetContactRequestRequestTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
+    GetEmailIdentityPoliciesResponseTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
     GuardianAttributesTypeDef,
     GuardianOptionsTypeDef,
     IdentityInfoTypeDef,
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
+    ListConfigurationSetsResponseTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
     ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListEmailTemplatesRequestRequestTypeDef,
     ListImportJobsRequestRequestTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsRequestRequestTypeDef,
@@ -434,40 +439,36 @@
     PutAccountSuppressionAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
     PutConfigurationSetSendingOptionsRequestRequestTypeDef,
     PutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
+    PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
+    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     PutSuppressedDestinationRequestRequestTypeDef,
     ReplacementTemplateTypeDef,
+    ResponseMetadataTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
     SuppressedDestinationAttributesTypeDef,
     TestRenderEmailTemplateRequestRequestTypeDef,
+    TestRenderEmailTemplateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     UpdateEmailIdentityPolicyRequestRequestTypeDef,
     AccountDetailsTypeDef,
     BatchGetMetricDataRequestRequestTypeDef,
     BatchGetMetricDataResponseTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
-    CreateImportJobResponseTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
-    GetEmailIdentityPoliciesResponseTypeDef,
-    ListConfigurationSetsResponseTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
-    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
-    TestRenderEmailTemplateResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
@@ -545,42 +546,42 @@
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

### Comparing `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/SOURCES.txt` & `mypy-boto3-sesv2-1.27.0/mypy_boto3_sesv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.26.88/setup.py` & `mypy-boto3-sesv2-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-sesv2.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sesv2",
-    version="1.26.88",
+    version="1.27.0",
     packages=["mypy_boto3_sesv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SESV2 1.26.88 service generated with mypy-boto3-builder 7.12.5"
+        "Type annotations for boto3.SESV2 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/",
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


# Comparing `tmp/mypy-boto3-ses-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-ses-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ses-1.26.0.post1.tar", last modified: Tue Nov  1 21:44:00 2022, max compression
+gzip compressed data, was "mypy-boto3-ses-1.27.0.tar", last modified: Mon Jul  3 19:51:27 2023, max compression
```

## Comparing `mypy-boto3-ses-1.26.0.post1.tar` & `mypy-boto3-ses-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:00.476850 mypy-boto3-ses-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    20413 2022-11-01 21:44:00.468850 mypy-boto3-ses-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18988 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:00.468850 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/
--rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    49195 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    49111 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10156 2022-11-01 21:41:22.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10154 2022-11-01 21:41:22.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6246 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6239 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    47902 2022-11-01 21:41:22.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    47839 2022-11-01 21:41:22.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:00.468850 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    20413 2022-11-01 21:44:00.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-11-01 21:44:00.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:00.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:00.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:44:00.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-01 21:44:00.000000 mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:44:00.476850 mypy-boto3-ses-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-11-01 21:41:21.000000 mypy-boto3-ses-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:27.664002 mypy-boto3-ses-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:04.000000 mypy-boto3-ses-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20431 2023-07-03 19:51:27.664002 mypy-boto3-ses-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-07-03 19:48:04.000000 mypy-boto3-ses-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:27.664002 mypy-boto3-ses-1.27.0/mypy_boto3_ses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-03 19:48:04.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-03 19:48:04.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:48:04.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49195 2023-07-03 19:48:05.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49111 2023-07-03 19:48:05.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-07-03 19:48:05.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-03 19:48:05.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-07-03 19:48:05.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-03 19:48:05.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:04.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47976 2023-07-03 19:48:06.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47913 2023-07-03 19:48:05.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:04.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-03 19:48:05.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-03 19:48:05.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:27.664002 mypy-boto3-ses-1.27.0/mypy_boto3_ses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20431 2023-07-03 19:51:27.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 19:51:27.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:27.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:27.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:27.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:27.000000 mypy-boto3-ses-1.27.0/mypy_boto3_ses.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:27.664002 mypy-boto3-ses-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:48:04.000000 mypy-boto3-ses-1.27.0/setup.py
```

### Comparing `mypy-boto3-ses-1.26.0.post1/LICENSE` & `mypy-boto3-ses-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-ses-1.26.0.post1/PKG-INFO` & `mypy-boto3-ses-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ses
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SES 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SES 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/
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
 
 <a id="mypy-boto3-ses"></a>
 
 # mypy-boto3-ses
 
 [![PyPI - mypy-boto3-ses](https://img.shields.io/pypi/v/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ses?color=blue)](https://pypistats.org/packages/mypy-boto3-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SES 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[boto3.SES 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
 See how it helps to find and fix potential bugs:
 
@@ -401,113 +402,113 @@
     DeleteReceiptFilterRequestRequestTypeDef,
     DeleteReceiptRuleRequestRequestTypeDef,
     DeleteReceiptRuleSetRequestRequestTypeDef,
     DeleteTemplateRequestRequestTypeDef,
     DeleteVerifiedEmailAddressRequestRequestTypeDef,
     DeliveryOptionsTypeDef,
     ReceiptRuleSetMetadataTypeDef,
-    ResponseMetadataTypeDef,
     DescribeConfigurationSetRequestRequestTypeDef,
     ReputationOptionsTypeDef,
     DescribeReceiptRuleRequestRequestTypeDef,
     DescribeReceiptRuleSetRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SNSDestinationTypeDef,
     ExtensionFieldTypeDef,
+    GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesRequestRequestTypeDef,
     IdentityDkimAttributesTypeDef,
     GetIdentityMailFromDomainAttributesRequestRequestTypeDef,
     IdentityMailFromDomainAttributesTypeDef,
     GetIdentityNotificationAttributesRequestRequestTypeDef,
     IdentityNotificationAttributesTypeDef,
     GetIdentityPoliciesRequestRequestTypeDef,
+    GetIdentityPoliciesResponseTypeDef,
     WaiterConfigTypeDef,
     GetIdentityVerificationAttributesRequestRequestTypeDef,
     IdentityVerificationAttributesTypeDef,
+    GetSendQuotaResponseTypeDef,
     SendDataPointTypeDef,
     GetTemplateRequestRequestTypeDef,
     LambdaActionTypeDef,
-    PaginatorConfigTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
+    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
+    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListIdentitiesRequestRequestTypeDef,
+    ListIdentitiesResponseTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
+    ListIdentityPoliciesResponseTypeDef,
+    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
+    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
+    ListVerifiedEmailAddressesResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
     RawMessageTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    SendBounceResponseTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    SendRawEmailResponseTypeDef,
+    SendTemplatedEmailResponseTypeDef,
     SetActiveReceiptRuleSetRequestRequestTypeDef,
     SetIdentityDkimEnabledRequestRequestTypeDef,
     SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef,
     SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef,
     SetIdentityMailFromDomainRequestRequestTypeDef,
     SetIdentityNotificationTopicRequestRequestTypeDef,
     SetReceiptRulePositionRequestRequestTypeDef,
     TestRenderTemplateRequestRequestTypeDef,
+    TestRenderTemplateResponseTypeDef,
     UpdateAccountSendingEnabledRequestRequestTypeDef,
     UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef,
     UpdateConfigurationSetSendingEnabledRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     VerifyDomainDkimRequestRequestTypeDef,
+    VerifyDomainDkimResponseTypeDef,
     VerifyDomainIdentityRequestRequestTypeDef,
+    VerifyDomainIdentityResponseTypeDef,
     VerifyEmailAddressRequestRequestTypeDef,
     VerifyEmailIdentityRequestRequestTypeDef,
     BodyTypeDef,
+    SendBulkTemplatedEmailResponseTypeDef,
     BulkEmailDestinationTypeDef,
     SendTemplatedEmailRequestRequestTypeDef,
     CloudWatchDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
+    ListConfigurationSetsResponseTypeDef,
     CreateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    UpdateTemplateRequestRequestTypeDef,
-    PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAccountSendingEnabledResponseTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
-    GetIdentityPoliciesResponseTypeDef,
-    GetSendQuotaResponseTypeDef,
     GetTemplateResponseTypeDef,
-    ListConfigurationSetsResponseTypeDef,
+    UpdateTemplateRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesResponseTypeDef,
-    ListIdentitiesResponseTypeDef,
-    ListIdentityPoliciesResponseTypeDef,
+    PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     ListReceiptRuleSetsResponseTypeDef,
-    ListVerifiedEmailAddressesResponseTypeDef,
-    SendBounceResponseTypeDef,
-    SendBulkTemplatedEmailResponseTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
-    SendRawEmailResponseTypeDef,
-    SendTemplatedEmailResponseTypeDef,
-    TestRenderTemplateResponseTypeDef,
-    VerifyDomainDkimResponseTypeDef,
-    VerifyDomainIdentityResponseTypeDef,
     MessageDsnTypeDef,
     RecipientDsnFieldsTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
-    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
-    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
-    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
-    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
     SendRawEmailRequestRequestTypeDef,
     ReceiptActionTypeDef,
     ReceiptFilterTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
     EventDestinationTypeDef,
@@ -535,42 +536,42 @@
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

### Comparing `mypy-boto3-ses-1.26.0.post1/README.md` & `mypy-boto3-ses-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ses"></a>
 
 # mypy-boto3-ses
 
 [![PyPI - mypy-boto3-ses](https://img.shields.io/pypi/v/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ses?color=blue)](https://pypistats.org/packages/mypy-boto3-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SES 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[boto3.SES 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
 See how it helps to find and fix potential bugs:
 
@@ -370,113 +370,113 @@
     DeleteReceiptFilterRequestRequestTypeDef,
     DeleteReceiptRuleRequestRequestTypeDef,
     DeleteReceiptRuleSetRequestRequestTypeDef,
     DeleteTemplateRequestRequestTypeDef,
     DeleteVerifiedEmailAddressRequestRequestTypeDef,
     DeliveryOptionsTypeDef,
     ReceiptRuleSetMetadataTypeDef,
-    ResponseMetadataTypeDef,
     DescribeConfigurationSetRequestRequestTypeDef,
     ReputationOptionsTypeDef,
     DescribeReceiptRuleRequestRequestTypeDef,
     DescribeReceiptRuleSetRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SNSDestinationTypeDef,
     ExtensionFieldTypeDef,
+    GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesRequestRequestTypeDef,
     IdentityDkimAttributesTypeDef,
     GetIdentityMailFromDomainAttributesRequestRequestTypeDef,
     IdentityMailFromDomainAttributesTypeDef,
     GetIdentityNotificationAttributesRequestRequestTypeDef,
     IdentityNotificationAttributesTypeDef,
     GetIdentityPoliciesRequestRequestTypeDef,
+    GetIdentityPoliciesResponseTypeDef,
     WaiterConfigTypeDef,
     GetIdentityVerificationAttributesRequestRequestTypeDef,
     IdentityVerificationAttributesTypeDef,
+    GetSendQuotaResponseTypeDef,
     SendDataPointTypeDef,
     GetTemplateRequestRequestTypeDef,
     LambdaActionTypeDef,
-    PaginatorConfigTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
+    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
+    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListIdentitiesRequestRequestTypeDef,
+    ListIdentitiesResponseTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
+    ListIdentityPoliciesResponseTypeDef,
+    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
+    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
+    ListVerifiedEmailAddressesResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
     RawMessageTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    SendBounceResponseTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    SendRawEmailResponseTypeDef,
+    SendTemplatedEmailResponseTypeDef,
     SetActiveReceiptRuleSetRequestRequestTypeDef,
     SetIdentityDkimEnabledRequestRequestTypeDef,
     SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef,
     SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef,
     SetIdentityMailFromDomainRequestRequestTypeDef,
     SetIdentityNotificationTopicRequestRequestTypeDef,
     SetReceiptRulePositionRequestRequestTypeDef,
     TestRenderTemplateRequestRequestTypeDef,
+    TestRenderTemplateResponseTypeDef,
     UpdateAccountSendingEnabledRequestRequestTypeDef,
     UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef,
     UpdateConfigurationSetSendingEnabledRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     VerifyDomainDkimRequestRequestTypeDef,
+    VerifyDomainDkimResponseTypeDef,
     VerifyDomainIdentityRequestRequestTypeDef,
+    VerifyDomainIdentityResponseTypeDef,
     VerifyEmailAddressRequestRequestTypeDef,
     VerifyEmailIdentityRequestRequestTypeDef,
     BodyTypeDef,
+    SendBulkTemplatedEmailResponseTypeDef,
     BulkEmailDestinationTypeDef,
     SendTemplatedEmailRequestRequestTypeDef,
     CloudWatchDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
+    ListConfigurationSetsResponseTypeDef,
     CreateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    UpdateTemplateRequestRequestTypeDef,
-    PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAccountSendingEnabledResponseTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
-    GetIdentityPoliciesResponseTypeDef,
-    GetSendQuotaResponseTypeDef,
     GetTemplateResponseTypeDef,
-    ListConfigurationSetsResponseTypeDef,
+    UpdateTemplateRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesResponseTypeDef,
-    ListIdentitiesResponseTypeDef,
-    ListIdentityPoliciesResponseTypeDef,
+    PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     ListReceiptRuleSetsResponseTypeDef,
-    ListVerifiedEmailAddressesResponseTypeDef,
-    SendBounceResponseTypeDef,
-    SendBulkTemplatedEmailResponseTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
-    SendRawEmailResponseTypeDef,
-    SendTemplatedEmailResponseTypeDef,
-    TestRenderTemplateResponseTypeDef,
-    VerifyDomainDkimResponseTypeDef,
-    VerifyDomainIdentityResponseTypeDef,
     MessageDsnTypeDef,
     RecipientDsnFieldsTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
-    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
-    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
-    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
-    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
     SendRawEmailRequestRequestTypeDef,
     ReceiptActionTypeDef,
     ReceiptFilterTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
     EventDestinationTypeDef,
@@ -504,42 +504,42 @@
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

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/__init__.py` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/__init__.pyi` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/__main__.py` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SES 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.SES 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES\nOther"
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

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/client.py` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/client.pyi` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/literals.py` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BehaviorOnMXFailureType",
     "BounceTypeType",
     "BulkEmailStatusType",
     "ConfigurationSetAttributeType",
     "CustomMailFromStatusType",
     "DimensionValueSourceType",
@@ -46,15 +45,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 BehaviorOnMXFailureType = Literal["RejectMessage", "UseDefaultValue"]
 BounceTypeType = Literal[
     "ContentRejected",
     "DoesNotExist",
     "ExceededQuota",
     "MessageTooLarge",
     "TemporaryFailure",
@@ -113,23 +111,25 @@
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
@@ -139,30 +139,35 @@
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
@@ -188,14 +193,15 @@
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
@@ -240,51 +246,57 @@
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
@@ -297,14 +309,15 @@
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
@@ -316,28 +329,35 @@
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
@@ -346,14 +366,15 @@
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
@@ -364,55 +385,64 @@
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
@@ -446,14 +476,15 @@
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

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/literals.pyi` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "BehaviorOnMXFailureType",
     "BounceTypeType",
     "BulkEmailStatusType",
     "ConfigurationSetAttributeType",
     "CustomMailFromStatusType",
     "DimensionValueSourceType",
@@ -45,14 +46,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 BehaviorOnMXFailureType = Literal["RejectMessage", "UseDefaultValue"]
 BounceTypeType = Literal[
     "ContentRejected",
     "DoesNotExist",
     "ExceededQuota",
     "MessageTooLarge",
     "TemporaryFailure",
@@ -111,23 +113,25 @@
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
@@ -137,30 +141,35 @@
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
@@ -186,14 +195,15 @@
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
@@ -238,51 +248,57 @@
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
@@ -295,14 +311,15 @@
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
@@ -314,28 +331,35 @@
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
@@ -344,14 +368,15 @@
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
@@ -362,55 +387,64 @@
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
@@ -444,14 +478,15 @@
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

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/paginator.py` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,30 +63,30 @@
 class ListConfigurationSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listconfigurationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfigurationSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listconfigurationsetspaginator)
         """
 
 
 class ListCustomVerificationEmailTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listcustomverificationemailtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomVerificationEmailTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listcustomverificationemailtemplatespaginator)
         """
 
 
@@ -96,43 +96,43 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listidentitiespaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityType: IdentityTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIdentitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listidentitiespaginator)
         """
 
 
 class ListReceiptRuleSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listreceiptrulesetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReceiptRuleSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listreceiptrulesetspaginator)
         """
 
 
 class ListTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listtemplatespaginator)
         """
```

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/paginator.pyi` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,29 +60,29 @@
 class ListConfigurationSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listconfigurationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfigurationSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listconfigurationsetspaginator)
         """
 
 class ListCustomVerificationEmailTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listcustomverificationemailtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomVerificationEmailTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listcustomverificationemailtemplatespaginator)
         """
 
 class ListIdentitiesPaginator(Paginator):
@@ -91,41 +91,41 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listidentitiespaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityType: IdentityTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIdentitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listidentitiespaginator)
         """
 
 class ListReceiptRuleSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listreceiptrulesetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReceiptRuleSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listreceiptrulesetspaginator)
         """
 
 class ListTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listtemplatespaginator)
         """
```

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/type_defs.py` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,113 +69,113 @@
     "DeleteReceiptFilterRequestRequestTypeDef",
     "DeleteReceiptRuleRequestRequestTypeDef",
     "DeleteReceiptRuleSetRequestRequestTypeDef",
     "DeleteTemplateRequestRequestTypeDef",
     "DeleteVerifiedEmailAddressRequestRequestTypeDef",
     "DeliveryOptionsTypeDef",
     "ReceiptRuleSetMetadataTypeDef",
-    "ResponseMetadataTypeDef",
     "DescribeConfigurationSetRequestRequestTypeDef",
     "ReputationOptionsTypeDef",
     "DescribeReceiptRuleRequestRequestTypeDef",
     "DescribeReceiptRuleSetRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SNSDestinationTypeDef",
     "ExtensionFieldTypeDef",
+    "GetAccountSendingEnabledResponseTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     "IdentityDkimAttributesTypeDef",
     "GetIdentityMailFromDomainAttributesRequestRequestTypeDef",
     "IdentityMailFromDomainAttributesTypeDef",
     "GetIdentityNotificationAttributesRequestRequestTypeDef",
     "IdentityNotificationAttributesTypeDef",
     "GetIdentityPoliciesRequestRequestTypeDef",
+    "GetIdentityPoliciesResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetIdentityVerificationAttributesRequestRequestTypeDef",
     "IdentityVerificationAttributesTypeDef",
+    "GetSendQuotaResponseTypeDef",
     "SendDataPointTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LambdaActionTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
+    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
+    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
     "ListIdentitiesRequestRequestTypeDef",
+    "ListIdentitiesResponseTypeDef",
     "ListIdentityPoliciesRequestRequestTypeDef",
+    "ListIdentityPoliciesResponseTypeDef",
+    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
     "ListReceiptRuleSetsRequestRequestTypeDef",
+    "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateMetadataTypeDef",
+    "ListVerifiedEmailAddressesResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutIdentityPolicyRequestRequestTypeDef",
     "RawMessageTypeDef",
     "S3ActionTypeDef",
     "SNSActionTypeDef",
     "StopActionTypeDef",
     "WorkmailActionTypeDef",
     "ReceiptIpFilterTypeDef",
     "ReorderReceiptRuleSetRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "SendBounceResponseTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
+    "SendCustomVerificationEmailResponseTypeDef",
+    "SendEmailResponseTypeDef",
+    "SendRawEmailResponseTypeDef",
+    "SendTemplatedEmailResponseTypeDef",
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     "SetIdentityDkimEnabledRequestRequestTypeDef",
     "SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef",
     "SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef",
     "SetIdentityMailFromDomainRequestRequestTypeDef",
     "SetIdentityNotificationTopicRequestRequestTypeDef",
     "SetReceiptRulePositionRequestRequestTypeDef",
     "TestRenderTemplateRequestRequestTypeDef",
+    "TestRenderTemplateResponseTypeDef",
     "UpdateAccountSendingEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetSendingEnabledRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "VerifyDomainDkimRequestRequestTypeDef",
+    "VerifyDomainDkimResponseTypeDef",
     "VerifyDomainIdentityRequestRequestTypeDef",
+    "VerifyDomainIdentityResponseTypeDef",
     "VerifyEmailAddressRequestRequestTypeDef",
     "VerifyEmailIdentityRequestRequestTypeDef",
     "BodyTypeDef",
+    "SendBulkTemplatedEmailResponseTypeDef",
     "BulkEmailDestinationTypeDef",
     "SendTemplatedEmailRequestRequestTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "UpdateTemplateRequestRequestTypeDef",
-    "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAccountSendingEnabledResponseTypeDef",
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
-    "GetIdentityPoliciesResponseTypeDef",
-    "GetSendQuotaResponseTypeDef",
     "GetTemplateResponseTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
+    "UpdateTemplateRequestRequestTypeDef",
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
-    "ListIdentitiesResponseTypeDef",
-    "ListIdentityPoliciesResponseTypeDef",
+    "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "ListReceiptRuleSetsResponseTypeDef",
-    "ListVerifiedEmailAddressesResponseTypeDef",
-    "SendBounceResponseTypeDef",
-    "SendBulkTemplatedEmailResponseTypeDef",
-    "SendCustomVerificationEmailResponseTypeDef",
-    "SendEmailResponseTypeDef",
-    "SendRawEmailResponseTypeDef",
-    "SendTemplatedEmailResponseTypeDef",
-    "TestRenderTemplateResponseTypeDef",
-    "VerifyDomainDkimResponseTypeDef",
-    "VerifyDomainIdentityResponseTypeDef",
     "MessageDsnTypeDef",
     "RecipientDsnFieldsTypeDef",
     "GetIdentityDkimAttributesResponseTypeDef",
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     "GetIdentityNotificationAttributesResponseTypeDef",
     "GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     "GetIdentityVerificationAttributesResponseTypeDef",
     "GetSendStatisticsResponseTypeDef",
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
-    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
-    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
-    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
-    "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesResponseTypeDef",
     "SendRawEmailRequestRequestTypeDef",
     "ReceiptActionTypeDef",
     "ReceiptFilterTypeDef",
     "MessageTypeDef",
     "SendBulkTemplatedEmailRequestRequestTypeDef",
     "EventDestinationTypeDef",
@@ -449,25 +449,14 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
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
 _RequiredDescribeConfigurationSetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalDescribeConfigurationSetRequestRequestTypeDef = TypedDict(
@@ -507,14 +496,21 @@
 DescribeReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "DescribeReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 KinesisFirehoseDestinationTypeDef = TypedDict(
     "KinesisFirehoseDestinationTypeDef",
     {
         "IAMRoleARN": str,
         "DeliveryStreamARN": str,
     },
 )
@@ -530,21 +526,42 @@
     "ExtensionFieldTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+GetAccountSendingEnabledResponseTypeDef = TypedDict(
+    "GetAccountSendingEnabledResponseTypeDef",
+    {
+        "Enabled": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 GetIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     {
         "Identities": Sequence[str],
     },
 )
 
@@ -623,14 +640,22 @@
     "GetIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyNames": Sequence[str],
     },
 )
 
+GetIdentityPoliciesResponseTypeDef = TypedDict(
+    "GetIdentityPoliciesResponseTypeDef",
+    {
+        "Policies": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -660,14 +685,24 @@
 
 class IdentityVerificationAttributesTypeDef(
     _RequiredIdentityVerificationAttributesTypeDef, _OptionalIdentityVerificationAttributesTypeDef
 ):
     pass
 
 
+GetSendQuotaResponseTypeDef = TypedDict(
+    "GetSendQuotaResponseTypeDef",
+    {
+        "Max24HourSend": float,
+        "MaxSendRate": float,
+        "SentLast24Hours": float,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SendDataPointTypeDef = TypedDict(
     "SendDataPointTypeDef",
     {
         "Timestamp": datetime,
         "DeliveryAttempts": int,
         "Bounces": int,
         "Complaints": int,
@@ -699,67 +734,115 @@
 )
 
 
 class LambdaActionTypeDef(_RequiredLambdaActionTypeDef, _OptionalLambdaActionTypeDef):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListConfigurationSetsRequestRequestTypeDef = TypedDict(
     "ListConfigurationSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = TypedDict(
+    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCustomVerificationEmailTemplatesRequestRequestTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListIdentitiesRequestListIdentitiesPaginateTypeDef = TypedDict(
+    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
+    {
+        "IdentityType": IdentityTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListIdentitiesRequestRequestTypeDef = TypedDict(
     "ListIdentitiesRequestRequestTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+ListIdentitiesResponseTypeDef = TypedDict(
+    "ListIdentitiesResponseTypeDef",
+    {
+        "Identities": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "ListIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
     },
 )
 
+ListIdentityPoliciesResponseTypeDef = TypedDict(
+    "ListIdentityPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = TypedDict(
+    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReceiptRuleSetsRequestRequestTypeDef = TypedDict(
     "ListReceiptRuleSetsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+ListTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
+    "ListTemplatesRequestListTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTemplatesRequestRequestTypeDef = TypedDict(
     "ListTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
@@ -770,14 +853,32 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
+ListVerifiedEmailAddressesResponseTypeDef = TypedDict(
+    "ListVerifiedEmailAddressesResponseTypeDef",
+    {
+        "VerifiedEmailAddresses": List[str],
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
 PutIdentityPolicyRequestRequestTypeDef = TypedDict(
     "PutIdentityPolicyRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyName": str,
         "Policy": str,
     },
@@ -880,14 +981,33 @@
     "ReorderReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleNames": Sequence[str],
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
+SendBounceResponseTypeDef = TypedDict(
+    "SendBounceResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -903,14 +1023,46 @@
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
+SendRawEmailResponseTypeDef = TypedDict(
+    "SendRawEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SendTemplatedEmailResponseTypeDef = TypedDict(
+    "SendTemplatedEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetActiveReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
     total=False,
 )
@@ -1013,14 +1165,22 @@
     "TestRenderTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
 
+TestRenderTemplateResponseTypeDef = TypedDict(
+    "TestRenderTemplateResponseTypeDef",
+    {
+        "RenderedTemplate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateAccountSendingEnabledRequestRequestTypeDef = TypedDict(
     "UpdateAccountSendingEnabledRequestRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1070,21 +1230,37 @@
 VerifyDomainDkimRequestRequestTypeDef = TypedDict(
     "VerifyDomainDkimRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
+VerifyDomainDkimResponseTypeDef = TypedDict(
+    "VerifyDomainDkimResponseTypeDef",
+    {
+        "DkimTokens": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VerifyDomainIdentityRequestRequestTypeDef = TypedDict(
     "VerifyDomainIdentityRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
+VerifyDomainIdentityResponseTypeDef = TypedDict(
+    "VerifyDomainIdentityResponseTypeDef",
+    {
+        "VerificationToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VerifyEmailAddressRequestRequestTypeDef = TypedDict(
     "VerifyEmailAddressRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
@@ -1100,14 +1276,22 @@
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
 )
 
+SendBulkTemplatedEmailResponseTypeDef = TypedDict(
+    "SendBulkTemplatedEmailResponseTypeDef",
+    {
+        "Status": List[BulkEmailDestinationStatusTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredBulkEmailDestinationTypeDef = TypedDict(
     "_RequiredBulkEmailDestinationTypeDef",
     {
         "Destination": DestinationTypeDef,
     },
 )
 _OptionalBulkEmailDestinationTypeDef = TypedDict(
@@ -1167,14 +1351,23 @@
 CreateConfigurationSetRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSet": ConfigurationSetTypeDef,
     },
 )
 
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[ConfigurationSetTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
     },
 )
@@ -1190,21 +1383,38 @@
 CreateTemplateRequestRequestTypeDef = TypedDict(
     "CreateTemplateRequestRequestTypeDef",
     {
         "Template": TemplateTypeDef,
     },
 )
 
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "Template": TemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateTemplateRequestRequestTypeDef = TypedDict(
     "UpdateTemplateRequestRequestTypeDef",
     {
         "Template": TemplateTypeDef,
     },
 )
 
+ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
+    "ListCustomVerificationEmailTemplatesResponseTypeDef",
+    {
+        "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef = TypedDict(
@@ -1219,189 +1429,20 @@
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccountSendingEnabledResponseTypeDef = TypedDict(
-    "GetAccountSendingEnabledResponseTypeDef",
-    {
-        "Enabled": bool,
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
-GetIdentityPoliciesResponseTypeDef = TypedDict(
-    "GetIdentityPoliciesResponseTypeDef",
-    {
-        "Policies": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSendQuotaResponseTypeDef = TypedDict(
-    "GetSendQuotaResponseTypeDef",
-    {
-        "Max24HourSend": float,
-        "MaxSendRate": float,
-        "SentLast24Hours": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "Template": TemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
-    {
-        "ConfigurationSets": List[ConfigurationSetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
-    "ListCustomVerificationEmailTemplatesResponseTypeDef",
-    {
-        "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListIdentitiesResponseTypeDef = TypedDict(
-    "ListIdentitiesResponseTypeDef",
-    {
-        "Identities": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListIdentityPoliciesResponseTypeDef = TypedDict(
-    "ListIdentityPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListReceiptRuleSetsResponseTypeDef = TypedDict(
     "ListReceiptRuleSetsResponseTypeDef",
     {
         "RuleSets": List[ReceiptRuleSetMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListVerifiedEmailAddressesResponseTypeDef = TypedDict(
-    "ListVerifiedEmailAddressesResponseTypeDef",
-    {
-        "VerifiedEmailAddresses": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendBounceResponseTypeDef = TypedDict(
-    "SendBounceResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendBulkTemplatedEmailResponseTypeDef = TypedDict(
-    "SendBulkTemplatedEmailResponseTypeDef",
-    {
-        "Status": List[BulkEmailDestinationStatusTypeDef],
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
-SendRawEmailResponseTypeDef = TypedDict(
-    "SendRawEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendTemplatedEmailResponseTypeDef = TypedDict(
-    "SendTemplatedEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestRenderTemplateResponseTypeDef = TypedDict(
-    "TestRenderTemplateResponseTypeDef",
-    {
-        "RenderedTemplate": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-VerifyDomainDkimResponseTypeDef = TypedDict(
-    "VerifyDomainDkimResponseTypeDef",
-    {
-        "DkimTokens": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-VerifyDomainIdentityResponseTypeDef = TypedDict(
-    "VerifyDomainIdentityResponseTypeDef",
-    {
-        "VerificationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMessageDsnTypeDef = TypedDict(
     "_RequiredMessageDsnTypeDef",
     {
         "ReportingMta": str,
@@ -1447,31 +1488,31 @@
     pass
 
 
 GetIdentityDkimAttributesResponseTypeDef = TypedDict(
     "GetIdentityDkimAttributesResponseTypeDef",
     {
         "DkimAttributes": Dict[str, IdentityDkimAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIdentityMailFromDomainAttributesResponseTypeDef = TypedDict(
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     {
         "MailFromDomainAttributes": Dict[str, IdentityMailFromDomainAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIdentityNotificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityNotificationAttributesResponseTypeDef",
     {
         "NotificationAttributes": Dict[str, IdentityNotificationAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef = TypedDict(
     "_RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     {
         "Identities": Sequence[str],
@@ -1493,73 +1534,32 @@
     pass
 
 
 GetIdentityVerificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityVerificationAttributesResponseTypeDef",
     {
         "VerificationAttributes": Dict[str, IdentityVerificationAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSendStatisticsResponseTypeDef = TypedDict(
     "GetSendStatisticsResponseTypeDef",
     {
         "SendDataPoints": List[SendDataPointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = TypedDict(
-    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListIdentitiesRequestListIdentitiesPaginateTypeDef = TypedDict(
-    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
-    {
-        "IdentityType": IdentityTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = TypedDict(
-    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
-    "ListTemplatesRequestListTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[TemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSendRawEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendRawEmailRequestRequestTypeDef",
     {
         "RawMessage": RawMessageTypeDef,
@@ -1723,15 +1723,15 @@
     },
 )
 
 ListReceiptFiltersResponseTypeDef = TypedDict(
     "ListReceiptFiltersResponseTypeDef",
     {
         "Filters": List[ReceiptFilterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Source": str,
@@ -1771,15 +1771,15 @@
     "DescribeConfigurationSetResponseTypeDef",
     {
         "ConfigurationSet": ConfigurationSetTypeDef,
         "EventDestinations": List[EventDestinationTypeDef],
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
@@ -1835,32 +1835,32 @@
 
 
 DescribeActiveReceiptRuleSetResponseTypeDef = TypedDict(
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     {
         "Metadata": ReceiptRuleSetMetadataTypeDef,
         "Rules": List[ReceiptRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReceiptRuleResponseTypeDef = TypedDict(
     "DescribeReceiptRuleResponseTypeDef",
     {
         "Rule": ReceiptRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReceiptRuleSetResponseTypeDef = TypedDict(
     "DescribeReceiptRuleSetResponseTypeDef",
     {
         "Metadata": ReceiptRuleSetMetadataTypeDef,
         "Rules": List[ReceiptRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateReceiptRuleRequestRequestTypeDef = TypedDict(
     "UpdateReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
```

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/type_defs.pyi` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -68,113 +68,113 @@
     "DeleteReceiptFilterRequestRequestTypeDef",
     "DeleteReceiptRuleRequestRequestTypeDef",
     "DeleteReceiptRuleSetRequestRequestTypeDef",
     "DeleteTemplateRequestRequestTypeDef",
     "DeleteVerifiedEmailAddressRequestRequestTypeDef",
     "DeliveryOptionsTypeDef",
     "ReceiptRuleSetMetadataTypeDef",
-    "ResponseMetadataTypeDef",
     "DescribeConfigurationSetRequestRequestTypeDef",
     "ReputationOptionsTypeDef",
     "DescribeReceiptRuleRequestRequestTypeDef",
     "DescribeReceiptRuleSetRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SNSDestinationTypeDef",
     "ExtensionFieldTypeDef",
+    "GetAccountSendingEnabledResponseTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     "IdentityDkimAttributesTypeDef",
     "GetIdentityMailFromDomainAttributesRequestRequestTypeDef",
     "IdentityMailFromDomainAttributesTypeDef",
     "GetIdentityNotificationAttributesRequestRequestTypeDef",
     "IdentityNotificationAttributesTypeDef",
     "GetIdentityPoliciesRequestRequestTypeDef",
+    "GetIdentityPoliciesResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetIdentityVerificationAttributesRequestRequestTypeDef",
     "IdentityVerificationAttributesTypeDef",
+    "GetSendQuotaResponseTypeDef",
     "SendDataPointTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LambdaActionTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
+    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
+    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
     "ListIdentitiesRequestRequestTypeDef",
+    "ListIdentitiesResponseTypeDef",
     "ListIdentityPoliciesRequestRequestTypeDef",
+    "ListIdentityPoliciesResponseTypeDef",
+    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
     "ListReceiptRuleSetsRequestRequestTypeDef",
+    "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateMetadataTypeDef",
+    "ListVerifiedEmailAddressesResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutIdentityPolicyRequestRequestTypeDef",
     "RawMessageTypeDef",
     "S3ActionTypeDef",
     "SNSActionTypeDef",
     "StopActionTypeDef",
     "WorkmailActionTypeDef",
     "ReceiptIpFilterTypeDef",
     "ReorderReceiptRuleSetRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "SendBounceResponseTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
+    "SendCustomVerificationEmailResponseTypeDef",
+    "SendEmailResponseTypeDef",
+    "SendRawEmailResponseTypeDef",
+    "SendTemplatedEmailResponseTypeDef",
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     "SetIdentityDkimEnabledRequestRequestTypeDef",
     "SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef",
     "SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef",
     "SetIdentityMailFromDomainRequestRequestTypeDef",
     "SetIdentityNotificationTopicRequestRequestTypeDef",
     "SetReceiptRulePositionRequestRequestTypeDef",
     "TestRenderTemplateRequestRequestTypeDef",
+    "TestRenderTemplateResponseTypeDef",
     "UpdateAccountSendingEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetSendingEnabledRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "VerifyDomainDkimRequestRequestTypeDef",
+    "VerifyDomainDkimResponseTypeDef",
     "VerifyDomainIdentityRequestRequestTypeDef",
+    "VerifyDomainIdentityResponseTypeDef",
     "VerifyEmailAddressRequestRequestTypeDef",
     "VerifyEmailIdentityRequestRequestTypeDef",
     "BodyTypeDef",
+    "SendBulkTemplatedEmailResponseTypeDef",
     "BulkEmailDestinationTypeDef",
     "SendTemplatedEmailRequestRequestTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "UpdateTemplateRequestRequestTypeDef",
-    "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAccountSendingEnabledResponseTypeDef",
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
-    "GetIdentityPoliciesResponseTypeDef",
-    "GetSendQuotaResponseTypeDef",
     "GetTemplateResponseTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
+    "UpdateTemplateRequestRequestTypeDef",
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
-    "ListIdentitiesResponseTypeDef",
-    "ListIdentityPoliciesResponseTypeDef",
+    "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "ListReceiptRuleSetsResponseTypeDef",
-    "ListVerifiedEmailAddressesResponseTypeDef",
-    "SendBounceResponseTypeDef",
-    "SendBulkTemplatedEmailResponseTypeDef",
-    "SendCustomVerificationEmailResponseTypeDef",
-    "SendEmailResponseTypeDef",
-    "SendRawEmailResponseTypeDef",
-    "SendTemplatedEmailResponseTypeDef",
-    "TestRenderTemplateResponseTypeDef",
-    "VerifyDomainDkimResponseTypeDef",
-    "VerifyDomainIdentityResponseTypeDef",
     "MessageDsnTypeDef",
     "RecipientDsnFieldsTypeDef",
     "GetIdentityDkimAttributesResponseTypeDef",
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     "GetIdentityNotificationAttributesResponseTypeDef",
     "GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     "GetIdentityVerificationAttributesResponseTypeDef",
     "GetSendStatisticsResponseTypeDef",
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
-    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
-    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
-    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
-    "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesResponseTypeDef",
     "SendRawEmailRequestRequestTypeDef",
     "ReceiptActionTypeDef",
     "ReceiptFilterTypeDef",
     "MessageTypeDef",
     "SendBulkTemplatedEmailRequestRequestTypeDef",
     "EventDestinationTypeDef",
@@ -442,25 +442,14 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
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
 _RequiredDescribeConfigurationSetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalDescribeConfigurationSetRequestRequestTypeDef = TypedDict(
@@ -498,14 +487,21 @@
 DescribeReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "DescribeReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 KinesisFirehoseDestinationTypeDef = TypedDict(
     "KinesisFirehoseDestinationTypeDef",
     {
         "IAMRoleARN": str,
         "DeliveryStreamARN": str,
     },
 )
@@ -521,21 +517,42 @@
     "ExtensionFieldTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+GetAccountSendingEnabledResponseTypeDef = TypedDict(
+    "GetAccountSendingEnabledResponseTypeDef",
+    {
+        "Enabled": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 GetIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     {
         "Identities": Sequence[str],
     },
 )
 
@@ -610,14 +627,22 @@
     "GetIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyNames": Sequence[str],
     },
 )
 
+GetIdentityPoliciesResponseTypeDef = TypedDict(
+    "GetIdentityPoliciesResponseTypeDef",
+    {
+        "Policies": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -645,14 +670,24 @@
 )
 
 class IdentityVerificationAttributesTypeDef(
     _RequiredIdentityVerificationAttributesTypeDef, _OptionalIdentityVerificationAttributesTypeDef
 ):
     pass
 
+GetSendQuotaResponseTypeDef = TypedDict(
+    "GetSendQuotaResponseTypeDef",
+    {
+        "Max24HourSend": float,
+        "MaxSendRate": float,
+        "SentLast24Hours": float,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SendDataPointTypeDef = TypedDict(
     "SendDataPointTypeDef",
     {
         "Timestamp": datetime,
         "DeliveryAttempts": int,
         "Bounces": int,
         "Complaints": int,
@@ -682,67 +717,115 @@
     },
     total=False,
 )
 
 class LambdaActionTypeDef(_RequiredLambdaActionTypeDef, _OptionalLambdaActionTypeDef):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListConfigurationSetsRequestRequestTypeDef = TypedDict(
     "ListConfigurationSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = TypedDict(
+    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCustomVerificationEmailTemplatesRequestRequestTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListIdentitiesRequestListIdentitiesPaginateTypeDef = TypedDict(
+    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
+    {
+        "IdentityType": IdentityTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListIdentitiesRequestRequestTypeDef = TypedDict(
     "ListIdentitiesRequestRequestTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+ListIdentitiesResponseTypeDef = TypedDict(
+    "ListIdentitiesResponseTypeDef",
+    {
+        "Identities": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "ListIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
     },
 )
 
+ListIdentityPoliciesResponseTypeDef = TypedDict(
+    "ListIdentityPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = TypedDict(
+    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReceiptRuleSetsRequestRequestTypeDef = TypedDict(
     "ListReceiptRuleSetsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+ListTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
+    "ListTemplatesRequestListTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTemplatesRequestRequestTypeDef = TypedDict(
     "ListTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
@@ -753,14 +836,32 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
+ListVerifiedEmailAddressesResponseTypeDef = TypedDict(
+    "ListVerifiedEmailAddressesResponseTypeDef",
+    {
+        "VerifiedEmailAddresses": List[str],
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
 PutIdentityPolicyRequestRequestTypeDef = TypedDict(
     "PutIdentityPolicyRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyName": str,
         "Policy": str,
     },
@@ -855,14 +956,33 @@
     "ReorderReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleNames": Sequence[str],
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
+SendBounceResponseTypeDef = TypedDict(
+    "SendBounceResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -876,14 +996,46 @@
 
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
+SendRawEmailResponseTypeDef = TypedDict(
+    "SendRawEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SendTemplatedEmailResponseTypeDef = TypedDict(
+    "SendTemplatedEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetActiveReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
     total=False,
 )
@@ -980,14 +1132,22 @@
     "TestRenderTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
 
+TestRenderTemplateResponseTypeDef = TypedDict(
+    "TestRenderTemplateResponseTypeDef",
+    {
+        "RenderedTemplate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateAccountSendingEnabledRequestRequestTypeDef = TypedDict(
     "UpdateAccountSendingEnabledRequestRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1035,21 +1195,37 @@
 VerifyDomainDkimRequestRequestTypeDef = TypedDict(
     "VerifyDomainDkimRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
+VerifyDomainDkimResponseTypeDef = TypedDict(
+    "VerifyDomainDkimResponseTypeDef",
+    {
+        "DkimTokens": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VerifyDomainIdentityRequestRequestTypeDef = TypedDict(
     "VerifyDomainIdentityRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
+VerifyDomainIdentityResponseTypeDef = TypedDict(
+    "VerifyDomainIdentityResponseTypeDef",
+    {
+        "VerificationToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VerifyEmailAddressRequestRequestTypeDef = TypedDict(
     "VerifyEmailAddressRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
@@ -1065,14 +1241,22 @@
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
 )
 
+SendBulkTemplatedEmailResponseTypeDef = TypedDict(
+    "SendBulkTemplatedEmailResponseTypeDef",
+    {
+        "Status": List[BulkEmailDestinationStatusTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredBulkEmailDestinationTypeDef = TypedDict(
     "_RequiredBulkEmailDestinationTypeDef",
     {
         "Destination": DestinationTypeDef,
     },
 )
 _OptionalBulkEmailDestinationTypeDef = TypedDict(
@@ -1128,14 +1312,23 @@
 CreateConfigurationSetRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSet": ConfigurationSetTypeDef,
     },
 )
 
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[ConfigurationSetTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
     },
 )
@@ -1151,21 +1344,38 @@
 CreateTemplateRequestRequestTypeDef = TypedDict(
     "CreateTemplateRequestRequestTypeDef",
     {
         "Template": TemplateTypeDef,
     },
 )
 
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "Template": TemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateTemplateRequestRequestTypeDef = TypedDict(
     "UpdateTemplateRequestRequestTypeDef",
     {
         "Template": TemplateTypeDef,
     },
 )
 
+ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
+    "ListCustomVerificationEmailTemplatesResponseTypeDef",
+    {
+        "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef = TypedDict(
@@ -1178,189 +1388,20 @@
 
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccountSendingEnabledResponseTypeDef = TypedDict(
-    "GetAccountSendingEnabledResponseTypeDef",
-    {
-        "Enabled": bool,
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
-GetIdentityPoliciesResponseTypeDef = TypedDict(
-    "GetIdentityPoliciesResponseTypeDef",
-    {
-        "Policies": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSendQuotaResponseTypeDef = TypedDict(
-    "GetSendQuotaResponseTypeDef",
-    {
-        "Max24HourSend": float,
-        "MaxSendRate": float,
-        "SentLast24Hours": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "Template": TemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
-    {
-        "ConfigurationSets": List[ConfigurationSetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
-    "ListCustomVerificationEmailTemplatesResponseTypeDef",
-    {
-        "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListIdentitiesResponseTypeDef = TypedDict(
-    "ListIdentitiesResponseTypeDef",
-    {
-        "Identities": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListIdentityPoliciesResponseTypeDef = TypedDict(
-    "ListIdentityPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListReceiptRuleSetsResponseTypeDef = TypedDict(
     "ListReceiptRuleSetsResponseTypeDef",
     {
         "RuleSets": List[ReceiptRuleSetMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListVerifiedEmailAddressesResponseTypeDef = TypedDict(
-    "ListVerifiedEmailAddressesResponseTypeDef",
-    {
-        "VerifiedEmailAddresses": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendBounceResponseTypeDef = TypedDict(
-    "SendBounceResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendBulkTemplatedEmailResponseTypeDef = TypedDict(
-    "SendBulkTemplatedEmailResponseTypeDef",
-    {
-        "Status": List[BulkEmailDestinationStatusTypeDef],
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
-SendRawEmailResponseTypeDef = TypedDict(
-    "SendRawEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendTemplatedEmailResponseTypeDef = TypedDict(
-    "SendTemplatedEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestRenderTemplateResponseTypeDef = TypedDict(
-    "TestRenderTemplateResponseTypeDef",
-    {
-        "RenderedTemplate": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-VerifyDomainDkimResponseTypeDef = TypedDict(
-    "VerifyDomainDkimResponseTypeDef",
-    {
-        "DkimTokens": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-VerifyDomainIdentityResponseTypeDef = TypedDict(
-    "VerifyDomainIdentityResponseTypeDef",
-    {
-        "VerificationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMessageDsnTypeDef = TypedDict(
     "_RequiredMessageDsnTypeDef",
     {
         "ReportingMta": str,
@@ -1402,31 +1443,31 @@
 ):
     pass
 
 GetIdentityDkimAttributesResponseTypeDef = TypedDict(
     "GetIdentityDkimAttributesResponseTypeDef",
     {
         "DkimAttributes": Dict[str, IdentityDkimAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIdentityMailFromDomainAttributesResponseTypeDef = TypedDict(
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     {
         "MailFromDomainAttributes": Dict[str, IdentityMailFromDomainAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIdentityNotificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityNotificationAttributesResponseTypeDef",
     {
         "NotificationAttributes": Dict[str, IdentityNotificationAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef = TypedDict(
     "_RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     {
         "Identities": Sequence[str],
@@ -1446,73 +1487,32 @@
 ):
     pass
 
 GetIdentityVerificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityVerificationAttributesResponseTypeDef",
     {
         "VerificationAttributes": Dict[str, IdentityVerificationAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSendStatisticsResponseTypeDef = TypedDict(
     "GetSendStatisticsResponseTypeDef",
     {
         "SendDataPoints": List[SendDataPointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = TypedDict(
-    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListIdentitiesRequestListIdentitiesPaginateTypeDef = TypedDict(
-    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
-    {
-        "IdentityType": IdentityTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = TypedDict(
-    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
-    "ListTemplatesRequestListTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[TemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSendRawEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendRawEmailRequestRequestTypeDef",
     {
         "RawMessage": RawMessageTypeDef,
@@ -1666,15 +1666,15 @@
     },
 )
 
 ListReceiptFiltersResponseTypeDef = TypedDict(
     "ListReceiptFiltersResponseTypeDef",
     {
         "Filters": List[ReceiptFilterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Source": str,
@@ -1712,15 +1712,15 @@
     "DescribeConfigurationSetResponseTypeDef",
     {
         "ConfigurationSet": ConfigurationSetTypeDef,
         "EventDestinations": List[EventDestinationTypeDef],
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
@@ -1772,32 +1772,32 @@
     pass
 
 DescribeActiveReceiptRuleSetResponseTypeDef = TypedDict(
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     {
         "Metadata": ReceiptRuleSetMetadataTypeDef,
         "Rules": List[ReceiptRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReceiptRuleResponseTypeDef = TypedDict(
     "DescribeReceiptRuleResponseTypeDef",
     {
         "Rule": ReceiptRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReceiptRuleSetResponseTypeDef = TypedDict(
     "DescribeReceiptRuleSetResponseTypeDef",
     {
         "Metadata": ReceiptRuleSetMetadataTypeDef,
         "Rules": List[ReceiptRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateReceiptRuleRequestRequestTypeDef = TypedDict(
     "UpdateReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
```

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/waiter.py` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses/waiter.pyi` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses.egg-info/PKG-INFO` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ses
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SES 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SES 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/
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
 
 <a id="mypy-boto3-ses"></a>
 
 # mypy-boto3-ses
 
 [![PyPI - mypy-boto3-ses](https://img.shields.io/pypi/v/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ses?color=blue)](https://pypistats.org/packages/mypy-boto3-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SES 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[boto3.SES 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
 See how it helps to find and fix potential bugs:
 
@@ -401,113 +402,113 @@
     DeleteReceiptFilterRequestRequestTypeDef,
     DeleteReceiptRuleRequestRequestTypeDef,
     DeleteReceiptRuleSetRequestRequestTypeDef,
     DeleteTemplateRequestRequestTypeDef,
     DeleteVerifiedEmailAddressRequestRequestTypeDef,
     DeliveryOptionsTypeDef,
     ReceiptRuleSetMetadataTypeDef,
-    ResponseMetadataTypeDef,
     DescribeConfigurationSetRequestRequestTypeDef,
     ReputationOptionsTypeDef,
     DescribeReceiptRuleRequestRequestTypeDef,
     DescribeReceiptRuleSetRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SNSDestinationTypeDef,
     ExtensionFieldTypeDef,
+    GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesRequestRequestTypeDef,
     IdentityDkimAttributesTypeDef,
     GetIdentityMailFromDomainAttributesRequestRequestTypeDef,
     IdentityMailFromDomainAttributesTypeDef,
     GetIdentityNotificationAttributesRequestRequestTypeDef,
     IdentityNotificationAttributesTypeDef,
     GetIdentityPoliciesRequestRequestTypeDef,
+    GetIdentityPoliciesResponseTypeDef,
     WaiterConfigTypeDef,
     GetIdentityVerificationAttributesRequestRequestTypeDef,
     IdentityVerificationAttributesTypeDef,
+    GetSendQuotaResponseTypeDef,
     SendDataPointTypeDef,
     GetTemplateRequestRequestTypeDef,
     LambdaActionTypeDef,
-    PaginatorConfigTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
+    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
+    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListIdentitiesRequestRequestTypeDef,
+    ListIdentitiesResponseTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
+    ListIdentityPoliciesResponseTypeDef,
+    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
+    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
+    ListVerifiedEmailAddressesResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
     RawMessageTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    SendBounceResponseTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    SendRawEmailResponseTypeDef,
+    SendTemplatedEmailResponseTypeDef,
     SetActiveReceiptRuleSetRequestRequestTypeDef,
     SetIdentityDkimEnabledRequestRequestTypeDef,
     SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef,
     SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef,
     SetIdentityMailFromDomainRequestRequestTypeDef,
     SetIdentityNotificationTopicRequestRequestTypeDef,
     SetReceiptRulePositionRequestRequestTypeDef,
     TestRenderTemplateRequestRequestTypeDef,
+    TestRenderTemplateResponseTypeDef,
     UpdateAccountSendingEnabledRequestRequestTypeDef,
     UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef,
     UpdateConfigurationSetSendingEnabledRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     VerifyDomainDkimRequestRequestTypeDef,
+    VerifyDomainDkimResponseTypeDef,
     VerifyDomainIdentityRequestRequestTypeDef,
+    VerifyDomainIdentityResponseTypeDef,
     VerifyEmailAddressRequestRequestTypeDef,
     VerifyEmailIdentityRequestRequestTypeDef,
     BodyTypeDef,
+    SendBulkTemplatedEmailResponseTypeDef,
     BulkEmailDestinationTypeDef,
     SendTemplatedEmailRequestRequestTypeDef,
     CloudWatchDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
+    ListConfigurationSetsResponseTypeDef,
     CreateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    UpdateTemplateRequestRequestTypeDef,
-    PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAccountSendingEnabledResponseTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
-    GetIdentityPoliciesResponseTypeDef,
-    GetSendQuotaResponseTypeDef,
     GetTemplateResponseTypeDef,
-    ListConfigurationSetsResponseTypeDef,
+    UpdateTemplateRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesResponseTypeDef,
-    ListIdentitiesResponseTypeDef,
-    ListIdentityPoliciesResponseTypeDef,
+    PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     ListReceiptRuleSetsResponseTypeDef,
-    ListVerifiedEmailAddressesResponseTypeDef,
-    SendBounceResponseTypeDef,
-    SendBulkTemplatedEmailResponseTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
-    SendRawEmailResponseTypeDef,
-    SendTemplatedEmailResponseTypeDef,
-    TestRenderTemplateResponseTypeDef,
-    VerifyDomainDkimResponseTypeDef,
-    VerifyDomainIdentityResponseTypeDef,
     MessageDsnTypeDef,
     RecipientDsnFieldsTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
-    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
-    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
-    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
-    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
     SendRawEmailRequestRequestTypeDef,
     ReceiptActionTypeDef,
     ReceiptFilterTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
     EventDestinationTypeDef,
@@ -535,42 +536,42 @@
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

### Comparing `mypy-boto3-ses-1.26.0.post1/mypy_boto3_ses.egg-info/SOURCES.txt` & `mypy-boto3-ses-1.27.0/mypy_boto3_ses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.26.0.post1/setup.py` & `mypy-boto3-ses-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-ses.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ses",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_ses"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SES 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.SES 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 ses type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_ses": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_ses": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/",
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


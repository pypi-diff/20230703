# Comparing `tmp/mypy-boto3-sns-1.26.69.tar.gz` & `tmp/mypy-boto3-sns-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sns-1.26.69.tar", last modified: Fri Feb 10 20:27:29 2023, max compression
+gzip compressed data, was "mypy-boto3-sns-1.27.0.tar", last modified: Mon Jul  3 19:51:29 2023, max compression
```

## Comparing `mypy-boto3-sns-1.26.69.tar` & `mypy-boto3-sns-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:27:29.498390 mypy-boto3-sns-1.26.69/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-10 20:27:16.000000 mypy-boto3-sns-1.26.69/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20965 2023-02-10 20:27:29.498390 mypy-boto3-sns-1.26.69/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19494 2023-02-10 20:27:16.000000 mypy-boto3-sns-1.26.69/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:27:29.498390 mypy-boto3-sns-1.26.69/mypy_boto3_sns/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-02-10 20:27:16.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-02-10 20:27:16.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-10 20:27:16.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33219 2023-02-10 20:27:17.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33162 2023-02-10 20:27:16.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-02-10 20:27:18.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-02-10 20:27:18.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-02-10 20:27:18.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-02-10 20:27:18.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 20:27:16.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33866 2023-02-10 20:27:18.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    33797 2023-02-10 20:27:18.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    35312 2023-02-10 20:27:19.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35265 2023-02-10 20:27:18.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-10 20:27:16.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:27:29.498390 mypy-boto3-sns-1.26.69/mypy_boto3_sns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20965 2023-02-10 20:27:29.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-02-10 20:27:29.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 20:27:29.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 20:27:29.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-10 20:27:29.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-10 20:27:29.000000 mypy-boto3-sns-1.26.69/mypy_boto3_sns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 20:27:29.498390 mypy-boto3-sns-1.26.69/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-10 20:27:16.000000 mypy-boto3-sns-1.26.69/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:29.776037 mypy-boto3-sns-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-07-03 19:51:29.772037 mypy-boto3-sns-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19276 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:29.768037 mypy-boto3-sns-1.27.0/mypy_boto3_sns/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33161 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33864 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33795 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34610 2023-07-03 19:48:24.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34563 2023-07-03 19:48:24.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:23.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:29.772037 mypy-boto3-sns-1.27.0/mypy_boto3_sns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-07-03 19:51:29.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-03 19:51:29.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:29.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:29.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:29.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:29.000000 mypy-boto3-sns-1.27.0/mypy_boto3_sns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:29.776037 mypy-boto3-sns-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:48:22.000000 mypy-boto3-sns-1.27.0/setup.py
```

### Comparing `mypy-boto3-sns-1.26.69/LICENSE` & `mypy-boto3-sns-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-sns-1.26.69/PKG-INFO` & `mypy-boto3-sns-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sns
-Version: 1.26.69
-Summary: Type annotations for boto3.SNS 1.26.69 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.SNS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sns"></a>
 
 # mypy-boto3-sns
 
 [![PyPI - mypy-boto3-sns](https://img.shields.io/pypi/v/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sns?color=blue)](https://pypistats.org/packages/mypy-boto3-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SNS 1.26.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[boto3.SNS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [mypy-boto3-sns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -437,102 +437,98 @@
 
 ```python
 from mypy_boto3_sns.type_defs import (
     AddPermissionInputRequestTypeDef,
     AddPermissionInputTopicAddPermissionTypeDef,
     BatchResultErrorEntryTypeDef,
     CheckIfPhoneNumberIsOptedOutInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CheckIfPhoneNumberIsOptedOutResponseTypeDef,
     ConfirmSubscriptionInputRequestTypeDef,
     ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
+    ConfirmSubscriptionResponseTypeDef,
+    CreateEndpointResponseTypeDef,
     CreatePlatformApplicationInputRequestTypeDef,
     CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef,
+    CreatePlatformApplicationResponseTypeDef,
     CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef,
     CreatePlatformEndpointInputRequestTypeDef,
     CreateSMSSandboxPhoneNumberInputRequestTypeDef,
     TagTypeDef,
+    CreateTopicResponseTypeDef,
     DeleteEndpointInputRequestTypeDef,
     DeletePlatformApplicationInputRequestTypeDef,
     DeleteSMSSandboxPhoneNumberInputRequestTypeDef,
     DeleteTopicInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointTypeDef,
     GetDataProtectionPolicyInputRequestTypeDef,
+    GetDataProtectionPolicyResponseTypeDef,
     GetEndpointAttributesInputRequestTypeDef,
+    GetEndpointAttributesResponseTypeDef,
     GetPlatformApplicationAttributesInputRequestTypeDef,
+    GetPlatformApplicationAttributesResponseTypeDef,
     GetSMSAttributesInputRequestTypeDef,
+    GetSMSAttributesResponseTypeDef,
+    GetSMSSandboxAccountStatusResultTypeDef,
     GetSubscriptionAttributesInputRequestTypeDef,
+    GetSubscriptionAttributesResponseTypeDef,
     GetTopicAttributesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetTopicAttributesResponseTypeDef,
+    ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
     ListEndpointsByPlatformApplicationInputRequestTypeDef,
+    ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
     ListOriginationNumbersRequestRequestTypeDef,
     PhoneNumberInformationTypeDef,
+    ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
     ListPhoneNumbersOptedOutInputRequestTypeDef,
+    ListPhoneNumbersOptedOutResponseTypeDef,
+    ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
     ListPlatformApplicationsInputRequestTypeDef,
     PlatformApplicationTypeDef,
+    ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
     ListSMSSandboxPhoneNumbersInputRequestTypeDef,
     SMSSandboxPhoneNumberTypeDef,
+    ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
     ListSubscriptionsByTopicInputRequestTypeDef,
     SubscriptionTypeDef,
+    ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
     ListSubscriptionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTopicsInputListTopicsPaginateTypeDef,
     ListTopicsInputRequestTypeDef,
     TopicTypeDef,
     MessageAttributeValueTypeDef,
     OptInPhoneNumberInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PublishBatchResultEntryTypeDef,
+    PublishResponseTypeDef,
     PutDataProtectionPolicyInputRequestTypeDef,
     RemovePermissionInputRequestTypeDef,
     RemovePermissionInputTopicRemovePermissionTypeDef,
-    ServiceResourcePlatformApplicationRequestTypeDef,
-    ServiceResourcePlatformEndpointRequestTypeDef,
-    ServiceResourceSubscriptionRequestTypeDef,
-    ServiceResourceTopicRequestTypeDef,
+    ResponseMetadataTypeDef,
     SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef,
     SetEndpointAttributesInputRequestTypeDef,
     SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef,
     SetPlatformApplicationAttributesInputRequestTypeDef,
     SetSMSAttributesInputRequestTypeDef,
     SetSubscriptionAttributesInputRequestTypeDef,
     SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef,
     SetTopicAttributesInputRequestTypeDef,
     SetTopicAttributesInputTopicSetAttributesTypeDef,
     SubscribeInputRequestTypeDef,
     SubscribeInputTopicSubscribeTypeDef,
+    SubscribeResponseTypeDef,
     UnsubscribeInputRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VerifySMSSandboxPhoneNumberInputRequestTypeDef,
-    CheckIfPhoneNumberIsOptedOutResponseTypeDef,
-    ConfirmSubscriptionResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreatePlatformApplicationResponseTypeDef,
-    CreateTopicResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDataProtectionPolicyResponseTypeDef,
-    GetEndpointAttributesResponseTypeDef,
-    GetPlatformApplicationAttributesResponseTypeDef,
-    GetSMSAttributesResponseTypeDef,
-    GetSMSSandboxAccountStatusResultTypeDef,
-    GetSubscriptionAttributesResponseTypeDef,
-    GetTopicAttributesResponseTypeDef,
-    ListPhoneNumbersOptedOutResponseTypeDef,
-    PublishResponseTypeDef,
-    SubscribeResponseTypeDef,
     CreateTopicInputRequestTypeDef,
     CreateTopicInputServiceResourceCreateTopicTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEndpointsByPlatformApplicationResponseTypeDef,
-    ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
-    ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
-    ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
-    ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
-    ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
-    ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
-    ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
-    ListTopicsInputListTopicsPaginateTypeDef,
     ListOriginationNumbersResultTypeDef,
     ListPlatformApplicationsResponseTypeDef,
     ListSMSSandboxPhoneNumbersResultTypeDef,
     ListSubscriptionsByTopicResponseTypeDef,
     ListSubscriptionsResponseTypeDef,
     ListTopicsResponseTypeDef,
     PublishBatchRequestEntryTypeDef,
@@ -551,42 +547,42 @@
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

### Comparing `mypy-boto3-sns-1.26.69/README.md` & `mypy-boto3-sns-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sns"></a>
 
 # mypy-boto3-sns
 
 [![PyPI - mypy-boto3-sns](https://img.shields.io/pypi/v/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sns?color=blue)](https://pypistats.org/packages/mypy-boto3-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SNS 1.26.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[boto3.SNS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [mypy-boto3-sns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -405,102 +405,98 @@
 
 ```python
 from mypy_boto3_sns.type_defs import (
     AddPermissionInputRequestTypeDef,
     AddPermissionInputTopicAddPermissionTypeDef,
     BatchResultErrorEntryTypeDef,
     CheckIfPhoneNumberIsOptedOutInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CheckIfPhoneNumberIsOptedOutResponseTypeDef,
     ConfirmSubscriptionInputRequestTypeDef,
     ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
+    ConfirmSubscriptionResponseTypeDef,
+    CreateEndpointResponseTypeDef,
     CreatePlatformApplicationInputRequestTypeDef,
     CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef,
+    CreatePlatformApplicationResponseTypeDef,
     CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef,
     CreatePlatformEndpointInputRequestTypeDef,
     CreateSMSSandboxPhoneNumberInputRequestTypeDef,
     TagTypeDef,
+    CreateTopicResponseTypeDef,
     DeleteEndpointInputRequestTypeDef,
     DeletePlatformApplicationInputRequestTypeDef,
     DeleteSMSSandboxPhoneNumberInputRequestTypeDef,
     DeleteTopicInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointTypeDef,
     GetDataProtectionPolicyInputRequestTypeDef,
+    GetDataProtectionPolicyResponseTypeDef,
     GetEndpointAttributesInputRequestTypeDef,
+    GetEndpointAttributesResponseTypeDef,
     GetPlatformApplicationAttributesInputRequestTypeDef,
+    GetPlatformApplicationAttributesResponseTypeDef,
     GetSMSAttributesInputRequestTypeDef,
+    GetSMSAttributesResponseTypeDef,
+    GetSMSSandboxAccountStatusResultTypeDef,
     GetSubscriptionAttributesInputRequestTypeDef,
+    GetSubscriptionAttributesResponseTypeDef,
     GetTopicAttributesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetTopicAttributesResponseTypeDef,
+    ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
     ListEndpointsByPlatformApplicationInputRequestTypeDef,
+    ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
     ListOriginationNumbersRequestRequestTypeDef,
     PhoneNumberInformationTypeDef,
+    ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
     ListPhoneNumbersOptedOutInputRequestTypeDef,
+    ListPhoneNumbersOptedOutResponseTypeDef,
+    ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
     ListPlatformApplicationsInputRequestTypeDef,
     PlatformApplicationTypeDef,
+    ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
     ListSMSSandboxPhoneNumbersInputRequestTypeDef,
     SMSSandboxPhoneNumberTypeDef,
+    ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
     ListSubscriptionsByTopicInputRequestTypeDef,
     SubscriptionTypeDef,
+    ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
     ListSubscriptionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTopicsInputListTopicsPaginateTypeDef,
     ListTopicsInputRequestTypeDef,
     TopicTypeDef,
     MessageAttributeValueTypeDef,
     OptInPhoneNumberInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PublishBatchResultEntryTypeDef,
+    PublishResponseTypeDef,
     PutDataProtectionPolicyInputRequestTypeDef,
     RemovePermissionInputRequestTypeDef,
     RemovePermissionInputTopicRemovePermissionTypeDef,
-    ServiceResourcePlatformApplicationRequestTypeDef,
-    ServiceResourcePlatformEndpointRequestTypeDef,
-    ServiceResourceSubscriptionRequestTypeDef,
-    ServiceResourceTopicRequestTypeDef,
+    ResponseMetadataTypeDef,
     SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef,
     SetEndpointAttributesInputRequestTypeDef,
     SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef,
     SetPlatformApplicationAttributesInputRequestTypeDef,
     SetSMSAttributesInputRequestTypeDef,
     SetSubscriptionAttributesInputRequestTypeDef,
     SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef,
     SetTopicAttributesInputRequestTypeDef,
     SetTopicAttributesInputTopicSetAttributesTypeDef,
     SubscribeInputRequestTypeDef,
     SubscribeInputTopicSubscribeTypeDef,
+    SubscribeResponseTypeDef,
     UnsubscribeInputRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VerifySMSSandboxPhoneNumberInputRequestTypeDef,
-    CheckIfPhoneNumberIsOptedOutResponseTypeDef,
-    ConfirmSubscriptionResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreatePlatformApplicationResponseTypeDef,
-    CreateTopicResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDataProtectionPolicyResponseTypeDef,
-    GetEndpointAttributesResponseTypeDef,
-    GetPlatformApplicationAttributesResponseTypeDef,
-    GetSMSAttributesResponseTypeDef,
-    GetSMSSandboxAccountStatusResultTypeDef,
-    GetSubscriptionAttributesResponseTypeDef,
-    GetTopicAttributesResponseTypeDef,
-    ListPhoneNumbersOptedOutResponseTypeDef,
-    PublishResponseTypeDef,
-    SubscribeResponseTypeDef,
     CreateTopicInputRequestTypeDef,
     CreateTopicInputServiceResourceCreateTopicTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEndpointsByPlatformApplicationResponseTypeDef,
-    ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
-    ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
-    ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
-    ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
-    ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
-    ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
-    ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
-    ListTopicsInputListTopicsPaginateTypeDef,
     ListOriginationNumbersResultTypeDef,
     ListPlatformApplicationsResponseTypeDef,
     ListSMSSandboxPhoneNumbersResultTypeDef,
     ListSubscriptionsByTopicResponseTypeDef,
     ListSubscriptionsResponseTypeDef,
     ListTopicsResponseTypeDef,
     PublishBatchRequestEntryTypeDef,
@@ -519,42 +515,42 @@
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

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/__init__.py` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/__init__.pyi` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/__main__.py` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SNS 1.26.69\nVersion:         1.26.69\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.SNS 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.69")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/client.py` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,15 @@
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> PublishResponseTypeDef:
         """
         Sends a message to an Amazon SNS topic, a text message (SMS message) directly to
         a phone number, or a message to a mobile platform endpoint (when you specify the
-        `TargetArn` ).
+        `TargetArn`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Client.publish)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/client/#publish)
         """
 
     def publish_batch(
         self,
```

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/client.pyi` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -426,15 +426,15 @@
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> PublishResponseTypeDef:
         """
         Sends a message to an Amazon SNS topic, a text message (SMS message) directly to
         a phone number, or a message to a mobile platform endpoint (when you specify the
-        `TargetArn` ).
+        `TargetArn`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Client.publish)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/client/#publish)
         """
     def publish_batch(
         self,
         *,
```

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/literals.py` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
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
@@ -125,14 +126,15 @@
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
@@ -211,14 +213,15 @@
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
@@ -229,14 +232,15 @@
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
@@ -272,14 +276,15 @@
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
@@ -298,16 +303,19 @@
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
@@ -387,18 +395,21 @@
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

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/literals.pyi` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
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
@@ -123,14 +124,15 @@
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
@@ -209,14 +211,15 @@
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
@@ -227,14 +230,15 @@
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
@@ -270,14 +274,15 @@
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
@@ -296,16 +301,19 @@
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
@@ -385,18 +393,21 @@
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

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/paginator.py` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,118 +74,118 @@
 class ListEndpointsByPlatformApplicationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListEndpointsByPlatformApplication)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listendpointsbyplatformapplicationpaginator)
     """
 
     def paginate(
-        self, *, PlatformApplicationArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PlatformApplicationArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEndpointsByPlatformApplicationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListEndpointsByPlatformApplication.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listendpointsbyplatformapplicationpaginator)
         """
 
 
 class ListOriginationNumbersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListOriginationNumbers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listoriginationnumberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOriginationNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListOriginationNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listoriginationnumberspaginator)
         """
 
 
 class ListPhoneNumbersOptedOutPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPhoneNumbersOptedOut)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listphonenumbersoptedoutpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPhoneNumbersOptedOutResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPhoneNumbersOptedOut.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listphonenumbersoptedoutpaginator)
         """
 
 
 class ListPlatformApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPlatformApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listplatformapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPlatformApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPlatformApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listplatformapplicationspaginator)
         """
 
 
 class ListSMSSandboxPhoneNumbersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSMSSandboxPhoneNumbers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsmssandboxphonenumberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSMSSandboxPhoneNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSMSSandboxPhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsmssandboxphonenumberspaginator)
         """
 
 
 class ListSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionspaginator)
         """
 
 
 class ListSubscriptionsByTopicPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptionsByTopic)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionsbytopicpaginator)
     """
 
     def paginate(
-        self, *, TopicArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TopicArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSubscriptionsByTopicResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptionsByTopic.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionsbytopicpaginator)
         """
 
 
 class ListTopicsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListTopics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listtopicspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTopicsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListTopics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listtopicspaginator)
         """
```

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/paginator.pyi` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -71,111 +71,111 @@
 class ListEndpointsByPlatformApplicationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListEndpointsByPlatformApplication)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listendpointsbyplatformapplicationpaginator)
     """
 
     def paginate(
-        self, *, PlatformApplicationArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PlatformApplicationArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEndpointsByPlatformApplicationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListEndpointsByPlatformApplication.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listendpointsbyplatformapplicationpaginator)
         """
 
 class ListOriginationNumbersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListOriginationNumbers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listoriginationnumberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOriginationNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListOriginationNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listoriginationnumberspaginator)
         """
 
 class ListPhoneNumbersOptedOutPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPhoneNumbersOptedOut)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listphonenumbersoptedoutpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPhoneNumbersOptedOutResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPhoneNumbersOptedOut.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listphonenumbersoptedoutpaginator)
         """
 
 class ListPlatformApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPlatformApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listplatformapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPlatformApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPlatformApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listplatformapplicationspaginator)
         """
 
 class ListSMSSandboxPhoneNumbersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSMSSandboxPhoneNumbers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsmssandboxphonenumberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSMSSandboxPhoneNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSMSSandboxPhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsmssandboxphonenumberspaginator)
         """
 
 class ListSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionspaginator)
         """
 
 class ListSubscriptionsByTopicPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptionsByTopic)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionsbytopicpaginator)
     """
 
     def paginate(
-        self, *, TopicArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TopicArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSubscriptionsByTopicResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptionsByTopic.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionsbytopicpaginator)
         """
 
 class ListTopicsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListTopics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listtopicspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTopicsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListTopics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listtopicspaginator)
         """
```

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/service_resource.py` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> PublishResponseTypeDef:
         """
         Sends a message to an Amazon SNS topic, a text message (SMS message) directly to
         a phone number, or a message to a mobile platform endpoint (when you specify the
-        `TargetArn` ).
+        `TargetArn`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.PlatformEndpoint.publish)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/service_resource/#platformendpointpublish-method)
         """
 
     def reload(self) -> None:
         """
@@ -547,15 +547,15 @@
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> PublishResponseTypeDef:
         """
         Sends a message to an Amazon SNS topic, a text message (SMS message) directly to
         a phone number, or a message to a mobile platform endpoint (when you specify the
-        `TargetArn` ).
+        `TargetArn`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Topic.publish)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/service_resource/#topicpublish-method)
         """
 
     def reload(self) -> None:
         """
```

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/service_resource.pyi` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> PublishResponseTypeDef:
         """
         Sends a message to an Amazon SNS topic, a text message (SMS message) directly to
         a phone number, or a message to a mobile platform endpoint (when you specify the
-        `TargetArn` ).
+        `TargetArn`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.PlatformEndpoint.publish)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/service_resource/#platformendpointpublish-method)
         """
     def reload(self) -> None:
         """
         Calls :py:meth:`SNS.Client.get_endpoint_attributes` to update the attributes of
@@ -491,15 +491,15 @@
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> PublishResponseTypeDef:
         """
         Sends a message to an Amazon SNS topic, a text message (SMS message) directly to
         a phone number, or a message to a mobile platform endpoint (when you specify the
-        `TargetArn` ).
+        `TargetArn`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Topic.publish)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/service_resource/#topicpublish-method)
         """
     def reload(self) -> None:
         """
         Calls :py:meth:`SNS.Client.get_topic_attributes` to update the attributes of the
```

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/type_defs.py` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,102 +31,98 @@
 
 
 __all__ = (
     "AddPermissionInputRequestTypeDef",
     "AddPermissionInputTopicAddPermissionTypeDef",
     "BatchResultErrorEntryTypeDef",
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
     "ConfirmSubscriptionInputRequestTypeDef",
     "ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef",
+    "ConfirmSubscriptionResponseTypeDef",
+    "CreateEndpointResponseTypeDef",
     "CreatePlatformApplicationInputRequestTypeDef",
     "CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef",
+    "CreatePlatformApplicationResponseTypeDef",
     "CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef",
     "CreatePlatformEndpointInputRequestTypeDef",
     "CreateSMSSandboxPhoneNumberInputRequestTypeDef",
     "TagTypeDef",
+    "CreateTopicResponseTypeDef",
     "DeleteEndpointInputRequestTypeDef",
     "DeletePlatformApplicationInputRequestTypeDef",
     "DeleteSMSSandboxPhoneNumberInputRequestTypeDef",
     "DeleteTopicInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EndpointTypeDef",
     "GetDataProtectionPolicyInputRequestTypeDef",
+    "GetDataProtectionPolicyResponseTypeDef",
     "GetEndpointAttributesInputRequestTypeDef",
+    "GetEndpointAttributesResponseTypeDef",
     "GetPlatformApplicationAttributesInputRequestTypeDef",
+    "GetPlatformApplicationAttributesResponseTypeDef",
     "GetSMSAttributesInputRequestTypeDef",
+    "GetSMSAttributesResponseTypeDef",
+    "GetSMSSandboxAccountStatusResultTypeDef",
     "GetSubscriptionAttributesInputRequestTypeDef",
+    "GetSubscriptionAttributesResponseTypeDef",
     "GetTopicAttributesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetTopicAttributesResponseTypeDef",
+    "ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
     "ListEndpointsByPlatformApplicationInputRequestTypeDef",
+    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
     "ListOriginationNumbersRequestRequestTypeDef",
     "PhoneNumberInformationTypeDef",
+    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
     "ListPhoneNumbersOptedOutInputRequestTypeDef",
+    "ListPhoneNumbersOptedOutResponseTypeDef",
+    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
     "ListPlatformApplicationsInputRequestTypeDef",
     "PlatformApplicationTypeDef",
+    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
     "ListSMSSandboxPhoneNumbersInputRequestTypeDef",
     "SMSSandboxPhoneNumberTypeDef",
+    "ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
     "ListSubscriptionsByTopicInputRequestTypeDef",
     "SubscriptionTypeDef",
+    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
     "ListSubscriptionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTopicsInputListTopicsPaginateTypeDef",
     "ListTopicsInputRequestTypeDef",
     "TopicTypeDef",
     "MessageAttributeValueTypeDef",
     "OptInPhoneNumberInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PublishBatchResultEntryTypeDef",
+    "PublishResponseTypeDef",
     "PutDataProtectionPolicyInputRequestTypeDef",
     "RemovePermissionInputRequestTypeDef",
     "RemovePermissionInputTopicRemovePermissionTypeDef",
-    "ServiceResourcePlatformApplicationRequestTypeDef",
-    "ServiceResourcePlatformEndpointRequestTypeDef",
-    "ServiceResourceSubscriptionRequestTypeDef",
-    "ServiceResourceTopicRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef",
     "SetEndpointAttributesInputRequestTypeDef",
     "SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef",
     "SetPlatformApplicationAttributesInputRequestTypeDef",
     "SetSMSAttributesInputRequestTypeDef",
     "SetSubscriptionAttributesInputRequestTypeDef",
     "SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef",
     "SetTopicAttributesInputRequestTypeDef",
     "SetTopicAttributesInputTopicSetAttributesTypeDef",
     "SubscribeInputRequestTypeDef",
     "SubscribeInputTopicSubscribeTypeDef",
+    "SubscribeResponseTypeDef",
     "UnsubscribeInputRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VerifySMSSandboxPhoneNumberInputRequestTypeDef",
-    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
-    "ConfirmSubscriptionResponseTypeDef",
-    "CreateEndpointResponseTypeDef",
-    "CreatePlatformApplicationResponseTypeDef",
-    "CreateTopicResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDataProtectionPolicyResponseTypeDef",
-    "GetEndpointAttributesResponseTypeDef",
-    "GetPlatformApplicationAttributesResponseTypeDef",
-    "GetSMSAttributesResponseTypeDef",
-    "GetSMSSandboxAccountStatusResultTypeDef",
-    "GetSubscriptionAttributesResponseTypeDef",
-    "GetTopicAttributesResponseTypeDef",
-    "ListPhoneNumbersOptedOutResponseTypeDef",
-    "PublishResponseTypeDef",
-    "SubscribeResponseTypeDef",
     "CreateTopicInputRequestTypeDef",
     "CreateTopicInputServiceResourceCreateTopicTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEndpointsByPlatformApplicationResponseTypeDef",
-    "ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
-    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
-    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
-    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
-    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
-    "ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
-    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
-    "ListTopicsInputListTopicsPaginateTypeDef",
     "ListOriginationNumbersResultTypeDef",
     "ListPlatformApplicationsResponseTypeDef",
     "ListSMSSandboxPhoneNumbersResultTypeDef",
     "ListSubscriptionsByTopicResponseTypeDef",
     "ListSubscriptionsResponseTypeDef",
     "ListTopicsResponseTypeDef",
     "PublishBatchRequestEntryTypeDef",
@@ -182,22 +178,19 @@
 CheckIfPhoneNumberIsOptedOutInputRequestTypeDef = TypedDict(
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
     {
         "phoneNumber": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CheckIfPhoneNumberIsOptedOutResponseTypeDef = TypedDict(
+    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "isOptedOut": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredConfirmSubscriptionInputRequestTypeDef = TypedDict(
     "_RequiredConfirmSubscriptionInputRequestTypeDef",
     {
         "TopicArn": str,
@@ -237,14 +230,30 @@
 class ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef(
     _RequiredConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
     _OptionalConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
 ):
     pass
 
 
+ConfirmSubscriptionResponseTypeDef = TypedDict(
+    "ConfirmSubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateEndpointResponseTypeDef = TypedDict(
+    "CreateEndpointResponseTypeDef",
+    {
+        "EndpointArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreatePlatformApplicationInputRequestTypeDef = TypedDict(
     "CreatePlatformApplicationInputRequestTypeDef",
     {
         "Name": str,
         "Platform": str,
         "Attributes": Mapping[str, str],
     },
@@ -255,14 +264,22 @@
     {
         "Name": str,
         "Platform": str,
         "Attributes": Mapping[str, str],
     },
 )
 
+CreatePlatformApplicationResponseTypeDef = TypedDict(
+    "CreatePlatformApplicationResponseTypeDef",
+    {
+        "PlatformApplicationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef = TypedDict(
     "_RequiredCreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef",
     {
         "Token": str,
     },
 )
 _OptionalCreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef = TypedDict(
@@ -332,14 +349,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateTopicResponseTypeDef = TypedDict(
+    "CreateTopicResponseTypeDef",
+    {
+        "TopicArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEndpointInputRequestTypeDef = TypedDict(
     "DeleteEndpointInputRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 
@@ -360,14 +385,21 @@
 DeleteTopicInputRequestTypeDef = TypedDict(
     "DeleteTopicInputRequestTypeDef",
     {
         "TopicArn": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "EndpointArn": str,
         "Attributes": Dict[str, str],
     },
     total=False,
@@ -376,60 +408,128 @@
 GetDataProtectionPolicyInputRequestTypeDef = TypedDict(
     "GetDataProtectionPolicyInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+GetDataProtectionPolicyResponseTypeDef = TypedDict(
+    "GetDataProtectionPolicyResponseTypeDef",
+    {
+        "DataProtectionPolicy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetEndpointAttributesInputRequestTypeDef = TypedDict(
     "GetEndpointAttributesInputRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 
+GetEndpointAttributesResponseTypeDef = TypedDict(
+    "GetEndpointAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPlatformApplicationAttributesInputRequestTypeDef = TypedDict(
     "GetPlatformApplicationAttributesInputRequestTypeDef",
     {
         "PlatformApplicationArn": str,
     },
 )
 
+GetPlatformApplicationAttributesResponseTypeDef = TypedDict(
+    "GetPlatformApplicationAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSMSAttributesInputRequestTypeDef = TypedDict(
     "GetSMSAttributesInputRequestTypeDef",
     {
         "attributes": Sequence[str],
     },
     total=False,
 )
 
+GetSMSAttributesResponseTypeDef = TypedDict(
+    "GetSMSAttributesResponseTypeDef",
+    {
+        "attributes": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSMSSandboxAccountStatusResultTypeDef = TypedDict(
+    "GetSMSSandboxAccountStatusResultTypeDef",
+    {
+        "IsInSandbox": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSubscriptionAttributesInputRequestTypeDef = TypedDict(
     "GetSubscriptionAttributesInputRequestTypeDef",
     {
         "SubscriptionArn": str,
     },
 )
 
+GetSubscriptionAttributesResponseTypeDef = TypedDict(
+    "GetSubscriptionAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTopicAttributesInputRequestTypeDef = TypedDict(
     "GetTopicAttributesInputRequestTypeDef",
     {
         "TopicArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetTopicAttributesResponseTypeDef = TypedDict(
+    "GetTopicAttributesResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
+    "_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
+    {
+        "PlatformApplicationArn": str,
+    },
+)
+_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
+    "_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef(
+    _RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+    _OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEndpointsByPlatformApplicationInputRequestTypeDef = TypedDict(
     "_RequiredListEndpointsByPlatformApplicationInputRequestTypeDef",
     {
         "PlatformApplicationArn": str,
     },
 )
 _OptionalListEndpointsByPlatformApplicationInputRequestTypeDef = TypedDict(
@@ -444,14 +544,22 @@
 class ListEndpointsByPlatformApplicationInputRequestTypeDef(
     _RequiredListEndpointsByPlatformApplicationInputRequestTypeDef,
     _OptionalListEndpointsByPlatformApplicationInputRequestTypeDef,
 ):
     pass
 
 
+ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef = TypedDict(
+    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOriginationNumbersRequestRequestTypeDef = TypedDict(
     "ListOriginationNumbersRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -466,22 +574,47 @@
         "Iso2CountryCode": str,
         "RouteType": RouteTypeType,
         "NumberCapabilities": List[NumberCapabilityType],
     },
     total=False,
 )
 
+ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef = TypedDict(
+    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPhoneNumbersOptedOutInputRequestTypeDef = TypedDict(
     "ListPhoneNumbersOptedOutInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+ListPhoneNumbersOptedOutResponseTypeDef = TypedDict(
+    "ListPhoneNumbersOptedOutResponseTypeDef",
+    {
+        "phoneNumbers": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef = TypedDict(
+    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPlatformApplicationsInputRequestTypeDef = TypedDict(
     "ListPlatformApplicationsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -491,14 +624,22 @@
     {
         "PlatformApplicationArn": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
+ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef = TypedDict(
+    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSMSSandboxPhoneNumbersInputRequestTypeDef = TypedDict(
     "ListSMSSandboxPhoneNumbersInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -509,14 +650,36 @@
     {
         "PhoneNumber": str,
         "Status": SMSSandboxPhoneNumberVerificationStatusType,
     },
     total=False,
 )
 
+_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
+    "_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
+    {
+        "TopicArn": str,
+    },
+)
+_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
+    "_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef(
+    _RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
+    _OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSubscriptionsByTopicInputRequestTypeDef = TypedDict(
     "_RequiredListSubscriptionsByTopicInputRequestTypeDef",
     {
         "TopicArn": str,
     },
 )
 _OptionalListSubscriptionsByTopicInputRequestTypeDef = TypedDict(
@@ -543,14 +706,22 @@
         "Protocol": str,
         "Endpoint": str,
         "TopicArn": str,
     },
     total=False,
 )
 
+ListSubscriptionsInputListSubscriptionsPaginateTypeDef = TypedDict(
+    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSubscriptionsInputRequestTypeDef = TypedDict(
     "ListSubscriptionsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -558,14 +729,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTopicsInputListTopicsPaginateTypeDef = TypedDict(
+    "ListTopicsInputListTopicsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTopicsInputRequestTypeDef = TypedDict(
     "ListTopicsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -603,24 +782,43 @@
 OptInPhoneNumberInputRequestTypeDef = TypedDict(
     "OptInPhoneNumberInputRequestTypeDef",
     {
         "phoneNumber": str,
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
 PublishBatchResultEntryTypeDef = TypedDict(
     "PublishBatchResultEntryTypeDef",
     {
         "Id": str,
         "MessageId": str,
         "SequenceNumber": str,
     },
     total=False,
 )
 
+PublishResponseTypeDef = TypedDict(
+    "PublishResponseTypeDef",
+    {
+        "MessageId": str,
+        "SequenceNumber": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutDataProtectionPolicyInputRequestTypeDef = TypedDict(
     "PutDataProtectionPolicyInputRequestTypeDef",
     {
         "ResourceArn": str,
         "DataProtectionPolicy": str,
     },
 )
@@ -636,39 +834,22 @@
 RemovePermissionInputTopicRemovePermissionTypeDef = TypedDict(
     "RemovePermissionInputTopicRemovePermissionTypeDef",
     {
         "Label": str,
     },
 )
 
-ServiceResourcePlatformApplicationRequestTypeDef = TypedDict(
-    "ServiceResourcePlatformApplicationRequestTypeDef",
-    {
-        "arn": str,
-    },
-)
-
-ServiceResourcePlatformEndpointRequestTypeDef = TypedDict(
-    "ServiceResourcePlatformEndpointRequestTypeDef",
-    {
-        "arn": str,
-    },
-)
-
-ServiceResourceSubscriptionRequestTypeDef = TypedDict(
-    "ServiceResourceSubscriptionRequestTypeDef",
-    {
-        "arn": str,
-    },
-)
-
-ServiceResourceTopicRequestTypeDef = TypedDict(
-    "ServiceResourceTopicRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef = TypedDict(
     "SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef",
     {
         "Attributes": Mapping[str, str],
@@ -837,14 +1018,22 @@
 
 class SubscribeInputTopicSubscribeTypeDef(
     _RequiredSubscribeInputTopicSubscribeTypeDef, _OptionalSubscribeInputTopicSubscribeTypeDef
 ):
     pass
 
 
+SubscribeResponseTypeDef = TypedDict(
+    "SubscribeResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UnsubscribeInputRequestTypeDef = TypedDict(
     "UnsubscribeInputRequestTypeDef",
     {
         "SubscriptionArn": str,
     },
 )
 
@@ -860,143 +1049,14 @@
     "VerifySMSSandboxPhoneNumberInputRequestTypeDef",
     {
         "PhoneNumber": str,
         "OneTimePassword": str,
     },
 )
 
-CheckIfPhoneNumberIsOptedOutResponseTypeDef = TypedDict(
-    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
-    {
-        "isOptedOut": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfirmSubscriptionResponseTypeDef = TypedDict(
-    "ConfirmSubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEndpointResponseTypeDef = TypedDict(
-    "CreateEndpointResponseTypeDef",
-    {
-        "EndpointArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePlatformApplicationResponseTypeDef = TypedDict(
-    "CreatePlatformApplicationResponseTypeDef",
-    {
-        "PlatformApplicationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTopicResponseTypeDef = TypedDict(
-    "CreateTopicResponseTypeDef",
-    {
-        "TopicArn": str,
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
-GetDataProtectionPolicyResponseTypeDef = TypedDict(
-    "GetDataProtectionPolicyResponseTypeDef",
-    {
-        "DataProtectionPolicy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetEndpointAttributesResponseTypeDef = TypedDict(
-    "GetEndpointAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPlatformApplicationAttributesResponseTypeDef = TypedDict(
-    "GetPlatformApplicationAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSMSAttributesResponseTypeDef = TypedDict(
-    "GetSMSAttributesResponseTypeDef",
-    {
-        "attributes": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSMSSandboxAccountStatusResultTypeDef = TypedDict(
-    "GetSMSSandboxAccountStatusResultTypeDef",
-    {
-        "IsInSandbox": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSubscriptionAttributesResponseTypeDef = TypedDict(
-    "GetSubscriptionAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTopicAttributesResponseTypeDef = TypedDict(
-    "GetTopicAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPhoneNumbersOptedOutResponseTypeDef = TypedDict(
-    "ListPhoneNumbersOptedOutResponseTypeDef",
-    {
-        "phoneNumbers": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PublishResponseTypeDef = TypedDict(
-    "PublishResponseTypeDef",
-    {
-        "MessageId": str,
-        "SequenceNumber": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SubscribeResponseTypeDef = TypedDict(
-    "SubscribeResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateTopicInputRequestTypeDef = TypedDict(
     "_RequiredCreateTopicInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateTopicInputRequestTypeDef = TypedDict(
@@ -1040,15 +1100,15 @@
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
@@ -1057,161 +1117,69 @@
 )
 
 ListEndpointsByPlatformApplicationResponseTypeDef = TypedDict(
     "ListEndpointsByPlatformApplicationResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
-    "_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
-    {
-        "PlatformApplicationArn": str,
-    },
-)
-_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
-    "_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-
-class ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef(
-    _RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
-    _OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
-):
-    pass
-
-
-ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef = TypedDict(
-    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef = TypedDict(
-    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef = TypedDict(
-    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef = TypedDict(
-    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
-    "_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
-    "_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef(
-    _RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
-    _OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
-):
-    pass
-
-
-ListSubscriptionsInputListSubscriptionsPaginateTypeDef = TypedDict(
-    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTopicsInputListTopicsPaginateTypeDef = TypedDict(
-    "ListTopicsInputListTopicsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListOriginationNumbersResultTypeDef = TypedDict(
     "ListOriginationNumbersResultTypeDef",
     {
         "NextToken": str,
         "PhoneNumbers": List[PhoneNumberInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPlatformApplicationsResponseTypeDef = TypedDict(
     "ListPlatformApplicationsResponseTypeDef",
     {
         "PlatformApplications": List[PlatformApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSMSSandboxPhoneNumbersResultTypeDef = TypedDict(
     "ListSMSSandboxPhoneNumbersResultTypeDef",
     {
         "PhoneNumbers": List[SMSSandboxPhoneNumberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSubscriptionsByTopicResponseTypeDef = TypedDict(
     "ListSubscriptionsByTopicResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSubscriptionsResponseTypeDef = TypedDict(
     "ListSubscriptionsResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTopicsResponseTypeDef = TypedDict(
     "ListTopicsResponseTypeDef",
     {
         "Topics": List[TopicTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPublishBatchRequestEntryTypeDef = TypedDict(
     "_RequiredPublishBatchRequestEntryTypeDef",
     {
         "Id": str,
@@ -1321,15 +1289,15 @@
 
 
 PublishBatchResponseTypeDef = TypedDict(
     "PublishBatchResponseTypeDef",
     {
         "Successful": List[PublishBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PublishBatchInputRequestTypeDef = TypedDict(
     "PublishBatchInputRequestTypeDef",
     {
         "TopicArn": str,
```

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns/type_defs.pyi` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -30,102 +30,98 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddPermissionInputRequestTypeDef",
     "AddPermissionInputTopicAddPermissionTypeDef",
     "BatchResultErrorEntryTypeDef",
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
     "ConfirmSubscriptionInputRequestTypeDef",
     "ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef",
+    "ConfirmSubscriptionResponseTypeDef",
+    "CreateEndpointResponseTypeDef",
     "CreatePlatformApplicationInputRequestTypeDef",
     "CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef",
+    "CreatePlatformApplicationResponseTypeDef",
     "CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef",
     "CreatePlatformEndpointInputRequestTypeDef",
     "CreateSMSSandboxPhoneNumberInputRequestTypeDef",
     "TagTypeDef",
+    "CreateTopicResponseTypeDef",
     "DeleteEndpointInputRequestTypeDef",
     "DeletePlatformApplicationInputRequestTypeDef",
     "DeleteSMSSandboxPhoneNumberInputRequestTypeDef",
     "DeleteTopicInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EndpointTypeDef",
     "GetDataProtectionPolicyInputRequestTypeDef",
+    "GetDataProtectionPolicyResponseTypeDef",
     "GetEndpointAttributesInputRequestTypeDef",
+    "GetEndpointAttributesResponseTypeDef",
     "GetPlatformApplicationAttributesInputRequestTypeDef",
+    "GetPlatformApplicationAttributesResponseTypeDef",
     "GetSMSAttributesInputRequestTypeDef",
+    "GetSMSAttributesResponseTypeDef",
+    "GetSMSSandboxAccountStatusResultTypeDef",
     "GetSubscriptionAttributesInputRequestTypeDef",
+    "GetSubscriptionAttributesResponseTypeDef",
     "GetTopicAttributesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetTopicAttributesResponseTypeDef",
+    "ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
     "ListEndpointsByPlatformApplicationInputRequestTypeDef",
+    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
     "ListOriginationNumbersRequestRequestTypeDef",
     "PhoneNumberInformationTypeDef",
+    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
     "ListPhoneNumbersOptedOutInputRequestTypeDef",
+    "ListPhoneNumbersOptedOutResponseTypeDef",
+    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
     "ListPlatformApplicationsInputRequestTypeDef",
     "PlatformApplicationTypeDef",
+    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
     "ListSMSSandboxPhoneNumbersInputRequestTypeDef",
     "SMSSandboxPhoneNumberTypeDef",
+    "ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
     "ListSubscriptionsByTopicInputRequestTypeDef",
     "SubscriptionTypeDef",
+    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
     "ListSubscriptionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTopicsInputListTopicsPaginateTypeDef",
     "ListTopicsInputRequestTypeDef",
     "TopicTypeDef",
     "MessageAttributeValueTypeDef",
     "OptInPhoneNumberInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PublishBatchResultEntryTypeDef",
+    "PublishResponseTypeDef",
     "PutDataProtectionPolicyInputRequestTypeDef",
     "RemovePermissionInputRequestTypeDef",
     "RemovePermissionInputTopicRemovePermissionTypeDef",
-    "ServiceResourcePlatformApplicationRequestTypeDef",
-    "ServiceResourcePlatformEndpointRequestTypeDef",
-    "ServiceResourceSubscriptionRequestTypeDef",
-    "ServiceResourceTopicRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef",
     "SetEndpointAttributesInputRequestTypeDef",
     "SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef",
     "SetPlatformApplicationAttributesInputRequestTypeDef",
     "SetSMSAttributesInputRequestTypeDef",
     "SetSubscriptionAttributesInputRequestTypeDef",
     "SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef",
     "SetTopicAttributesInputRequestTypeDef",
     "SetTopicAttributesInputTopicSetAttributesTypeDef",
     "SubscribeInputRequestTypeDef",
     "SubscribeInputTopicSubscribeTypeDef",
+    "SubscribeResponseTypeDef",
     "UnsubscribeInputRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VerifySMSSandboxPhoneNumberInputRequestTypeDef",
-    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
-    "ConfirmSubscriptionResponseTypeDef",
-    "CreateEndpointResponseTypeDef",
-    "CreatePlatformApplicationResponseTypeDef",
-    "CreateTopicResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDataProtectionPolicyResponseTypeDef",
-    "GetEndpointAttributesResponseTypeDef",
-    "GetPlatformApplicationAttributesResponseTypeDef",
-    "GetSMSAttributesResponseTypeDef",
-    "GetSMSSandboxAccountStatusResultTypeDef",
-    "GetSubscriptionAttributesResponseTypeDef",
-    "GetTopicAttributesResponseTypeDef",
-    "ListPhoneNumbersOptedOutResponseTypeDef",
-    "PublishResponseTypeDef",
-    "SubscribeResponseTypeDef",
     "CreateTopicInputRequestTypeDef",
     "CreateTopicInputServiceResourceCreateTopicTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEndpointsByPlatformApplicationResponseTypeDef",
-    "ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
-    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
-    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
-    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
-    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
-    "ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
-    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
-    "ListTopicsInputListTopicsPaginateTypeDef",
     "ListOriginationNumbersResultTypeDef",
     "ListPlatformApplicationsResponseTypeDef",
     "ListSMSSandboxPhoneNumbersResultTypeDef",
     "ListSubscriptionsByTopicResponseTypeDef",
     "ListSubscriptionsResponseTypeDef",
     "ListTopicsResponseTypeDef",
     "PublishBatchRequestEntryTypeDef",
@@ -179,22 +175,19 @@
 CheckIfPhoneNumberIsOptedOutInputRequestTypeDef = TypedDict(
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
     {
         "phoneNumber": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CheckIfPhoneNumberIsOptedOutResponseTypeDef = TypedDict(
+    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "isOptedOut": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredConfirmSubscriptionInputRequestTypeDef = TypedDict(
     "_RequiredConfirmSubscriptionInputRequestTypeDef",
     {
         "TopicArn": str,
@@ -230,14 +223,30 @@
 
 class ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef(
     _RequiredConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
     _OptionalConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
 ):
     pass
 
+ConfirmSubscriptionResponseTypeDef = TypedDict(
+    "ConfirmSubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateEndpointResponseTypeDef = TypedDict(
+    "CreateEndpointResponseTypeDef",
+    {
+        "EndpointArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreatePlatformApplicationInputRequestTypeDef = TypedDict(
     "CreatePlatformApplicationInputRequestTypeDef",
     {
         "Name": str,
         "Platform": str,
         "Attributes": Mapping[str, str],
     },
@@ -248,14 +257,22 @@
     {
         "Name": str,
         "Platform": str,
         "Attributes": Mapping[str, str],
     },
 )
 
+CreatePlatformApplicationResponseTypeDef = TypedDict(
+    "CreatePlatformApplicationResponseTypeDef",
+    {
+        "PlatformApplicationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef = TypedDict(
     "_RequiredCreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef",
     {
         "Token": str,
     },
 )
 _OptionalCreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef = TypedDict(
@@ -319,14 +336,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateTopicResponseTypeDef = TypedDict(
+    "CreateTopicResponseTypeDef",
+    {
+        "TopicArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEndpointInputRequestTypeDef = TypedDict(
     "DeleteEndpointInputRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 
@@ -347,14 +372,21 @@
 DeleteTopicInputRequestTypeDef = TypedDict(
     "DeleteTopicInputRequestTypeDef",
     {
         "TopicArn": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "EndpointArn": str,
         "Attributes": Dict[str, str],
     },
     total=False,
@@ -363,60 +395,126 @@
 GetDataProtectionPolicyInputRequestTypeDef = TypedDict(
     "GetDataProtectionPolicyInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+GetDataProtectionPolicyResponseTypeDef = TypedDict(
+    "GetDataProtectionPolicyResponseTypeDef",
+    {
+        "DataProtectionPolicy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetEndpointAttributesInputRequestTypeDef = TypedDict(
     "GetEndpointAttributesInputRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 
+GetEndpointAttributesResponseTypeDef = TypedDict(
+    "GetEndpointAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPlatformApplicationAttributesInputRequestTypeDef = TypedDict(
     "GetPlatformApplicationAttributesInputRequestTypeDef",
     {
         "PlatformApplicationArn": str,
     },
 )
 
+GetPlatformApplicationAttributesResponseTypeDef = TypedDict(
+    "GetPlatformApplicationAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSMSAttributesInputRequestTypeDef = TypedDict(
     "GetSMSAttributesInputRequestTypeDef",
     {
         "attributes": Sequence[str],
     },
     total=False,
 )
 
+GetSMSAttributesResponseTypeDef = TypedDict(
+    "GetSMSAttributesResponseTypeDef",
+    {
+        "attributes": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSMSSandboxAccountStatusResultTypeDef = TypedDict(
+    "GetSMSSandboxAccountStatusResultTypeDef",
+    {
+        "IsInSandbox": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSubscriptionAttributesInputRequestTypeDef = TypedDict(
     "GetSubscriptionAttributesInputRequestTypeDef",
     {
         "SubscriptionArn": str,
     },
 )
 
+GetSubscriptionAttributesResponseTypeDef = TypedDict(
+    "GetSubscriptionAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTopicAttributesInputRequestTypeDef = TypedDict(
     "GetTopicAttributesInputRequestTypeDef",
     {
         "TopicArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetTopicAttributesResponseTypeDef = TypedDict(
+    "GetTopicAttributesResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
+    "_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
+    {
+        "PlatformApplicationArn": str,
+    },
+)
+_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
+    "_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef(
+    _RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+    _OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+):
+    pass
+
 _RequiredListEndpointsByPlatformApplicationInputRequestTypeDef = TypedDict(
     "_RequiredListEndpointsByPlatformApplicationInputRequestTypeDef",
     {
         "PlatformApplicationArn": str,
     },
 )
 _OptionalListEndpointsByPlatformApplicationInputRequestTypeDef = TypedDict(
@@ -429,14 +527,22 @@
 
 class ListEndpointsByPlatformApplicationInputRequestTypeDef(
     _RequiredListEndpointsByPlatformApplicationInputRequestTypeDef,
     _OptionalListEndpointsByPlatformApplicationInputRequestTypeDef,
 ):
     pass
 
+ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef = TypedDict(
+    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOriginationNumbersRequestRequestTypeDef = TypedDict(
     "ListOriginationNumbersRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -451,22 +557,47 @@
         "Iso2CountryCode": str,
         "RouteType": RouteTypeType,
         "NumberCapabilities": List[NumberCapabilityType],
     },
     total=False,
 )
 
+ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef = TypedDict(
+    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPhoneNumbersOptedOutInputRequestTypeDef = TypedDict(
     "ListPhoneNumbersOptedOutInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+ListPhoneNumbersOptedOutResponseTypeDef = TypedDict(
+    "ListPhoneNumbersOptedOutResponseTypeDef",
+    {
+        "phoneNumbers": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef = TypedDict(
+    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPlatformApplicationsInputRequestTypeDef = TypedDict(
     "ListPlatformApplicationsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -476,14 +607,22 @@
     {
         "PlatformApplicationArn": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
+ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef = TypedDict(
+    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSMSSandboxPhoneNumbersInputRequestTypeDef = TypedDict(
     "ListSMSSandboxPhoneNumbersInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -494,14 +633,34 @@
     {
         "PhoneNumber": str,
         "Status": SMSSandboxPhoneNumberVerificationStatusType,
     },
     total=False,
 )
 
+_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
+    "_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
+    {
+        "TopicArn": str,
+    },
+)
+_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
+    "_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef(
+    _RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
+    _OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
+):
+    pass
+
 _RequiredListSubscriptionsByTopicInputRequestTypeDef = TypedDict(
     "_RequiredListSubscriptionsByTopicInputRequestTypeDef",
     {
         "TopicArn": str,
     },
 )
 _OptionalListSubscriptionsByTopicInputRequestTypeDef = TypedDict(
@@ -526,14 +685,22 @@
         "Protocol": str,
         "Endpoint": str,
         "TopicArn": str,
     },
     total=False,
 )
 
+ListSubscriptionsInputListSubscriptionsPaginateTypeDef = TypedDict(
+    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSubscriptionsInputRequestTypeDef = TypedDict(
     "ListSubscriptionsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -541,14 +708,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTopicsInputListTopicsPaginateTypeDef = TypedDict(
+    "ListTopicsInputListTopicsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTopicsInputRequestTypeDef = TypedDict(
     "ListTopicsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -584,24 +759,43 @@
 OptInPhoneNumberInputRequestTypeDef = TypedDict(
     "OptInPhoneNumberInputRequestTypeDef",
     {
         "phoneNumber": str,
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
 PublishBatchResultEntryTypeDef = TypedDict(
     "PublishBatchResultEntryTypeDef",
     {
         "Id": str,
         "MessageId": str,
         "SequenceNumber": str,
     },
     total=False,
 )
 
+PublishResponseTypeDef = TypedDict(
+    "PublishResponseTypeDef",
+    {
+        "MessageId": str,
+        "SequenceNumber": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutDataProtectionPolicyInputRequestTypeDef = TypedDict(
     "PutDataProtectionPolicyInputRequestTypeDef",
     {
         "ResourceArn": str,
         "DataProtectionPolicy": str,
     },
 )
@@ -617,39 +811,22 @@
 RemovePermissionInputTopicRemovePermissionTypeDef = TypedDict(
     "RemovePermissionInputTopicRemovePermissionTypeDef",
     {
         "Label": str,
     },
 )
 
-ServiceResourcePlatformApplicationRequestTypeDef = TypedDict(
-    "ServiceResourcePlatformApplicationRequestTypeDef",
-    {
-        "arn": str,
-    },
-)
-
-ServiceResourcePlatformEndpointRequestTypeDef = TypedDict(
-    "ServiceResourcePlatformEndpointRequestTypeDef",
-    {
-        "arn": str,
-    },
-)
-
-ServiceResourceSubscriptionRequestTypeDef = TypedDict(
-    "ServiceResourceSubscriptionRequestTypeDef",
-    {
-        "arn": str,
-    },
-)
-
-ServiceResourceTopicRequestTypeDef = TypedDict(
-    "ServiceResourceTopicRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef = TypedDict(
     "SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef",
     {
         "Attributes": Mapping[str, str],
@@ -806,14 +983,22 @@
 )
 
 class SubscribeInputTopicSubscribeTypeDef(
     _RequiredSubscribeInputTopicSubscribeTypeDef, _OptionalSubscribeInputTopicSubscribeTypeDef
 ):
     pass
 
+SubscribeResponseTypeDef = TypedDict(
+    "SubscribeResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UnsubscribeInputRequestTypeDef = TypedDict(
     "UnsubscribeInputRequestTypeDef",
     {
         "SubscriptionArn": str,
     },
 )
 
@@ -829,143 +1014,14 @@
     "VerifySMSSandboxPhoneNumberInputRequestTypeDef",
     {
         "PhoneNumber": str,
         "OneTimePassword": str,
     },
 )
 
-CheckIfPhoneNumberIsOptedOutResponseTypeDef = TypedDict(
-    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
-    {
-        "isOptedOut": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfirmSubscriptionResponseTypeDef = TypedDict(
-    "ConfirmSubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEndpointResponseTypeDef = TypedDict(
-    "CreateEndpointResponseTypeDef",
-    {
-        "EndpointArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePlatformApplicationResponseTypeDef = TypedDict(
-    "CreatePlatformApplicationResponseTypeDef",
-    {
-        "PlatformApplicationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTopicResponseTypeDef = TypedDict(
-    "CreateTopicResponseTypeDef",
-    {
-        "TopicArn": str,
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
-GetDataProtectionPolicyResponseTypeDef = TypedDict(
-    "GetDataProtectionPolicyResponseTypeDef",
-    {
-        "DataProtectionPolicy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetEndpointAttributesResponseTypeDef = TypedDict(
-    "GetEndpointAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPlatformApplicationAttributesResponseTypeDef = TypedDict(
-    "GetPlatformApplicationAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSMSAttributesResponseTypeDef = TypedDict(
-    "GetSMSAttributesResponseTypeDef",
-    {
-        "attributes": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSMSSandboxAccountStatusResultTypeDef = TypedDict(
-    "GetSMSSandboxAccountStatusResultTypeDef",
-    {
-        "IsInSandbox": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSubscriptionAttributesResponseTypeDef = TypedDict(
-    "GetSubscriptionAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTopicAttributesResponseTypeDef = TypedDict(
-    "GetTopicAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPhoneNumbersOptedOutResponseTypeDef = TypedDict(
-    "ListPhoneNumbersOptedOutResponseTypeDef",
-    {
-        "phoneNumbers": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PublishResponseTypeDef = TypedDict(
-    "PublishResponseTypeDef",
-    {
-        "MessageId": str,
-        "SequenceNumber": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SubscribeResponseTypeDef = TypedDict(
-    "SubscribeResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateTopicInputRequestTypeDef = TypedDict(
     "_RequiredCreateTopicInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateTopicInputRequestTypeDef = TypedDict(
@@ -1005,15 +1061,15 @@
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
@@ -1022,157 +1078,69 @@
 )
 
 ListEndpointsByPlatformApplicationResponseTypeDef = TypedDict(
     "ListEndpointsByPlatformApplicationResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
-    "_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
-    {
-        "PlatformApplicationArn": str,
-    },
-)
-_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
-    "_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef(
-    _RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
-    _OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
-):
-    pass
-
-ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef = TypedDict(
-    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef = TypedDict(
-    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef = TypedDict(
-    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef = TypedDict(
-    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
-    "_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
-    "_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef(
-    _RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
-    _OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
-):
-    pass
-
-ListSubscriptionsInputListSubscriptionsPaginateTypeDef = TypedDict(
-    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTopicsInputListTopicsPaginateTypeDef = TypedDict(
-    "ListTopicsInputListTopicsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListOriginationNumbersResultTypeDef = TypedDict(
     "ListOriginationNumbersResultTypeDef",
     {
         "NextToken": str,
         "PhoneNumbers": List[PhoneNumberInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPlatformApplicationsResponseTypeDef = TypedDict(
     "ListPlatformApplicationsResponseTypeDef",
     {
         "PlatformApplications": List[PlatformApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSMSSandboxPhoneNumbersResultTypeDef = TypedDict(
     "ListSMSSandboxPhoneNumbersResultTypeDef",
     {
         "PhoneNumbers": List[SMSSandboxPhoneNumberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSubscriptionsByTopicResponseTypeDef = TypedDict(
     "ListSubscriptionsByTopicResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSubscriptionsResponseTypeDef = TypedDict(
     "ListSubscriptionsResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTopicsResponseTypeDef = TypedDict(
     "ListTopicsResponseTypeDef",
     {
         "Topics": List[TopicTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPublishBatchRequestEntryTypeDef = TypedDict(
     "_RequiredPublishBatchRequestEntryTypeDef",
     {
         "Id": str,
@@ -1274,15 +1242,15 @@
     pass
 
 PublishBatchResponseTypeDef = TypedDict(
     "PublishBatchResponseTypeDef",
     {
         "Successful": List[PublishBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PublishBatchInputRequestTypeDef = TypedDict(
     "PublishBatchInputRequestTypeDef",
     {
         "TopicArn": str,
```

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns.egg-info/PKG-INFO` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sns
-Version: 1.26.69
-Summary: Type annotations for boto3.SNS 1.26.69 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.SNS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sns"></a>
 
 # mypy-boto3-sns
 
 [![PyPI - mypy-boto3-sns](https://img.shields.io/pypi/v/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sns?color=blue)](https://pypistats.org/packages/mypy-boto3-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SNS 1.26.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[boto3.SNS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [mypy-boto3-sns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -437,102 +437,98 @@
 
 ```python
 from mypy_boto3_sns.type_defs import (
     AddPermissionInputRequestTypeDef,
     AddPermissionInputTopicAddPermissionTypeDef,
     BatchResultErrorEntryTypeDef,
     CheckIfPhoneNumberIsOptedOutInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CheckIfPhoneNumberIsOptedOutResponseTypeDef,
     ConfirmSubscriptionInputRequestTypeDef,
     ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
+    ConfirmSubscriptionResponseTypeDef,
+    CreateEndpointResponseTypeDef,
     CreatePlatformApplicationInputRequestTypeDef,
     CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef,
+    CreatePlatformApplicationResponseTypeDef,
     CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef,
     CreatePlatformEndpointInputRequestTypeDef,
     CreateSMSSandboxPhoneNumberInputRequestTypeDef,
     TagTypeDef,
+    CreateTopicResponseTypeDef,
     DeleteEndpointInputRequestTypeDef,
     DeletePlatformApplicationInputRequestTypeDef,
     DeleteSMSSandboxPhoneNumberInputRequestTypeDef,
     DeleteTopicInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointTypeDef,
     GetDataProtectionPolicyInputRequestTypeDef,
+    GetDataProtectionPolicyResponseTypeDef,
     GetEndpointAttributesInputRequestTypeDef,
+    GetEndpointAttributesResponseTypeDef,
     GetPlatformApplicationAttributesInputRequestTypeDef,
+    GetPlatformApplicationAttributesResponseTypeDef,
     GetSMSAttributesInputRequestTypeDef,
+    GetSMSAttributesResponseTypeDef,
+    GetSMSSandboxAccountStatusResultTypeDef,
     GetSubscriptionAttributesInputRequestTypeDef,
+    GetSubscriptionAttributesResponseTypeDef,
     GetTopicAttributesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetTopicAttributesResponseTypeDef,
+    ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
     ListEndpointsByPlatformApplicationInputRequestTypeDef,
+    ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
     ListOriginationNumbersRequestRequestTypeDef,
     PhoneNumberInformationTypeDef,
+    ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
     ListPhoneNumbersOptedOutInputRequestTypeDef,
+    ListPhoneNumbersOptedOutResponseTypeDef,
+    ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
     ListPlatformApplicationsInputRequestTypeDef,
     PlatformApplicationTypeDef,
+    ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
     ListSMSSandboxPhoneNumbersInputRequestTypeDef,
     SMSSandboxPhoneNumberTypeDef,
+    ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
     ListSubscriptionsByTopicInputRequestTypeDef,
     SubscriptionTypeDef,
+    ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
     ListSubscriptionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTopicsInputListTopicsPaginateTypeDef,
     ListTopicsInputRequestTypeDef,
     TopicTypeDef,
     MessageAttributeValueTypeDef,
     OptInPhoneNumberInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PublishBatchResultEntryTypeDef,
+    PublishResponseTypeDef,
     PutDataProtectionPolicyInputRequestTypeDef,
     RemovePermissionInputRequestTypeDef,
     RemovePermissionInputTopicRemovePermissionTypeDef,
-    ServiceResourcePlatformApplicationRequestTypeDef,
-    ServiceResourcePlatformEndpointRequestTypeDef,
-    ServiceResourceSubscriptionRequestTypeDef,
-    ServiceResourceTopicRequestTypeDef,
+    ResponseMetadataTypeDef,
     SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef,
     SetEndpointAttributesInputRequestTypeDef,
     SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef,
     SetPlatformApplicationAttributesInputRequestTypeDef,
     SetSMSAttributesInputRequestTypeDef,
     SetSubscriptionAttributesInputRequestTypeDef,
     SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef,
     SetTopicAttributesInputRequestTypeDef,
     SetTopicAttributesInputTopicSetAttributesTypeDef,
     SubscribeInputRequestTypeDef,
     SubscribeInputTopicSubscribeTypeDef,
+    SubscribeResponseTypeDef,
     UnsubscribeInputRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VerifySMSSandboxPhoneNumberInputRequestTypeDef,
-    CheckIfPhoneNumberIsOptedOutResponseTypeDef,
-    ConfirmSubscriptionResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreatePlatformApplicationResponseTypeDef,
-    CreateTopicResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDataProtectionPolicyResponseTypeDef,
-    GetEndpointAttributesResponseTypeDef,
-    GetPlatformApplicationAttributesResponseTypeDef,
-    GetSMSAttributesResponseTypeDef,
-    GetSMSSandboxAccountStatusResultTypeDef,
-    GetSubscriptionAttributesResponseTypeDef,
-    GetTopicAttributesResponseTypeDef,
-    ListPhoneNumbersOptedOutResponseTypeDef,
-    PublishResponseTypeDef,
-    SubscribeResponseTypeDef,
     CreateTopicInputRequestTypeDef,
     CreateTopicInputServiceResourceCreateTopicTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEndpointsByPlatformApplicationResponseTypeDef,
-    ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
-    ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
-    ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
-    ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
-    ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
-    ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
-    ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
-    ListTopicsInputListTopicsPaginateTypeDef,
     ListOriginationNumbersResultTypeDef,
     ListPlatformApplicationsResponseTypeDef,
     ListSMSSandboxPhoneNumbersResultTypeDef,
     ListSubscriptionsByTopicResponseTypeDef,
     ListSubscriptionsResponseTypeDef,
     ListTopicsResponseTypeDef,
     PublishBatchRequestEntryTypeDef,
@@ -551,42 +547,42 @@
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

### Comparing `mypy-boto3-sns-1.26.69/mypy_boto3_sns.egg-info/SOURCES.txt` & `mypy-boto3-sns-1.27.0/mypy_boto3_sns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.26.69/setup.py` & `mypy-boto3-sns-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-sns.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sns",
-    version="1.26.69",
+    version="1.27.0",
     packages=["mypy_boto3_sns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SNS 1.26.69 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.SNS 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/",
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


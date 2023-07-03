# Comparing `tmp/mypy-boto3-route53domains-1.26.34.tar.gz` & `tmp/mypy-boto3-route53domains-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53domains-1.26.34.tar", last modified: Tue Dec 20 20:26:41 2022, max compression
+gzip compressed data, was "mypy-boto3-route53domains-1.27.0.tar", last modified: Mon Jul  3 19:51:22 2023, max compression
```

## Comparing `mypy-boto3-route53domains-1.26.34.tar` & `mypy-boto3-route53domains-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:41.046595 mypy-boto3-route53domains-1.26.34/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2022-12-20 20:26:41.046595 mypy-boto3-route53domains-1.26.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:41.046595 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28925 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28880 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27512 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27491 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:41.046595 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2022-12-20 20:26:40.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-20 20:26:40.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 20:26:40.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 20:26:40.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-20 20:26:40.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-20 20:26:40.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 20:26:41.046595 mypy-boto3-route53domains-1.26.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:22.075907 mypy-boto3-route53domains-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-07-03 19:51:22.075907 mypy-boto3-route53domains-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:22.071907 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28933 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28888 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-07-03 19:46:36.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27578 2023-07-03 19:46:36.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27557 2023-07-03 19:46:36.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:22.075907 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-07-03 19:51:21.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:51:21.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:21.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:21.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:21.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:51:21.000000 mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:22.075907 mypy-boto3-route53domains-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-03 19:46:35.000000 mypy-boto3-route53domains-1.27.0/setup.py
```

### Comparing `mypy-boto3-route53domains-1.26.34/LICENSE` & `mypy-boto3-route53domains-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-route53domains-1.26.34/PKG-INFO` & `mypy-boto3-route53domains-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53domains
-Version: 1.26.34
-Summary: Type annotations for boto3.Route53Domains 1.26.34 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.Route53Domains 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-route53domains"></a>
 
 # mypy-boto3-route53domains
 
 [![PyPI - mypy-boto3-route53domains](https://img.shields.io/pypi/v/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53domains?color=blue)](https://pypistats.org/packages/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.26.34](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,88 +345,88 @@
 
 `mypy_boto3_route53domains.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53domains.type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     DnssecSigningAttributesTypeDef,
+    AssociateDelegationSignerToDomainResponseTypeDef,
     BillingRecordTypeDef,
     CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef,
+    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityRequestRequestTypeDef,
+    CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityRequestRequestTypeDef,
     DomainTransferabilityTypeDef,
     ConsentTypeDef,
     ExtraParamTypeDef,
     DeleteDomainRequestRequestTypeDef,
+    DeleteDomainResponseTypeDef,
     DeleteTagsForDomainRequestRequestTypeDef,
     DisableDomainAutoRenewRequestRequestTypeDef,
     DisableDomainTransferLockRequestRequestTypeDef,
+    DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainRequestRequestTypeDef,
+    DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecKeyTypeDef,
     PriceWithCurrencyTypeDef,
     DomainSuggestionTypeDef,
     DomainSummaryTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableDomainAutoRenewRequestRequestTypeDef,
     EnableDomainTransferLockRequestRequestTypeDef,
+    EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
     GetContactReachabilityStatusRequestRequestTypeDef,
+    GetContactReachabilityStatusResponseTypeDef,
     GetDomainDetailRequestRequestTypeDef,
     NameserverTypeDef,
     GetDomainSuggestionsRequestRequestTypeDef,
     GetOperationDetailRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetOperationDetailResponseTypeDef,
     SortConditionTypeDef,
+    ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
+    ListPricesRequestListPricesPaginateTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
     TagTypeDef,
+    PaginatorConfigTypeDef,
     PushDomainRequestRequestTypeDef,
+    RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
+    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainRequestRequestTypeDef,
+    RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
+    ResendContactReachabilityEmailResponseTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
-    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
-    UpdateDomainContactPrivacyRequestRequestTypeDef,
-    ViewBillingRequestRequestTypeDef,
-    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
-    AssociateDelegationSignerToDomainResponseTypeDef,
-    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
-    CheckDomainAvailabilityResponseTypeDef,
-    DeleteDomainResponseTypeDef,
-    DisableDomainTransferLockResponseTypeDef,
-    DisassociateDelegationSignerFromDomainResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnableDomainTransferLockResponseTypeDef,
-    GetContactReachabilityStatusResponseTypeDef,
-    GetOperationDetailResponseTypeDef,
-    RegisterDomainResponseTypeDef,
-    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
-    RenewDomainResponseTypeDef,
-    ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     TransferDomainResponseTypeDef,
+    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
+    UpdateDomainContactPrivacyRequestRequestTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
+    ViewBillingRequestRequestTypeDef,
+    ViewBillingRequestViewBillingPaginateTypeDef,
     AssociateDelegationSignerToDomainRequestRequestTypeDef,
     ViewBillingResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ContactDetailTypeDef,
     DomainPriceTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     ListDomainsResponseTypeDef,
     UpdateDomainNameserversRequestRequestTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
-    ListPricesRequestListPricesPaginateTypeDef,
-    ViewBillingRequestViewBillingPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
     GetDomainDetailResponseTypeDef,
     RegisterDomainRequestRequestTypeDef,
@@ -443,42 +443,42 @@
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

### Comparing `mypy-boto3-route53domains-1.26.34/README.md` & `mypy-boto3-route53domains-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-route53domains"></a>
 
 # mypy-boto3-route53domains
 
 [![PyPI - mypy-boto3-route53domains](https://img.shields.io/pypi/v/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53domains?color=blue)](https://pypistats.org/packages/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.26.34](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,88 +313,88 @@
 
 `mypy_boto3_route53domains.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53domains.type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     DnssecSigningAttributesTypeDef,
+    AssociateDelegationSignerToDomainResponseTypeDef,
     BillingRecordTypeDef,
     CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef,
+    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityRequestRequestTypeDef,
+    CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityRequestRequestTypeDef,
     DomainTransferabilityTypeDef,
     ConsentTypeDef,
     ExtraParamTypeDef,
     DeleteDomainRequestRequestTypeDef,
+    DeleteDomainResponseTypeDef,
     DeleteTagsForDomainRequestRequestTypeDef,
     DisableDomainAutoRenewRequestRequestTypeDef,
     DisableDomainTransferLockRequestRequestTypeDef,
+    DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainRequestRequestTypeDef,
+    DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecKeyTypeDef,
     PriceWithCurrencyTypeDef,
     DomainSuggestionTypeDef,
     DomainSummaryTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableDomainAutoRenewRequestRequestTypeDef,
     EnableDomainTransferLockRequestRequestTypeDef,
+    EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
     GetContactReachabilityStatusRequestRequestTypeDef,
+    GetContactReachabilityStatusResponseTypeDef,
     GetDomainDetailRequestRequestTypeDef,
     NameserverTypeDef,
     GetDomainSuggestionsRequestRequestTypeDef,
     GetOperationDetailRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetOperationDetailResponseTypeDef,
     SortConditionTypeDef,
+    ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
+    ListPricesRequestListPricesPaginateTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
     TagTypeDef,
+    PaginatorConfigTypeDef,
     PushDomainRequestRequestTypeDef,
+    RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
+    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainRequestRequestTypeDef,
+    RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
+    ResendContactReachabilityEmailResponseTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
-    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
-    UpdateDomainContactPrivacyRequestRequestTypeDef,
-    ViewBillingRequestRequestTypeDef,
-    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
-    AssociateDelegationSignerToDomainResponseTypeDef,
-    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
-    CheckDomainAvailabilityResponseTypeDef,
-    DeleteDomainResponseTypeDef,
-    DisableDomainTransferLockResponseTypeDef,
-    DisassociateDelegationSignerFromDomainResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnableDomainTransferLockResponseTypeDef,
-    GetContactReachabilityStatusResponseTypeDef,
-    GetOperationDetailResponseTypeDef,
-    RegisterDomainResponseTypeDef,
-    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
-    RenewDomainResponseTypeDef,
-    ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     TransferDomainResponseTypeDef,
+    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
+    UpdateDomainContactPrivacyRequestRequestTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
+    ViewBillingRequestRequestTypeDef,
+    ViewBillingRequestViewBillingPaginateTypeDef,
     AssociateDelegationSignerToDomainRequestRequestTypeDef,
     ViewBillingResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ContactDetailTypeDef,
     DomainPriceTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     ListDomainsResponseTypeDef,
     UpdateDomainNameserversRequestRequestTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
-    ListPricesRequestListPricesPaginateTypeDef,
-    ViewBillingRequestViewBillingPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
     GetDomainDetailResponseTypeDef,
     RegisterDomainRequestRequestTypeDef,
@@ -411,42 +411,42 @@
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

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/__init__.py` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/__init__.pyi` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/__main__.py` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53Domains 1.26.34\nVersion:         1.26.34\nBuilder"
-        " version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.Route53Domains 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.34")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/client.py` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,17 +338,17 @@
         """
 
     def list_prices(
         self, *, Tld: str = ..., Marker: str = ..., MaxItems: int = ...
     ) -> ListPricesResponseTypeDef:
         """
         Lists the following prices for either all the TLDs supported by Route 53, or the
-        specified TLD * Registration * Transfer * Owner change * Domain renewal * Domain
-        restoration See also: `AWS API Documentation
-        <https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-1...`.
+        specified TLD: * Registration * Transfer * Owner change * Domain renewal *
+        Domain restoration See also: `AWS API Documentation
+        <https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-15/ListP...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_prices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_prices)
         """
 
     def list_tags_for_domain(self, *, DomainName: str) -> ListTagsForDomainResponseTypeDef:
         """
```

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/client.pyi` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -312,17 +312,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_operations)
         """
     def list_prices(
         self, *, Tld: str = ..., Marker: str = ..., MaxItems: int = ...
     ) -> ListPricesResponseTypeDef:
         """
         Lists the following prices for either all the TLDs supported by Route 53, or the
-        specified TLD * Registration * Transfer * Owner change * Domain renewal * Domain
-        restoration See also: `AWS API Documentation
-        <https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-1...`.
+        specified TLD: * Registration * Transfer * Owner change * Domain renewal *
+        Domain restoration See also: `AWS API Documentation
+        <https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-15/ListP...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_prices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_prices)
         """
     def list_tags_for_domain(self, *, DomainName: str) -> ListTagsForDomainResponseTypeDef:
         """
         This operation returns all of the tags that are associated with the specified
```

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/literals.py` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -399,14 +399,15 @@
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
@@ -427,31 +428,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -530,14 +534,15 @@
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
@@ -548,18 +553,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -569,14 +576,15 @@
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
@@ -589,14 +597,15 @@
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
@@ -615,16 +624,19 @@
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
@@ -704,18 +716,21 @@
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

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/literals.pyi` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -397,14 +397,15 @@
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
@@ -425,31 +426,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -528,14 +532,15 @@
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
@@ -546,18 +551,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -567,14 +574,15 @@
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
@@ -587,14 +595,15 @@
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
@@ -613,16 +622,19 @@
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
@@ -702,18 +714,21 @@
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

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/paginator.py` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """
 
     def paginate(
         self,
         *,
         FilterConditions: Sequence[FilterConditionTypeDef] = ...,
         SortCondition: SortConditionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listdomainspaginator)
         """
 
 
@@ -95,30 +95,30 @@
         self,
         *,
         SubmittedSince: Union[datetime, str] = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listoperationspaginator)
         """
 
 
 class ListPricesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListPrices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listpricespaginator)
     """
 
     def paginate(
-        self, *, Tld: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Tld: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListPrices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listpricespaginator)
         """
 
 
@@ -129,13 +129,13 @@
     """
 
     def paginate(
         self,
         *,
         Start: Union[datetime, str] = ...,
         End: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ViewBillingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#viewbillingpaginator)
         """
```

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/paginator.pyi` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     """
 
     def paginate(
         self,
         *,
         FilterConditions: Sequence[FilterConditionTypeDef] = ...,
         SortCondition: SortConditionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listdomainspaginator)
         """
 
 class ListOperationsPaginator(Paginator):
@@ -90,29 +90,29 @@
         self,
         *,
         SubmittedSince: Union[datetime, str] = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listoperationspaginator)
         """
 
 class ListPricesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListPrices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listpricespaginator)
     """
 
     def paginate(
-        self, *, Tld: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Tld: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListPrices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listpricespaginator)
         """
 
 class ViewBillingPaginator(Paginator):
@@ -122,13 +122,13 @@
     """
 
     def paginate(
         self,
         *,
         Start: Union[datetime, str] = ...,
         End: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ViewBillingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#viewbillingpaginator)
         """
```

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/type_defs.py` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,88 +38,88 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     "DnssecSigningAttributesTypeDef",
+    "AssociateDelegationSignerToDomainResponseTypeDef",
     "BillingRecordTypeDef",
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
+    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     "CheckDomainAvailabilityRequestRequestTypeDef",
+    "CheckDomainAvailabilityResponseTypeDef",
     "CheckDomainTransferabilityRequestRequestTypeDef",
     "DomainTransferabilityTypeDef",
     "ConsentTypeDef",
     "ExtraParamTypeDef",
     "DeleteDomainRequestRequestTypeDef",
+    "DeleteDomainResponseTypeDef",
     "DeleteTagsForDomainRequestRequestTypeDef",
     "DisableDomainAutoRenewRequestRequestTypeDef",
     "DisableDomainTransferLockRequestRequestTypeDef",
+    "DisableDomainTransferLockResponseTypeDef",
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
+    "DisassociateDelegationSignerFromDomainResponseTypeDef",
     "DnssecKeyTypeDef",
     "PriceWithCurrencyTypeDef",
     "DomainSuggestionTypeDef",
     "DomainSummaryTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableDomainAutoRenewRequestRequestTypeDef",
     "EnableDomainTransferLockRequestRequestTypeDef",
+    "EnableDomainTransferLockResponseTypeDef",
     "FilterConditionTypeDef",
     "GetContactReachabilityStatusRequestRequestTypeDef",
+    "GetContactReachabilityStatusResponseTypeDef",
     "GetDomainDetailRequestRequestTypeDef",
     "NameserverTypeDef",
     "GetDomainSuggestionsRequestRequestTypeDef",
     "GetOperationDetailRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetOperationDetailResponseTypeDef",
     "SortConditionTypeDef",
+    "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "OperationSummaryTypeDef",
+    "ListPricesRequestListPricesPaginateTypeDef",
     "ListPricesRequestRequestTypeDef",
     "ListTagsForDomainRequestRequestTypeDef",
     "TagTypeDef",
+    "PaginatorConfigTypeDef",
     "PushDomainRequestRequestTypeDef",
+    "RegisterDomainResponseTypeDef",
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
+    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
     "RenewDomainRequestRequestTypeDef",
+    "RenewDomainResponseTypeDef",
     "ResendContactReachabilityEmailRequestRequestTypeDef",
+    "ResendContactReachabilityEmailResponseTypeDef",
     "ResendOperationAuthorizationRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
-    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
-    "UpdateDomainContactPrivacyRequestRequestTypeDef",
-    "ViewBillingRequestRequestTypeDef",
-    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
-    "AssociateDelegationSignerToDomainResponseTypeDef",
-    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
-    "CheckDomainAvailabilityResponseTypeDef",
-    "DeleteDomainResponseTypeDef",
-    "DisableDomainTransferLockResponseTypeDef",
-    "DisassociateDelegationSignerFromDomainResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EnableDomainTransferLockResponseTypeDef",
-    "GetContactReachabilityStatusResponseTypeDef",
-    "GetOperationDetailResponseTypeDef",
-    "RegisterDomainResponseTypeDef",
-    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
-    "RenewDomainResponseTypeDef",
-    "ResendContactReachabilityEmailResponseTypeDef",
     "RetrieveDomainAuthCodeResponseTypeDef",
     "TransferDomainResponseTypeDef",
+    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     "TransferDomainToAnotherAwsAccountResponseTypeDef",
+    "UpdateDomainContactPrivacyRequestRequestTypeDef",
     "UpdateDomainContactPrivacyResponseTypeDef",
     "UpdateDomainContactResponseTypeDef",
     "UpdateDomainNameserversResponseTypeDef",
+    "ViewBillingRequestRequestTypeDef",
+    "ViewBillingRequestViewBillingPaginateTypeDef",
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     "ViewBillingResponseTypeDef",
     "CheckDomainTransferabilityResponseTypeDef",
     "ContactDetailTypeDef",
     "DomainPriceTypeDef",
     "GetDomainSuggestionsResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "UpdateDomainNameserversRequestRequestTypeDef",
-    "ListOperationsRequestListOperationsPaginateTypeDef",
-    "ListPricesRequestListPricesPaginateTypeDef",
-    "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListTagsForDomainResponseTypeDef",
     "UpdateTagsForDomainRequestRequestTypeDef",
     "GetDomainDetailResponseTypeDef",
     "RegisterDomainRequestRequestTypeDef",
@@ -132,35 +132,40 @@
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "Password": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
+    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DnssecSigningAttributesTypeDef = TypedDict(
     "DnssecSigningAttributesTypeDef",
     {
         "Algorithm": int,
         "Flags": int,
         "PublicKey": str,
     },
     total=False,
 )
 
+AssociateDelegationSignerToDomainResponseTypeDef = TypedDict(
+    "AssociateDelegationSignerToDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BillingRecordTypeDef = TypedDict(
     "BillingRecordTypeDef",
     {
         "DomainName": str,
         "Operation": OperationTypeType,
         "InvoiceId": str,
         "BillDate": datetime,
@@ -172,14 +177,22 @@
 CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+CancelDomainTransferToAnotherAwsAccountResponseTypeDef = TypedDict(
+    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCheckDomainAvailabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCheckDomainAvailabilityRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCheckDomainAvailabilityRequestRequestTypeDef = TypedDict(
@@ -194,14 +207,22 @@
 class CheckDomainAvailabilityRequestRequestTypeDef(
     _RequiredCheckDomainAvailabilityRequestRequestTypeDef,
     _OptionalCheckDomainAvailabilityRequestRequestTypeDef,
 ):
     pass
 
 
+CheckDomainAvailabilityResponseTypeDef = TypedDict(
+    "CheckDomainAvailabilityResponseTypeDef",
+    {
+        "Availability": DomainAvailabilityType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCheckDomainTransferabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCheckDomainTransferabilityRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCheckDomainTransferabilityRequestRequestTypeDef = TypedDict(
@@ -247,14 +268,22 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTagsForDomainRequestRequestTypeDef = TypedDict(
     "DeleteTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "TagsToDelete": Sequence[str],
     },
 )
@@ -269,22 +298,38 @@
 DisableDomainTransferLockRequestRequestTypeDef = TypedDict(
     "DisableDomainTransferLockRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+DisableDomainTransferLockResponseTypeDef = TypedDict(
+    "DisableDomainTransferLockResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateDelegationSignerFromDomainRequestRequestTypeDef = TypedDict(
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Id": str,
     },
 )
 
+DisassociateDelegationSignerFromDomainResponseTypeDef = TypedDict(
+    "DisassociateDelegationSignerFromDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DnssecKeyTypeDef = TypedDict(
     "DnssecKeyTypeDef",
     {
         "Algorithm": int,
         "Flags": int,
         "PublicKey": str,
         "DigestType": int,
@@ -319,28 +364,43 @@
         "AutoRenew": bool,
         "TransferLock": bool,
         "Expiry": datetime,
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
 EnableDomainAutoRenewRequestRequestTypeDef = TypedDict(
     "EnableDomainAutoRenewRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
 EnableDomainTransferLockRequestRequestTypeDef = TypedDict(
     "EnableDomainTransferLockRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+EnableDomainTransferLockResponseTypeDef = TypedDict(
+    "EnableDomainTransferLockResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "Operator": OperatorType,
         "Values": Sequence[str],
     },
@@ -350,14 +410,23 @@
     "GetContactReachabilityStatusRequestRequestTypeDef",
     {
         "domainName": str,
     },
     total=False,
 )
 
+GetContactReachabilityStatusResponseTypeDef = TypedDict(
+    "GetContactReachabilityStatusResponseTypeDef",
+    {
+        "domainName": str,
+        "status": ReachabilityStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDomainDetailRequestRequestTypeDef = TypedDict(
     "GetDomainDetailRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -392,32 +461,50 @@
 GetOperationDetailRequestRequestTypeDef = TypedDict(
     "GetOperationDetailRequestRequestTypeDef",
     {
         "OperationId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetOperationDetailResponseTypeDef = TypedDict(
+    "GetOperationDetailResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "OperationId": str,
+        "Status": OperationStatusType,
+        "Message": str,
+        "DomainName": str,
+        "Type": OperationTypeType,
+        "SubmittedDate": datetime,
+        "LastUpdatedDate": datetime,
+        "StatusFlag": StatusFlagType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 SortConditionTypeDef = TypedDict(
     "SortConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "SortOrder": SortOrderType,
     },
 )
 
+ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
+    "ListOperationsRequestListOperationsPaginateTypeDef",
+    {
+        "SubmittedSince": Union[datetime, str],
+        "Status": Sequence[OperationStatusType],
+        "Type": Sequence[OperationTypeType],
+        "SortBy": Literal["SubmittedDate"],
+        "SortOrder": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOperationsRequestRequestTypeDef = TypedDict(
     "ListOperationsRequestRequestTypeDef",
     {
         "SubmittedSince": Union[datetime, str],
         "Marker": str,
         "MaxItems": int,
         "Status": Sequence[OperationStatusType],
@@ -439,14 +526,23 @@
         "Message": str,
         "StatusFlag": StatusFlagType,
         "LastUpdatedDate": datetime,
     },
     total=False,
 )
 
+ListPricesRequestListPricesPaginateTypeDef = TypedDict(
+    "ListPricesRequestListPricesPaginateTypeDef",
+    {
+        "Tld": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPricesRequestRequestTypeDef = TypedDict(
     "ListPricesRequestRequestTypeDef",
     {
         "Tld": str,
         "Marker": str,
         "MaxItems": int,
     },
@@ -465,29 +561,55 @@
     {
         "Key": str,
         "Value": str,
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
 PushDomainRequestRequestTypeDef = TypedDict(
     "PushDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Target": str,
     },
 )
 
+RegisterDomainResponseTypeDef = TypedDict(
+    "RegisterDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+RejectDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
+    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRenewDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRenewDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "CurrentExpiryYear": int,
     },
 )
@@ -502,255 +624,165 @@
 
 class RenewDomainRequestRequestTypeDef(
     _RequiredRenewDomainRequestRequestTypeDef, _OptionalRenewDomainRequestRequestTypeDef
 ):
     pass
 
 
-ResendContactReachabilityEmailRequestRequestTypeDef = TypedDict(
-    "ResendContactReachabilityEmailRequestRequestTypeDef",
-    {
-        "domainName": str,
-    },
-    total=False,
-)
-
-ResendOperationAuthorizationRequestRequestTypeDef = TypedDict(
-    "ResendOperationAuthorizationRequestRequestTypeDef",
+RenewDomainResponseTypeDef = TypedDict(
+    "RenewDomainResponseTypeDef",
     {
         "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RetrieveDomainAuthCodeRequestRequestTypeDef = TypedDict(
-    "RetrieveDomainAuthCodeRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-
-TransferDomainToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
-    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "AccountId": str,
-    },
-)
-
-_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef",
-    {
-        "AdminPrivacy": bool,
-        "RegistrantPrivacy": bool,
-        "TechPrivacy": bool,
-    },
-    total=False,
-)
-
-
-class UpdateDomainContactPrivacyRequestRequestTypeDef(
-    _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef,
-    _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef,
-):
-    pass
-
-
-ViewBillingRequestRequestTypeDef = TypedDict(
-    "ViewBillingRequestRequestTypeDef",
+ResendContactReachabilityEmailRequestRequestTypeDef = TypedDict(
+    "ResendContactReachabilityEmailRequestRequestTypeDef",
     {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "Marker": str,
-        "MaxItems": int,
+        "domainName": str,
     },
     total=False,
 )
 
-AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
-    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateDelegationSignerToDomainResponseTypeDef = TypedDict(
-    "AssociateDelegationSignerToDomainResponseTypeDef",
+ResendContactReachabilityEmailResponseTypeDef = TypedDict(
+    "ResendContactReachabilityEmailResponseTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "domainName": str,
+        "emailAddress": str,
+        "isAlreadyVerified": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelDomainTransferToAnotherAwsAccountResponseTypeDef = TypedDict(
-    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
+ResendOperationAuthorizationRequestRequestTypeDef = TypedDict(
+    "ResendOperationAuthorizationRequestRequestTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CheckDomainAvailabilityResponseTypeDef = TypedDict(
-    "CheckDomainAvailabilityResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Availability": DomainAvailabilityType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
+RetrieveDomainAuthCodeRequestRequestTypeDef = TypedDict(
+    "RetrieveDomainAuthCodeRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DomainName": str,
     },
 )
 
-DisableDomainTransferLockResponseTypeDef = TypedDict(
-    "DisableDomainTransferLockResponseTypeDef",
+RetrieveDomainAuthCodeResponseTypeDef = TypedDict(
+    "RetrieveDomainAuthCodeResponseTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AuthCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DisassociateDelegationSignerFromDomainResponseTypeDef = TypedDict(
-    "DisassociateDelegationSignerFromDomainResponseTypeDef",
+TransferDomainResponseTypeDef = TypedDict(
+    "TransferDomainResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+TransferDomainToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
+    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DomainName": str,
+        "AccountId": str,
     },
 )
 
-EnableDomainTransferLockResponseTypeDef = TypedDict(
-    "EnableDomainTransferLockResponseTypeDef",
+TransferDomainToAnotherAwsAccountResponseTypeDef = TypedDict(
+    "TransferDomainToAnotherAwsAccountResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetContactReachabilityStatusResponseTypeDef = TypedDict(
-    "GetContactReachabilityStatusResponseTypeDef",
-    {
-        "domainName": str,
-        "status": ReachabilityStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Password": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetOperationDetailResponseTypeDef = TypedDict(
-    "GetOperationDetailResponseTypeDef",
+_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "Status": OperationStatusType,
-        "Message": str,
         "DomainName": str,
-        "Type": OperationTypeType,
-        "SubmittedDate": datetime,
-        "LastUpdatedDate": datetime,
-        "StatusFlag": StatusFlagType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-RegisterDomainResponseTypeDef = TypedDict(
-    "RegisterDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RejectDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
-    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
+_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AdminPrivacy": bool,
+        "RegistrantPrivacy": bool,
+        "TechPrivacy": bool,
     },
+    total=False,
 )
 
-RenewDomainResponseTypeDef = TypedDict(
-    "RenewDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-ResendContactReachabilityEmailResponseTypeDef = TypedDict(
-    "ResendContactReachabilityEmailResponseTypeDef",
-    {
-        "domainName": str,
-        "emailAddress": str,
-        "isAlreadyVerified": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateDomainContactPrivacyRequestRequestTypeDef(
+    _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef,
+    _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef,
+):
+    pass
 
-RetrieveDomainAuthCodeResponseTypeDef = TypedDict(
-    "RetrieveDomainAuthCodeResponseTypeDef",
-    {
-        "AuthCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-TransferDomainResponseTypeDef = TypedDict(
-    "TransferDomainResponseTypeDef",
+UpdateDomainContactPrivacyResponseTypeDef = TypedDict(
+    "UpdateDomainContactPrivacyResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TransferDomainToAnotherAwsAccountResponseTypeDef = TypedDict(
-    "TransferDomainToAnotherAwsAccountResponseTypeDef",
+UpdateDomainContactResponseTypeDef = TypedDict(
+    "UpdateDomainContactResponseTypeDef",
     {
         "OperationId": str,
-        "Password": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateDomainContactPrivacyResponseTypeDef = TypedDict(
-    "UpdateDomainContactPrivacyResponseTypeDef",
+UpdateDomainNameserversResponseTypeDef = TypedDict(
+    "UpdateDomainNameserversResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateDomainContactResponseTypeDef = TypedDict(
-    "UpdateDomainContactResponseTypeDef",
+ViewBillingRequestRequestTypeDef = TypedDict(
+    "ViewBillingRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Start": Union[datetime, str],
+        "End": Union[datetime, str],
+        "Marker": str,
+        "MaxItems": int,
     },
+    total=False,
 )
 
-UpdateDomainNameserversResponseTypeDef = TypedDict(
-    "UpdateDomainNameserversResponseTypeDef",
+ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
+    "ViewBillingRequestViewBillingPaginateTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Start": Union[datetime, str],
+        "End": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
 AssociateDelegationSignerToDomainRequestRequestTypeDef = TypedDict(
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "SigningAttributes": DnssecSigningAttributesTypeDef,
@@ -758,23 +790,23 @@
 )
 
 ViewBillingResponseTypeDef = TypedDict(
     "ViewBillingResponseTypeDef",
     {
         "NextPageMarker": str,
         "BillingRecords": List[BillingRecordTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CheckDomainTransferabilityResponseTypeDef = TypedDict(
     "CheckDomainTransferabilityResponseTypeDef",
     {
         "Transferability": DomainTransferabilityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ContactDetailTypeDef = TypedDict(
     "ContactDetailTypeDef",
     {
         "FirstName": str,
@@ -808,24 +840,24 @@
     total=False,
 )
 
 GetDomainSuggestionsResponseTypeDef = TypedDict(
     "GetDomainSuggestionsResponseTypeDef",
     {
         "SuggestionsList": List[DomainSuggestionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -844,52 +876,20 @@
 class UpdateDomainNameserversRequestRequestTypeDef(
     _RequiredUpdateDomainNameserversRequestRequestTypeDef,
     _OptionalUpdateDomainNameserversRequestRequestTypeDef,
 ):
     pass
 
 
-ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
-    "ListOperationsRequestListOperationsPaginateTypeDef",
-    {
-        "SubmittedSince": Union[datetime, str],
-        "Status": Sequence[OperationStatusType],
-        "Type": Sequence[OperationTypeType],
-        "SortBy": Literal["SubmittedDate"],
-        "SortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPricesRequestListPricesPaginateTypeDef = TypedDict(
-    "ListPricesRequestListPricesPaginateTypeDef",
-    {
-        "Tld": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
-    "ViewBillingRequestViewBillingPaginateTypeDef",
-    {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
     "ListDomainsRequestListDomainsPaginateTypeDef",
     {
         "FilterConditions": Sequence[FilterConditionTypeDef],
         "SortCondition": SortConditionTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
@@ -902,23 +902,23 @@
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForDomainResponseTypeDef = TypedDict(
     "ListTagsForDomainResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -961,15 +961,15 @@
         "CreationDate": datetime,
         "UpdatedDate": datetime,
         "ExpirationDate": datetime,
         "Reseller": str,
         "DnsSec": str,
         "StatusList": List[str],
         "DnssecKeys": List[DnssecKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1055,10 +1055,10 @@
 
 
 ListPricesResponseTypeDef = TypedDict(
     "ListPricesResponseTypeDef",
     {
         "Prices": List[DomainPriceTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/type_defs.pyi` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -37,88 +37,88 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     "DnssecSigningAttributesTypeDef",
+    "AssociateDelegationSignerToDomainResponseTypeDef",
     "BillingRecordTypeDef",
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
+    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     "CheckDomainAvailabilityRequestRequestTypeDef",
+    "CheckDomainAvailabilityResponseTypeDef",
     "CheckDomainTransferabilityRequestRequestTypeDef",
     "DomainTransferabilityTypeDef",
     "ConsentTypeDef",
     "ExtraParamTypeDef",
     "DeleteDomainRequestRequestTypeDef",
+    "DeleteDomainResponseTypeDef",
     "DeleteTagsForDomainRequestRequestTypeDef",
     "DisableDomainAutoRenewRequestRequestTypeDef",
     "DisableDomainTransferLockRequestRequestTypeDef",
+    "DisableDomainTransferLockResponseTypeDef",
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
+    "DisassociateDelegationSignerFromDomainResponseTypeDef",
     "DnssecKeyTypeDef",
     "PriceWithCurrencyTypeDef",
     "DomainSuggestionTypeDef",
     "DomainSummaryTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableDomainAutoRenewRequestRequestTypeDef",
     "EnableDomainTransferLockRequestRequestTypeDef",
+    "EnableDomainTransferLockResponseTypeDef",
     "FilterConditionTypeDef",
     "GetContactReachabilityStatusRequestRequestTypeDef",
+    "GetContactReachabilityStatusResponseTypeDef",
     "GetDomainDetailRequestRequestTypeDef",
     "NameserverTypeDef",
     "GetDomainSuggestionsRequestRequestTypeDef",
     "GetOperationDetailRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetOperationDetailResponseTypeDef",
     "SortConditionTypeDef",
+    "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "OperationSummaryTypeDef",
+    "ListPricesRequestListPricesPaginateTypeDef",
     "ListPricesRequestRequestTypeDef",
     "ListTagsForDomainRequestRequestTypeDef",
     "TagTypeDef",
+    "PaginatorConfigTypeDef",
     "PushDomainRequestRequestTypeDef",
+    "RegisterDomainResponseTypeDef",
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
+    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
     "RenewDomainRequestRequestTypeDef",
+    "RenewDomainResponseTypeDef",
     "ResendContactReachabilityEmailRequestRequestTypeDef",
+    "ResendContactReachabilityEmailResponseTypeDef",
     "ResendOperationAuthorizationRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
-    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
-    "UpdateDomainContactPrivacyRequestRequestTypeDef",
-    "ViewBillingRequestRequestTypeDef",
-    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
-    "AssociateDelegationSignerToDomainResponseTypeDef",
-    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
-    "CheckDomainAvailabilityResponseTypeDef",
-    "DeleteDomainResponseTypeDef",
-    "DisableDomainTransferLockResponseTypeDef",
-    "DisassociateDelegationSignerFromDomainResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EnableDomainTransferLockResponseTypeDef",
-    "GetContactReachabilityStatusResponseTypeDef",
-    "GetOperationDetailResponseTypeDef",
-    "RegisterDomainResponseTypeDef",
-    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
-    "RenewDomainResponseTypeDef",
-    "ResendContactReachabilityEmailResponseTypeDef",
     "RetrieveDomainAuthCodeResponseTypeDef",
     "TransferDomainResponseTypeDef",
+    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     "TransferDomainToAnotherAwsAccountResponseTypeDef",
+    "UpdateDomainContactPrivacyRequestRequestTypeDef",
     "UpdateDomainContactPrivacyResponseTypeDef",
     "UpdateDomainContactResponseTypeDef",
     "UpdateDomainNameserversResponseTypeDef",
+    "ViewBillingRequestRequestTypeDef",
+    "ViewBillingRequestViewBillingPaginateTypeDef",
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     "ViewBillingResponseTypeDef",
     "CheckDomainTransferabilityResponseTypeDef",
     "ContactDetailTypeDef",
     "DomainPriceTypeDef",
     "GetDomainSuggestionsResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "UpdateDomainNameserversRequestRequestTypeDef",
-    "ListOperationsRequestListOperationsPaginateTypeDef",
-    "ListPricesRequestListPricesPaginateTypeDef",
-    "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListTagsForDomainResponseTypeDef",
     "UpdateTagsForDomainRequestRequestTypeDef",
     "GetDomainDetailResponseTypeDef",
     "RegisterDomainRequestRequestTypeDef",
@@ -131,35 +131,40 @@
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "Password": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
+    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DnssecSigningAttributesTypeDef = TypedDict(
     "DnssecSigningAttributesTypeDef",
     {
         "Algorithm": int,
         "Flags": int,
         "PublicKey": str,
     },
     total=False,
 )
 
+AssociateDelegationSignerToDomainResponseTypeDef = TypedDict(
+    "AssociateDelegationSignerToDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BillingRecordTypeDef = TypedDict(
     "BillingRecordTypeDef",
     {
         "DomainName": str,
         "Operation": OperationTypeType,
         "InvoiceId": str,
         "BillDate": datetime,
@@ -171,14 +176,22 @@
 CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+CancelDomainTransferToAnotherAwsAccountResponseTypeDef = TypedDict(
+    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCheckDomainAvailabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCheckDomainAvailabilityRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCheckDomainAvailabilityRequestRequestTypeDef = TypedDict(
@@ -191,14 +204,22 @@
 
 class CheckDomainAvailabilityRequestRequestTypeDef(
     _RequiredCheckDomainAvailabilityRequestRequestTypeDef,
     _OptionalCheckDomainAvailabilityRequestRequestTypeDef,
 ):
     pass
 
+CheckDomainAvailabilityResponseTypeDef = TypedDict(
+    "CheckDomainAvailabilityResponseTypeDef",
+    {
+        "Availability": DomainAvailabilityType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCheckDomainTransferabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCheckDomainTransferabilityRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCheckDomainTransferabilityRequestRequestTypeDef = TypedDict(
@@ -242,14 +263,22 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTagsForDomainRequestRequestTypeDef = TypedDict(
     "DeleteTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "TagsToDelete": Sequence[str],
     },
 )
@@ -264,22 +293,38 @@
 DisableDomainTransferLockRequestRequestTypeDef = TypedDict(
     "DisableDomainTransferLockRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+DisableDomainTransferLockResponseTypeDef = TypedDict(
+    "DisableDomainTransferLockResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateDelegationSignerFromDomainRequestRequestTypeDef = TypedDict(
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Id": str,
     },
 )
 
+DisassociateDelegationSignerFromDomainResponseTypeDef = TypedDict(
+    "DisassociateDelegationSignerFromDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DnssecKeyTypeDef = TypedDict(
     "DnssecKeyTypeDef",
     {
         "Algorithm": int,
         "Flags": int,
         "PublicKey": str,
         "DigestType": int,
@@ -314,28 +359,43 @@
         "AutoRenew": bool,
         "TransferLock": bool,
         "Expiry": datetime,
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
 EnableDomainAutoRenewRequestRequestTypeDef = TypedDict(
     "EnableDomainAutoRenewRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
 EnableDomainTransferLockRequestRequestTypeDef = TypedDict(
     "EnableDomainTransferLockRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+EnableDomainTransferLockResponseTypeDef = TypedDict(
+    "EnableDomainTransferLockResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "Operator": OperatorType,
         "Values": Sequence[str],
     },
@@ -345,14 +405,23 @@
     "GetContactReachabilityStatusRequestRequestTypeDef",
     {
         "domainName": str,
     },
     total=False,
 )
 
+GetContactReachabilityStatusResponseTypeDef = TypedDict(
+    "GetContactReachabilityStatusResponseTypeDef",
+    {
+        "domainName": str,
+        "status": ReachabilityStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDomainDetailRequestRequestTypeDef = TypedDict(
     "GetDomainDetailRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -385,32 +454,50 @@
 GetOperationDetailRequestRequestTypeDef = TypedDict(
     "GetOperationDetailRequestRequestTypeDef",
     {
         "OperationId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetOperationDetailResponseTypeDef = TypedDict(
+    "GetOperationDetailResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "OperationId": str,
+        "Status": OperationStatusType,
+        "Message": str,
+        "DomainName": str,
+        "Type": OperationTypeType,
+        "SubmittedDate": datetime,
+        "LastUpdatedDate": datetime,
+        "StatusFlag": StatusFlagType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 SortConditionTypeDef = TypedDict(
     "SortConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "SortOrder": SortOrderType,
     },
 )
 
+ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
+    "ListOperationsRequestListOperationsPaginateTypeDef",
+    {
+        "SubmittedSince": Union[datetime, str],
+        "Status": Sequence[OperationStatusType],
+        "Type": Sequence[OperationTypeType],
+        "SortBy": Literal["SubmittedDate"],
+        "SortOrder": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOperationsRequestRequestTypeDef = TypedDict(
     "ListOperationsRequestRequestTypeDef",
     {
         "SubmittedSince": Union[datetime, str],
         "Marker": str,
         "MaxItems": int,
         "Status": Sequence[OperationStatusType],
@@ -432,14 +519,23 @@
         "Message": str,
         "StatusFlag": StatusFlagType,
         "LastUpdatedDate": datetime,
     },
     total=False,
 )
 
+ListPricesRequestListPricesPaginateTypeDef = TypedDict(
+    "ListPricesRequestListPricesPaginateTypeDef",
+    {
+        "Tld": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPricesRequestRequestTypeDef = TypedDict(
     "ListPricesRequestRequestTypeDef",
     {
         "Tld": str,
         "Marker": str,
         "MaxItems": int,
     },
@@ -458,29 +554,55 @@
     {
         "Key": str,
         "Value": str,
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
 PushDomainRequestRequestTypeDef = TypedDict(
     "PushDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Target": str,
     },
 )
 
+RegisterDomainResponseTypeDef = TypedDict(
+    "RegisterDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+RejectDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
+    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRenewDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRenewDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "CurrentExpiryYear": int,
     },
 )
@@ -493,253 +615,163 @@
 )
 
 class RenewDomainRequestRequestTypeDef(
     _RequiredRenewDomainRequestRequestTypeDef, _OptionalRenewDomainRequestRequestTypeDef
 ):
     pass
 
-ResendContactReachabilityEmailRequestRequestTypeDef = TypedDict(
-    "ResendContactReachabilityEmailRequestRequestTypeDef",
-    {
-        "domainName": str,
-    },
-    total=False,
-)
-
-ResendOperationAuthorizationRequestRequestTypeDef = TypedDict(
-    "ResendOperationAuthorizationRequestRequestTypeDef",
+RenewDomainResponseTypeDef = TypedDict(
+    "RenewDomainResponseTypeDef",
     {
         "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RetrieveDomainAuthCodeRequestRequestTypeDef = TypedDict(
-    "RetrieveDomainAuthCodeRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-
-TransferDomainToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
-    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "AccountId": str,
-    },
-)
-
-_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef",
-    {
-        "AdminPrivacy": bool,
-        "RegistrantPrivacy": bool,
-        "TechPrivacy": bool,
-    },
-    total=False,
-)
-
-class UpdateDomainContactPrivacyRequestRequestTypeDef(
-    _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef,
-    _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef,
-):
-    pass
-
-ViewBillingRequestRequestTypeDef = TypedDict(
-    "ViewBillingRequestRequestTypeDef",
+ResendContactReachabilityEmailRequestRequestTypeDef = TypedDict(
+    "ResendContactReachabilityEmailRequestRequestTypeDef",
     {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "Marker": str,
-        "MaxItems": int,
+        "domainName": str,
     },
     total=False,
 )
 
-AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
-    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateDelegationSignerToDomainResponseTypeDef = TypedDict(
-    "AssociateDelegationSignerToDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelDomainTransferToAnotherAwsAccountResponseTypeDef = TypedDict(
-    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CheckDomainAvailabilityResponseTypeDef = TypedDict(
-    "CheckDomainAvailabilityResponseTypeDef",
+ResendContactReachabilityEmailResponseTypeDef = TypedDict(
+    "ResendContactReachabilityEmailResponseTypeDef",
     {
-        "Availability": DomainAvailabilityType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "domainName": str,
+        "emailAddress": str,
+        "isAlreadyVerified": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
+ResendOperationAuthorizationRequestRequestTypeDef = TypedDict(
+    "ResendOperationAuthorizationRequestRequestTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisableDomainTransferLockResponseTypeDef = TypedDict(
-    "DisableDomainTransferLockResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-DisassociateDelegationSignerFromDomainResponseTypeDef = TypedDict(
-    "DisassociateDelegationSignerFromDomainResponseTypeDef",
+RetrieveDomainAuthCodeRequestRequestTypeDef = TypedDict(
+    "RetrieveDomainAuthCodeRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DomainName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+RetrieveDomainAuthCodeResponseTypeDef = TypedDict(
+    "RetrieveDomainAuthCodeResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AuthCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EnableDomainTransferLockResponseTypeDef = TypedDict(
-    "EnableDomainTransferLockResponseTypeDef",
+TransferDomainResponseTypeDef = TypedDict(
+    "TransferDomainResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetContactReachabilityStatusResponseTypeDef = TypedDict(
-    "GetContactReachabilityStatusResponseTypeDef",
-    {
-        "domainName": str,
-        "status": ReachabilityStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetOperationDetailResponseTypeDef = TypedDict(
-    "GetOperationDetailResponseTypeDef",
+TransferDomainToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
+    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "Status": OperationStatusType,
-        "Message": str,
         "DomainName": str,
-        "Type": OperationTypeType,
-        "SubmittedDate": datetime,
-        "LastUpdatedDate": datetime,
-        "StatusFlag": StatusFlagType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterDomainResponseTypeDef = TypedDict(
-    "RegisterDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AccountId": str,
     },
 )
 
-RejectDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
-    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
+TransferDomainToAnotherAwsAccountResponseTypeDef = TypedDict(
+    "TransferDomainToAnotherAwsAccountResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Password": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RenewDomainResponseTypeDef = TypedDict(
-    "RenewDomainResponseTypeDef",
+_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DomainName": str,
     },
 )
-
-ResendContactReachabilityEmailResponseTypeDef = TypedDict(
-    "ResendContactReachabilityEmailResponseTypeDef",
+_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainContactPrivacyRequestRequestTypeDef",
     {
-        "domainName": str,
-        "emailAddress": str,
-        "isAlreadyVerified": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AdminPrivacy": bool,
+        "RegistrantPrivacy": bool,
+        "TechPrivacy": bool,
     },
+    total=False,
 )
 
-RetrieveDomainAuthCodeResponseTypeDef = TypedDict(
-    "RetrieveDomainAuthCodeResponseTypeDef",
-    {
-        "AuthCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateDomainContactPrivacyRequestRequestTypeDef(
+    _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef,
+    _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef,
+):
+    pass
 
-TransferDomainResponseTypeDef = TypedDict(
-    "TransferDomainResponseTypeDef",
+UpdateDomainContactPrivacyResponseTypeDef = TypedDict(
+    "UpdateDomainContactPrivacyResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TransferDomainToAnotherAwsAccountResponseTypeDef = TypedDict(
-    "TransferDomainToAnotherAwsAccountResponseTypeDef",
+UpdateDomainContactResponseTypeDef = TypedDict(
+    "UpdateDomainContactResponseTypeDef",
     {
         "OperationId": str,
-        "Password": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateDomainContactPrivacyResponseTypeDef = TypedDict(
-    "UpdateDomainContactPrivacyResponseTypeDef",
+UpdateDomainNameserversResponseTypeDef = TypedDict(
+    "UpdateDomainNameserversResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateDomainContactResponseTypeDef = TypedDict(
-    "UpdateDomainContactResponseTypeDef",
+ViewBillingRequestRequestTypeDef = TypedDict(
+    "ViewBillingRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Start": Union[datetime, str],
+        "End": Union[datetime, str],
+        "Marker": str,
+        "MaxItems": int,
     },
+    total=False,
 )
 
-UpdateDomainNameserversResponseTypeDef = TypedDict(
-    "UpdateDomainNameserversResponseTypeDef",
+ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
+    "ViewBillingRequestViewBillingPaginateTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Start": Union[datetime, str],
+        "End": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
 AssociateDelegationSignerToDomainRequestRequestTypeDef = TypedDict(
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "SigningAttributes": DnssecSigningAttributesTypeDef,
@@ -747,23 +779,23 @@
 )
 
 ViewBillingResponseTypeDef = TypedDict(
     "ViewBillingResponseTypeDef",
     {
         "NextPageMarker": str,
         "BillingRecords": List[BillingRecordTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CheckDomainTransferabilityResponseTypeDef = TypedDict(
     "CheckDomainTransferabilityResponseTypeDef",
     {
         "Transferability": DomainTransferabilityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ContactDetailTypeDef = TypedDict(
     "ContactDetailTypeDef",
     {
         "FirstName": str,
@@ -797,24 +829,24 @@
     total=False,
 )
 
 GetDomainSuggestionsResponseTypeDef = TypedDict(
     "GetDomainSuggestionsResponseTypeDef",
     {
         "SuggestionsList": List[DomainSuggestionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -831,52 +863,20 @@
 
 class UpdateDomainNameserversRequestRequestTypeDef(
     _RequiredUpdateDomainNameserversRequestRequestTypeDef,
     _OptionalUpdateDomainNameserversRequestRequestTypeDef,
 ):
     pass
 
-ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
-    "ListOperationsRequestListOperationsPaginateTypeDef",
-    {
-        "SubmittedSince": Union[datetime, str],
-        "Status": Sequence[OperationStatusType],
-        "Type": Sequence[OperationTypeType],
-        "SortBy": Literal["SubmittedDate"],
-        "SortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPricesRequestListPricesPaginateTypeDef = TypedDict(
-    "ListPricesRequestListPricesPaginateTypeDef",
-    {
-        "Tld": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
-    "ViewBillingRequestViewBillingPaginateTypeDef",
-    {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
     "ListDomainsRequestListDomainsPaginateTypeDef",
     {
         "FilterConditions": Sequence[FilterConditionTypeDef],
         "SortCondition": SortConditionTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
@@ -889,23 +889,23 @@
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForDomainResponseTypeDef = TypedDict(
     "ListTagsForDomainResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -946,15 +946,15 @@
         "CreationDate": datetime,
         "UpdatedDate": datetime,
         "ExpirationDate": datetime,
         "Reseller": str,
         "DnsSec": str,
         "StatusList": List[str],
         "DnssecKeys": List[DnssecKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1034,10 +1034,10 @@
     pass
 
 ListPricesResponseTypeDef = TypedDict(
     "ListPricesResponseTypeDef",
     {
         "Prices": List[DomainPriceTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/PKG-INFO` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53domains
-Version: 1.26.34
-Summary: Type annotations for boto3.Route53Domains 1.26.34 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.Route53Domains 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-route53domains"></a>
 
 # mypy-boto3-route53domains
 
 [![PyPI - mypy-boto3-route53domains](https://img.shields.io/pypi/v/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53domains?color=blue)](https://pypistats.org/packages/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.26.34](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,88 +345,88 @@
 
 `mypy_boto3_route53domains.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53domains.type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     DnssecSigningAttributesTypeDef,
+    AssociateDelegationSignerToDomainResponseTypeDef,
     BillingRecordTypeDef,
     CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef,
+    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityRequestRequestTypeDef,
+    CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityRequestRequestTypeDef,
     DomainTransferabilityTypeDef,
     ConsentTypeDef,
     ExtraParamTypeDef,
     DeleteDomainRequestRequestTypeDef,
+    DeleteDomainResponseTypeDef,
     DeleteTagsForDomainRequestRequestTypeDef,
     DisableDomainAutoRenewRequestRequestTypeDef,
     DisableDomainTransferLockRequestRequestTypeDef,
+    DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainRequestRequestTypeDef,
+    DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecKeyTypeDef,
     PriceWithCurrencyTypeDef,
     DomainSuggestionTypeDef,
     DomainSummaryTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableDomainAutoRenewRequestRequestTypeDef,
     EnableDomainTransferLockRequestRequestTypeDef,
+    EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
     GetContactReachabilityStatusRequestRequestTypeDef,
+    GetContactReachabilityStatusResponseTypeDef,
     GetDomainDetailRequestRequestTypeDef,
     NameserverTypeDef,
     GetDomainSuggestionsRequestRequestTypeDef,
     GetOperationDetailRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetOperationDetailResponseTypeDef,
     SortConditionTypeDef,
+    ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
+    ListPricesRequestListPricesPaginateTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
     TagTypeDef,
+    PaginatorConfigTypeDef,
     PushDomainRequestRequestTypeDef,
+    RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
+    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainRequestRequestTypeDef,
+    RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
+    ResendContactReachabilityEmailResponseTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
-    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
-    UpdateDomainContactPrivacyRequestRequestTypeDef,
-    ViewBillingRequestRequestTypeDef,
-    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
-    AssociateDelegationSignerToDomainResponseTypeDef,
-    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
-    CheckDomainAvailabilityResponseTypeDef,
-    DeleteDomainResponseTypeDef,
-    DisableDomainTransferLockResponseTypeDef,
-    DisassociateDelegationSignerFromDomainResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnableDomainTransferLockResponseTypeDef,
-    GetContactReachabilityStatusResponseTypeDef,
-    GetOperationDetailResponseTypeDef,
-    RegisterDomainResponseTypeDef,
-    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
-    RenewDomainResponseTypeDef,
-    ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     TransferDomainResponseTypeDef,
+    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
+    UpdateDomainContactPrivacyRequestRequestTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
+    ViewBillingRequestRequestTypeDef,
+    ViewBillingRequestViewBillingPaginateTypeDef,
     AssociateDelegationSignerToDomainRequestRequestTypeDef,
     ViewBillingResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ContactDetailTypeDef,
     DomainPriceTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     ListDomainsResponseTypeDef,
     UpdateDomainNameserversRequestRequestTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
-    ListPricesRequestListPricesPaginateTypeDef,
-    ViewBillingRequestViewBillingPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
     GetDomainDetailResponseTypeDef,
     RegisterDomainRequestRequestTypeDef,
@@ -443,42 +443,42 @@
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

### Comparing `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/SOURCES.txt` & `mypy-boto3-route53domains-1.27.0/mypy_boto3_route53domains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.26.34/setup.py` & `mypy-boto3-route53domains-1.27.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-route53domains.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53domains",
-    version="1.26.34",
+    version="1.27.0",
     packages=["mypy_boto3_route53domains"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53Domains 1.26.34 service generated with"
-        " mypy-boto3-builder 7.12.0"
+        "Type annotations for boto3.Route53Domains 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/",
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


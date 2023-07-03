# Comparing `tmp/mypy-boto3-service-quotas-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-service-quotas-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-service-quotas-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:59 2022, max compression
+gzip compressed data, was "mypy-boto3-service-quotas-1.27.0.tar", last modified: Mon Jul  3 19:51:26 2023, max compression
```

## Comparing `mypy-boto3-service-quotas-1.26.0.post1.tar` & `mypy-boto3-service-quotas-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:59.504849 mypy-boto3-service-quotas-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16714 2022-11-01 21:43:59.504849 mypy-boto3-service-quotas-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15246 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:59.496849 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19444 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    19412 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9064 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9062 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8737 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8729 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    17522 2022-11-01 21:41:13.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    17509 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:59.504849 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16714 2022-11-01 21:43:59.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-01 21:43:59.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:59.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:59.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:59.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-01 21:43:59.000000 mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:59.504849 mypy-boto3-service-quotas-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-11-01 21:41:12.000000 mypy-boto3-service-quotas-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.783986 mypy-boto3-service-quotas-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-07-03 19:51:26.783986 mypy-boto3-service-quotas-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.783986 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17562 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17549 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.783986 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-07-03 19:51:26.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:51:26.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:26.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:26.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:26.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:51:26.000000 mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:26.783986 mypy-boto3-service-quotas-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-03 19:47:54.000000 mypy-boto3-service-quotas-1.27.0/setup.py
```

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/LICENSE` & `mypy-boto3-service-quotas-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/PKG-INFO` & `mypy-boto3-service-quotas-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-service-quotas
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ServiceQuotas 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ServiceQuotas 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/
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
 
 <a id="mypy-boto3-service-quotas"></a>
 
 # mypy-boto3-service-quotas
 
 [![PyPI - mypy-boto3-service-quotas](https://img.shields.io/pypi/v/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-service-quotas?color=blue)](https://pypistats.org/packages/mypy-boto3-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceQuotas 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[boto3.ServiceQuotas 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [mypy-boto3-service-quotas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,49 +354,49 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_service_quotas.type_defs import (
     DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ErrorReasonTypeDef,
     GetAWSDefaultServiceQuotaRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeRequestRequestTypeDef,
     RequestedServiceQuotaChangeTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ServiceQuotaIncreaseRequestInTemplateTypeDef,
     GetServiceQuotaRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
     ListAWSDefaultServiceQuotasRequestRequestTypeDef,
+    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
+    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
+    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
+    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
     ListServiceQuotasRequestRequestTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     MetricInfoTypeDef,
+    PaginatorConfigTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
     QuotaPeriodTypeDef,
     RequestServiceQuotaIncreaseRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
     RequestServiceQuotaIncreaseResponseTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef,
-    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
-    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ServiceQuotaTypeDef,
     GetAWSDefaultServiceQuotaResponseTypeDef,
     GetServiceQuotaResponseTypeDef,
     ListAWSDefaultServiceQuotasResponseTypeDef,
@@ -410,42 +411,42 @@
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

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/README.md` & `mypy-boto3-service-quotas-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-service-quotas"></a>
 
 # mypy-boto3-service-quotas
 
 [![PyPI - mypy-boto3-service-quotas](https://img.shields.io/pypi/v/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-service-quotas?color=blue)](https://pypistats.org/packages/mypy-boto3-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceQuotas 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[boto3.ServiceQuotas 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [mypy-boto3-service-quotas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,49 +322,49 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_service_quotas.type_defs import (
     DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ErrorReasonTypeDef,
     GetAWSDefaultServiceQuotaRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeRequestRequestTypeDef,
     RequestedServiceQuotaChangeTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ServiceQuotaIncreaseRequestInTemplateTypeDef,
     GetServiceQuotaRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
     ListAWSDefaultServiceQuotasRequestRequestTypeDef,
+    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
+    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
+    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
+    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
     ListServiceQuotasRequestRequestTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     MetricInfoTypeDef,
+    PaginatorConfigTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
     QuotaPeriodTypeDef,
     RequestServiceQuotaIncreaseRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
     RequestServiceQuotaIncreaseResponseTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef,
-    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
-    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ServiceQuotaTypeDef,
     GetAWSDefaultServiceQuotaResponseTypeDef,
     GetServiceQuotaResponseTypeDef,
     ListAWSDefaultServiceQuotasResponseTypeDef,
@@ -379,42 +379,42 @@
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

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/__init__.py` & `mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/__init__.pyi` & `mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/client.py` & `mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/client.pyi` & `mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/literals.py` & `mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,23 +71,25 @@
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
@@ -97,30 +99,35 @@
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
@@ -146,14 +153,15 @@
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
@@ -198,51 +206,57 @@
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
@@ -255,14 +269,15 @@
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
@@ -274,28 +289,35 @@
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
@@ -304,14 +326,15 @@
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
@@ -322,55 +345,64 @@
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
@@ -403,24 +435,29 @@
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

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/literals.pyi` & `mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -69,23 +69,25 @@
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
@@ -95,30 +97,35 @@
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
@@ -144,14 +151,15 @@
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
@@ -196,51 +204,57 @@
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
@@ -253,14 +267,15 @@
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
@@ -272,28 +287,35 @@
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
@@ -302,14 +324,15 @@
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
@@ -320,55 +343,64 @@
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
@@ -401,24 +433,29 @@
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

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/paginator.py` & `mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,119 +49,111 @@
     "ListRequestedServiceQuotaChangeHistoryPaginator",
     "ListRequestedServiceQuotaChangeHistoryByQuotaPaginator",
     "ListServiceQuotaIncreaseRequestsInTemplatePaginator",
     "ListServiceQuotasPaginator",
     "ListServicesPaginator",
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
 class ListAWSDefaultServiceQuotasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listawsdefaultservicequotaspaginator)
     """
 
     def paginate(
-        self, *, ServiceCode: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ServiceCode: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAWSDefaultServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listawsdefaultservicequotaspaginator)
         """
 
-
 class ListRequestedServiceQuotaChangeHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listrequestedservicequotachangehistorypaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         Status: RequestStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRequestedServiceQuotaChangeHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listrequestedservicequotachangehistorypaginator)
         """
 
-
 class ListRequestedServiceQuotaChangeHistoryByQuotaPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistoryByQuota)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listrequestedservicequotachangehistorybyquotapaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         QuotaCode: str,
         Status: RequestStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistoryByQuota.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listrequestedservicequotachangehistorybyquotapaginator)
         """
 
-
 class ListServiceQuotaIncreaseRequestsInTemplatePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotaIncreaseRequestsInTemplate)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaincreaserequestsintemplatepaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         AwsRegion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotaIncreaseRequestsInTemplate.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaincreaserequestsintemplatepaginator)
         """
 
-
 class ListServiceQuotasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaspaginator)
     """
 
     def paginate(
-        self, *, ServiceCode: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ServiceCode: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaspaginator)
         """
 
-
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicespaginator)
         """
```

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/paginator.pyi` & `mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,111 +49,119 @@
     "ListRequestedServiceQuotaChangeHistoryPaginator",
     "ListRequestedServiceQuotaChangeHistoryByQuotaPaginator",
     "ListServiceQuotaIncreaseRequestsInTemplatePaginator",
     "ListServiceQuotasPaginator",
     "ListServicesPaginator",
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
 class ListAWSDefaultServiceQuotasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listawsdefaultservicequotaspaginator)
     """
 
     def paginate(
-        self, *, ServiceCode: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ServiceCode: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAWSDefaultServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listawsdefaultservicequotaspaginator)
         """
 
+
 class ListRequestedServiceQuotaChangeHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listrequestedservicequotachangehistorypaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         Status: RequestStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRequestedServiceQuotaChangeHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listrequestedservicequotachangehistorypaginator)
         """
 
+
 class ListRequestedServiceQuotaChangeHistoryByQuotaPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistoryByQuota)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listrequestedservicequotachangehistorybyquotapaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         QuotaCode: str,
         Status: RequestStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistoryByQuota.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listrequestedservicequotachangehistorybyquotapaginator)
         """
 
+
 class ListServiceQuotaIncreaseRequestsInTemplatePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotaIncreaseRequestsInTemplate)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaincreaserequestsintemplatepaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         AwsRegion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotaIncreaseRequestsInTemplate.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaincreaserequestsintemplatepaginator)
         """
 
+
 class ListServiceQuotasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaspaginator)
     """
 
     def paginate(
-        self, *, ServiceCode: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ServiceCode: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaspaginator)
         """
 
+
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicespaginator)
         """
```

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/type_defs.py` & `mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,49 +28,49 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ErrorReasonTypeDef",
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     "RequestedServiceQuotaChangeTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ServiceQuotaIncreaseRequestInTemplateTypeDef",
     "GetServiceQuotaRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
     "ListAWSDefaultServiceQuotasRequestRequestTypeDef",
+    "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
+    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
+    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
+    "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
     "ListServiceQuotasRequestRequestTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ServiceInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "MetricInfoTypeDef",
+    "PaginatorConfigTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     "QuotaPeriodTypeDef",
     "RequestServiceQuotaIncreaseRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     "RequestServiceQuotaIncreaseResponseTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef",
-    "ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
-    "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
-    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
-    "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ServiceQuotaTypeDef",
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     "GetServiceQuotaResponseTypeDef",
     "ListAWSDefaultServiceQuotasResponseTypeDef",
@@ -99,22 +99,19 @@
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetAssociationForServiceQuotaTemplateResponseTypeDef = TypedDict(
+    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ServiceQuotaTemplateAssociationStatus": ServiceQuotaTemplateAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRequestedServiceQuotaChangeRequestRequestTypeDef = TypedDict(
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     {
         "RequestId": str,
@@ -170,24 +167,36 @@
     "GetServiceQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
+    "_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ServiceCode": str,
+    },
+)
+_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
+    "_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef(
+    _RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    _OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef = TypedDict(
     "_RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalListAWSDefaultServiceQuotasRequestRequestTypeDef = TypedDict(
@@ -203,14 +212,38 @@
 class ListAWSDefaultServiceQuotasRequestRequestTypeDef(
     _RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef,
     _OptionalListAWSDefaultServiceQuotasRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
+    "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "QuotaCode": str,
+    },
+)
+_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
+    "_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    {
+        "Status": RequestStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef(
+    _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+    _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef = TypedDict(
     "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
@@ -228,36 +261,78 @@
 class ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef(
     _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
     _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
 ):
     pass
 
 
+ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef = TypedDict(
+    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "Status": RequestStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "Status": RequestStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef = TypedDict(
+    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "AwsRegion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef = TypedDict(
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "AwsRegion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
+    "_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    {
+        "ServiceCode": str,
+    },
+)
+_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
+    "_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListServiceQuotasRequestListServiceQuotasPaginateTypeDef(
+    _RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+    _OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListServiceQuotasRequestRequestTypeDef = TypedDict(
     "_RequiredListServiceQuotasRequestRequestTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalListServiceQuotasRequestRequestTypeDef = TypedDict(
@@ -272,14 +347,22 @@
 
 class ListServiceQuotasRequestRequestTypeDef(
     _RequiredListServiceQuotasRequestRequestTypeDef, _OptionalListServiceQuotasRequestRequestTypeDef
 ):
     pass
 
 
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -316,14 +399,24 @@
         "MetricName": str,
         "MetricDimensions": Dict[str, str],
         "MetricStatisticRecommendation": str,
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
 PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef = TypedDict(
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     {
         "QuotaCode": str,
         "ServiceCode": str,
         "AwsRegion": str,
         "DesiredValue": float,
@@ -344,201 +437,108 @@
     {
         "ServiceCode": str,
         "QuotaCode": str,
         "DesiredValue": float,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-GetAssociationForServiceQuotaTemplateResponseTypeDef = TypedDict(
-    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "ServiceQuotaTemplateAssociationStatus": ServiceQuotaTemplateAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
 
 GetRequestedServiceQuotaChangeResponseTypeDef = TypedDict(
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     {
         "RequestedQuota": RequestedServiceQuotaChangeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     {
         "NextToken": str,
         "RequestedQuotas": List[RequestedServiceQuotaChangeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRequestedServiceQuotaChangeHistoryResponseTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     {
         "NextToken": str,
         "RequestedQuotas": List[RequestedServiceQuotaChangeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RequestServiceQuotaIncreaseResponseTypeDef = TypedDict(
     "RequestServiceQuotaIncreaseResponseTypeDef",
     {
         "RequestedQuota": RequestedServiceQuotaChangeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef = TypedDict(
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplate": ServiceQuotaIncreaseRequestInTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef = TypedDict(
     "ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplateList": List[
             ServiceQuotaIncreaseRequestInTemplateTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef = TypedDict(
     "PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplate": ServiceQuotaIncreaseRequestInTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
-    "_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
-    {
-        "ServiceCode": str,
-    },
-)
-_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
-    "_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef(
-    _RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-    _OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
-    "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "QuotaCode": str,
-    },
-)
-_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
-    "_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    {
-        "Status": RequestStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef(
-    _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-    _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-):
-    pass
-
-
-ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef = TypedDict(
-    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "Status": RequestStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef = TypedDict(
-    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "AwsRegion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
-    "_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    {
-        "ServiceCode": str,
-    },
-)
-_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
-    "_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListServiceQuotasRequestListServiceQuotasPaginateTypeDef(
-    _RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-    _OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-):
-    pass
-
-
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "NextToken": str,
         "Services": List[ServiceInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
         "ResourceARN": str,
@@ -565,36 +565,36 @@
     total=False,
 )
 
 GetAWSDefaultServiceQuotaResponseTypeDef = TypedDict(
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceQuotaResponseTypeDef = TypedDict(
     "GetServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAWSDefaultServiceQuotasResponseTypeDef = TypedDict(
     "ListAWSDefaultServiceQuotasResponseTypeDef",
     {
         "NextToken": str,
         "Quotas": List[ServiceQuotaTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceQuotasResponseTypeDef = TypedDict(
     "ListServiceQuotasResponseTypeDef",
     {
         "NextToken": str,
         "Quotas": List[ServiceQuotaTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas/type_defs.pyi` & `mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -27,49 +27,49 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ErrorReasonTypeDef",
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     "RequestedServiceQuotaChangeTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ServiceQuotaIncreaseRequestInTemplateTypeDef",
     "GetServiceQuotaRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
     "ListAWSDefaultServiceQuotasRequestRequestTypeDef",
+    "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
+    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
+    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
+    "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
     "ListServiceQuotasRequestRequestTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ServiceInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "MetricInfoTypeDef",
+    "PaginatorConfigTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     "QuotaPeriodTypeDef",
     "RequestServiceQuotaIncreaseRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     "RequestServiceQuotaIncreaseResponseTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef",
-    "ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
-    "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
-    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
-    "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ServiceQuotaTypeDef",
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     "GetServiceQuotaResponseTypeDef",
     "ListAWSDefaultServiceQuotasResponseTypeDef",
@@ -98,22 +98,19 @@
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetAssociationForServiceQuotaTemplateResponseTypeDef = TypedDict(
+    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ServiceQuotaTemplateAssociationStatus": ServiceQuotaTemplateAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRequestedServiceQuotaChangeRequestRequestTypeDef = TypedDict(
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     {
         "RequestId": str,
@@ -169,24 +166,34 @@
     "GetServiceQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
+    "_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ServiceCode": str,
+    },
+)
+_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
+    "_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef(
+    _RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    _OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+):
+    pass
+
 _RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef = TypedDict(
     "_RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalListAWSDefaultServiceQuotasRequestRequestTypeDef = TypedDict(
@@ -200,14 +207,36 @@
 
 class ListAWSDefaultServiceQuotasRequestRequestTypeDef(
     _RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef,
     _OptionalListAWSDefaultServiceQuotasRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
+    "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "QuotaCode": str,
+    },
+)
+_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
+    "_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    {
+        "Status": RequestStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef(
+    _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+    _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+):
+    pass
+
 _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef = TypedDict(
     "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
@@ -223,36 +252,76 @@
 
 class ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef(
     _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
     _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
 ):
     pass
 
+ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef = TypedDict(
+    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "Status": RequestStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "Status": RequestStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef = TypedDict(
+    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "AwsRegion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef = TypedDict(
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "AwsRegion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
+    "_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    {
+        "ServiceCode": str,
+    },
+)
+_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
+    "_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListServiceQuotasRequestListServiceQuotasPaginateTypeDef(
+    _RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+    _OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+):
+    pass
+
 _RequiredListServiceQuotasRequestRequestTypeDef = TypedDict(
     "_RequiredListServiceQuotasRequestRequestTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalListServiceQuotasRequestRequestTypeDef = TypedDict(
@@ -265,14 +334,22 @@
 )
 
 class ListServiceQuotasRequestRequestTypeDef(
     _RequiredListServiceQuotasRequestRequestTypeDef, _OptionalListServiceQuotasRequestRequestTypeDef
 ):
     pass
 
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -309,14 +386,24 @@
         "MetricName": str,
         "MetricDimensions": Dict[str, str],
         "MetricStatisticRecommendation": str,
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
 PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef = TypedDict(
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     {
         "QuotaCode": str,
         "ServiceCode": str,
         "AwsRegion": str,
         "DesiredValue": float,
@@ -337,195 +424,108 @@
     {
         "ServiceCode": str,
         "QuotaCode": str,
         "DesiredValue": float,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-GetAssociationForServiceQuotaTemplateResponseTypeDef = TypedDict(
-    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "ServiceQuotaTemplateAssociationStatus": ServiceQuotaTemplateAssociationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
 
 GetRequestedServiceQuotaChangeResponseTypeDef = TypedDict(
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     {
         "RequestedQuota": RequestedServiceQuotaChangeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     {
         "NextToken": str,
         "RequestedQuotas": List[RequestedServiceQuotaChangeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRequestedServiceQuotaChangeHistoryResponseTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     {
         "NextToken": str,
         "RequestedQuotas": List[RequestedServiceQuotaChangeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RequestServiceQuotaIncreaseResponseTypeDef = TypedDict(
     "RequestServiceQuotaIncreaseResponseTypeDef",
     {
         "RequestedQuota": RequestedServiceQuotaChangeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef = TypedDict(
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplate": ServiceQuotaIncreaseRequestInTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef = TypedDict(
     "ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplateList": List[
             ServiceQuotaIncreaseRequestInTemplateTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef = TypedDict(
     "PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplate": ServiceQuotaIncreaseRequestInTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
-    "_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
-    {
-        "ServiceCode": str,
-    },
-)
-_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
-    "_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef(
-    _RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-    _OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-):
-    pass
-
-_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
-    "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "QuotaCode": str,
-    },
-)
-_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
-    "_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    {
-        "Status": RequestStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef(
-    _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-    _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-):
-    pass
-
-ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef = TypedDict(
-    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "Status": RequestStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef = TypedDict(
-    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "AwsRegion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
-    "_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    {
-        "ServiceCode": str,
-    },
-)
-_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
-    "_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-class ListServiceQuotasRequestListServiceQuotasPaginateTypeDef(
-    _RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-    _OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-):
-    pass
-
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "NextToken": str,
         "Services": List[ServiceInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
         "ResourceARN": str,
@@ -552,36 +552,36 @@
     total=False,
 )
 
 GetAWSDefaultServiceQuotaResponseTypeDef = TypedDict(
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceQuotaResponseTypeDef = TypedDict(
     "GetServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAWSDefaultServiceQuotasResponseTypeDef = TypedDict(
     "ListAWSDefaultServiceQuotasResponseTypeDef",
     {
         "NextToken": str,
         "Quotas": List[ServiceQuotaTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceQuotasResponseTypeDef = TypedDict(
     "ListServiceQuotasResponseTypeDef",
     {
         "NextToken": str,
         "Quotas": List[ServiceQuotaTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas.egg-info/PKG-INFO` & `mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-service-quotas
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ServiceQuotas 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ServiceQuotas 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/
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
 
 <a id="mypy-boto3-service-quotas"></a>
 
 # mypy-boto3-service-quotas
 
 [![PyPI - mypy-boto3-service-quotas](https://img.shields.io/pypi/v/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-service-quotas?color=blue)](https://pypistats.org/packages/mypy-boto3-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceQuotas 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[boto3.ServiceQuotas 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [mypy-boto3-service-quotas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,49 +354,49 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_service_quotas.type_defs import (
     DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ErrorReasonTypeDef,
     GetAWSDefaultServiceQuotaRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeRequestRequestTypeDef,
     RequestedServiceQuotaChangeTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ServiceQuotaIncreaseRequestInTemplateTypeDef,
     GetServiceQuotaRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
     ListAWSDefaultServiceQuotasRequestRequestTypeDef,
+    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
+    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
+    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
+    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
     ListServiceQuotasRequestRequestTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     MetricInfoTypeDef,
+    PaginatorConfigTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
     QuotaPeriodTypeDef,
     RequestServiceQuotaIncreaseRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
     RequestServiceQuotaIncreaseResponseTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef,
-    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
-    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ServiceQuotaTypeDef,
     GetAWSDefaultServiceQuotaResponseTypeDef,
     GetServiceQuotaResponseTypeDef,
     ListAWSDefaultServiceQuotasResponseTypeDef,
@@ -410,42 +411,42 @@
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

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/mypy_boto3_service_quotas.egg-info/SOURCES.txt` & `mypy-boto3-service-quotas-1.27.0/mypy_boto3_service_quotas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.26.0.post1/setup.py` & `mypy-boto3-service-quotas-1.27.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-service-quotas.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-service-quotas",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_service_quotas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServiceQuotas 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.ServiceQuotas 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 service-quotas type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_service_quotas": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_service_quotas": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/",
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


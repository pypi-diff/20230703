# Comparing `tmp/mypy-boto3-es-1.26.7.tar.gz` & `tmp/mypy-boto3-es-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-es-1.26.7.tar", last modified: Thu Nov 10 20:32:39 2022, max compression
+gzip compressed data, was "mypy-boto3-es-1.27.0.tar", last modified: Mon Jul  3 19:50:45 2023, max compression
```

## Comparing `mypy-boto3-es-1.26.7.tar` & `mypy-boto3-es-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:39.505201 mypy-boto3-es-1.26.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-10 20:32:25.000000 mypy-boto3-es-1.26.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    22268 2022-11-10 20:32:39.501201 mypy-boto3-es-1.26.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20835 2022-11-10 20:32:25.000000 mypy-boto3-es-1.26.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:39.493201 mypy-boto3-es-1.26.7/mypy_boto3_es/
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-11-10 20:32:25.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-11-10 20:32:25.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-10 20:32:25.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40848 2022-11-10 20:32:26.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    40786 2022-11-10 20:32:26.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13793 2022-11-10 20:32:26.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    13791 2022-11-10 20:32:26.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7209 2022-11-10 20:32:26.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7202 2022-11-10 20:32:26.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:25.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    63575 2022-11-10 20:32:27.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    63528 2022-11-10 20:32:27.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-10 20:32:25.000000 mypy-boto3-es-1.26.7/mypy_boto3_es/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:39.501201 mypy-boto3-es-1.26.7/mypy_boto3_es.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22268 2022-11-10 20:32:39.000000 mypy-boto3-es-1.26.7/mypy_boto3_es.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-11-10 20:32:39.000000 mypy-boto3-es-1.26.7/mypy_boto3_es.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 20:32:39.000000 mypy-boto3-es-1.26.7/mypy_boto3_es.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 20:32:39.000000 mypy-boto3-es-1.26.7/mypy_boto3_es.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-10 20:32:39.000000 mypy-boto3-es-1.26.7/mypy_boto3_es.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-10 20:32:39.000000 mypy-boto3-es-1.26.7/mypy_boto3_es.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 20:32:39.505201 mypy-boto3-es-1.26.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-11-10 20:32:25.000000 mypy-boto3-es-1.26.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.531234 mypy-boto3-es-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22291 2023-07-03 19:50:45.527234 mypy-boto3-es-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20808 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.527234 mypy-boto3-es-1.27.0/mypy_boto3_es/
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40848 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40786 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14514 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63679 2023-07-03 19:37:37.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63632 2023-07-03 19:37:36.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/mypy_boto3_es/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.527234 mypy-boto3-es-1.27.0/mypy_boto3_es.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22291 2023-07-03 19:50:45.000000 mypy-boto3-es-1.27.0/mypy_boto3_es.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-03 19:50:45.000000 mypy-boto3-es-1.27.0/mypy_boto3_es.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-es-1.27.0/mypy_boto3_es.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-es-1.27.0/mypy_boto3_es.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:45.000000 mypy-boto3-es-1.27.0/mypy_boto3_es.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 19:50:45.000000 mypy-boto3-es-1.27.0/mypy_boto3_es.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:45.531234 mypy-boto3-es-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-03 19:37:34.000000 mypy-boto3-es-1.27.0/setup.py
```

### Comparing `mypy-boto3-es-1.26.7/LICENSE` & `mypy-boto3-es-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-es-1.26.7/PKG-INFO` & `mypy-boto3-es-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-es
-Version: 1.26.7
-Summary: Type annotations for boto3.ElasticsearchService 1.26.7 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ElasticsearchService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/
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
 
 <a id="mypy-boto3-es"></a>
 
 # mypy-boto3-es
 
 [![PyPI - mypy-boto3-es](https://img.shields.io/pypi/v/mypy-boto3-es.svg?color=blue)](https://pypi.org/project/mypy-boto3-es)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-es.svg?color=blue)](https://pypi.org/project/mypy-boto3-es)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-es?color=blue)](https://pypistats.org/packages/mypy-boto3-es)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticsearchService 1.26.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
+[boto3.ElasticsearchService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
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
 [mypy-boto3-es docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,15 +370,14 @@
 
 `mypy_boto3_es.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_es.type_defs import (
     AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
@@ -412,56 +412,62 @@
     DescribeDomainChangeProgressRequestRequestTypeDef,
     DescribeElasticsearchDomainConfigRequestRequestTypeDef,
     DescribeElasticsearchDomainRequestRequestTypeDef,
     DescribeElasticsearchDomainsRequestRequestTypeDef,
     DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef,
     FilterTypeDef,
     DescribePackagesFilterTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef,
     DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef,
+    DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef,
     DescribeReservedElasticsearchInstancesRequestRequestTypeDef,
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
     DryRunResultsTypeDef,
     ZoneAwarenessConfigTypeDef,
     VPCDerivedInfoTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCompatibleElasticsearchVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
+    GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
+    GetUpgradeStatusResponseTypeDef,
     InboundCrossClusterSearchConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
+    ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
     ListElasticsearchInstanceTypesRequestRequestTypeDef,
+    ListElasticsearchInstanceTypesResponseTypeDef,
+    ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef,
     ListElasticsearchVersionsRequestRequestTypeDef,
+    ListElasticsearchVersionsResponseTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
+    PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpgradeElasticsearchDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetUpgradeStatusResponseTypeDef,
-    ListElasticsearchInstanceTypesResponseTypeDef,
-    ListElasticsearchVersionsResponseTypeDef,
-    PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     ElasticsearchVersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
@@ -488,19 +494,14 @@
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef,
     DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
-    DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef,
-    DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef,
-    GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
-    ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
-    ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
     ElasticsearchClusterConfigTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
@@ -564,42 +565,42 @@
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

### Comparing `mypy-boto3-es-1.26.7/README.md` & `mypy-boto3-es-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-es"></a>
 
 # mypy-boto3-es
 
 [![PyPI - mypy-boto3-es](https://img.shields.io/pypi/v/mypy-boto3-es.svg?color=blue)](https://pypi.org/project/mypy-boto3-es)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-es.svg?color=blue)](https://pypi.org/project/mypy-boto3-es)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-es?color=blue)](https://pypistats.org/packages/mypy-boto3-es)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticsearchService 1.26.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
+[boto3.ElasticsearchService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
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
 [mypy-boto3-es docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,15 +338,14 @@
 
 `mypy_boto3_es.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_es.type_defs import (
     AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
@@ -381,56 +380,62 @@
     DescribeDomainChangeProgressRequestRequestTypeDef,
     DescribeElasticsearchDomainConfigRequestRequestTypeDef,
     DescribeElasticsearchDomainRequestRequestTypeDef,
     DescribeElasticsearchDomainsRequestRequestTypeDef,
     DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef,
     FilterTypeDef,
     DescribePackagesFilterTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef,
     DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef,
+    DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef,
     DescribeReservedElasticsearchInstancesRequestRequestTypeDef,
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
     DryRunResultsTypeDef,
     ZoneAwarenessConfigTypeDef,
     VPCDerivedInfoTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCompatibleElasticsearchVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
+    GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
+    GetUpgradeStatusResponseTypeDef,
     InboundCrossClusterSearchConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
+    ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
     ListElasticsearchInstanceTypesRequestRequestTypeDef,
+    ListElasticsearchInstanceTypesResponseTypeDef,
+    ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef,
     ListElasticsearchVersionsRequestRequestTypeDef,
+    ListElasticsearchVersionsResponseTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
+    PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpgradeElasticsearchDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetUpgradeStatusResponseTypeDef,
-    ListElasticsearchInstanceTypesResponseTypeDef,
-    ListElasticsearchVersionsResponseTypeDef,
-    PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     ElasticsearchVersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
@@ -457,19 +462,14 @@
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef,
     DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
-    DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef,
-    DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef,
-    GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
-    ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
-    ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
     ElasticsearchClusterConfigTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
@@ -533,42 +533,42 @@
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

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es/__init__.py` & `mypy-boto3-es-1.27.0/mypy_boto3_es/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es/__init__.pyi` & `mypy-boto3-es-1.27.0/mypy_boto3_es/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es/__main__.py` & `mypy-boto3-es-1.27.0/mypy_boto3_es/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticsearchService 1.26.7\nVersion:         1.26.7\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.ElasticsearchService 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.7")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es/client.py` & `mypy-boto3-es-1.27.0/mypy_boto3_es/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es/client.pyi` & `mypy-boto3-es-1.27.0/mypy_boto3_es/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es/literals.py` & `mypy-boto3-es-1.27.0/mypy_boto3_es/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -209,23 +209,25 @@
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
@@ -235,30 +237,35 @@
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
@@ -284,14 +291,15 @@
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
@@ -336,51 +344,57 @@
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
@@ -393,14 +407,15 @@
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
@@ -412,28 +427,35 @@
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
@@ -461,56 +483,64 @@
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
@@ -542,22 +572,25 @@
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
     "eu-central-2",
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

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es/literals.pyi` & `mypy-boto3-es-1.27.0/mypy_boto3_es/literals.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -207,23 +207,25 @@
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
@@ -233,30 +235,35 @@
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
@@ -282,14 +289,15 @@
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
@@ -334,51 +342,57 @@
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
@@ -391,14 +405,15 @@
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
@@ -410,28 +425,35 @@
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
@@ -459,56 +481,64 @@
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
@@ -540,22 +570,25 @@
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
     "eu-central-2",
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

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es/paginator.py` & `mypy-boto3-es-1.27.0/mypy_boto3_es/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#describereservedelasticsearchinstanceofferingspaginator)
     """
 
     def paginate(
         self,
         *,
         ReservedElasticsearchInstanceOfferingId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstanceOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#describereservedelasticsearchinstanceofferingspaginator)
         """
 
 
@@ -83,30 +83,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#describereservedelasticsearchinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         ReservedElasticsearchInstanceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReservedElasticsearchInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#describereservedelasticsearchinstancespaginator)
         """
 
 
 class GetUpgradeHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.GetUpgradeHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#getupgradehistorypaginator)
     """
 
     def paginate(
-        self, *, DomainName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DomainName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetUpgradeHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.GetUpgradeHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#getupgradehistorypaginator)
         """
 
 
@@ -117,28 +117,28 @@
     """
 
     def paginate(
         self,
         *,
         ElasticsearchVersion: str,
         DomainName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListElasticsearchInstanceTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchInstanceTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#listelasticsearchinstancetypespaginator)
         """
 
 
 class ListElasticsearchVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#listelasticsearchversionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListElasticsearchVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#listelasticsearchversionspaginator)
         """
```

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es/paginator.pyi` & `mypy-boto3-es-1.27.0/mypy_boto3_es/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#describereservedelasticsearchinstanceofferingspaginator)
     """
 
     def paginate(
         self,
         *,
         ReservedElasticsearchInstanceOfferingId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstanceOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#describereservedelasticsearchinstanceofferingspaginator)
         """
 
 class DescribeReservedElasticsearchInstancesPaginator(Paginator):
@@ -79,29 +79,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#describereservedelasticsearchinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         ReservedElasticsearchInstanceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReservedElasticsearchInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#describereservedelasticsearchinstancespaginator)
         """
 
 class GetUpgradeHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.GetUpgradeHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#getupgradehistorypaginator)
     """
 
     def paginate(
-        self, *, DomainName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DomainName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetUpgradeHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.GetUpgradeHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#getupgradehistorypaginator)
         """
 
 class ListElasticsearchInstanceTypesPaginator(Paginator):
@@ -111,27 +111,27 @@
     """
 
     def paginate(
         self,
         *,
         ElasticsearchVersion: str,
         DomainName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListElasticsearchInstanceTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchInstanceTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#listelasticsearchinstancetypespaginator)
         """
 
 class ListElasticsearchVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#listelasticsearchversionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListElasticsearchVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/paginators/#listelasticsearchversionspaginator)
         """
```

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es/type_defs.py` & `mypy-boto3-es-1.27.0/mypy_boto3_es/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "OptionStatusTypeDef",
     "TagTypeDef",
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
     "AssociatePackageRequestRequestTypeDef",
     "AuthorizeVpcEndpointAccessRequestRequestTypeDef",
     "AuthorizedPrincipalTypeDef",
@@ -94,56 +93,62 @@
     "DescribeDomainChangeProgressRequestRequestTypeDef",
     "DescribeElasticsearchDomainConfigRequestRequestTypeDef",
     "DescribeElasticsearchDomainRequestRequestTypeDef",
     "DescribeElasticsearchDomainsRequestRequestTypeDef",
     "DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef",
     "FilterTypeDef",
     "DescribePackagesFilterTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
     "DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef",
+    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
     "DescribeReservedElasticsearchInstancesRequestRequestTypeDef",
     "DescribeVpcEndpointsRequestRequestTypeDef",
     "VpcEndpointErrorTypeDef",
     "DissociatePackageRequestRequestTypeDef",
     "DomainInfoTypeDef",
     "ErrorDetailsTypeDef",
     "DryRunResultsTypeDef",
     "ZoneAwarenessConfigTypeDef",
     "VPCDerivedInfoTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetCompatibleElasticsearchVersionsRequestRequestTypeDef",
     "GetPackageVersionHistoryRequestRequestTypeDef",
     "PackageVersionHistoryTypeDef",
+    "GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
     "GetUpgradeHistoryRequestRequestTypeDef",
     "GetUpgradeStatusRequestRequestTypeDef",
+    "GetUpgradeStatusResponseTypeDef",
     "InboundCrossClusterSearchConnectionStatusTypeDef",
     "InstanceCountLimitsTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
+    "ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
     "ListElasticsearchInstanceTypesRequestRequestTypeDef",
+    "ListElasticsearchInstanceTypesResponseTypeDef",
+    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
     "ListElasticsearchVersionsRequestRequestTypeDef",
+    "ListElasticsearchVersionsResponseTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef",
+    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     "SAMLIdpTypeDef",
     "StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
     "UpgradeElasticsearchDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetUpgradeStatusResponseTypeDef",
-    "ListElasticsearchInstanceTypesResponseTypeDef",
-    "ListElasticsearchVersionsResponseTypeDef",
-    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AdvancedOptionsStatusTypeDef",
     "ElasticsearchVersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
@@ -170,19 +175,14 @@
     "UpdatePackageRequestRequestTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "ListVpcEndpointsForDomainResponseTypeDef",
     "ListVpcEndpointsResponseTypeDef",
     "DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef",
     "DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef",
     "DescribePackagesRequestRequestTypeDef",
-    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
-    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
-    "GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
-    "ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
-    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
     "ListDomainNamesResponseTypeDef",
     "DomainPackageDetailsTypeDef",
     "PackageDetailsTypeDef",
     "ElasticsearchClusterConfigTypeDef",
     "VPCDerivedInfoStatusTypeDef",
     "VpcEndpointTypeDef",
     "GetPackageVersionHistoryResponseTypeDef",
@@ -241,25 +241,14 @@
 AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef = TypedDict(
     "AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef",
     {
         "CrossClusterSearchConnectionId": str,
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
 _RequiredOptionStatusTypeDef = TypedDict(
     "_RequiredOptionStatusTypeDef",
     {
         "CreationDate": datetime,
         "UpdateDate": datetime,
         "State": OptionStateType,
     },
@@ -707,34 +696,42 @@
     {
         "Name": DescribePackagesFilterNameType,
         "Value": Sequence[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ReservedElasticsearchInstanceOfferingId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef",
     {
         "ReservedElasticsearchInstanceOfferingId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef = TypedDict(
+    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
+    {
+        "ReservedElasticsearchInstanceId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedElasticsearchInstancesRequestRequestTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstancesRequestRequestTypeDef",
     {
         "ReservedElasticsearchInstanceId": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -808,14 +805,21 @@
         "SubnetIds": List[str],
         "AvailabilityZones": List[str],
         "SecurityGroupIds": List[str],
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
 GetCompatibleElasticsearchVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleElasticsearchVersionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
     total=False,
 )
@@ -849,14 +853,36 @@
         "PackageVersion": str,
         "CommitMessage": str,
         "CreatedAt": datetime,
     },
     total=False,
 )
 
+_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef(
+    _RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
+    _OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetUpgradeHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetUpgradeHistoryRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetUpgradeHistoryRequestRequestTypeDef = TypedDict(
@@ -878,14 +904,24 @@
 GetUpgradeStatusRequestRequestTypeDef = TypedDict(
     "GetUpgradeStatusRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+GetUpgradeStatusResponseTypeDef = TypedDict(
+    "GetUpgradeStatusResponseTypeDef",
+    {
+        "UpgradeStep": UpgradeStepType,
+        "StepStatus": UpgradeStatusType,
+        "UpgradeName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InboundCrossClusterSearchConnectionStatusTypeDef = TypedDict(
     "InboundCrossClusterSearchConnectionStatusTypeDef",
     {
         "StatusCode": InboundCrossClusterSearchConnectionStatusCodeType,
         "Message": str,
     },
     total=False,
@@ -927,14 +963,37 @@
 class ListDomainsForPackageRequestRequestTypeDef(
     _RequiredListDomainsForPackageRequestRequestTypeDef,
     _OptionalListDomainsForPackageRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
+    "_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
+    {
+        "ElasticsearchVersion": str,
+    },
+)
+_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
+    "_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
+    {
+        "DomainName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef(
+    _RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
+    _OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListElasticsearchInstanceTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListElasticsearchInstanceTypesRequestRequestTypeDef",
     {
         "ElasticsearchVersion": str,
     },
 )
 _OptionalListElasticsearchInstanceTypesRequestRequestTypeDef = TypedDict(
@@ -951,23 +1010,49 @@
 class ListElasticsearchInstanceTypesRequestRequestTypeDef(
     _RequiredListElasticsearchInstanceTypesRequestRequestTypeDef,
     _OptionalListElasticsearchInstanceTypesRequestRequestTypeDef,
 ):
     pass
 
 
+ListElasticsearchInstanceTypesResponseTypeDef = TypedDict(
+    "ListElasticsearchInstanceTypesResponseTypeDef",
+    {
+        "ElasticsearchInstanceTypes": List[ESPartitionInstanceTypeType],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef = TypedDict(
+    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListElasticsearchVersionsRequestRequestTypeDef = TypedDict(
     "ListElasticsearchVersionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListElasticsearchVersionsResponseTypeDef = TypedDict(
+    "ListElasticsearchVersionsResponseTypeDef",
+    {
+        "ElasticsearchVersions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListPackagesForDomainRequestRequestTypeDef = TypedDict(
     "_RequiredListPackagesForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListPackagesForDomainRequestRequestTypeDef = TypedDict(
@@ -1042,14 +1127,24 @@
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
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
 _RequiredPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef",
     {
         "ReservedElasticsearchInstanceOfferingId": str,
         "ReservationName": str,
     },
 )
@@ -1065,14 +1160,23 @@
 class PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef(
     _RequiredPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
     _OptionalPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
 ):
     pass
 
 
+PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef = TypedDict(
+    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
+    {
+        "ReservedElasticsearchInstanceId": str,
+        "ReservationName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "RecurringChargeAmount": float,
         "RecurringChargeFrequency": str,
     },
     total=False,
@@ -1089,14 +1193,25 @@
     "RemoveTagsRequestRequestTypeDef",
     {
         "ARN": str,
         "TagKeys": Sequence[str],
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
 RevokeVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
         "Account": str,
     },
 )
@@ -1155,58 +1270,14 @@
         "UpgradeStepStatus": UpgradeStatusType,
         "Issues": List[str],
         "ProgressPercent": float,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUpgradeStatusResponseTypeDef = TypedDict(
-    "GetUpgradeStatusResponseTypeDef",
-    {
-        "UpgradeStep": UpgradeStepType,
-        "StepStatus": UpgradeStatusType,
-        "UpgradeName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListElasticsearchInstanceTypesResponseTypeDef = TypedDict(
-    "ListElasticsearchInstanceTypesResponseTypeDef",
-    {
-        "ElasticsearchInstanceTypes": List[ESPartitionInstanceTypeType],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListElasticsearchVersionsResponseTypeDef = TypedDict(
-    "ListElasticsearchVersionsResponseTypeDef",
-    {
-        "ElasticsearchVersions": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef = TypedDict(
-    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
-    {
-        "ReservedElasticsearchInstanceId": str,
-        "ReservationName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AccessPoliciesStatusTypeDef = TypedDict(
     "AccessPoliciesStatusTypeDef",
     {
         "Options": str,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -1235,32 +1306,32 @@
     },
 )
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthorizeVpcEndpointAccessResponseTypeDef = TypedDict(
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipal": AuthorizedPrincipalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointAccessResponseTypeDef = TypedDict(
     "ListVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipalList": List[AuthorizedPrincipalTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoTuneDetailsTypeDef = TypedDict(
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": ScheduledAutoTuneDetailsTypeDef,
@@ -1278,34 +1349,34 @@
     total=False,
 )
 
 CancelElasticsearchServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "CancelElasticsearchServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartElasticsearchServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "StartElasticsearchServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpgradeElasticsearchDomainResponseTypeDef = TypedDict(
     "UpgradeElasticsearchDomainResponseTypeDef",
     {
         "DomainName": str,
         "TargetVersion": str,
         "PerformCheckOnly": bool,
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeProgressStatusDetailsTypeDef = TypedDict(
     "ChangeProgressStatusDetailsTypeDef",
     {
         "ChangeId": str,
@@ -1327,15 +1398,15 @@
     },
 )
 
 GetCompatibleElasticsearchVersionsResponseTypeDef = TypedDict(
     "GetCompatibleElasticsearchVersionsResponseTypeDef",
     {
         "CompatibleElasticsearchVersions": List[CompatibleVersionsMapTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainEndpointOptionsStatusTypeDef = TypedDict(
     "DomainEndpointOptionsStatusTypeDef",
     {
         "Options": DomainEndpointOptionsTypeDef,
@@ -1427,15 +1498,15 @@
     "CreateOutboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "SourceDomainInfo": DomainInformationTypeDef,
         "DestinationDomainInfo": DomainInformationTypeDef,
         "ConnectionAlias": str,
         "ConnectionStatus": OutboundCrossClusterSearchConnectionStatusTypeDef,
         "CrossClusterSearchConnectionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OutboundCrossClusterSearchConnectionTypeDef = TypedDict(
     "OutboundCrossClusterSearchConnectionTypeDef",
     {
         "SourceDomainInfo": DomainInformationTypeDef,
@@ -1493,33 +1564,33 @@
     pass
 
 
 DeleteVpcEndpointResponseTypeDef = TypedDict(
     "DeleteVpcEndpointResponseTypeDef",
     {
         "VpcEndpointSummary": VpcEndpointSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointsForDomainResponseTypeDef = TypedDict(
     "ListVpcEndpointsForDomainResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointsResponseTypeDef = TypedDict(
     "ListVpcEndpointsResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef = TypedDict(
     "DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -1545,90 +1616,19 @@
         "Filters": Sequence[DescribePackagesFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
-    {
-        "ReservedElasticsearchInstanceOfferingId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef = TypedDict(
-    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
-    {
-        "ReservedElasticsearchInstanceId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef(
-    _RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
-    _OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
-    "_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
-    {
-        "ElasticsearchVersion": str,
-    },
-)
-_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
-    "_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
-    {
-        "DomainName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef(
-    _RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
-    _OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
-):
-    pass
-
-
-ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef = TypedDict(
-    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "DomainNames": List[DomainInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainPackageDetailsTypeDef = TypedDict(
     "DomainPackageDetailsTypeDef",
     {
         "PackageID": str,
@@ -1701,15 +1701,15 @@
 
 GetPackageVersionHistoryResponseTypeDef = TypedDict(
     "GetPackageVersionHistoryResponseTypeDef",
     {
         "PackageID": str,
         "PackageVersionHistoryList": List[PackageVersionHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InboundCrossClusterSearchConnectionTypeDef = TypedDict(
     "InboundCrossClusterSearchConnectionTypeDef",
     {
         "SourceDomainInfo": DomainInformationTypeDef,
@@ -1838,99 +1838,99 @@
     total=False,
 )
 
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatus": ChangeProgressStatusDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteOutboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": OutboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef = TypedDict(
     "DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef",
     {
         "CrossClusterSearchConnections": List[OutboundCrossClusterSearchConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociatePackageResponseTypeDef = TypedDict(
     "AssociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DissociatePackageResponseTypeDef = TypedDict(
     "DissociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsForPackageResponseTypeDef = TypedDict(
     "ListDomainsForPackageResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPackagesForDomainResponseTypeDef = TypedDict(
     "ListPackagesForDomainResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePackageResponseTypeDef = TypedDict(
     "DeletePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackagesResponseTypeDef = TypedDict(
     "DescribePackagesResponseTypeDef",
     {
         "PackageDetailsList": List[PackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePackageResponseTypeDef = TypedDict(
     "UpdatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ElasticsearchClusterConfigStatusTypeDef = TypedDict(
     "ElasticsearchClusterConfigStatusTypeDef",
     {
         "Options": ElasticsearchClusterConfigTypeDef,
@@ -1938,85 +1938,85 @@
     },
 )
 
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVpcEndpointsResponseTypeDef = TypedDict(
     "DescribeVpcEndpointsResponseTypeDef",
     {
         "VpcEndpoints": List[VpcEndpointTypeDef],
         "VpcEndpointErrors": List[VpcEndpointErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVpcEndpointResponseTypeDef = TypedDict(
     "UpdateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AcceptInboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "AcceptInboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": InboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "DeleteInboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": InboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInboundCrossClusterSearchConnectionsResponseTypeDef = TypedDict(
     "DescribeInboundCrossClusterSearchConnectionsResponseTypeDef",
     {
         "CrossClusterSearchConnections": List[InboundCrossClusterSearchConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RejectInboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "RejectInboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": InboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedElasticsearchInstanceOfferings": List[
             ReservedElasticsearchInstanceOfferingTypeDef
         ],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservedElasticsearchInstancesResponseTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstancesResponseTypeDef",
     {
         "NextToken": str,
         "ReservedElasticsearchInstances": List[ReservedElasticsearchInstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdvancedSecurityOptionsInputTypeDef = TypedDict(
     "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": bool,
@@ -2051,24 +2051,24 @@
 )
 
 GetUpgradeHistoryResponseTypeDef = TypedDict(
     "GetUpgradeHistoryResponseTypeDef",
     {
         "UpgradeHistories": List[UpgradeHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainAutoTunesResponseTypeDef = TypedDict(
     "DescribeDomainAutoTunesResponseTypeDef",
     {
         "AutoTunes": List[AutoTuneTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
         "Options": AutoTuneOptionsTypeDef,
@@ -2200,15 +2200,15 @@
     pass
 
 
 DescribeElasticsearchInstanceTypeLimitsResponseTypeDef = TypedDict(
     "DescribeElasticsearchInstanceTypeLimitsResponseTypeDef",
     {
         "LimitsByRole": Dict[str, LimitsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ElasticsearchDomainConfigTypeDef = TypedDict(
     "ElasticsearchDomainConfigTypeDef",
     {
         "ElasticsearchVersion": ElasticsearchVersionStatusTypeDef,
@@ -2230,51 +2230,51 @@
     total=False,
 )
 
 CreateElasticsearchDomainResponseTypeDef = TypedDict(
     "CreateElasticsearchDomainResponseTypeDef",
     {
         "DomainStatus": ElasticsearchDomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteElasticsearchDomainResponseTypeDef = TypedDict(
     "DeleteElasticsearchDomainResponseTypeDef",
     {
         "DomainStatus": ElasticsearchDomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeElasticsearchDomainResponseTypeDef = TypedDict(
     "DescribeElasticsearchDomainResponseTypeDef",
     {
         "DomainStatus": ElasticsearchDomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeElasticsearchDomainsResponseTypeDef = TypedDict(
     "DescribeElasticsearchDomainsResponseTypeDef",
     {
         "DomainStatusList": List[ElasticsearchDomainStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeElasticsearchDomainConfigResponseTypeDef = TypedDict(
     "DescribeElasticsearchDomainConfigResponseTypeDef",
     {
         "DomainConfig": ElasticsearchDomainConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateElasticsearchDomainConfigResponseTypeDef = TypedDict(
     "UpdateElasticsearchDomainConfigResponseTypeDef",
     {
         "DomainConfig": ElasticsearchDomainConfigTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es/type_defs.pyi` & `mypy-boto3-es-1.27.0/mypy_boto3_es/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "OptionStatusTypeDef",
     "TagTypeDef",
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
     "AssociatePackageRequestRequestTypeDef",
     "AuthorizeVpcEndpointAccessRequestRequestTypeDef",
     "AuthorizedPrincipalTypeDef",
@@ -93,56 +92,62 @@
     "DescribeDomainChangeProgressRequestRequestTypeDef",
     "DescribeElasticsearchDomainConfigRequestRequestTypeDef",
     "DescribeElasticsearchDomainRequestRequestTypeDef",
     "DescribeElasticsearchDomainsRequestRequestTypeDef",
     "DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef",
     "FilterTypeDef",
     "DescribePackagesFilterTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
     "DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef",
+    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
     "DescribeReservedElasticsearchInstancesRequestRequestTypeDef",
     "DescribeVpcEndpointsRequestRequestTypeDef",
     "VpcEndpointErrorTypeDef",
     "DissociatePackageRequestRequestTypeDef",
     "DomainInfoTypeDef",
     "ErrorDetailsTypeDef",
     "DryRunResultsTypeDef",
     "ZoneAwarenessConfigTypeDef",
     "VPCDerivedInfoTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetCompatibleElasticsearchVersionsRequestRequestTypeDef",
     "GetPackageVersionHistoryRequestRequestTypeDef",
     "PackageVersionHistoryTypeDef",
+    "GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
     "GetUpgradeHistoryRequestRequestTypeDef",
     "GetUpgradeStatusRequestRequestTypeDef",
+    "GetUpgradeStatusResponseTypeDef",
     "InboundCrossClusterSearchConnectionStatusTypeDef",
     "InstanceCountLimitsTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
+    "ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
     "ListElasticsearchInstanceTypesRequestRequestTypeDef",
+    "ListElasticsearchInstanceTypesResponseTypeDef",
+    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
     "ListElasticsearchVersionsRequestRequestTypeDef",
+    "ListElasticsearchVersionsResponseTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef",
+    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     "SAMLIdpTypeDef",
     "StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
     "UpgradeElasticsearchDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetUpgradeStatusResponseTypeDef",
-    "ListElasticsearchInstanceTypesResponseTypeDef",
-    "ListElasticsearchVersionsResponseTypeDef",
-    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AdvancedOptionsStatusTypeDef",
     "ElasticsearchVersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
@@ -169,19 +174,14 @@
     "UpdatePackageRequestRequestTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "ListVpcEndpointsForDomainResponseTypeDef",
     "ListVpcEndpointsResponseTypeDef",
     "DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef",
     "DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef",
     "DescribePackagesRequestRequestTypeDef",
-    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
-    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
-    "GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
-    "ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
-    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
     "ListDomainNamesResponseTypeDef",
     "DomainPackageDetailsTypeDef",
     "PackageDetailsTypeDef",
     "ElasticsearchClusterConfigTypeDef",
     "VPCDerivedInfoStatusTypeDef",
     "VpcEndpointTypeDef",
     "GetPackageVersionHistoryResponseTypeDef",
@@ -240,25 +240,14 @@
 AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef = TypedDict(
     "AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef",
     {
         "CrossClusterSearchConnectionId": str,
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
 _RequiredOptionStatusTypeDef = TypedDict(
     "_RequiredOptionStatusTypeDef",
     {
         "CreationDate": datetime,
         "UpdateDate": datetime,
         "State": OptionStateType,
     },
@@ -694,34 +683,42 @@
     {
         "Name": DescribePackagesFilterNameType,
         "Value": Sequence[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ReservedElasticsearchInstanceOfferingId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef",
     {
         "ReservedElasticsearchInstanceOfferingId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef = TypedDict(
+    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
+    {
+        "ReservedElasticsearchInstanceId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedElasticsearchInstancesRequestRequestTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstancesRequestRequestTypeDef",
     {
         "ReservedElasticsearchInstanceId": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -795,14 +792,21 @@
         "SubnetIds": List[str],
         "AvailabilityZones": List[str],
         "SecurityGroupIds": List[str],
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
 GetCompatibleElasticsearchVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleElasticsearchVersionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
     total=False,
 )
@@ -834,14 +838,34 @@
         "PackageVersion": str,
         "CommitMessage": str,
         "CreatedAt": datetime,
     },
     total=False,
 )
 
+_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef(
+    _RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
+    _OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
+):
+    pass
+
 _RequiredGetUpgradeHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetUpgradeHistoryRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetUpgradeHistoryRequestRequestTypeDef = TypedDict(
@@ -861,14 +885,24 @@
 GetUpgradeStatusRequestRequestTypeDef = TypedDict(
     "GetUpgradeStatusRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+GetUpgradeStatusResponseTypeDef = TypedDict(
+    "GetUpgradeStatusResponseTypeDef",
+    {
+        "UpgradeStep": UpgradeStepType,
+        "StepStatus": UpgradeStatusType,
+        "UpgradeName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InboundCrossClusterSearchConnectionStatusTypeDef = TypedDict(
     "InboundCrossClusterSearchConnectionStatusTypeDef",
     {
         "StatusCode": InboundCrossClusterSearchConnectionStatusCodeType,
         "Message": str,
     },
     total=False,
@@ -908,14 +942,35 @@
 
 class ListDomainsForPackageRequestRequestTypeDef(
     _RequiredListDomainsForPackageRequestRequestTypeDef,
     _OptionalListDomainsForPackageRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
+    "_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
+    {
+        "ElasticsearchVersion": str,
+    },
+)
+_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
+    "_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
+    {
+        "DomainName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef(
+    _RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
+    _OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
+):
+    pass
+
 _RequiredListElasticsearchInstanceTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListElasticsearchInstanceTypesRequestRequestTypeDef",
     {
         "ElasticsearchVersion": str,
     },
 )
 _OptionalListElasticsearchInstanceTypesRequestRequestTypeDef = TypedDict(
@@ -930,23 +985,49 @@
 
 class ListElasticsearchInstanceTypesRequestRequestTypeDef(
     _RequiredListElasticsearchInstanceTypesRequestRequestTypeDef,
     _OptionalListElasticsearchInstanceTypesRequestRequestTypeDef,
 ):
     pass
 
+ListElasticsearchInstanceTypesResponseTypeDef = TypedDict(
+    "ListElasticsearchInstanceTypesResponseTypeDef",
+    {
+        "ElasticsearchInstanceTypes": List[ESPartitionInstanceTypeType],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef = TypedDict(
+    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListElasticsearchVersionsRequestRequestTypeDef = TypedDict(
     "ListElasticsearchVersionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListElasticsearchVersionsResponseTypeDef = TypedDict(
+    "ListElasticsearchVersionsResponseTypeDef",
+    {
+        "ElasticsearchVersions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListPackagesForDomainRequestRequestTypeDef = TypedDict(
     "_RequiredListPackagesForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListPackagesForDomainRequestRequestTypeDef = TypedDict(
@@ -1015,14 +1096,24 @@
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
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
 _RequiredPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef",
     {
         "ReservedElasticsearchInstanceOfferingId": str,
         "ReservationName": str,
     },
 )
@@ -1036,14 +1127,23 @@
 
 class PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef(
     _RequiredPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
     _OptionalPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
 ):
     pass
 
+PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef = TypedDict(
+    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
+    {
+        "ReservedElasticsearchInstanceId": str,
+        "ReservationName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "RecurringChargeAmount": float,
         "RecurringChargeFrequency": str,
     },
     total=False,
@@ -1060,14 +1160,25 @@
     "RemoveTagsRequestRequestTypeDef",
     {
         "ARN": str,
         "TagKeys": Sequence[str],
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
 RevokeVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
         "Account": str,
     },
 )
@@ -1124,58 +1235,14 @@
         "UpgradeStepStatus": UpgradeStatusType,
         "Issues": List[str],
         "ProgressPercent": float,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUpgradeStatusResponseTypeDef = TypedDict(
-    "GetUpgradeStatusResponseTypeDef",
-    {
-        "UpgradeStep": UpgradeStepType,
-        "StepStatus": UpgradeStatusType,
-        "UpgradeName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListElasticsearchInstanceTypesResponseTypeDef = TypedDict(
-    "ListElasticsearchInstanceTypesResponseTypeDef",
-    {
-        "ElasticsearchInstanceTypes": List[ESPartitionInstanceTypeType],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListElasticsearchVersionsResponseTypeDef = TypedDict(
-    "ListElasticsearchVersionsResponseTypeDef",
-    {
-        "ElasticsearchVersions": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef = TypedDict(
-    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
-    {
-        "ReservedElasticsearchInstanceId": str,
-        "ReservationName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AccessPoliciesStatusTypeDef = TypedDict(
     "AccessPoliciesStatusTypeDef",
     {
         "Options": str,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -1204,32 +1271,32 @@
     },
 )
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthorizeVpcEndpointAccessResponseTypeDef = TypedDict(
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipal": AuthorizedPrincipalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointAccessResponseTypeDef = TypedDict(
     "ListVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipalList": List[AuthorizedPrincipalTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoTuneDetailsTypeDef = TypedDict(
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": ScheduledAutoTuneDetailsTypeDef,
@@ -1247,34 +1314,34 @@
     total=False,
 )
 
 CancelElasticsearchServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "CancelElasticsearchServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartElasticsearchServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "StartElasticsearchServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpgradeElasticsearchDomainResponseTypeDef = TypedDict(
     "UpgradeElasticsearchDomainResponseTypeDef",
     {
         "DomainName": str,
         "TargetVersion": str,
         "PerformCheckOnly": bool,
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeProgressStatusDetailsTypeDef = TypedDict(
     "ChangeProgressStatusDetailsTypeDef",
     {
         "ChangeId": str,
@@ -1296,15 +1363,15 @@
     },
 )
 
 GetCompatibleElasticsearchVersionsResponseTypeDef = TypedDict(
     "GetCompatibleElasticsearchVersionsResponseTypeDef",
     {
         "CompatibleElasticsearchVersions": List[CompatibleVersionsMapTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainEndpointOptionsStatusTypeDef = TypedDict(
     "DomainEndpointOptionsStatusTypeDef",
     {
         "Options": DomainEndpointOptionsTypeDef,
@@ -1394,15 +1461,15 @@
     "CreateOutboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "SourceDomainInfo": DomainInformationTypeDef,
         "DestinationDomainInfo": DomainInformationTypeDef,
         "ConnectionAlias": str,
         "ConnectionStatus": OutboundCrossClusterSearchConnectionStatusTypeDef,
         "CrossClusterSearchConnectionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OutboundCrossClusterSearchConnectionTypeDef = TypedDict(
     "OutboundCrossClusterSearchConnectionTypeDef",
     {
         "SourceDomainInfo": DomainInformationTypeDef,
@@ -1456,33 +1523,33 @@
 ):
     pass
 
 DeleteVpcEndpointResponseTypeDef = TypedDict(
     "DeleteVpcEndpointResponseTypeDef",
     {
         "VpcEndpointSummary": VpcEndpointSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointsForDomainResponseTypeDef = TypedDict(
     "ListVpcEndpointsForDomainResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointsResponseTypeDef = TypedDict(
     "ListVpcEndpointsResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef = TypedDict(
     "DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -1508,86 +1575,19 @@
         "Filters": Sequence[DescribePackagesFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
-    {
-        "ReservedElasticsearchInstanceOfferingId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef = TypedDict(
-    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
-    {
-        "ReservedElasticsearchInstanceId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef(
-    _RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
-    _OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
-):
-    pass
-
-_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
-    "_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
-    {
-        "ElasticsearchVersion": str,
-    },
-)
-_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
-    "_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
-    {
-        "DomainName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef(
-    _RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
-    _OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
-):
-    pass
-
-ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef = TypedDict(
-    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "DomainNames": List[DomainInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainPackageDetailsTypeDef = TypedDict(
     "DomainPackageDetailsTypeDef",
     {
         "PackageID": str,
@@ -1660,15 +1660,15 @@
 
 GetPackageVersionHistoryResponseTypeDef = TypedDict(
     "GetPackageVersionHistoryResponseTypeDef",
     {
         "PackageID": str,
         "PackageVersionHistoryList": List[PackageVersionHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InboundCrossClusterSearchConnectionTypeDef = TypedDict(
     "InboundCrossClusterSearchConnectionTypeDef",
     {
         "SourceDomainInfo": DomainInformationTypeDef,
@@ -1797,99 +1797,99 @@
     total=False,
 )
 
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatus": ChangeProgressStatusDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteOutboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": OutboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef = TypedDict(
     "DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef",
     {
         "CrossClusterSearchConnections": List[OutboundCrossClusterSearchConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociatePackageResponseTypeDef = TypedDict(
     "AssociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DissociatePackageResponseTypeDef = TypedDict(
     "DissociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsForPackageResponseTypeDef = TypedDict(
     "ListDomainsForPackageResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPackagesForDomainResponseTypeDef = TypedDict(
     "ListPackagesForDomainResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePackageResponseTypeDef = TypedDict(
     "DeletePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackagesResponseTypeDef = TypedDict(
     "DescribePackagesResponseTypeDef",
     {
         "PackageDetailsList": List[PackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePackageResponseTypeDef = TypedDict(
     "UpdatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ElasticsearchClusterConfigStatusTypeDef = TypedDict(
     "ElasticsearchClusterConfigStatusTypeDef",
     {
         "Options": ElasticsearchClusterConfigTypeDef,
@@ -1897,85 +1897,85 @@
     },
 )
 
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVpcEndpointsResponseTypeDef = TypedDict(
     "DescribeVpcEndpointsResponseTypeDef",
     {
         "VpcEndpoints": List[VpcEndpointTypeDef],
         "VpcEndpointErrors": List[VpcEndpointErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVpcEndpointResponseTypeDef = TypedDict(
     "UpdateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AcceptInboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "AcceptInboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": InboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "DeleteInboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": InboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInboundCrossClusterSearchConnectionsResponseTypeDef = TypedDict(
     "DescribeInboundCrossClusterSearchConnectionsResponseTypeDef",
     {
         "CrossClusterSearchConnections": List[InboundCrossClusterSearchConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RejectInboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "RejectInboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": InboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedElasticsearchInstanceOfferings": List[
             ReservedElasticsearchInstanceOfferingTypeDef
         ],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservedElasticsearchInstancesResponseTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstancesResponseTypeDef",
     {
         "NextToken": str,
         "ReservedElasticsearchInstances": List[ReservedElasticsearchInstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdvancedSecurityOptionsInputTypeDef = TypedDict(
     "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": bool,
@@ -2010,24 +2010,24 @@
 )
 
 GetUpgradeHistoryResponseTypeDef = TypedDict(
     "GetUpgradeHistoryResponseTypeDef",
     {
         "UpgradeHistories": List[UpgradeHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainAutoTunesResponseTypeDef = TypedDict(
     "DescribeDomainAutoTunesResponseTypeDef",
     {
         "AutoTunes": List[AutoTuneTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
         "Options": AutoTuneOptionsTypeDef,
@@ -2153,15 +2153,15 @@
 ):
     pass
 
 DescribeElasticsearchInstanceTypeLimitsResponseTypeDef = TypedDict(
     "DescribeElasticsearchInstanceTypeLimitsResponseTypeDef",
     {
         "LimitsByRole": Dict[str, LimitsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ElasticsearchDomainConfigTypeDef = TypedDict(
     "ElasticsearchDomainConfigTypeDef",
     {
         "ElasticsearchVersion": ElasticsearchVersionStatusTypeDef,
@@ -2183,51 +2183,51 @@
     total=False,
 )
 
 CreateElasticsearchDomainResponseTypeDef = TypedDict(
     "CreateElasticsearchDomainResponseTypeDef",
     {
         "DomainStatus": ElasticsearchDomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteElasticsearchDomainResponseTypeDef = TypedDict(
     "DeleteElasticsearchDomainResponseTypeDef",
     {
         "DomainStatus": ElasticsearchDomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeElasticsearchDomainResponseTypeDef = TypedDict(
     "DescribeElasticsearchDomainResponseTypeDef",
     {
         "DomainStatus": ElasticsearchDomainStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeElasticsearchDomainsResponseTypeDef = TypedDict(
     "DescribeElasticsearchDomainsResponseTypeDef",
     {
         "DomainStatusList": List[ElasticsearchDomainStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeElasticsearchDomainConfigResponseTypeDef = TypedDict(
     "DescribeElasticsearchDomainConfigResponseTypeDef",
     {
         "DomainConfig": ElasticsearchDomainConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateElasticsearchDomainConfigResponseTypeDef = TypedDict(
     "UpdateElasticsearchDomainConfigResponseTypeDef",
     {
         "DomainConfig": ElasticsearchDomainConfigTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es.egg-info/PKG-INFO` & `mypy-boto3-es-1.27.0/mypy_boto3_es.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-es
-Version: 1.26.7
-Summary: Type annotations for boto3.ElasticsearchService 1.26.7 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ElasticsearchService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/
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
 
 <a id="mypy-boto3-es"></a>
 
 # mypy-boto3-es
 
 [![PyPI - mypy-boto3-es](https://img.shields.io/pypi/v/mypy-boto3-es.svg?color=blue)](https://pypi.org/project/mypy-boto3-es)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-es.svg?color=blue)](https://pypi.org/project/mypy-boto3-es)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-es?color=blue)](https://pypistats.org/packages/mypy-boto3-es)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticsearchService 1.26.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
+[boto3.ElasticsearchService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
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
 [mypy-boto3-es docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,15 +370,14 @@
 
 `mypy_boto3_es.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_es.type_defs import (
     AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
@@ -412,56 +412,62 @@
     DescribeDomainChangeProgressRequestRequestTypeDef,
     DescribeElasticsearchDomainConfigRequestRequestTypeDef,
     DescribeElasticsearchDomainRequestRequestTypeDef,
     DescribeElasticsearchDomainsRequestRequestTypeDef,
     DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef,
     FilterTypeDef,
     DescribePackagesFilterTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef,
     DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef,
+    DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef,
     DescribeReservedElasticsearchInstancesRequestRequestTypeDef,
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
     DryRunResultsTypeDef,
     ZoneAwarenessConfigTypeDef,
     VPCDerivedInfoTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCompatibleElasticsearchVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
+    GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
+    GetUpgradeStatusResponseTypeDef,
     InboundCrossClusterSearchConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
+    ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
     ListElasticsearchInstanceTypesRequestRequestTypeDef,
+    ListElasticsearchInstanceTypesResponseTypeDef,
+    ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef,
     ListElasticsearchVersionsRequestRequestTypeDef,
+    ListElasticsearchVersionsResponseTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
+    PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpgradeElasticsearchDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetUpgradeStatusResponseTypeDef,
-    ListElasticsearchInstanceTypesResponseTypeDef,
-    ListElasticsearchVersionsResponseTypeDef,
-    PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     ElasticsearchVersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
@@ -488,19 +494,14 @@
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef,
     DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
-    DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef,
-    DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef,
-    GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
-    ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
-    ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
     ElasticsearchClusterConfigTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
@@ -564,42 +565,42 @@
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

### Comparing `mypy-boto3-es-1.26.7/mypy_boto3_es.egg-info/SOURCES.txt` & `mypy-boto3-es-1.27.0/mypy_boto3_es.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-es-1.26.7/setup.py` & `mypy-boto3-es-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-es.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-es",
-    version="1.26.7",
+    version="1.27.0",
     packages=["mypy_boto3_es"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticsearchService 1.26.7 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.ElasticsearchService 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
     keywords="boto3 es type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_es": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_es": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_es/",
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


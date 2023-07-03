# Comparing `tmp/mypy-boto3-worklink-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-worklink-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-worklink-1.26.0.post1.tar", last modified: Tue Nov  1 21:44:07 2022, max compression
+gzip compressed data, was "mypy-boto3-worklink-1.27.0.tar", last modified: Mon Jul  3 19:51:36 2023, max compression
```

## Comparing `mypy-boto3-worklink-1.26.0.post1.tar` & `mypy-boto3-worklink-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:07.692856 mypy-boto3-worklink-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:42:35.000000 mypy-boto3-worklink-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14597 2022-11-01 21:44:07.692856 mypy-boto3-worklink-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13152 2022-11-01 21:42:35.000000 mypy-boto3-worklink-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:07.692856 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-11-01 21:42:35.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-11-01 21:42:35.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-01 21:42:35.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22013 2022-11-01 21:42:35.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    21973 2022-11-01 21:42:35.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7439 2022-11-01 21:42:35.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7437 2022-11-01 21:42:35.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:42:35.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    21219 2022-11-01 21:42:38.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    21188 2022-11-01 21:42:38.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:42:35.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:07.692856 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14597 2022-11-01 21:44:07.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-01 21:44:07.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:07.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:07.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:44:07.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-01 21:44:07.000000 mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:44:07.692856 mypy-boto3-worklink-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2022-11-01 21:42:35.000000 mypy-boto3-worklink-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:36.812154 mypy-boto3-worklink-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-07-03 19:51:36.812154 mypy-boto3-worklink-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:36.812154 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22013 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21253 2023-07-03 19:49:48.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:36.812154 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-07-03 19:51:36.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-03 19:51:36.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:36.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:36.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:36.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:36.000000 mypy-boto3-worklink-1.27.0/mypy_boto3_worklink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:36.812154 mypy-boto3-worklink-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:49:47.000000 mypy-boto3-worklink-1.27.0/setup.py
```

### Comparing `mypy-boto3-worklink-1.26.0.post1/LICENSE` & `mypy-boto3-worklink-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-worklink-1.26.0.post1/PKG-INFO` & `mypy-boto3-worklink-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-worklink
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.WorkLink 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.WorkLink 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/
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
 
 <a id="mypy-boto3-worklink"></a>
 
 # mypy-boto3-worklink
 
 [![PyPI - mypy-boto3-worklink](https://img.shields.io/pypi/v/mypy-boto3-worklink.svg?color=blue)](https://pypi.org/project/mypy-boto3-worklink)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-worklink.svg?color=blue)](https://pypi.org/project/mypy-boto3-worklink)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-worklink?color=blue)](https://pypistats.org/packages/mypy-boto3-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkLink 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
+[boto3.WorkLink 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
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
 [mypy-boto3-worklink docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,63 +301,63 @@
 `mypy_boto3_worklink.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_worklink.type_defs import (
     AssociateDomainRequestRequestTypeDef,
     AssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateWebsiteAuthorizationProviderResponseTypeDef,
     AssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
+    AssociateWebsiteCertificateAuthorityResponseTypeDef,
     CreateFleetRequestRequestTypeDef,
+    CreateFleetResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DescribeAuditStreamConfigurationRequestRequestTypeDef,
+    DescribeAuditStreamConfigurationResponseTypeDef,
     DescribeCompanyNetworkConfigurationRequestRequestTypeDef,
+    DescribeCompanyNetworkConfigurationResponseTypeDef,
     DescribeDevicePolicyConfigurationRequestRequestTypeDef,
+    DescribeDevicePolicyConfigurationResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
+    DescribeDeviceResponseTypeDef,
     DescribeDomainRequestRequestTypeDef,
+    DescribeDomainResponseTypeDef,
     DescribeFleetMetadataRequestRequestTypeDef,
+    DescribeFleetMetadataResponseTypeDef,
     DescribeIdentityProviderConfigurationRequestRequestTypeDef,
+    DescribeIdentityProviderConfigurationResponseTypeDef,
     DescribeWebsiteCertificateAuthorityRequestRequestTypeDef,
+    DescribeWebsiteCertificateAuthorityResponseTypeDef,
     DeviceSummaryTypeDef,
     DisassociateDomainRequestRequestTypeDef,
     DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     DomainSummaryTypeDef,
     FleetSummaryTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFleetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWebsiteAuthorizationProvidersRequestRequestTypeDef,
     WebsiteAuthorizationProviderSummaryTypeDef,
     ListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
     WebsiteCaSummaryTypeDef,
+    ResponseMetadataTypeDef,
     RestoreDomainAccessRequestRequestTypeDef,
     RevokeDomainAccessRequestRequestTypeDef,
     SignOutUserRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuditStreamConfigurationRequestRequestTypeDef,
     UpdateCompanyNetworkConfigurationRequestRequestTypeDef,
     UpdateDevicePolicyConfigurationRequestRequestTypeDef,
     UpdateDomainMetadataRequestRequestTypeDef,
     UpdateFleetMetadataRequestRequestTypeDef,
     UpdateIdentityProviderConfigurationRequestRequestTypeDef,
-    AssociateWebsiteAuthorizationProviderResponseTypeDef,
-    AssociateWebsiteCertificateAuthorityResponseTypeDef,
-    CreateFleetResponseTypeDef,
-    DescribeAuditStreamConfigurationResponseTypeDef,
-    DescribeCompanyNetworkConfigurationResponseTypeDef,
-    DescribeDevicePolicyConfigurationResponseTypeDef,
-    DescribeDeviceResponseTypeDef,
-    DescribeDomainResponseTypeDef,
-    DescribeFleetMetadataResponseTypeDef,
-    DescribeIdentityProviderConfigurationResponseTypeDef,
-    DescribeWebsiteCertificateAuthorityResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ListWebsiteAuthorizationProvidersResponseTypeDef,
     ListWebsiteCertificateAuthoritiesResponseTypeDef,
 )
 
@@ -368,42 +369,42 @@
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

### Comparing `mypy-boto3-worklink-1.26.0.post1/README.md` & `mypy-boto3-worklink-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-worklink"></a>
 
 # mypy-boto3-worklink
 
 [![PyPI - mypy-boto3-worklink](https://img.shields.io/pypi/v/mypy-boto3-worklink.svg?color=blue)](https://pypi.org/project/mypy-boto3-worklink)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-worklink.svg?color=blue)](https://pypi.org/project/mypy-boto3-worklink)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-worklink?color=blue)](https://pypistats.org/packages/mypy-boto3-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkLink 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
+[boto3.WorkLink 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
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
 [mypy-boto3-worklink docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,63 +269,63 @@
 `mypy_boto3_worklink.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_worklink.type_defs import (
     AssociateDomainRequestRequestTypeDef,
     AssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateWebsiteAuthorizationProviderResponseTypeDef,
     AssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
+    AssociateWebsiteCertificateAuthorityResponseTypeDef,
     CreateFleetRequestRequestTypeDef,
+    CreateFleetResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DescribeAuditStreamConfigurationRequestRequestTypeDef,
+    DescribeAuditStreamConfigurationResponseTypeDef,
     DescribeCompanyNetworkConfigurationRequestRequestTypeDef,
+    DescribeCompanyNetworkConfigurationResponseTypeDef,
     DescribeDevicePolicyConfigurationRequestRequestTypeDef,
+    DescribeDevicePolicyConfigurationResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
+    DescribeDeviceResponseTypeDef,
     DescribeDomainRequestRequestTypeDef,
+    DescribeDomainResponseTypeDef,
     DescribeFleetMetadataRequestRequestTypeDef,
+    DescribeFleetMetadataResponseTypeDef,
     DescribeIdentityProviderConfigurationRequestRequestTypeDef,
+    DescribeIdentityProviderConfigurationResponseTypeDef,
     DescribeWebsiteCertificateAuthorityRequestRequestTypeDef,
+    DescribeWebsiteCertificateAuthorityResponseTypeDef,
     DeviceSummaryTypeDef,
     DisassociateDomainRequestRequestTypeDef,
     DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     DomainSummaryTypeDef,
     FleetSummaryTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFleetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWebsiteAuthorizationProvidersRequestRequestTypeDef,
     WebsiteAuthorizationProviderSummaryTypeDef,
     ListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
     WebsiteCaSummaryTypeDef,
+    ResponseMetadataTypeDef,
     RestoreDomainAccessRequestRequestTypeDef,
     RevokeDomainAccessRequestRequestTypeDef,
     SignOutUserRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuditStreamConfigurationRequestRequestTypeDef,
     UpdateCompanyNetworkConfigurationRequestRequestTypeDef,
     UpdateDevicePolicyConfigurationRequestRequestTypeDef,
     UpdateDomainMetadataRequestRequestTypeDef,
     UpdateFleetMetadataRequestRequestTypeDef,
     UpdateIdentityProviderConfigurationRequestRequestTypeDef,
-    AssociateWebsiteAuthorizationProviderResponseTypeDef,
-    AssociateWebsiteCertificateAuthorityResponseTypeDef,
-    CreateFleetResponseTypeDef,
-    DescribeAuditStreamConfigurationResponseTypeDef,
-    DescribeCompanyNetworkConfigurationResponseTypeDef,
-    DescribeDevicePolicyConfigurationResponseTypeDef,
-    DescribeDeviceResponseTypeDef,
-    DescribeDomainResponseTypeDef,
-    DescribeFleetMetadataResponseTypeDef,
-    DescribeIdentityProviderConfigurationResponseTypeDef,
-    DescribeWebsiteCertificateAuthorityResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ListWebsiteAuthorizationProvidersResponseTypeDef,
     ListWebsiteCertificateAuthoritiesResponseTypeDef,
 )
 
@@ -337,42 +337,42 @@
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

### Comparing `mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/__main__.py` & `mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkLink 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.WorkLink 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink\nOther"
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

### Comparing `mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/client.py` & `mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/client.pyi` & `mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/literals.py` & `mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,23 +59,25 @@
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
@@ -85,30 +87,35 @@
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
@@ -134,14 +141,15 @@
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
@@ -186,51 +194,57 @@
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
@@ -243,14 +257,15 @@
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
@@ -262,28 +277,35 @@
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
@@ -292,14 +314,15 @@
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
@@ -310,55 +333,64 @@
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
```

### Comparing `mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/literals.pyi` & `mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -57,23 +57,25 @@
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
@@ -83,30 +85,35 @@
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
@@ -132,14 +139,15 @@
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
@@ -184,51 +192,57 @@
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
@@ -241,14 +255,15 @@
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
@@ -260,28 +275,35 @@
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
@@ -290,14 +312,15 @@
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
@@ -308,55 +331,64 @@
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
```

### Comparing `mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/type_defs.py` & `mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,63 +26,63 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateDomainRequestRequestTypeDef",
     "AssociateWebsiteAuthorizationProviderRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
     "AssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
+    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
     "CreateFleetRequestRequestTypeDef",
+    "CreateFleetResponseTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DescribeAuditStreamConfigurationRequestRequestTypeDef",
+    "DescribeAuditStreamConfigurationResponseTypeDef",
     "DescribeCompanyNetworkConfigurationRequestRequestTypeDef",
+    "DescribeCompanyNetworkConfigurationResponseTypeDef",
     "DescribeDevicePolicyConfigurationRequestRequestTypeDef",
+    "DescribeDevicePolicyConfigurationResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
+    "DescribeDeviceResponseTypeDef",
     "DescribeDomainRequestRequestTypeDef",
+    "DescribeDomainResponseTypeDef",
     "DescribeFleetMetadataRequestRequestTypeDef",
+    "DescribeFleetMetadataResponseTypeDef",
     "DescribeIdentityProviderConfigurationRequestRequestTypeDef",
+    "DescribeIdentityProviderConfigurationResponseTypeDef",
     "DescribeWebsiteCertificateAuthorityRequestRequestTypeDef",
+    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
     "DeviceSummaryTypeDef",
     "DisassociateDomainRequestRequestTypeDef",
     "DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef",
     "DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     "DomainSummaryTypeDef",
     "FleetSummaryTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFleetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListWebsiteAuthorizationProvidersRequestRequestTypeDef",
     "WebsiteAuthorizationProviderSummaryTypeDef",
     "ListWebsiteCertificateAuthoritiesRequestRequestTypeDef",
     "WebsiteCaSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreDomainAccessRequestRequestTypeDef",
     "RevokeDomainAccessRequestRequestTypeDef",
     "SignOutUserRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuditStreamConfigurationRequestRequestTypeDef",
     "UpdateCompanyNetworkConfigurationRequestRequestTypeDef",
     "UpdateDevicePolicyConfigurationRequestRequestTypeDef",
     "UpdateDomainMetadataRequestRequestTypeDef",
     "UpdateFleetMetadataRequestRequestTypeDef",
     "UpdateIdentityProviderConfigurationRequestRequestTypeDef",
-    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
-    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
-    "CreateFleetResponseTypeDef",
-    "DescribeAuditStreamConfigurationResponseTypeDef",
-    "DescribeCompanyNetworkConfigurationResponseTypeDef",
-    "DescribeDevicePolicyConfigurationResponseTypeDef",
-    "DescribeDeviceResponseTypeDef",
-    "DescribeDomainResponseTypeDef",
-    "DescribeFleetMetadataResponseTypeDef",
-    "DescribeIdentityProviderConfigurationResponseTypeDef",
-    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "ListFleetsResponseTypeDef",
     "ListWebsiteAuthorizationProvidersResponseTypeDef",
     "ListWebsiteCertificateAuthoritiesResponseTypeDef",
 )
 
@@ -128,22 +128,19 @@
 class AssociateWebsiteAuthorizationProviderRequestRequestTypeDef(
     _RequiredAssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     _OptionalAssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateWebsiteAuthorizationProviderResponseTypeDef = TypedDict(
+    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AuthorizationProviderId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "FleetArn": str,
@@ -162,14 +159,22 @@
 class AssociateWebsiteCertificateAuthorityRequestRequestTypeDef(
     _RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     _OptionalAssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
 
+AssociateWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
+    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
+    {
+        "WebsiteCaId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetRequestRequestTypeDef",
     {
         "FleetName": str,
     },
 )
 _OptionalCreateFleetRequestRequestTypeDef = TypedDict(
@@ -185,80 +190,177 @@
 
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
 
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "FleetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteFleetRequestRequestTypeDef = TypedDict(
     "DeleteFleetRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
 DescribeAuditStreamConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeAuditStreamConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
+DescribeAuditStreamConfigurationResponseTypeDef = TypedDict(
+    "DescribeAuditStreamConfigurationResponseTypeDef",
+    {
+        "AuditStreamArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeCompanyNetworkConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeCompanyNetworkConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
+DescribeCompanyNetworkConfigurationResponseTypeDef = TypedDict(
+    "DescribeCompanyNetworkConfigurationResponseTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDevicePolicyConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeDevicePolicyConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
+DescribeDevicePolicyConfigurationResponseTypeDef = TypedDict(
+    "DescribeDevicePolicyConfigurationResponseTypeDef",
+    {
+        "DeviceCaCertificate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DeviceId": str,
     },
 )
 
+DescribeDeviceResponseTypeDef = TypedDict(
+    "DescribeDeviceResponseTypeDef",
+    {
+        "Status": DeviceStatusType,
+        "Model": str,
+        "Manufacturer": str,
+        "OperatingSystem": str,
+        "OperatingSystemVersion": str,
+        "PatchLevel": str,
+        "FirstAccessedTime": datetime,
+        "LastAccessedTime": datetime,
+        "Username": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDomainRequestRequestTypeDef = TypedDict(
     "DescribeDomainRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
 
+DescribeDomainResponseTypeDef = TypedDict(
+    "DescribeDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DisplayName": str,
+        "CreatedTime": datetime,
+        "DomainStatus": DomainStatusType,
+        "AcmCertificateArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeFleetMetadataRequestRequestTypeDef = TypedDict(
     "DescribeFleetMetadataRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
+DescribeFleetMetadataResponseTypeDef = TypedDict(
+    "DescribeFleetMetadataResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "FleetName": str,
+        "DisplayName": str,
+        "OptimizeForEndUserLocation": bool,
+        "CompanyCode": str,
+        "FleetStatus": FleetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeIdentityProviderConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeIdentityProviderConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
+DescribeIdentityProviderConfigurationResponseTypeDef = TypedDict(
+    "DescribeIdentityProviderConfigurationResponseTypeDef",
+    {
+        "IdentityProviderType": Literal["SAML"],
+        "ServiceProviderSamlMetadata": str,
+        "IdentityProviderSamlMetadata": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeWebsiteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "DescribeWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "FleetArn": str,
         "WebsiteCaId": str,
     },
 )
 
+DescribeWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
+    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
+    {
+        "Certificate": str,
+        "CreatedTime": datetime,
+        "DisplayName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "DeviceId": str,
         "DeviceStatus": DeviceStatusType,
     },
     total=False,
@@ -380,14 +482,22 @@
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
 _RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef = TypedDict(
     "_RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 _OptionalListWebsiteAuthorizationProvidersRequestRequestTypeDef = TypedDict(
@@ -460,14 +570,25 @@
         "WebsiteCaId": str,
         "CreatedTime": datetime,
         "DisplayName": str,
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
 RestoreDomainAccessRequestRequestTypeDef = TypedDict(
     "RestoreDomainAccessRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
@@ -623,172 +744,51 @@
 class UpdateIdentityProviderConfigurationRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderConfigurationRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateWebsiteAuthorizationProviderResponseTypeDef = TypedDict(
-    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
-    {
-        "AuthorizationProviderId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
-    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
-    {
-        "WebsiteCaId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "FleetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAuditStreamConfigurationResponseTypeDef = TypedDict(
-    "DescribeAuditStreamConfigurationResponseTypeDef",
-    {
-        "AuditStreamArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeCompanyNetworkConfigurationResponseTypeDef = TypedDict(
-    "DescribeCompanyNetworkConfigurationResponseTypeDef",
-    {
-        "VpcId": str,
-        "SubnetIds": List[str],
-        "SecurityGroupIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDevicePolicyConfigurationResponseTypeDef = TypedDict(
-    "DescribeDevicePolicyConfigurationResponseTypeDef",
-    {
-        "DeviceCaCertificate": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDeviceResponseTypeDef = TypedDict(
-    "DescribeDeviceResponseTypeDef",
-    {
-        "Status": DeviceStatusType,
-        "Model": str,
-        "Manufacturer": str,
-        "OperatingSystem": str,
-        "OperatingSystemVersion": str,
-        "PatchLevel": str,
-        "FirstAccessedTime": datetime,
-        "LastAccessedTime": datetime,
-        "Username": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDomainResponseTypeDef = TypedDict(
-    "DescribeDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DisplayName": str,
-        "CreatedTime": datetime,
-        "DomainStatus": DomainStatusType,
-        "AcmCertificateArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFleetMetadataResponseTypeDef = TypedDict(
-    "DescribeFleetMetadataResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "FleetName": str,
-        "DisplayName": str,
-        "OptimizeForEndUserLocation": bool,
-        "CompanyCode": str,
-        "FleetStatus": FleetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeIdentityProviderConfigurationResponseTypeDef = TypedDict(
-    "DescribeIdentityProviderConfigurationResponseTypeDef",
-    {
-        "IdentityProviderType": Literal["SAML"],
-        "ServiceProviderSamlMetadata": str,
-        "IdentityProviderSamlMetadata": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
-    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
-    {
-        "Certificate": str,
-        "CreatedTime": datetime,
-        "DisplayName": str,
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
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFleetsResponseTypeDef = TypedDict(
     "ListFleetsResponseTypeDef",
     {
         "FleetSummaryList": List[FleetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWebsiteAuthorizationProvidersResponseTypeDef = TypedDict(
     "ListWebsiteAuthorizationProvidersResponseTypeDef",
     {
         "WebsiteAuthorizationProviders": List[WebsiteAuthorizationProviderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWebsiteCertificateAuthoritiesResponseTypeDef = TypedDict(
     "ListWebsiteCertificateAuthoritiesResponseTypeDef",
     {
         "WebsiteCertificateAuthorities": List[WebsiteCaSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink/type_defs.pyi` & `mypy-boto3-worklink-1.27.0/mypy_boto3_worklink/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -25,63 +25,63 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateDomainRequestRequestTypeDef",
     "AssociateWebsiteAuthorizationProviderRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
     "AssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
+    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
     "CreateFleetRequestRequestTypeDef",
+    "CreateFleetResponseTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DescribeAuditStreamConfigurationRequestRequestTypeDef",
+    "DescribeAuditStreamConfigurationResponseTypeDef",
     "DescribeCompanyNetworkConfigurationRequestRequestTypeDef",
+    "DescribeCompanyNetworkConfigurationResponseTypeDef",
     "DescribeDevicePolicyConfigurationRequestRequestTypeDef",
+    "DescribeDevicePolicyConfigurationResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
+    "DescribeDeviceResponseTypeDef",
     "DescribeDomainRequestRequestTypeDef",
+    "DescribeDomainResponseTypeDef",
     "DescribeFleetMetadataRequestRequestTypeDef",
+    "DescribeFleetMetadataResponseTypeDef",
     "DescribeIdentityProviderConfigurationRequestRequestTypeDef",
+    "DescribeIdentityProviderConfigurationResponseTypeDef",
     "DescribeWebsiteCertificateAuthorityRequestRequestTypeDef",
+    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
     "DeviceSummaryTypeDef",
     "DisassociateDomainRequestRequestTypeDef",
     "DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef",
     "DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     "DomainSummaryTypeDef",
     "FleetSummaryTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFleetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListWebsiteAuthorizationProvidersRequestRequestTypeDef",
     "WebsiteAuthorizationProviderSummaryTypeDef",
     "ListWebsiteCertificateAuthoritiesRequestRequestTypeDef",
     "WebsiteCaSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreDomainAccessRequestRequestTypeDef",
     "RevokeDomainAccessRequestRequestTypeDef",
     "SignOutUserRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuditStreamConfigurationRequestRequestTypeDef",
     "UpdateCompanyNetworkConfigurationRequestRequestTypeDef",
     "UpdateDevicePolicyConfigurationRequestRequestTypeDef",
     "UpdateDomainMetadataRequestRequestTypeDef",
     "UpdateFleetMetadataRequestRequestTypeDef",
     "UpdateIdentityProviderConfigurationRequestRequestTypeDef",
-    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
-    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
-    "CreateFleetResponseTypeDef",
-    "DescribeAuditStreamConfigurationResponseTypeDef",
-    "DescribeCompanyNetworkConfigurationResponseTypeDef",
-    "DescribeDevicePolicyConfigurationResponseTypeDef",
-    "DescribeDeviceResponseTypeDef",
-    "DescribeDomainResponseTypeDef",
-    "DescribeFleetMetadataResponseTypeDef",
-    "DescribeIdentityProviderConfigurationResponseTypeDef",
-    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "ListFleetsResponseTypeDef",
     "ListWebsiteAuthorizationProvidersResponseTypeDef",
     "ListWebsiteCertificateAuthoritiesResponseTypeDef",
 )
 
@@ -123,22 +123,19 @@
 
 class AssociateWebsiteAuthorizationProviderRequestRequestTypeDef(
     _RequiredAssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     _OptionalAssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateWebsiteAuthorizationProviderResponseTypeDef = TypedDict(
+    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AuthorizationProviderId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "FleetArn": str,
@@ -155,14 +152,22 @@
 
 class AssociateWebsiteCertificateAuthorityRequestRequestTypeDef(
     _RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     _OptionalAssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
+AssociateWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
+    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
+    {
+        "WebsiteCaId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetRequestRequestTypeDef",
     {
         "FleetName": str,
     },
 )
 _OptionalCreateFleetRequestRequestTypeDef = TypedDict(
@@ -176,80 +181,177 @@
 )
 
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "FleetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteFleetRequestRequestTypeDef = TypedDict(
     "DeleteFleetRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
 DescribeAuditStreamConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeAuditStreamConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
+DescribeAuditStreamConfigurationResponseTypeDef = TypedDict(
+    "DescribeAuditStreamConfigurationResponseTypeDef",
+    {
+        "AuditStreamArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeCompanyNetworkConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeCompanyNetworkConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
+DescribeCompanyNetworkConfigurationResponseTypeDef = TypedDict(
+    "DescribeCompanyNetworkConfigurationResponseTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDevicePolicyConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeDevicePolicyConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
+DescribeDevicePolicyConfigurationResponseTypeDef = TypedDict(
+    "DescribeDevicePolicyConfigurationResponseTypeDef",
+    {
+        "DeviceCaCertificate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DeviceId": str,
     },
 )
 
+DescribeDeviceResponseTypeDef = TypedDict(
+    "DescribeDeviceResponseTypeDef",
+    {
+        "Status": DeviceStatusType,
+        "Model": str,
+        "Manufacturer": str,
+        "OperatingSystem": str,
+        "OperatingSystemVersion": str,
+        "PatchLevel": str,
+        "FirstAccessedTime": datetime,
+        "LastAccessedTime": datetime,
+        "Username": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDomainRequestRequestTypeDef = TypedDict(
     "DescribeDomainRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
 
+DescribeDomainResponseTypeDef = TypedDict(
+    "DescribeDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DisplayName": str,
+        "CreatedTime": datetime,
+        "DomainStatus": DomainStatusType,
+        "AcmCertificateArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeFleetMetadataRequestRequestTypeDef = TypedDict(
     "DescribeFleetMetadataRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
+DescribeFleetMetadataResponseTypeDef = TypedDict(
+    "DescribeFleetMetadataResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "FleetName": str,
+        "DisplayName": str,
+        "OptimizeForEndUserLocation": bool,
+        "CompanyCode": str,
+        "FleetStatus": FleetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeIdentityProviderConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeIdentityProviderConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
+DescribeIdentityProviderConfigurationResponseTypeDef = TypedDict(
+    "DescribeIdentityProviderConfigurationResponseTypeDef",
+    {
+        "IdentityProviderType": Literal["SAML"],
+        "ServiceProviderSamlMetadata": str,
+        "IdentityProviderSamlMetadata": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeWebsiteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "DescribeWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "FleetArn": str,
         "WebsiteCaId": str,
     },
 )
 
+DescribeWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
+    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
+    {
+        "Certificate": str,
+        "CreatedTime": datetime,
+        "DisplayName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "DeviceId": str,
         "DeviceStatus": DeviceStatusType,
     },
     total=False,
@@ -365,14 +467,22 @@
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
 _RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef = TypedDict(
     "_RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 _OptionalListWebsiteAuthorizationProvidersRequestRequestTypeDef = TypedDict(
@@ -439,14 +549,25 @@
         "WebsiteCaId": str,
         "CreatedTime": datetime,
         "DisplayName": str,
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
 RestoreDomainAccessRequestRequestTypeDef = TypedDict(
     "RestoreDomainAccessRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
@@ -592,172 +713,51 @@
 
 class UpdateIdentityProviderConfigurationRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderConfigurationRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderConfigurationRequestRequestTypeDef,
 ):
     pass
 
-AssociateWebsiteAuthorizationProviderResponseTypeDef = TypedDict(
-    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
-    {
-        "AuthorizationProviderId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
-    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
-    {
-        "WebsiteCaId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "FleetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAuditStreamConfigurationResponseTypeDef = TypedDict(
-    "DescribeAuditStreamConfigurationResponseTypeDef",
-    {
-        "AuditStreamArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeCompanyNetworkConfigurationResponseTypeDef = TypedDict(
-    "DescribeCompanyNetworkConfigurationResponseTypeDef",
-    {
-        "VpcId": str,
-        "SubnetIds": List[str],
-        "SecurityGroupIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDevicePolicyConfigurationResponseTypeDef = TypedDict(
-    "DescribeDevicePolicyConfigurationResponseTypeDef",
-    {
-        "DeviceCaCertificate": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDeviceResponseTypeDef = TypedDict(
-    "DescribeDeviceResponseTypeDef",
-    {
-        "Status": DeviceStatusType,
-        "Model": str,
-        "Manufacturer": str,
-        "OperatingSystem": str,
-        "OperatingSystemVersion": str,
-        "PatchLevel": str,
-        "FirstAccessedTime": datetime,
-        "LastAccessedTime": datetime,
-        "Username": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDomainResponseTypeDef = TypedDict(
-    "DescribeDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DisplayName": str,
-        "CreatedTime": datetime,
-        "DomainStatus": DomainStatusType,
-        "AcmCertificateArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFleetMetadataResponseTypeDef = TypedDict(
-    "DescribeFleetMetadataResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "FleetName": str,
-        "DisplayName": str,
-        "OptimizeForEndUserLocation": bool,
-        "CompanyCode": str,
-        "FleetStatus": FleetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeIdentityProviderConfigurationResponseTypeDef = TypedDict(
-    "DescribeIdentityProviderConfigurationResponseTypeDef",
-    {
-        "IdentityProviderType": Literal["SAML"],
-        "ServiceProviderSamlMetadata": str,
-        "IdentityProviderSamlMetadata": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
-    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
-    {
-        "Certificate": str,
-        "CreatedTime": datetime,
-        "DisplayName": str,
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
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFleetsResponseTypeDef = TypedDict(
     "ListFleetsResponseTypeDef",
     {
         "FleetSummaryList": List[FleetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWebsiteAuthorizationProvidersResponseTypeDef = TypedDict(
     "ListWebsiteAuthorizationProvidersResponseTypeDef",
     {
         "WebsiteAuthorizationProviders": List[WebsiteAuthorizationProviderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWebsiteCertificateAuthoritiesResponseTypeDef = TypedDict(
     "ListWebsiteCertificateAuthoritiesResponseTypeDef",
     {
         "WebsiteCertificateAuthorities": List[WebsiteCaSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink.egg-info/PKG-INFO` & `mypy-boto3-worklink-1.27.0/mypy_boto3_worklink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-worklink
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.WorkLink 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.WorkLink 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/
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
 
 <a id="mypy-boto3-worklink"></a>
 
 # mypy-boto3-worklink
 
 [![PyPI - mypy-boto3-worklink](https://img.shields.io/pypi/v/mypy-boto3-worklink.svg?color=blue)](https://pypi.org/project/mypy-boto3-worklink)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-worklink.svg?color=blue)](https://pypi.org/project/mypy-boto3-worklink)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-worklink?color=blue)](https://pypistats.org/packages/mypy-boto3-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkLink 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
+[boto3.WorkLink 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
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
 [mypy-boto3-worklink docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,63 +301,63 @@
 `mypy_boto3_worklink.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_worklink.type_defs import (
     AssociateDomainRequestRequestTypeDef,
     AssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateWebsiteAuthorizationProviderResponseTypeDef,
     AssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
+    AssociateWebsiteCertificateAuthorityResponseTypeDef,
     CreateFleetRequestRequestTypeDef,
+    CreateFleetResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DescribeAuditStreamConfigurationRequestRequestTypeDef,
+    DescribeAuditStreamConfigurationResponseTypeDef,
     DescribeCompanyNetworkConfigurationRequestRequestTypeDef,
+    DescribeCompanyNetworkConfigurationResponseTypeDef,
     DescribeDevicePolicyConfigurationRequestRequestTypeDef,
+    DescribeDevicePolicyConfigurationResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
+    DescribeDeviceResponseTypeDef,
     DescribeDomainRequestRequestTypeDef,
+    DescribeDomainResponseTypeDef,
     DescribeFleetMetadataRequestRequestTypeDef,
+    DescribeFleetMetadataResponseTypeDef,
     DescribeIdentityProviderConfigurationRequestRequestTypeDef,
+    DescribeIdentityProviderConfigurationResponseTypeDef,
     DescribeWebsiteCertificateAuthorityRequestRequestTypeDef,
+    DescribeWebsiteCertificateAuthorityResponseTypeDef,
     DeviceSummaryTypeDef,
     DisassociateDomainRequestRequestTypeDef,
     DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     DomainSummaryTypeDef,
     FleetSummaryTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFleetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWebsiteAuthorizationProvidersRequestRequestTypeDef,
     WebsiteAuthorizationProviderSummaryTypeDef,
     ListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
     WebsiteCaSummaryTypeDef,
+    ResponseMetadataTypeDef,
     RestoreDomainAccessRequestRequestTypeDef,
     RevokeDomainAccessRequestRequestTypeDef,
     SignOutUserRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuditStreamConfigurationRequestRequestTypeDef,
     UpdateCompanyNetworkConfigurationRequestRequestTypeDef,
     UpdateDevicePolicyConfigurationRequestRequestTypeDef,
     UpdateDomainMetadataRequestRequestTypeDef,
     UpdateFleetMetadataRequestRequestTypeDef,
     UpdateIdentityProviderConfigurationRequestRequestTypeDef,
-    AssociateWebsiteAuthorizationProviderResponseTypeDef,
-    AssociateWebsiteCertificateAuthorityResponseTypeDef,
-    CreateFleetResponseTypeDef,
-    DescribeAuditStreamConfigurationResponseTypeDef,
-    DescribeCompanyNetworkConfigurationResponseTypeDef,
-    DescribeDevicePolicyConfigurationResponseTypeDef,
-    DescribeDeviceResponseTypeDef,
-    DescribeDomainResponseTypeDef,
-    DescribeFleetMetadataResponseTypeDef,
-    DescribeIdentityProviderConfigurationResponseTypeDef,
-    DescribeWebsiteCertificateAuthorityResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ListWebsiteAuthorizationProvidersResponseTypeDef,
     ListWebsiteCertificateAuthoritiesResponseTypeDef,
 )
 
@@ -368,42 +369,42 @@
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

### Comparing `mypy-boto3-worklink-1.26.0.post1/mypy_boto3_worklink.egg-info/SOURCES.txt` & `mypy-boto3-worklink-1.27.0/mypy_boto3_worklink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-worklink-1.26.0.post1/setup.py` & `mypy-boto3-worklink-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-worklink.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-worklink",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_worklink"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkLink 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.WorkLink 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 worklink type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_worklink": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_worklink": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/",
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


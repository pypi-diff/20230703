# Comparing `tmp/mypy-boto3-opensearchserverless-1.26.19.tar.gz` & `tmp/mypy-boto3-opensearchserverless-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opensearchserverless-1.26.19.tar", last modified: Tue Nov 29 20:35:12 2022, max compression
+gzip compressed data, was "mypy-boto3-opensearchserverless-1.27.0.tar", last modified: Mon Jul  3 19:51:12 2023, max compression
```

## Comparing `mypy-boto3-opensearchserverless-1.26.19.tar` & `mypy-boto3-opensearchserverless-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.121234 mypy-boto3-opensearchserverless-1.26.19/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-29 20:34:57.000000 mypy-boto3-opensearchserverless-1.26.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    15823 2022-11-29 20:35:12.121234 mypy-boto3-opensearchserverless-1.26.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14327 2022-11-29 20:34:57.000000 mypy-boto3-opensearchserverless-1.26.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.113234 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/
--rw-r--r--   0 runner    (1001) docker     (122)      512 2022-11-29 20:34:57.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      511 2022-11-29 20:34:57.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      985 2022-11-29 20:34:57.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23818 2022-11-29 20:34:57.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    23780 2022-11-29 20:34:57.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     7636 2022-11-29 20:34:58.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)     7634 2022-11-29 20:34:57.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 20:34:57.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    29351 2022-11-29 20:34:59.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    29312 2022-11-29 20:34:58.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-29 20:34:57.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.121234 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15823 2022-11-29 20:35:11.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      836 2022-11-29 20:35:11.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 20:35:11.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 20:35:11.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-29 20:35:11.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2022-11-29 20:35:11.000000 mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 20:35:12.121234 mypy-boto3-opensearchserverless-1.26.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2022-11-29 20:34:57.000000 mypy-boto3-opensearchserverless-1.26.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:12.499759 mypy-boto3-opensearchserverless-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:02.000000 mypy-boto3-opensearchserverless-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15877 2023-07-03 19:51:12.499759 mypy-boto3-opensearchserverless-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-07-03 19:43:02.000000 mypy-boto3-opensearchserverless-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:12.499759 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 19:43:02.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-03 19:43:02.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-03 19:43:02.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23936 2023-07-03 19:43:02.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23898 2023-07-03 19:43:02.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-03 19:43:03.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-03 19:43:02.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:02.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29403 2023-07-03 19:43:05.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29364 2023-07-03 19:43:03.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:02.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:12.499759 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15877 2023-07-03 19:51:12.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-03 19:51:12.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:12.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:12.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:12.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 19:51:12.000000 mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:12.499759 mypy-boto3-opensearchserverless-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-03 19:43:02.000000 mypy-boto3-opensearchserverless-1.27.0/setup.py
```

### Comparing `mypy-boto3-opensearchserverless-1.26.19/LICENSE` & `mypy-boto3-opensearchserverless-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-opensearchserverless-1.26.19/PKG-INFO` & `mypy-boto3-opensearchserverless-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearchserverless
-Version: 1.26.19
-Summary: Type annotations for boto3.OpenSearchServiceServerless 1.26.19 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.OpenSearchServiceServerless 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/
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
 
 <a id="mypy-boto3-opensearchserverless"></a>
 
 # mypy-boto3-opensearchserverless
 
 [![PyPI - mypy-boto3-opensearchserverless](https://img.shields.io/pypi/v/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearchserverless?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchServiceServerless 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[boto3.OpenSearchServiceServerless 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opensearchserverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -285,14 +286,15 @@
     CollectionTypeType,
     SecurityConfigTypeType,
     SecurityPolicyTypeType,
     VpcEndpointStatusType,
     OpenSearchServiceServerlessServiceName,
     ServiceName,
     ResourceServiceName,
+    RegionName,
 )
 
 
 def check_value(value: AccessPolicyTypeType) -> bool:
     ...
 ```
 
@@ -308,15 +310,14 @@
     AccessPolicyDetailTypeDef,
     AccessPolicyStatsTypeDef,
     AccessPolicySummaryTypeDef,
     CapacityLimitsTypeDef,
     BatchGetCollectionRequestRequestTypeDef,
     CollectionDetailTypeDef,
     CollectionErrorDetailTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetVpcEndpointRequestRequestTypeDef,
     VpcEndpointDetailTypeDef,
     VpcEndpointErrorDetailTypeDef,
     CollectionFiltersTypeDef,
     CollectionSummaryTypeDef,
     CreateAccessPolicyRequestRequestTypeDef,
     CreateCollectionDetailTypeDef,
@@ -342,28 +343,29 @@
     ListSecurityConfigsRequestRequestTypeDef,
     SecurityConfigSummaryTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
     SecurityPolicySummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     VpcEndpointFiltersTypeDef,
     VpcEndpointSummaryTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     UpdateCollectionDetailTypeDef,
     UpdateCollectionRequestRequestTypeDef,
     UpdateSecurityPolicyRequestRequestTypeDef,
     UpdateVpcEndpointDetailTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
-    AccountSettingsDetailTypeDef,
-    UpdateAccountSettingsRequestRequestTypeDef,
-    BatchGetCollectionResponseTypeDef,
     CreateAccessPolicyResponseTypeDef,
     GetAccessPolicyResponseTypeDef,
-    ListAccessPoliciesResponseTypeDef,
     UpdateAccessPolicyResponseTypeDef,
+    ListAccessPoliciesResponseTypeDef,
+    AccountSettingsDetailTypeDef,
+    UpdateAccountSettingsRequestRequestTypeDef,
+    BatchGetCollectionResponseTypeDef,
     BatchGetVpcEndpointResponseTypeDef,
     ListCollectionsRequestRequestTypeDef,
     ListCollectionsResponseTypeDef,
     CreateCollectionResponseTypeDef,
     CreateCollectionRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -398,42 +400,42 @@
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

### Comparing `mypy-boto3-opensearchserverless-1.26.19/README.md` & `mypy-boto3-opensearchserverless-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-opensearchserverless"></a>
 
 # mypy-boto3-opensearchserverless
 
 [![PyPI - mypy-boto3-opensearchserverless](https://img.shields.io/pypi/v/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearchserverless?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchServiceServerless 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[boto3.OpenSearchServiceServerless 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opensearchserverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -254,14 +254,15 @@
     CollectionTypeType,
     SecurityConfigTypeType,
     SecurityPolicyTypeType,
     VpcEndpointStatusType,
     OpenSearchServiceServerlessServiceName,
     ServiceName,
     ResourceServiceName,
+    RegionName,
 )
 
 
 def check_value(value: AccessPolicyTypeType) -> bool:
     ...
 ```
 
@@ -277,15 +278,14 @@
     AccessPolicyDetailTypeDef,
     AccessPolicyStatsTypeDef,
     AccessPolicySummaryTypeDef,
     CapacityLimitsTypeDef,
     BatchGetCollectionRequestRequestTypeDef,
     CollectionDetailTypeDef,
     CollectionErrorDetailTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetVpcEndpointRequestRequestTypeDef,
     VpcEndpointDetailTypeDef,
     VpcEndpointErrorDetailTypeDef,
     CollectionFiltersTypeDef,
     CollectionSummaryTypeDef,
     CreateAccessPolicyRequestRequestTypeDef,
     CreateCollectionDetailTypeDef,
@@ -311,28 +311,29 @@
     ListSecurityConfigsRequestRequestTypeDef,
     SecurityConfigSummaryTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
     SecurityPolicySummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     VpcEndpointFiltersTypeDef,
     VpcEndpointSummaryTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     UpdateCollectionDetailTypeDef,
     UpdateCollectionRequestRequestTypeDef,
     UpdateSecurityPolicyRequestRequestTypeDef,
     UpdateVpcEndpointDetailTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
-    AccountSettingsDetailTypeDef,
-    UpdateAccountSettingsRequestRequestTypeDef,
-    BatchGetCollectionResponseTypeDef,
     CreateAccessPolicyResponseTypeDef,
     GetAccessPolicyResponseTypeDef,
-    ListAccessPoliciesResponseTypeDef,
     UpdateAccessPolicyResponseTypeDef,
+    ListAccessPoliciesResponseTypeDef,
+    AccountSettingsDetailTypeDef,
+    UpdateAccountSettingsRequestRequestTypeDef,
+    BatchGetCollectionResponseTypeDef,
     BatchGetVpcEndpointResponseTypeDef,
     ListCollectionsRequestRequestTypeDef,
     ListCollectionsResponseTypeDef,
     CreateCollectionResponseTypeDef,
     CreateCollectionRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -367,42 +368,42 @@
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

### Comparing `mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/__init__.py` & `mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/__main__.py` & `mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchServiceServerless 1.26.19\nVersion:        "
-        " 1.26.19\nBuilder version: 7.11.11\nDocs:           "
+        "Type annotations for boto3.OpenSearchServiceServerless 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.19")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/client.py` & `mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,17 @@
         self.operation_name: str
 
 
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
+    OcuLimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
+    ServiceQuotaExceededException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 
 class OpenSearchServiceServerlessClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/client/)
```

### Comparing `mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/client.pyi` & `mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,17 @@
         self.response: Dict[str, Any]
         self.operation_name: str
 
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
+    OcuLimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
+    ServiceQuotaExceededException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 class OpenSearchServiceServerlessClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/client/)
     """
```

### Comparing `mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/literals.py` & `mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "CollectionTypeType",
     "SecurityConfigTypeType",
     "SecurityPolicyTypeType",
     "VpcEndpointStatusType",
     "OpenSearchServiceServerlessServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "RegionName",
 )
 
 
 AccessPolicyTypeType = Literal["data"]
 CollectionStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 CollectionTypeType = Literal["SEARCH", "TIMESERIES"]
 SecurityConfigTypeType = Literal["saml"]
@@ -50,14 +51,15 @@
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
@@ -78,30 +80,34 @@
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
@@ -127,14 +133,15 @@
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
@@ -179,14 +186,15 @@
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
@@ -197,34 +205,38 @@
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
@@ -237,14 +249,15 @@
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
@@ -263,24 +276,28 @@
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
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -308,14 +325,16 @@
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
@@ -349,18 +368,21 @@
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
@@ -378,7 +400,17 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+RegionName = Literal[
+    "ap-northeast-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "eu-central-1",
+    "eu-west-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/literals.pyi` & `mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "CollectionTypeType",
     "SecurityConfigTypeType",
     "SecurityPolicyTypeType",
     "VpcEndpointStatusType",
     "OpenSearchServiceServerlessServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "RegionName",
 )
 
 AccessPolicyTypeType = Literal["data"]
 CollectionStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 CollectionTypeType = Literal["SEARCH", "TIMESERIES"]
 SecurityConfigTypeType = Literal["saml"]
 SecurityPolicyTypeType = Literal["encryption", "network"]
@@ -48,14 +49,15 @@
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
@@ -76,30 +78,34 @@
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
@@ -125,14 +131,15 @@
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
@@ -177,14 +184,15 @@
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
@@ -195,34 +203,38 @@
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
@@ -235,14 +247,15 @@
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
@@ -261,24 +274,28 @@
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
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -306,14 +323,16 @@
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
@@ -347,18 +366,21 @@
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
@@ -376,7 +398,17 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+RegionName = Literal[
+    "ap-northeast-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "eu-central-1",
+    "eu-west-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/type_defs.py` & `mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     "AccessPolicyDetailTypeDef",
     "AccessPolicyStatsTypeDef",
     "AccessPolicySummaryTypeDef",
     "CapacityLimitsTypeDef",
     "BatchGetCollectionRequestRequestTypeDef",
     "CollectionDetailTypeDef",
     "CollectionErrorDetailTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetVpcEndpointRequestRequestTypeDef",
     "VpcEndpointDetailTypeDef",
     "VpcEndpointErrorDetailTypeDef",
     "CollectionFiltersTypeDef",
     "CollectionSummaryTypeDef",
     "CreateAccessPolicyRequestRequestTypeDef",
     "CreateCollectionDetailTypeDef",
@@ -69,28 +68,29 @@
     "ListSecurityConfigsRequestRequestTypeDef",
     "SecurityConfigSummaryTypeDef",
     "ListSecurityPoliciesRequestRequestTypeDef",
     "SecurityPolicySummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "VpcEndpointFiltersTypeDef",
     "VpcEndpointSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessPolicyRequestRequestTypeDef",
     "UpdateCollectionDetailTypeDef",
     "UpdateCollectionRequestRequestTypeDef",
     "UpdateSecurityPolicyRequestRequestTypeDef",
     "UpdateVpcEndpointDetailTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
-    "AccountSettingsDetailTypeDef",
-    "UpdateAccountSettingsRequestRequestTypeDef",
-    "BatchGetCollectionResponseTypeDef",
     "CreateAccessPolicyResponseTypeDef",
     "GetAccessPolicyResponseTypeDef",
-    "ListAccessPoliciesResponseTypeDef",
     "UpdateAccessPolicyResponseTypeDef",
+    "ListAccessPoliciesResponseTypeDef",
+    "AccountSettingsDetailTypeDef",
+    "UpdateAccountSettingsRequestRequestTypeDef",
+    "BatchGetCollectionResponseTypeDef",
     "BatchGetVpcEndpointResponseTypeDef",
     "ListCollectionsRequestRequestTypeDef",
     "ListCollectionsResponseTypeDef",
     "CreateCollectionResponseTypeDef",
     "CreateCollectionRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -195,25 +195,14 @@
         "errorMessage": str,
         "id": str,
         "name": str,
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
 BatchGetVpcEndpointRequestRequestTypeDef = TypedDict(
     "BatchGetVpcEndpointRequestRequestTypeDef",
     {
         "ids": Sequence[str],
     },
 )
 
@@ -694,14 +683,25 @@
         "id": str,
         "name": str,
         "status": VpcEndpointStatusType,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -829,78 +829,78 @@
 
 class UpdateVpcEndpointRequestRequestTypeDef(
     _RequiredUpdateVpcEndpointRequestRequestTypeDef, _OptionalUpdateVpcEndpointRequestRequestTypeDef
 ):
     pass
 
 
-AccountSettingsDetailTypeDef = TypedDict(
-    "AccountSettingsDetailTypeDef",
+CreateAccessPolicyResponseTypeDef = TypedDict(
+    "CreateAccessPolicyResponseTypeDef",
     {
-        "capacityLimits": CapacityLimitsTypeDef,
+        "accessPolicyDetail": AccessPolicyDetailTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateAccountSettingsRequestRequestTypeDef",
+GetAccessPolicyResponseTypeDef = TypedDict(
+    "GetAccessPolicyResponseTypeDef",
     {
-        "capacityLimits": CapacityLimitsTypeDef,
+        "accessPolicyDetail": AccessPolicyDetailTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-BatchGetCollectionResponseTypeDef = TypedDict(
-    "BatchGetCollectionResponseTypeDef",
+UpdateAccessPolicyResponseTypeDef = TypedDict(
+    "UpdateAccessPolicyResponseTypeDef",
     {
-        "collectionDetails": List[CollectionDetailTypeDef],
-        "collectionErrorDetails": List[CollectionErrorDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "accessPolicyDetail": AccessPolicyDetailTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateAccessPolicyResponseTypeDef = TypedDict(
-    "CreateAccessPolicyResponseTypeDef",
+ListAccessPoliciesResponseTypeDef = TypedDict(
+    "ListAccessPoliciesResponseTypeDef",
     {
-        "accessPolicyDetail": AccessPolicyDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "accessPolicySummaries": List[AccessPolicySummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAccessPolicyResponseTypeDef = TypedDict(
-    "GetAccessPolicyResponseTypeDef",
+AccountSettingsDetailTypeDef = TypedDict(
+    "AccountSettingsDetailTypeDef",
     {
-        "accessPolicyDetail": AccessPolicyDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "capacityLimits": CapacityLimitsTypeDef,
     },
+    total=False,
 )
 
-ListAccessPoliciesResponseTypeDef = TypedDict(
-    "ListAccessPoliciesResponseTypeDef",
+UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateAccountSettingsRequestRequestTypeDef",
     {
-        "accessPolicySummaries": List[AccessPolicySummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "capacityLimits": CapacityLimitsTypeDef,
     },
+    total=False,
 )
 
-UpdateAccessPolicyResponseTypeDef = TypedDict(
-    "UpdateAccessPolicyResponseTypeDef",
+BatchGetCollectionResponseTypeDef = TypedDict(
+    "BatchGetCollectionResponseTypeDef",
     {
-        "accessPolicyDetail": AccessPolicyDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "collectionDetails": List[CollectionDetailTypeDef],
+        "collectionErrorDetails": List[CollectionErrorDetailTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetVpcEndpointResponseTypeDef = TypedDict(
     "BatchGetVpcEndpointResponseTypeDef",
     {
         "vpcEndpointDetails": List[VpcEndpointDetailTypeDef],
         "vpcEndpointErrorDetails": List[VpcEndpointErrorDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCollectionsRequestRequestTypeDef = TypedDict(
     "ListCollectionsRequestRequestTypeDef",
     {
         "collectionFilters": CollectionFiltersTypeDef,
@@ -911,23 +911,23 @@
 )
 
 ListCollectionsResponseTypeDef = TypedDict(
     "ListCollectionsResponseTypeDef",
     {
         "collectionSummaries": List[CollectionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCollectionResponseTypeDef = TypedDict(
     "CreateCollectionResponseTypeDef",
     {
         "createCollectionDetail": CreateCollectionDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCollectionRequestRequestTypeDef",
     {
         "name": str,
@@ -951,15 +951,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1031,84 +1031,84 @@
     pass
 
 
 CreateSecurityPolicyResponseTypeDef = TypedDict(
     "CreateSecurityPolicyResponseTypeDef",
     {
         "securityPolicyDetail": SecurityPolicyDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSecurityPolicyResponseTypeDef = TypedDict(
     "GetSecurityPolicyResponseTypeDef",
     {
         "securityPolicyDetail": SecurityPolicyDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSecurityPolicyResponseTypeDef = TypedDict(
     "UpdateSecurityPolicyResponseTypeDef",
     {
         "securityPolicyDetail": SecurityPolicyDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "createVpcEndpointDetail": CreateVpcEndpointDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCollectionResponseTypeDef = TypedDict(
     "DeleteCollectionResponseTypeDef",
     {
         "deleteCollectionDetail": DeleteCollectionDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVpcEndpointResponseTypeDef = TypedDict(
     "DeleteVpcEndpointResponseTypeDef",
     {
         "deleteVpcEndpointDetail": DeleteVpcEndpointDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPoliciesStatsResponseTypeDef = TypedDict(
     "GetPoliciesStatsResponseTypeDef",
     {
         "AccessPolicyStats": AccessPolicyStatsTypeDef,
         "SecurityConfigStats": SecurityConfigStatsTypeDef,
         "SecurityPolicyStats": SecurityPolicyStatsTypeDef,
         "TotalPolicyCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSecurityConfigsResponseTypeDef = TypedDict(
     "ListSecurityConfigsResponseTypeDef",
     {
         "nextToken": str,
         "securityConfigSummaries": List[SecurityConfigSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSecurityPoliciesResponseTypeDef = TypedDict(
     "ListSecurityPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "securityPolicySummaries": List[SecurityPolicySummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointsRequestRequestTypeDef = TypedDict(
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "maxResults": int,
@@ -1119,66 +1119,66 @@
 )
 
 ListVpcEndpointsResponseTypeDef = TypedDict(
     "ListVpcEndpointsResponseTypeDef",
     {
         "nextToken": str,
         "vpcEndpointSummaries": List[VpcEndpointSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCollectionResponseTypeDef = TypedDict(
     "UpdateCollectionResponseTypeDef",
     {
         "updateCollectionDetail": UpdateCollectionDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVpcEndpointResponseTypeDef = TypedDict(
     "UpdateVpcEndpointResponseTypeDef",
     {
         "UpdateVpcEndpointDetail": UpdateVpcEndpointDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccountSettingsResponseTypeDef = TypedDict(
     "GetAccountSettingsResponseTypeDef",
     {
         "accountSettingsDetail": AccountSettingsDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountSettingsResponseTypeDef = TypedDict(
     "UpdateAccountSettingsResponseTypeDef",
     {
         "accountSettingsDetail": AccountSettingsDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSecurityConfigResponseTypeDef = TypedDict(
     "CreateSecurityConfigResponseTypeDef",
     {
         "securityConfigDetail": SecurityConfigDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSecurityConfigResponseTypeDef = TypedDict(
     "GetSecurityConfigResponseTypeDef",
     {
         "securityConfigDetail": SecurityConfigDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSecurityConfigResponseTypeDef = TypedDict(
     "UpdateSecurityConfigResponseTypeDef",
     {
         "securityConfigDetail": SecurityConfigDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless/type_defs.pyi` & `mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     "AccessPolicyDetailTypeDef",
     "AccessPolicyStatsTypeDef",
     "AccessPolicySummaryTypeDef",
     "CapacityLimitsTypeDef",
     "BatchGetCollectionRequestRequestTypeDef",
     "CollectionDetailTypeDef",
     "CollectionErrorDetailTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetVpcEndpointRequestRequestTypeDef",
     "VpcEndpointDetailTypeDef",
     "VpcEndpointErrorDetailTypeDef",
     "CollectionFiltersTypeDef",
     "CollectionSummaryTypeDef",
     "CreateAccessPolicyRequestRequestTypeDef",
     "CreateCollectionDetailTypeDef",
@@ -68,28 +67,29 @@
     "ListSecurityConfigsRequestRequestTypeDef",
     "SecurityConfigSummaryTypeDef",
     "ListSecurityPoliciesRequestRequestTypeDef",
     "SecurityPolicySummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "VpcEndpointFiltersTypeDef",
     "VpcEndpointSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessPolicyRequestRequestTypeDef",
     "UpdateCollectionDetailTypeDef",
     "UpdateCollectionRequestRequestTypeDef",
     "UpdateSecurityPolicyRequestRequestTypeDef",
     "UpdateVpcEndpointDetailTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
-    "AccountSettingsDetailTypeDef",
-    "UpdateAccountSettingsRequestRequestTypeDef",
-    "BatchGetCollectionResponseTypeDef",
     "CreateAccessPolicyResponseTypeDef",
     "GetAccessPolicyResponseTypeDef",
-    "ListAccessPoliciesResponseTypeDef",
     "UpdateAccessPolicyResponseTypeDef",
+    "ListAccessPoliciesResponseTypeDef",
+    "AccountSettingsDetailTypeDef",
+    "UpdateAccountSettingsRequestRequestTypeDef",
+    "BatchGetCollectionResponseTypeDef",
     "BatchGetVpcEndpointResponseTypeDef",
     "ListCollectionsRequestRequestTypeDef",
     "ListCollectionsResponseTypeDef",
     "CreateCollectionResponseTypeDef",
     "CreateCollectionRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -194,25 +194,14 @@
         "errorMessage": str,
         "id": str,
         "name": str,
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
 BatchGetVpcEndpointRequestRequestTypeDef = TypedDict(
     "BatchGetVpcEndpointRequestRequestTypeDef",
     {
         "ids": Sequence[str],
     },
 )
 
@@ -669,14 +658,25 @@
         "id": str,
         "name": str,
         "status": VpcEndpointStatusType,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -796,78 +796,78 @@
 )
 
 class UpdateVpcEndpointRequestRequestTypeDef(
     _RequiredUpdateVpcEndpointRequestRequestTypeDef, _OptionalUpdateVpcEndpointRequestRequestTypeDef
 ):
     pass
 
-AccountSettingsDetailTypeDef = TypedDict(
-    "AccountSettingsDetailTypeDef",
+CreateAccessPolicyResponseTypeDef = TypedDict(
+    "CreateAccessPolicyResponseTypeDef",
     {
-        "capacityLimits": CapacityLimitsTypeDef,
+        "accessPolicyDetail": AccessPolicyDetailTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateAccountSettingsRequestRequestTypeDef",
+GetAccessPolicyResponseTypeDef = TypedDict(
+    "GetAccessPolicyResponseTypeDef",
     {
-        "capacityLimits": CapacityLimitsTypeDef,
+        "accessPolicyDetail": AccessPolicyDetailTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-BatchGetCollectionResponseTypeDef = TypedDict(
-    "BatchGetCollectionResponseTypeDef",
+UpdateAccessPolicyResponseTypeDef = TypedDict(
+    "UpdateAccessPolicyResponseTypeDef",
     {
-        "collectionDetails": List[CollectionDetailTypeDef],
-        "collectionErrorDetails": List[CollectionErrorDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "accessPolicyDetail": AccessPolicyDetailTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateAccessPolicyResponseTypeDef = TypedDict(
-    "CreateAccessPolicyResponseTypeDef",
+ListAccessPoliciesResponseTypeDef = TypedDict(
+    "ListAccessPoliciesResponseTypeDef",
     {
-        "accessPolicyDetail": AccessPolicyDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "accessPolicySummaries": List[AccessPolicySummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAccessPolicyResponseTypeDef = TypedDict(
-    "GetAccessPolicyResponseTypeDef",
+AccountSettingsDetailTypeDef = TypedDict(
+    "AccountSettingsDetailTypeDef",
     {
-        "accessPolicyDetail": AccessPolicyDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "capacityLimits": CapacityLimitsTypeDef,
     },
+    total=False,
 )
 
-ListAccessPoliciesResponseTypeDef = TypedDict(
-    "ListAccessPoliciesResponseTypeDef",
+UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateAccountSettingsRequestRequestTypeDef",
     {
-        "accessPolicySummaries": List[AccessPolicySummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "capacityLimits": CapacityLimitsTypeDef,
     },
+    total=False,
 )
 
-UpdateAccessPolicyResponseTypeDef = TypedDict(
-    "UpdateAccessPolicyResponseTypeDef",
+BatchGetCollectionResponseTypeDef = TypedDict(
+    "BatchGetCollectionResponseTypeDef",
     {
-        "accessPolicyDetail": AccessPolicyDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "collectionDetails": List[CollectionDetailTypeDef],
+        "collectionErrorDetails": List[CollectionErrorDetailTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetVpcEndpointResponseTypeDef = TypedDict(
     "BatchGetVpcEndpointResponseTypeDef",
     {
         "vpcEndpointDetails": List[VpcEndpointDetailTypeDef],
         "vpcEndpointErrorDetails": List[VpcEndpointErrorDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCollectionsRequestRequestTypeDef = TypedDict(
     "ListCollectionsRequestRequestTypeDef",
     {
         "collectionFilters": CollectionFiltersTypeDef,
@@ -878,23 +878,23 @@
 )
 
 ListCollectionsResponseTypeDef = TypedDict(
     "ListCollectionsResponseTypeDef",
     {
         "collectionSummaries": List[CollectionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCollectionResponseTypeDef = TypedDict(
     "CreateCollectionResponseTypeDef",
     {
         "createCollectionDetail": CreateCollectionDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCollectionRequestRequestTypeDef",
     {
         "name": str,
@@ -916,15 +916,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -992,84 +992,84 @@
 ):
     pass
 
 CreateSecurityPolicyResponseTypeDef = TypedDict(
     "CreateSecurityPolicyResponseTypeDef",
     {
         "securityPolicyDetail": SecurityPolicyDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSecurityPolicyResponseTypeDef = TypedDict(
     "GetSecurityPolicyResponseTypeDef",
     {
         "securityPolicyDetail": SecurityPolicyDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSecurityPolicyResponseTypeDef = TypedDict(
     "UpdateSecurityPolicyResponseTypeDef",
     {
         "securityPolicyDetail": SecurityPolicyDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "createVpcEndpointDetail": CreateVpcEndpointDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCollectionResponseTypeDef = TypedDict(
     "DeleteCollectionResponseTypeDef",
     {
         "deleteCollectionDetail": DeleteCollectionDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVpcEndpointResponseTypeDef = TypedDict(
     "DeleteVpcEndpointResponseTypeDef",
     {
         "deleteVpcEndpointDetail": DeleteVpcEndpointDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPoliciesStatsResponseTypeDef = TypedDict(
     "GetPoliciesStatsResponseTypeDef",
     {
         "AccessPolicyStats": AccessPolicyStatsTypeDef,
         "SecurityConfigStats": SecurityConfigStatsTypeDef,
         "SecurityPolicyStats": SecurityPolicyStatsTypeDef,
         "TotalPolicyCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSecurityConfigsResponseTypeDef = TypedDict(
     "ListSecurityConfigsResponseTypeDef",
     {
         "nextToken": str,
         "securityConfigSummaries": List[SecurityConfigSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSecurityPoliciesResponseTypeDef = TypedDict(
     "ListSecurityPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "securityPolicySummaries": List[SecurityPolicySummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcEndpointsRequestRequestTypeDef = TypedDict(
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "maxResults": int,
@@ -1080,66 +1080,66 @@
 )
 
 ListVpcEndpointsResponseTypeDef = TypedDict(
     "ListVpcEndpointsResponseTypeDef",
     {
         "nextToken": str,
         "vpcEndpointSummaries": List[VpcEndpointSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCollectionResponseTypeDef = TypedDict(
     "UpdateCollectionResponseTypeDef",
     {
         "updateCollectionDetail": UpdateCollectionDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVpcEndpointResponseTypeDef = TypedDict(
     "UpdateVpcEndpointResponseTypeDef",
     {
         "UpdateVpcEndpointDetail": UpdateVpcEndpointDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccountSettingsResponseTypeDef = TypedDict(
     "GetAccountSettingsResponseTypeDef",
     {
         "accountSettingsDetail": AccountSettingsDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountSettingsResponseTypeDef = TypedDict(
     "UpdateAccountSettingsResponseTypeDef",
     {
         "accountSettingsDetail": AccountSettingsDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSecurityConfigResponseTypeDef = TypedDict(
     "CreateSecurityConfigResponseTypeDef",
     {
         "securityConfigDetail": SecurityConfigDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSecurityConfigResponseTypeDef = TypedDict(
     "GetSecurityConfigResponseTypeDef",
     {
         "securityConfigDetail": SecurityConfigDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSecurityConfigResponseTypeDef = TypedDict(
     "UpdateSecurityConfigResponseTypeDef",
     {
         "securityConfigDetail": SecurityConfigDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless.egg-info/PKG-INFO` & `mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearchserverless
-Version: 1.26.19
-Summary: Type annotations for boto3.OpenSearchServiceServerless 1.26.19 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.OpenSearchServiceServerless 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/
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
 
 <a id="mypy-boto3-opensearchserverless"></a>
 
 # mypy-boto3-opensearchserverless
 
 [![PyPI - mypy-boto3-opensearchserverless](https://img.shields.io/pypi/v/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearchserverless?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchServiceServerless 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[boto3.OpenSearchServiceServerless 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opensearchserverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -285,14 +286,15 @@
     CollectionTypeType,
     SecurityConfigTypeType,
     SecurityPolicyTypeType,
     VpcEndpointStatusType,
     OpenSearchServiceServerlessServiceName,
     ServiceName,
     ResourceServiceName,
+    RegionName,
 )
 
 
 def check_value(value: AccessPolicyTypeType) -> bool:
     ...
 ```
 
@@ -308,15 +310,14 @@
     AccessPolicyDetailTypeDef,
     AccessPolicyStatsTypeDef,
     AccessPolicySummaryTypeDef,
     CapacityLimitsTypeDef,
     BatchGetCollectionRequestRequestTypeDef,
     CollectionDetailTypeDef,
     CollectionErrorDetailTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetVpcEndpointRequestRequestTypeDef,
     VpcEndpointDetailTypeDef,
     VpcEndpointErrorDetailTypeDef,
     CollectionFiltersTypeDef,
     CollectionSummaryTypeDef,
     CreateAccessPolicyRequestRequestTypeDef,
     CreateCollectionDetailTypeDef,
@@ -342,28 +343,29 @@
     ListSecurityConfigsRequestRequestTypeDef,
     SecurityConfigSummaryTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
     SecurityPolicySummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     VpcEndpointFiltersTypeDef,
     VpcEndpointSummaryTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     UpdateCollectionDetailTypeDef,
     UpdateCollectionRequestRequestTypeDef,
     UpdateSecurityPolicyRequestRequestTypeDef,
     UpdateVpcEndpointDetailTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
-    AccountSettingsDetailTypeDef,
-    UpdateAccountSettingsRequestRequestTypeDef,
-    BatchGetCollectionResponseTypeDef,
     CreateAccessPolicyResponseTypeDef,
     GetAccessPolicyResponseTypeDef,
-    ListAccessPoliciesResponseTypeDef,
     UpdateAccessPolicyResponseTypeDef,
+    ListAccessPoliciesResponseTypeDef,
+    AccountSettingsDetailTypeDef,
+    UpdateAccountSettingsRequestRequestTypeDef,
+    BatchGetCollectionResponseTypeDef,
     BatchGetVpcEndpointResponseTypeDef,
     ListCollectionsRequestRequestTypeDef,
     ListCollectionsResponseTypeDef,
     CreateCollectionResponseTypeDef,
     CreateCollectionRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -398,42 +400,42 @@
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

### Comparing `mypy-boto3-opensearchserverless-1.26.19/mypy_boto3_opensearchserverless.egg-info/SOURCES.txt` & `mypy-boto3-opensearchserverless-1.27.0/mypy_boto3_opensearchserverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.26.19/setup.py` & `mypy-boto3-opensearchserverless-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """
 Setup script for mypy-boto3-opensearchserverless.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opensearchserverless",
-    version="1.26.19",
+    version="1.27.0",
     packages=["mypy_boto3_opensearchserverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchServiceServerless 1.26.19 service generated with"
-        " mypy-boto3-builder 7.11.11"
+        "Type annotations for boto3.OpenSearchServiceServerless 1.27.0 service generated with"
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
     keywords="boto3 opensearchserverless type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_opensearchserverless": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_opensearchserverless": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/"
         ),
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


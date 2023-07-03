# Comparing `tmp/mypy-boto3-managedblockchain-1.26.9.tar.gz` & `tmp/mypy-boto3-managedblockchain-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-managedblockchain-1.26.9.tar", last modified: Mon Nov 14 20:49:29 2022, max compression
+gzip compressed data, was "mypy-boto3-managedblockchain-1.27.0.tar", last modified: Mon Jul  3 19:51:05 2023, max compression
```

## Comparing `mypy-boto3-managedblockchain-1.26.9.tar` & `mypy-boto3-managedblockchain-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.644561 mypy-boto3-managedblockchain-1.26.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16116 2022-11-14 20:49:29.640561 mypy-boto3-managedblockchain-1.26.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14641 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.636561 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20302 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    20267 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8519 2022-11-14 20:48:57.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8517 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1928 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    26054 2022-11-14 20:48:57.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    26027 2022-11-14 20:48:57.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.640561 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16116 2022-11-14 20:49:29.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-11-14 20:49:29.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 20:49:29.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 20:49:29.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-14 20:49:29.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-14 20:49:29.000000 mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 20:49:29.644561 mypy-boto3-managedblockchain-1.26.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-11-14 20:48:56.000000 mypy-boto3-managedblockchain-1.26.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:05.467630 mypy-boto3-managedblockchain-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-07-03 19:51:05.467630 mypy-boto3-managedblockchain-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:05.467630 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20594 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20559 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26462 2023-07-03 19:41:36.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:05.467630 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-07-03 19:51:05.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 19:51:05.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:05.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:05.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:05.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:51:05.000000 mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:05.467630 mypy-boto3-managedblockchain-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-03 19:41:35.000000 mypy-boto3-managedblockchain-1.27.0/setup.py
```

### Comparing `mypy-boto3-managedblockchain-1.26.9/LICENSE` & `mypy-boto3-managedblockchain-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-managedblockchain-1.26.9/PKG-INFO` & `mypy-boto3-managedblockchain-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain
-Version: 1.26.9
-Summary: Type annotations for boto3.ManagedBlockchain 1.26.9 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ManagedBlockchain 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
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
 
 <a id="mypy-boto3-managedblockchain"></a>
 
 # mypy-boto3-managedblockchain
 
 [![PyPI - mypy-boto3-managedblockchain](https://img.shields.io/pypi/v/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-managedblockchain?color=blue)](https://pypistats.org/packages/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,63 +336,63 @@
 
 ```python
 from mypy_boto3_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAccessorOutputTypeDef,
+    CreateMemberOutputTypeDef,
+    CreateNetworkOutputTypeDef,
+    CreateNodeOutputTypeDef,
+    CreateProposalOutputTypeDef,
     DeleteAccessorInputRequestTypeDef,
     DeleteMemberInputRequestTypeDef,
     DeleteNodeInputRequestTypeDef,
     GetAccessorInputRequestTypeDef,
     GetMemberInputRequestTypeDef,
     GetNetworkInputRequestTypeDef,
     GetNodeInputRequestTypeDef,
     GetProposalInputRequestTypeDef,
     NetworkSummaryTypeDef,
     InviteActionTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccessorsInputListAccessorsPaginateTypeDef,
     ListAccessorsInputRequestTypeDef,
     ListInvitationsInputRequestTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
     ListNetworksInputRequestTypeDef,
     ListNodesInputRequestTypeDef,
     NodeSummaryTypeDef,
     ListProposalVotesInputRequestTypeDef,
     VoteSummaryTypeDef,
     ListProposalsInputRequestTypeDef,
     ProposalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LogConfigurationTypeDef,
     MemberFabricAttributesTypeDef,
     MemberFabricConfigurationTypeDef,
     NetworkEthereumAttributesTypeDef,
     NetworkFabricAttributesTypeDef,
     NetworkFabricConfigurationTypeDef,
     NodeEthereumAttributesTypeDef,
     NodeFabricAttributesTypeDef,
+    PaginatorConfigTypeDef,
     RemoveActionTypeDef,
     RejectInvitationInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VoteOnProposalInputRequestTypeDef,
-    VotingPolicyTypeDef,
-    CreateAccessorOutputTypeDef,
-    CreateMemberOutputTypeDef,
-    CreateNetworkOutputTypeDef,
-    CreateNodeOutputTypeDef,
-    CreateProposalOutputTypeDef,
-    GetAccessorOutputTypeDef,
     ListAccessorsOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    GetAccessorOutputTypeDef,
+    VotingPolicyTypeDef,
     InvitationTypeDef,
     ListNetworksOutputTypeDef,
-    ListAccessorsInputListAccessorsPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListNodesOutputTypeDef,
     ListProposalVotesOutputTypeDef,
     ListProposalsOutputTypeDef,
     LogConfigurationsTypeDef,
     MemberFrameworkAttributesTypeDef,
     MemberFrameworkConfigurationTypeDef,
@@ -430,42 +431,42 @@
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

### Comparing `mypy-boto3-managedblockchain-1.26.9/README.md` & `mypy-boto3-managedblockchain-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-managedblockchain"></a>
 
 # mypy-boto3-managedblockchain
 
 [![PyPI - mypy-boto3-managedblockchain](https://img.shields.io/pypi/v/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-managedblockchain?color=blue)](https://pypistats.org/packages/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,63 +304,63 @@
 
 ```python
 from mypy_boto3_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAccessorOutputTypeDef,
+    CreateMemberOutputTypeDef,
+    CreateNetworkOutputTypeDef,
+    CreateNodeOutputTypeDef,
+    CreateProposalOutputTypeDef,
     DeleteAccessorInputRequestTypeDef,
     DeleteMemberInputRequestTypeDef,
     DeleteNodeInputRequestTypeDef,
     GetAccessorInputRequestTypeDef,
     GetMemberInputRequestTypeDef,
     GetNetworkInputRequestTypeDef,
     GetNodeInputRequestTypeDef,
     GetProposalInputRequestTypeDef,
     NetworkSummaryTypeDef,
     InviteActionTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccessorsInputListAccessorsPaginateTypeDef,
     ListAccessorsInputRequestTypeDef,
     ListInvitationsInputRequestTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
     ListNetworksInputRequestTypeDef,
     ListNodesInputRequestTypeDef,
     NodeSummaryTypeDef,
     ListProposalVotesInputRequestTypeDef,
     VoteSummaryTypeDef,
     ListProposalsInputRequestTypeDef,
     ProposalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LogConfigurationTypeDef,
     MemberFabricAttributesTypeDef,
     MemberFabricConfigurationTypeDef,
     NetworkEthereumAttributesTypeDef,
     NetworkFabricAttributesTypeDef,
     NetworkFabricConfigurationTypeDef,
     NodeEthereumAttributesTypeDef,
     NodeFabricAttributesTypeDef,
+    PaginatorConfigTypeDef,
     RemoveActionTypeDef,
     RejectInvitationInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VoteOnProposalInputRequestTypeDef,
-    VotingPolicyTypeDef,
-    CreateAccessorOutputTypeDef,
-    CreateMemberOutputTypeDef,
-    CreateNetworkOutputTypeDef,
-    CreateNodeOutputTypeDef,
-    CreateProposalOutputTypeDef,
-    GetAccessorOutputTypeDef,
     ListAccessorsOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    GetAccessorOutputTypeDef,
+    VotingPolicyTypeDef,
     InvitationTypeDef,
     ListNetworksOutputTypeDef,
-    ListAccessorsInputListAccessorsPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListNodesOutputTypeDef,
     ListProposalVotesOutputTypeDef,
     ListProposalsOutputTypeDef,
     LogConfigurationsTypeDef,
     MemberFrameworkAttributesTypeDef,
     MemberFrameworkConfigurationTypeDef,
@@ -399,42 +399,42 @@
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

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/__init__.py` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/__init__.pyi` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/__main__.py` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedBlockchain 1.26.9\nVersion:         1.26.9\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.ManagedBlockchain 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.9")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/client.py` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,40 +55,36 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ManagedBlockchainClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     IllegalActionException: Type[BotocoreClientError]
     InternalServiceErrorException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceLimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceNotReadyException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
-
 class ManagedBlockchainClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/)
     """
 
     meta: ClientMeta
@@ -97,56 +93,55 @@
     def exceptions(self) -> Exceptions:
         """
         ManagedBlockchainClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#close)
         """
-
     def create_accessor(
-        self, *, ClientRequestToken: str, AccessorType: Literal["BILLING_TOKEN"]
+        self,
+        *,
+        ClientRequestToken: str,
+        AccessorType: Literal["BILLING_TOKEN"],
+        Tags: Mapping[str, str] = ...
     ) -> CreateAccessorOutputTypeDef:
         """
-        .
+        Creates a new accessor for use with Managed Blockchain Ethereum nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_accessor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_accessor)
         """
-
     def create_member(
         self,
         *,
         ClientRequestToken: str,
         InvitationId: str,
         NetworkId: str,
         MemberConfiguration: MemberConfigurationTypeDef
     ) -> CreateMemberOutputTypeDef:
         """
         Creates a member within a Managed Blockchain network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_member)
         """
-
     def create_network(
         self,
         *,
         ClientRequestToken: str,
         Name: str,
         Framework: FrameworkType,
         FrameworkVersion: str,
@@ -158,15 +153,14 @@
     ) -> CreateNetworkOutputTypeDef:
         """
         Creates a new blockchain network using Amazon Managed Blockchain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_network)
         """
-
     def create_node(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         NodeConfiguration: NodeConfigurationTypeDef,
         MemberId: str = ...,
@@ -174,15 +168,14 @@
     ) -> CreateNodeOutputTypeDef:
         """
         Creates a node on the specified blockchain network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_node)
         """
-
     def create_proposal(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         MemberId: str,
         Actions: ProposalActionsTypeDef,
@@ -192,113 +185,101 @@
         """
         Creates a proposal for a change to the network that other members of the network
         can vote on, for example, a proposal to add a new member to the network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_proposal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_proposal)
         """
-
     def delete_accessor(self, *, AccessorId: str) -> Dict[str, Any]:
         """
-        .
+        Deletes an accessor that your Amazon Web Services account owns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.delete_accessor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#delete_accessor)
         """
-
     def delete_member(self, *, NetworkId: str, MemberId: str) -> Dict[str, Any]:
         """
         Deletes a member.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.delete_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#delete_member)
         """
-
     def delete_node(self, *, NetworkId: str, NodeId: str, MemberId: str = ...) -> Dict[str, Any]:
         """
         Deletes a node that your Amazon Web Services account owns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.delete_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#delete_node)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#generate_presigned_url)
         """
-
     def get_accessor(self, *, AccessorId: str) -> GetAccessorOutputTypeDef:
         """
-        .
+        Returns detailed information about an accessor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_accessor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_accessor)
         """
-
     def get_member(self, *, NetworkId: str, MemberId: str) -> GetMemberOutputTypeDef:
         """
         Returns detailed information about a member.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_member)
         """
-
     def get_network(self, *, NetworkId: str) -> GetNetworkOutputTypeDef:
         """
         Returns detailed information about a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_network)
         """
-
     def get_node(self, *, NetworkId: str, NodeId: str, MemberId: str = ...) -> GetNodeOutputTypeDef:
         """
         Returns detailed information about a node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_node)
         """
-
     def get_proposal(self, *, NetworkId: str, ProposalId: str) -> GetProposalOutputTypeDef:
         """
         Returns detailed information about a proposal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_proposal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_proposal)
         """
-
     def list_accessors(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAccessorsOutputTypeDef:
         """
-        .
+        Returns a list of the accessors and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_accessors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_accessors)
         """
-
     def list_invitations(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInvitationsOutputTypeDef:
         """
         Returns a list of all invitations for the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_invitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_invitations)
         """
-
     def list_members(
         self,
         *,
         NetworkId: str,
         Name: str = ...,
         Status: MemberStatusType = ...,
         IsOwned: bool = ...,
@@ -308,15 +289,14 @@
         """
         Returns a list of the members in a network and properties of their
         configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_members)
         """
-
     def list_networks(
         self,
         *,
         Name: str = ...,
         Framework: FrameworkType = ...,
         Status: NetworkStatusType = ...,
         MaxResults: int = ...,
@@ -325,15 +305,14 @@
         """
         Returns information about the networks in which the current Amazon Web Services
         account participates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_networks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_networks)
         """
-
     def list_nodes(
         self,
         *,
         NetworkId: str,
         MemberId: str = ...,
         Status: NodeStatusType = ...,
         MaxResults: int = ...,
@@ -341,106 +320,96 @@
     ) -> ListNodesOutputTypeDef:
         """
         Returns information about the nodes within a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_nodes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_nodes)
         """
-
     def list_proposal_votes(
         self, *, NetworkId: str, ProposalId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListProposalVotesOutputTypeDef:
         """
         Returns the list of votes for a specified proposal, including the value of each
         vote and the unique identifier of the member that cast the vote.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_proposal_votes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_proposal_votes)
         """
-
     def list_proposals(
         self, *, NetworkId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListProposalsOutputTypeDef:
         """
         Returns a list of proposals for the network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_proposals)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_proposals)
         """
-
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_tags_for_resource)
         """
-
     def reject_invitation(self, *, InvitationId: str) -> Dict[str, Any]:
         """
         Rejects an invitation to join a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.reject_invitation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#reject_invitation)
         """
-
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds or overwrites the specified tags for the specified Amazon Managed
         Blockchain resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the specified tags from the Amazon Managed Blockchain resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#untag_resource)
         """
-
     def update_member(
         self,
         *,
         NetworkId: str,
         MemberId: str,
         LogPublishingConfiguration: MemberLogPublishingConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a member configuration with new parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#update_member)
         """
-
     def update_node(
         self,
         *,
         NetworkId: str,
         NodeId: str,
         MemberId: str = ...,
         LogPublishingConfiguration: NodeLogPublishingConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a node configuration with new parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#update_node)
         """
-
     def vote_on_proposal(
         self, *, NetworkId: str, ProposalId: str, VoterMemberId: str, Vote: VoteValueType
     ) -> Dict[str, Any]:
         """
         Casts a vote for a specified `ProposalId` on behalf of a member.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.vote_on_proposal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#vote_on_proposal)
         """
-
     def get_paginator(self, operation_name: Literal["list_accessors"]) -> ListAccessorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/client.pyi` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,36 +55,40 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("ManagedBlockchainClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     IllegalActionException: Type[BotocoreClientError]
     InternalServiceErrorException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceLimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceNotReadyException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
+
 class ManagedBlockchainClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/)
     """
 
     meta: ClientMeta
@@ -93,51 +97,60 @@
     def exceptions(self) -> Exceptions:
         """
         ManagedBlockchainClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#close)
         """
+
     def create_accessor(
-        self, *, ClientRequestToken: str, AccessorType: Literal["BILLING_TOKEN"]
+        self,
+        *,
+        ClientRequestToken: str,
+        AccessorType: Literal["BILLING_TOKEN"],
+        Tags: Mapping[str, str] = ...
     ) -> CreateAccessorOutputTypeDef:
         """
-        .
+        Creates a new accessor for use with Managed Blockchain Ethereum nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_accessor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_accessor)
         """
+
     def create_member(
         self,
         *,
         ClientRequestToken: str,
         InvitationId: str,
         NetworkId: str,
         MemberConfiguration: MemberConfigurationTypeDef
     ) -> CreateMemberOutputTypeDef:
         """
         Creates a member within a Managed Blockchain network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_member)
         """
+
     def create_network(
         self,
         *,
         ClientRequestToken: str,
         Name: str,
         Framework: FrameworkType,
         FrameworkVersion: str,
@@ -149,14 +162,15 @@
     ) -> CreateNetworkOutputTypeDef:
         """
         Creates a new blockchain network using Amazon Managed Blockchain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_network)
         """
+
     def create_node(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         NodeConfiguration: NodeConfigurationTypeDef,
         MemberId: str = ...,
@@ -164,14 +178,15 @@
     ) -> CreateNodeOutputTypeDef:
         """
         Creates a node on the specified blockchain network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_node)
         """
+
     def create_proposal(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         MemberId: str,
         Actions: ProposalActionsTypeDef,
@@ -181,101 +196,113 @@
         """
         Creates a proposal for a change to the network that other members of the network
         can vote on, for example, a proposal to add a new member to the network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_proposal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_proposal)
         """
+
     def delete_accessor(self, *, AccessorId: str) -> Dict[str, Any]:
         """
-        .
+        Deletes an accessor that your Amazon Web Services account owns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.delete_accessor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#delete_accessor)
         """
+
     def delete_member(self, *, NetworkId: str, MemberId: str) -> Dict[str, Any]:
         """
         Deletes a member.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.delete_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#delete_member)
         """
+
     def delete_node(self, *, NetworkId: str, NodeId: str, MemberId: str = ...) -> Dict[str, Any]:
         """
         Deletes a node that your Amazon Web Services account owns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.delete_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#delete_node)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#generate_presigned_url)
         """
+
     def get_accessor(self, *, AccessorId: str) -> GetAccessorOutputTypeDef:
         """
-        .
+        Returns detailed information about an accessor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_accessor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_accessor)
         """
+
     def get_member(self, *, NetworkId: str, MemberId: str) -> GetMemberOutputTypeDef:
         """
         Returns detailed information about a member.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_member)
         """
+
     def get_network(self, *, NetworkId: str) -> GetNetworkOutputTypeDef:
         """
         Returns detailed information about a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_network)
         """
+
     def get_node(self, *, NetworkId: str, NodeId: str, MemberId: str = ...) -> GetNodeOutputTypeDef:
         """
         Returns detailed information about a node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_node)
         """
+
     def get_proposal(self, *, NetworkId: str, ProposalId: str) -> GetProposalOutputTypeDef:
         """
         Returns detailed information about a proposal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_proposal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_proposal)
         """
+
     def list_accessors(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAccessorsOutputTypeDef:
         """
-        .
+        Returns a list of the accessors and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_accessors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_accessors)
         """
+
     def list_invitations(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInvitationsOutputTypeDef:
         """
         Returns a list of all invitations for the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_invitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_invitations)
         """
+
     def list_members(
         self,
         *,
         NetworkId: str,
         Name: str = ...,
         Status: MemberStatusType = ...,
         IsOwned: bool = ...,
@@ -285,14 +312,15 @@
         """
         Returns a list of the members in a network and properties of their
         configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_members)
         """
+
     def list_networks(
         self,
         *,
         Name: str = ...,
         Framework: FrameworkType = ...,
         Status: NetworkStatusType = ...,
         MaxResults: int = ...,
@@ -301,14 +329,15 @@
         """
         Returns information about the networks in which the current Amazon Web Services
         account participates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_networks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_networks)
         """
+
     def list_nodes(
         self,
         *,
         NetworkId: str,
         MemberId: str = ...,
         Status: NodeStatusType = ...,
         MaxResults: int = ...,
@@ -316,96 +345,106 @@
     ) -> ListNodesOutputTypeDef:
         """
         Returns information about the nodes within a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_nodes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_nodes)
         """
+
     def list_proposal_votes(
         self, *, NetworkId: str, ProposalId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListProposalVotesOutputTypeDef:
         """
         Returns the list of votes for a specified proposal, including the value of each
         vote and the unique identifier of the member that cast the vote.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_proposal_votes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_proposal_votes)
         """
+
     def list_proposals(
         self, *, NetworkId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListProposalsOutputTypeDef:
         """
         Returns a list of proposals for the network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_proposals)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_proposals)
         """
+
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_tags_for_resource)
         """
+
     def reject_invitation(self, *, InvitationId: str) -> Dict[str, Any]:
         """
         Rejects an invitation to join a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.reject_invitation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#reject_invitation)
         """
+
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds or overwrites the specified tags for the specified Amazon Managed
         Blockchain resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the specified tags from the Amazon Managed Blockchain resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#untag_resource)
         """
+
     def update_member(
         self,
         *,
         NetworkId: str,
         MemberId: str,
         LogPublishingConfiguration: MemberLogPublishingConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a member configuration with new parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#update_member)
         """
+
     def update_node(
         self,
         *,
         NetworkId: str,
         NodeId: str,
         MemberId: str = ...,
         LogPublishingConfiguration: NodeLogPublishingConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a node configuration with new parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#update_node)
         """
+
     def vote_on_proposal(
         self, *, NetworkId: str, ProposalId: str, VoterMemberId: str, Vote: VoteValueType
     ) -> Dict[str, Any]:
         """
         Casts a vote for a specified `ProposalId` on behalf of a member.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.vote_on_proposal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#vote_on_proposal)
         """
+
     def get_paginator(self, operation_name: Literal["list_accessors"]) -> ListAccessorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/literals.py` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,23 +84,25 @@
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
@@ -110,30 +112,35 @@
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
@@ -159,14 +166,15 @@
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
@@ -211,51 +219,57 @@
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
@@ -268,14 +282,15 @@
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
@@ -287,28 +302,35 @@
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
@@ -336,56 +358,64 @@
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

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/literals.pyi` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -82,23 +82,25 @@
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
@@ -108,30 +110,35 @@
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
@@ -157,14 +164,15 @@
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
@@ -209,51 +217,57 @@
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
@@ -266,14 +280,15 @@
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
@@ -285,28 +300,35 @@
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
@@ -334,56 +356,64 @@
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

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/paginator.py` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListAccessorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/paginators/#listaccessorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccessorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/paginators/#listaccessorspaginator)
         """
```

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/paginator.pyi` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListAccessorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/paginators/#listaccessorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccessorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/paginators/#listaccessorspaginator)
         """
```

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/type_defs.py` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,63 +40,63 @@
 
 
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAccessorOutputTypeDef",
+    "CreateMemberOutputTypeDef",
+    "CreateNetworkOutputTypeDef",
+    "CreateNodeOutputTypeDef",
+    "CreateProposalOutputTypeDef",
     "DeleteAccessorInputRequestTypeDef",
     "DeleteMemberInputRequestTypeDef",
     "DeleteNodeInputRequestTypeDef",
     "GetAccessorInputRequestTypeDef",
     "GetMemberInputRequestTypeDef",
     "GetNetworkInputRequestTypeDef",
     "GetNodeInputRequestTypeDef",
     "GetProposalInputRequestTypeDef",
     "NetworkSummaryTypeDef",
     "InviteActionTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccessorsInputListAccessorsPaginateTypeDef",
     "ListAccessorsInputRequestTypeDef",
     "ListInvitationsInputRequestTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
     "ListNetworksInputRequestTypeDef",
     "ListNodesInputRequestTypeDef",
     "NodeSummaryTypeDef",
     "ListProposalVotesInputRequestTypeDef",
     "VoteSummaryTypeDef",
     "ListProposalsInputRequestTypeDef",
     "ProposalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "LogConfigurationTypeDef",
     "MemberFabricAttributesTypeDef",
     "MemberFabricConfigurationTypeDef",
     "NetworkEthereumAttributesTypeDef",
     "NetworkFabricAttributesTypeDef",
     "NetworkFabricConfigurationTypeDef",
     "NodeEthereumAttributesTypeDef",
     "NodeFabricAttributesTypeDef",
+    "PaginatorConfigTypeDef",
     "RemoveActionTypeDef",
     "RejectInvitationInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VoteOnProposalInputRequestTypeDef",
-    "VotingPolicyTypeDef",
-    "CreateAccessorOutputTypeDef",
-    "CreateMemberOutputTypeDef",
-    "CreateNetworkOutputTypeDef",
-    "CreateNodeOutputTypeDef",
-    "CreateProposalOutputTypeDef",
-    "GetAccessorOutputTypeDef",
     "ListAccessorsOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "GetAccessorOutputTypeDef",
+    "VotingPolicyTypeDef",
     "InvitationTypeDef",
     "ListNetworksOutputTypeDef",
-    "ListAccessorsInputListAccessorsPaginateTypeDef",
     "ListMembersOutputTypeDef",
     "ListNodesOutputTypeDef",
     "ListProposalVotesOutputTypeDef",
     "ListProposalsOutputTypeDef",
     "LogConfigurationsTypeDef",
     "MemberFrameworkAttributesTypeDef",
     "MemberFrameworkConfigurationTypeDef",
@@ -144,44 +144,90 @@
     {
         "Id": str,
         "Type": Literal["BILLING_TOKEN"],
         "BillingToken": str,
         "Status": AccessorStatusType,
         "CreationDate": datetime,
         "Arn": str,
+        "Tags": Dict[str, str],
     },
     total=False,
 )
 
 ApprovalThresholdPolicyTypeDef = TypedDict(
     "ApprovalThresholdPolicyTypeDef",
     {
         "ThresholdPercentage": int,
         "ProposalDurationInHours": int,
         "ThresholdComparator": ThresholdComparatorType,
     },
     total=False,
 )
 
-CreateAccessorInputRequestTypeDef = TypedDict(
-    "CreateAccessorInputRequestTypeDef",
+_RequiredCreateAccessorInputRequestTypeDef = TypedDict(
+    "_RequiredCreateAccessorInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "AccessorType": Literal["BILLING_TOKEN"],
     },
 )
+_OptionalCreateAccessorInputRequestTypeDef = TypedDict(
+    "_OptionalCreateAccessorInputRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+class CreateAccessorInputRequestTypeDef(
+    _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
+):
+    pass
+
+
+CreateAccessorOutputTypeDef = TypedDict(
+    "CreateAccessorOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AccessorId": str,
+        "BillingToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateMemberOutputTypeDef = TypedDict(
+    "CreateMemberOutputTypeDef",
+    {
+        "MemberId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateNetworkOutputTypeDef = TypedDict(
+    "CreateNetworkOutputTypeDef",
+    {
+        "NetworkId": str,
+        "MemberId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateNodeOutputTypeDef = TypedDict(
+    "CreateNodeOutputTypeDef",
+    {
+        "NodeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateProposalOutputTypeDef = TypedDict(
+    "CreateProposalOutputTypeDef",
+    {
+        "ProposalId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAccessorInputRequestTypeDef = TypedDict(
     "DeleteAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
@@ -288,20 +334,18 @@
 InviteActionTypeDef = TypedDict(
     "InviteActionTypeDef",
     {
         "Principal": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
+    "ListAccessorsInputListAccessorsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAccessorsInputRequestTypeDef = TypedDict(
     "ListAccessorsInputRequestTypeDef",
     {
@@ -481,14 +525,22 @@
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
 LogConfigurationTypeDef = TypedDict(
     "LogConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -548,28 +600,49 @@
     {
         "PeerEndpoint": str,
         "PeerEventEndpoint": str,
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
 RemoveActionTypeDef = TypedDict(
     "RemoveActionTypeDef",
     {
         "MemberId": str,
     },
 )
 
 RejectInvitationInputRequestTypeDef = TypedDict(
     "RejectInvitationInputRequestTypeDef",
     {
         "InvitationId": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -588,87 +661,37 @@
         "NetworkId": str,
         "ProposalId": str,
         "VoterMemberId": str,
         "Vote": VoteValueType,
     },
 )
 
-VotingPolicyTypeDef = TypedDict(
-    "VotingPolicyTypeDef",
-    {
-        "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
-    },
-    total=False,
-)
-
-CreateAccessorOutputTypeDef = TypedDict(
-    "CreateAccessorOutputTypeDef",
-    {
-        "AccessorId": str,
-        "BillingToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMemberOutputTypeDef = TypedDict(
-    "CreateMemberOutputTypeDef",
-    {
-        "MemberId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateNetworkOutputTypeDef = TypedDict(
-    "CreateNetworkOutputTypeDef",
-    {
-        "NetworkId": str,
-        "MemberId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateNodeOutputTypeDef = TypedDict(
-    "CreateNodeOutputTypeDef",
-    {
-        "NodeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProposalOutputTypeDef = TypedDict(
-    "CreateProposalOutputTypeDef",
+ListAccessorsOutputTypeDef = TypedDict(
+    "ListAccessorsOutputTypeDef",
     {
-        "ProposalId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Accessors": List[AccessorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccessorOutputTypeDef = TypedDict(
     "GetAccessorOutputTypeDef",
     {
         "Accessor": AccessorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAccessorsOutputTypeDef = TypedDict(
-    "ListAccessorsOutputTypeDef",
-    {
-        "Accessors": List[AccessorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+VotingPolicyTypeDef = TypedDict(
+    "VotingPolicyTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
     },
+    total=False,
 )
 
 InvitationTypeDef = TypedDict(
     "InvitationTypeDef",
     {
         "InvitationId": str,
         "CreationDate": datetime,
@@ -681,59 +704,51 @@
 )
 
 ListNetworksOutputTypeDef = TypedDict(
     "ListNetworksOutputTypeDef",
     {
         "Networks": List[NetworkSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
-    "ListAccessorsInputListAccessorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "Members": List[MemberSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNodesOutputTypeDef = TypedDict(
     "ListNodesOutputTypeDef",
     {
         "Nodes": List[NodeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProposalVotesOutputTypeDef = TypedDict(
     "ListProposalVotesOutputTypeDef",
     {
         "ProposalVotes": List[VoteSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProposalsOutputTypeDef = TypedDict(
     "ListProposalsOutputTypeDef",
     {
         "Proposals": List[ProposalSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LogConfigurationsTypeDef = TypedDict(
     "LogConfigurationsTypeDef",
     {
         "Cloudwatch": LogConfigurationTypeDef,
@@ -793,15 +808,15 @@
 )
 
 ListInvitationsOutputTypeDef = TypedDict(
     "ListInvitationsOutputTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MemberFabricLogPublishingConfigurationTypeDef = TypedDict(
     "MemberFabricLogPublishingConfigurationTypeDef",
     {
         "CaLogs": LogConfigurationsTypeDef,
@@ -899,23 +914,23 @@
     total=False,
 )
 
 GetNetworkOutputTypeDef = TypedDict(
     "GetNetworkOutputTypeDef",
     {
         "Network": NetworkTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProposalOutputTypeDef = TypedDict(
     "GetProposalOutputTypeDef",
     {
         "Proposal": ProposalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMemberConfigurationTypeDef = TypedDict(
     "_RequiredMemberConfigurationTypeDef",
     {
         "Name": str,
@@ -1084,15 +1099,15 @@
     pass
 
 
 GetMemberOutputTypeDef = TypedDict(
     "GetMemberOutputTypeDef",
     {
         "Member": MemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateNodeInputRequestTypeDef",
     {
         "ClientRequestToken": str,
@@ -1116,10 +1131,10 @@
     pass
 
 
 GetNodeOutputTypeDef = TypedDict(
     "GetNodeOutputTypeDef",
     {
         "Node": NodeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain/type_defs.pyi` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -39,63 +39,63 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAccessorOutputTypeDef",
+    "CreateMemberOutputTypeDef",
+    "CreateNetworkOutputTypeDef",
+    "CreateNodeOutputTypeDef",
+    "CreateProposalOutputTypeDef",
     "DeleteAccessorInputRequestTypeDef",
     "DeleteMemberInputRequestTypeDef",
     "DeleteNodeInputRequestTypeDef",
     "GetAccessorInputRequestTypeDef",
     "GetMemberInputRequestTypeDef",
     "GetNetworkInputRequestTypeDef",
     "GetNodeInputRequestTypeDef",
     "GetProposalInputRequestTypeDef",
     "NetworkSummaryTypeDef",
     "InviteActionTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccessorsInputListAccessorsPaginateTypeDef",
     "ListAccessorsInputRequestTypeDef",
     "ListInvitationsInputRequestTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
     "ListNetworksInputRequestTypeDef",
     "ListNodesInputRequestTypeDef",
     "NodeSummaryTypeDef",
     "ListProposalVotesInputRequestTypeDef",
     "VoteSummaryTypeDef",
     "ListProposalsInputRequestTypeDef",
     "ProposalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "LogConfigurationTypeDef",
     "MemberFabricAttributesTypeDef",
     "MemberFabricConfigurationTypeDef",
     "NetworkEthereumAttributesTypeDef",
     "NetworkFabricAttributesTypeDef",
     "NetworkFabricConfigurationTypeDef",
     "NodeEthereumAttributesTypeDef",
     "NodeFabricAttributesTypeDef",
+    "PaginatorConfigTypeDef",
     "RemoveActionTypeDef",
     "RejectInvitationInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VoteOnProposalInputRequestTypeDef",
-    "VotingPolicyTypeDef",
-    "CreateAccessorOutputTypeDef",
-    "CreateMemberOutputTypeDef",
-    "CreateNetworkOutputTypeDef",
-    "CreateNodeOutputTypeDef",
-    "CreateProposalOutputTypeDef",
-    "GetAccessorOutputTypeDef",
     "ListAccessorsOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "GetAccessorOutputTypeDef",
+    "VotingPolicyTypeDef",
     "InvitationTypeDef",
     "ListNetworksOutputTypeDef",
-    "ListAccessorsInputListAccessorsPaginateTypeDef",
     "ListMembersOutputTypeDef",
     "ListNodesOutputTypeDef",
     "ListProposalVotesOutputTypeDef",
     "ListProposalsOutputTypeDef",
     "LogConfigurationsTypeDef",
     "MemberFrameworkAttributesTypeDef",
     "MemberFrameworkConfigurationTypeDef",
@@ -143,44 +143,88 @@
     {
         "Id": str,
         "Type": Literal["BILLING_TOKEN"],
         "BillingToken": str,
         "Status": AccessorStatusType,
         "CreationDate": datetime,
         "Arn": str,
+        "Tags": Dict[str, str],
     },
     total=False,
 )
 
 ApprovalThresholdPolicyTypeDef = TypedDict(
     "ApprovalThresholdPolicyTypeDef",
     {
         "ThresholdPercentage": int,
         "ProposalDurationInHours": int,
         "ThresholdComparator": ThresholdComparatorType,
     },
     total=False,
 )
 
-CreateAccessorInputRequestTypeDef = TypedDict(
-    "CreateAccessorInputRequestTypeDef",
+_RequiredCreateAccessorInputRequestTypeDef = TypedDict(
+    "_RequiredCreateAccessorInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "AccessorType": Literal["BILLING_TOKEN"],
     },
 )
+_OptionalCreateAccessorInputRequestTypeDef = TypedDict(
+    "_OptionalCreateAccessorInputRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+class CreateAccessorInputRequestTypeDef(
+    _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
+):
+    pass
+
+CreateAccessorOutputTypeDef = TypedDict(
+    "CreateAccessorOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AccessorId": str,
+        "BillingToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateMemberOutputTypeDef = TypedDict(
+    "CreateMemberOutputTypeDef",
+    {
+        "MemberId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateNetworkOutputTypeDef = TypedDict(
+    "CreateNetworkOutputTypeDef",
+    {
+        "NetworkId": str,
+        "MemberId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateNodeOutputTypeDef = TypedDict(
+    "CreateNodeOutputTypeDef",
+    {
+        "NodeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateProposalOutputTypeDef = TypedDict(
+    "CreateProposalOutputTypeDef",
+    {
+        "ProposalId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAccessorInputRequestTypeDef = TypedDict(
     "DeleteAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
@@ -283,20 +327,18 @@
 InviteActionTypeDef = TypedDict(
     "InviteActionTypeDef",
     {
         "Principal": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
+    "ListAccessorsInputListAccessorsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAccessorsInputRequestTypeDef = TypedDict(
     "ListAccessorsInputRequestTypeDef",
     {
@@ -468,14 +510,22 @@
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
 LogConfigurationTypeDef = TypedDict(
     "LogConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -535,28 +585,49 @@
     {
         "PeerEndpoint": str,
         "PeerEventEndpoint": str,
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
 RemoveActionTypeDef = TypedDict(
     "RemoveActionTypeDef",
     {
         "MemberId": str,
     },
 )
 
 RejectInvitationInputRequestTypeDef = TypedDict(
     "RejectInvitationInputRequestTypeDef",
     {
         "InvitationId": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -575,87 +646,37 @@
         "NetworkId": str,
         "ProposalId": str,
         "VoterMemberId": str,
         "Vote": VoteValueType,
     },
 )
 
-VotingPolicyTypeDef = TypedDict(
-    "VotingPolicyTypeDef",
-    {
-        "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
-    },
-    total=False,
-)
-
-CreateAccessorOutputTypeDef = TypedDict(
-    "CreateAccessorOutputTypeDef",
-    {
-        "AccessorId": str,
-        "BillingToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMemberOutputTypeDef = TypedDict(
-    "CreateMemberOutputTypeDef",
-    {
-        "MemberId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateNetworkOutputTypeDef = TypedDict(
-    "CreateNetworkOutputTypeDef",
-    {
-        "NetworkId": str,
-        "MemberId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateNodeOutputTypeDef = TypedDict(
-    "CreateNodeOutputTypeDef",
-    {
-        "NodeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProposalOutputTypeDef = TypedDict(
-    "CreateProposalOutputTypeDef",
+ListAccessorsOutputTypeDef = TypedDict(
+    "ListAccessorsOutputTypeDef",
     {
-        "ProposalId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Accessors": List[AccessorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccessorOutputTypeDef = TypedDict(
     "GetAccessorOutputTypeDef",
     {
         "Accessor": AccessorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAccessorsOutputTypeDef = TypedDict(
-    "ListAccessorsOutputTypeDef",
-    {
-        "Accessors": List[AccessorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+VotingPolicyTypeDef = TypedDict(
+    "VotingPolicyTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
     },
+    total=False,
 )
 
 InvitationTypeDef = TypedDict(
     "InvitationTypeDef",
     {
         "InvitationId": str,
         "CreationDate": datetime,
@@ -668,59 +689,51 @@
 )
 
 ListNetworksOutputTypeDef = TypedDict(
     "ListNetworksOutputTypeDef",
     {
         "Networks": List[NetworkSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
-    "ListAccessorsInputListAccessorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "Members": List[MemberSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNodesOutputTypeDef = TypedDict(
     "ListNodesOutputTypeDef",
     {
         "Nodes": List[NodeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProposalVotesOutputTypeDef = TypedDict(
     "ListProposalVotesOutputTypeDef",
     {
         "ProposalVotes": List[VoteSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProposalsOutputTypeDef = TypedDict(
     "ListProposalsOutputTypeDef",
     {
         "Proposals": List[ProposalSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LogConfigurationsTypeDef = TypedDict(
     "LogConfigurationsTypeDef",
     {
         "Cloudwatch": LogConfigurationTypeDef,
@@ -780,15 +793,15 @@
 )
 
 ListInvitationsOutputTypeDef = TypedDict(
     "ListInvitationsOutputTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MemberFabricLogPublishingConfigurationTypeDef = TypedDict(
     "MemberFabricLogPublishingConfigurationTypeDef",
     {
         "CaLogs": LogConfigurationsTypeDef,
@@ -884,23 +897,23 @@
     total=False,
 )
 
 GetNetworkOutputTypeDef = TypedDict(
     "GetNetworkOutputTypeDef",
     {
         "Network": NetworkTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProposalOutputTypeDef = TypedDict(
     "GetProposalOutputTypeDef",
     {
         "Proposal": ProposalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMemberConfigurationTypeDef = TypedDict(
     "_RequiredMemberConfigurationTypeDef",
     {
         "Name": str,
@@ -1059,15 +1072,15 @@
 ):
     pass
 
 GetMemberOutputTypeDef = TypedDict(
     "GetMemberOutputTypeDef",
     {
         "Member": MemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateNodeInputRequestTypeDef",
     {
         "ClientRequestToken": str,
@@ -1089,10 +1102,10 @@
 ):
     pass
 
 GetNodeOutputTypeDef = TypedDict(
     "GetNodeOutputTypeDef",
     {
         "Node": NodeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/PKG-INFO` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain
-Version: 1.26.9
-Summary: Type annotations for boto3.ManagedBlockchain 1.26.9 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ManagedBlockchain 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
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
 
 <a id="mypy-boto3-managedblockchain"></a>
 
 # mypy-boto3-managedblockchain
 
 [![PyPI - mypy-boto3-managedblockchain](https://img.shields.io/pypi/v/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-managedblockchain?color=blue)](https://pypistats.org/packages/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,63 +336,63 @@
 
 ```python
 from mypy_boto3_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAccessorOutputTypeDef,
+    CreateMemberOutputTypeDef,
+    CreateNetworkOutputTypeDef,
+    CreateNodeOutputTypeDef,
+    CreateProposalOutputTypeDef,
     DeleteAccessorInputRequestTypeDef,
     DeleteMemberInputRequestTypeDef,
     DeleteNodeInputRequestTypeDef,
     GetAccessorInputRequestTypeDef,
     GetMemberInputRequestTypeDef,
     GetNetworkInputRequestTypeDef,
     GetNodeInputRequestTypeDef,
     GetProposalInputRequestTypeDef,
     NetworkSummaryTypeDef,
     InviteActionTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccessorsInputListAccessorsPaginateTypeDef,
     ListAccessorsInputRequestTypeDef,
     ListInvitationsInputRequestTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
     ListNetworksInputRequestTypeDef,
     ListNodesInputRequestTypeDef,
     NodeSummaryTypeDef,
     ListProposalVotesInputRequestTypeDef,
     VoteSummaryTypeDef,
     ListProposalsInputRequestTypeDef,
     ProposalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LogConfigurationTypeDef,
     MemberFabricAttributesTypeDef,
     MemberFabricConfigurationTypeDef,
     NetworkEthereumAttributesTypeDef,
     NetworkFabricAttributesTypeDef,
     NetworkFabricConfigurationTypeDef,
     NodeEthereumAttributesTypeDef,
     NodeFabricAttributesTypeDef,
+    PaginatorConfigTypeDef,
     RemoveActionTypeDef,
     RejectInvitationInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VoteOnProposalInputRequestTypeDef,
-    VotingPolicyTypeDef,
-    CreateAccessorOutputTypeDef,
-    CreateMemberOutputTypeDef,
-    CreateNetworkOutputTypeDef,
-    CreateNodeOutputTypeDef,
-    CreateProposalOutputTypeDef,
-    GetAccessorOutputTypeDef,
     ListAccessorsOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    GetAccessorOutputTypeDef,
+    VotingPolicyTypeDef,
     InvitationTypeDef,
     ListNetworksOutputTypeDef,
-    ListAccessorsInputListAccessorsPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListNodesOutputTypeDef,
     ListProposalVotesOutputTypeDef,
     ListProposalsOutputTypeDef,
     LogConfigurationsTypeDef,
     MemberFrameworkAttributesTypeDef,
     MemberFrameworkConfigurationTypeDef,
@@ -430,42 +431,42 @@
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

### Comparing `mypy-boto3-managedblockchain-1.26.9/mypy_boto3_managedblockchain.egg-info/SOURCES.txt` & `mypy-boto3-managedblockchain-1.27.0/mypy_boto3_managedblockchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.26.9/setup.py` & `mypy-boto3-managedblockchain-1.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-managedblockchain.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-managedblockchain",
-    version="1.26.9",
+    version="1.27.0",
     packages=["mypy_boto3_managedblockchain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ManagedBlockchain 1.26.9 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.ManagedBlockchain 1.27.0 service generated with"
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
     keywords="boto3 managedblockchain type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_managedblockchain": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_managedblockchain": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/",
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


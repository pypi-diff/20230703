# Comparing `tmp/mypy-boto3-eks-1.26.31.tar.gz` & `tmp/mypy-boto3-eks-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-eks-1.26.31.tar", last modified: Thu Dec 15 20:33:05 2022, max compression
+gzip compressed data, was "mypy-boto3-eks-1.27.0.tar", last modified: Mon Jul  3 19:50:43 2023, max compression
```

## Comparing `mypy-boto3-eks-1.26.31.tar` & `mypy-boto3-eks-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:05.720165 mypy-boto3-eks-1.26.31/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-15 20:32:09.000000 mypy-boto3-eks-1.26.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20627 2022-12-15 20:33:05.712165 mypy-boto3-eks-1.26.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19156 2022-12-15 20:32:09.000000 mypy-boto3-eks-1.26.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:05.708165 mypy-boto3-eks-1.26.31/mypy_boto3_eks/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2022-12-15 20:32:09.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2022-12-15 20:32:09.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2022-12-15 20:32:09.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33061 2022-12-15 20:32:10.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33004 2022-12-15 20:32:09.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13753 2022-12-15 20:32:10.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13751 2022-12-15 20:32:10.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2022-12-15 20:32:10.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8315 2022-12-15 20:32:10.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 20:32:09.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50600 2022-12-15 20:32:11.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50527 2022-12-15 20:32:10.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-15 20:32:09.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2022-12-15 20:32:10.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2022-12-15 20:32:10.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:05.712165 mypy-boto3-eks-1.26.31/mypy_boto3_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20627 2022-12-15 20:33:05.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2022-12-15 20:33:05.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 20:33:05.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 20:33:05.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-15 20:33:05.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-15 20:33:05.000000 mypy-boto3-eks-1.26.31/mypy_boto3_eks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 20:33:05.720165 mypy-boto3-eks-1.26.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2022-12-15 20:32:09.000000 mypy-boto3-eks-1.26.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.191191 mypy-boto3-eks-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-07-03 19:50:43.191191 mypy-boto3-eks-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.191191 mypy-boto3-eks-1.27.0/mypy_boto3_eks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33061 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33004 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-03 19:37:08.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-03 19:37:08.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50680 2023-07-03 19:37:09.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50607 2023-07-03 19:37:08.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.191191 mypy-boto3-eks-1.27.0/mypy_boto3_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-07-03 19:50:43.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 19:50:43.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:43.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:43.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:43.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:43.000000 mypy-boto3-eks-1.27.0/mypy_boto3_eks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:43.191191 mypy-boto3-eks-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:37:07.000000 mypy-boto3-eks-1.27.0/setup.py
```

### Comparing `mypy-boto3-eks-1.26.31/LICENSE` & `mypy-boto3-eks-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-eks-1.26.31/PKG-INFO` & `mypy-boto3-eks-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-eks
-Version: 1.26.31
-Summary: Type annotations for boto3.EKS 1.26.31 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.EKS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-eks"></a>
 
 # mypy-boto3-eks
 
 [![PyPI - mypy-boto3-eks](https://img.shields.io/pypi/v/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-eks?color=blue)](https://pypistats.org/packages/mypy-boto3-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EKS 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[boto3.EKS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [mypy-boto3-eks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -414,15 +414,14 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_eks.type_defs import (
     AddonIssueTypeDef,
     MarketplaceInformationTypeDef,
     CompatibilityTypeDef,
-    ResponseMetadataTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     AutoScalingGroupTypeDef,
     CertificateTypeDef,
     ClusterIssueTypeDef,
     ConnectorConfigResponseTypeDef,
     KubernetesNetworkConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
@@ -440,51 +439,59 @@
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteFargateProfileRequestRequestTypeDef,
     DeleteNodegroupRequestRequestTypeDef,
     DeregisterClusterRequestRequestTypeDef,
     DescribeAddonConfigurationRequestRequestTypeDef,
+    DescribeAddonConfigurationResponseTypeDef,
     WaiterConfigTypeDef,
     DescribeAddonRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
     DescribeAddonVersionsRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
+    ListAddonsRequestListAddonsPaginateTypeDef,
     ListAddonsRequestRequestTypeDef,
+    ListAddonsResponseTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListClustersResponseTypeDef,
+    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
+    ListFargateProfilesResponseTypeDef,
+    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
+    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListNodegroupsRequestRequestTypeDef,
+    ListNodegroupsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUpdatesRequestListUpdatesPaginateTypeDef,
     ListUpdatesRequestRequestTypeDef,
+    ListUpdatesResponseTypeDef,
     LogSetupTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddonRequestRequestTypeDef,
     UpdateClusterVersionRequestRequestTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateParamTypeDef,
     AddonHealthTypeDef,
     AddonVersionInfoTypeDef,
-    DescribeAddonConfigurationResponseTypeDef,
-    ListAddonsResponseTypeDef,
-    ListClustersResponseTypeDef,
-    ListFargateProfilesResponseTypeDef,
-    ListNodegroupsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
     CreateFargateProfileRequestRequestTypeDef,
@@ -496,21 +503,14 @@
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     DescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     DescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
-    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
-    ListAddonsRequestListAddonsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
-    ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     EncryptionConfigTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
@@ -559,42 +559,42 @@
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

### Comparing `mypy-boto3-eks-1.26.31/README.md` & `mypy-boto3-eks-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-eks"></a>
 
 # mypy-boto3-eks
 
 [![PyPI - mypy-boto3-eks](https://img.shields.io/pypi/v/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-eks?color=blue)](https://pypistats.org/packages/mypy-boto3-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EKS 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[boto3.EKS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [mypy-boto3-eks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -382,15 +382,14 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_eks.type_defs import (
     AddonIssueTypeDef,
     MarketplaceInformationTypeDef,
     CompatibilityTypeDef,
-    ResponseMetadataTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     AutoScalingGroupTypeDef,
     CertificateTypeDef,
     ClusterIssueTypeDef,
     ConnectorConfigResponseTypeDef,
     KubernetesNetworkConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
@@ -408,51 +407,59 @@
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteFargateProfileRequestRequestTypeDef,
     DeleteNodegroupRequestRequestTypeDef,
     DeregisterClusterRequestRequestTypeDef,
     DescribeAddonConfigurationRequestRequestTypeDef,
+    DescribeAddonConfigurationResponseTypeDef,
     WaiterConfigTypeDef,
     DescribeAddonRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
     DescribeAddonVersionsRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
+    ListAddonsRequestListAddonsPaginateTypeDef,
     ListAddonsRequestRequestTypeDef,
+    ListAddonsResponseTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListClustersResponseTypeDef,
+    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
+    ListFargateProfilesResponseTypeDef,
+    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
+    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListNodegroupsRequestRequestTypeDef,
+    ListNodegroupsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUpdatesRequestListUpdatesPaginateTypeDef,
     ListUpdatesRequestRequestTypeDef,
+    ListUpdatesResponseTypeDef,
     LogSetupTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddonRequestRequestTypeDef,
     UpdateClusterVersionRequestRequestTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateParamTypeDef,
     AddonHealthTypeDef,
     AddonVersionInfoTypeDef,
-    DescribeAddonConfigurationResponseTypeDef,
-    ListAddonsResponseTypeDef,
-    ListClustersResponseTypeDef,
-    ListFargateProfilesResponseTypeDef,
-    ListNodegroupsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
     CreateFargateProfileRequestRequestTypeDef,
@@ -464,21 +471,14 @@
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     DescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     DescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
-    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
-    ListAddonsRequestListAddonsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
-    ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     EncryptionConfigTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
@@ -527,42 +527,42 @@
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

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/__init__.py` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/__init__.pyi` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/__main__.py` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EKS 1.26.31\nVersion:         1.26.31\nBuilder version:"
-        " 7.12.0\nDocs:           "
+        "Type annotations for boto3.EKS 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.31")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/client.py` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/client.pyi` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/literals.py` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,15 @@
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
@@ -252,31 +253,34 @@
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
@@ -355,14 +359,15 @@
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
@@ -373,34 +378,38 @@
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
@@ -413,14 +422,15 @@
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
@@ -439,16 +449,19 @@
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
@@ -528,18 +541,21 @@
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
@@ -583,21 +599,25 @@
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
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/literals.pyi` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -222,14 +222,15 @@
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
@@ -250,31 +251,34 @@
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
@@ -353,14 +357,15 @@
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
@@ -371,34 +376,38 @@
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
@@ -411,14 +420,15 @@
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
@@ -437,16 +447,19 @@
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
@@ -526,18 +539,21 @@
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
@@ -581,21 +597,25 @@
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
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/paginator.py` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -52,133 +52,124 @@
     "ListClustersPaginator",
     "ListFargateProfilesPaginator",
     "ListIdentityProviderConfigsPaginator",
     "ListNodegroupsPaginator",
     "ListUpdatesPaginator",
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
 class DescribeAddonVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#describeaddonversionspaginator)
     """
 
     def paginate(
         self,
         *,
         kubernetesVersion: str = ...,
         addonName: str = ...,
         types: Sequence[str] = ...,
         publishers: Sequence[str] = ...,
         owners: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAddonVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#describeaddonversionspaginator)
         """
 
-
 class ListAddonsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listaddonspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAddonsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listaddonspaginator)
         """
 
-
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, include: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, include: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listclusterspaginator)
         """
 
-
 class ListFargateProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listfargateprofilespaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFargateProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listfargateprofilespaginator)
         """
 
-
 class ListIdentityProviderConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listidentityproviderconfigspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIdentityProviderConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listidentityproviderconfigspaginator)
         """
 
-
 class ListNodegroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listnodegroupspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNodegroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listnodegroupspaginator)
         """
 
-
 class ListUpdatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listupdatespaginator)
     """
 
     def paginate(
         self,
         *,
         name: str,
         nodegroupName: str = ...,
         addonName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listupdatespaginator)
         """
```

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/paginator.pyi` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/paginator.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,124 +52,133 @@
     "ListClustersPaginator",
     "ListFargateProfilesPaginator",
     "ListIdentityProviderConfigsPaginator",
     "ListNodegroupsPaginator",
     "ListUpdatesPaginator",
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
 class DescribeAddonVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#describeaddonversionspaginator)
     """
 
     def paginate(
         self,
         *,
         kubernetesVersion: str = ...,
         addonName: str = ...,
         types: Sequence[str] = ...,
         publishers: Sequence[str] = ...,
         owners: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAddonVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#describeaddonversionspaginator)
         """
 
+
 class ListAddonsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listaddonspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAddonsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listaddonspaginator)
         """
 
+
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, include: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, include: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listclusterspaginator)
         """
 
+
 class ListFargateProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listfargateprofilespaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFargateProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listfargateprofilespaginator)
         """
 
+
 class ListIdentityProviderConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listidentityproviderconfigspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIdentityProviderConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listidentityproviderconfigspaginator)
         """
 
+
 class ListNodegroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listnodegroupspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNodegroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listnodegroupspaginator)
         """
 
+
 class ListUpdatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listupdatespaginator)
     """
 
     def paginate(
         self,
         *,
         name: str,
         nodegroupName: str = ...,
         addonName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listupdatespaginator)
         """
```

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/type_defs.py` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddonIssueTypeDef",
     "MarketplaceInformationTypeDef",
     "CompatibilityTypeDef",
-    "ResponseMetadataTypeDef",
     "OidcIdentityProviderConfigRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "CertificateTypeDef",
     "ClusterIssueTypeDef",
     "ConnectorConfigResponseTypeDef",
     "KubernetesNetworkConfigResponseTypeDef",
     "VpcConfigResponseTypeDef",
@@ -69,51 +68,59 @@
     "TaintTypeDef",
     "DeleteAddonRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteFargateProfileRequestRequestTypeDef",
     "DeleteNodegroupRequestRequestTypeDef",
     "DeregisterClusterRequestRequestTypeDef",
     "DescribeAddonConfigurationRequestRequestTypeDef",
+    "DescribeAddonConfigurationResponseTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAddonRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
     "DescribeAddonVersionsRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
     "ProviderTypeDef",
     "ErrorDetailTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
+    "ListAddonsRequestListAddonsPaginateTypeDef",
     "ListAddonsRequestRequestTypeDef",
+    "ListAddonsResponseTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListClustersResponseTypeDef",
+    "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
     "ListFargateProfilesRequestRequestTypeDef",
+    "ListFargateProfilesResponseTypeDef",
+    "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
     "ListIdentityProviderConfigsRequestRequestTypeDef",
+    "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
     "ListNodegroupsRequestRequestTypeDef",
+    "ListNodegroupsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "ListUpdatesRequestRequestTypeDef",
+    "ListUpdatesResponseTypeDef",
     "LogSetupTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddonRequestRequestTypeDef",
     "UpdateClusterVersionRequestRequestTypeDef",
     "UpdateLabelsPayloadTypeDef",
     "UpdateParamTypeDef",
     "AddonHealthTypeDef",
     "AddonVersionInfoTypeDef",
-    "DescribeAddonConfigurationResponseTypeDef",
-    "ListAddonsResponseTypeDef",
-    "ListClustersResponseTypeDef",
-    "ListFargateProfilesResponseTypeDef",
-    "ListNodegroupsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUpdatesResponseTypeDef",
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
     "CreateFargateProfileRequestRequestTypeDef",
@@ -125,21 +132,14 @@
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef",
     "DescribeNodegroupRequestNodegroupActiveWaitTypeDef",
     "DescribeNodegroupRequestNodegroupDeletedWaitTypeDef",
-    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
-    "ListAddonsRequestListAddonsPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
     "ListIdentityProviderConfigsResponseTypeDef",
     "EncryptionConfigTypeDef",
     "IdentityProviderConfigResponseTypeDef",
     "IdentityTypeDef",
     "NodegroupHealthTypeDef",
@@ -205,25 +205,14 @@
         "clusterVersion": str,
         "platformVersions": List[str],
         "defaultVersion": bool,
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
 _RequiredOidcIdentityProviderConfigRequestTypeDef = TypedDict(
     "_RequiredOidcIdentityProviderConfigRequestTypeDef",
     {
         "identityProviderConfigName": str,
         "issuerUrl": str,
         "clientId": str,
     },
@@ -495,14 +484,24 @@
     "DescribeAddonConfigurationRequestRequestTypeDef",
     {
         "addonName": str,
         "addonVersion": str,
     },
 )
 
+DescribeAddonConfigurationResponseTypeDef = TypedDict(
+    "DescribeAddonConfigurationResponseTypeDef",
+    {
+        "addonName": str,
+        "addonVersion": str,
+        "configurationSchema": str,
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
@@ -512,20 +511,23 @@
     "DescribeAddonRequestRequestTypeDef",
     {
         "clusterName": str,
         "addonName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = TypedDict(
+    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "kubernetesVersion": str,
+        "addonName": str,
+        "types": Sequence[str],
+        "publishers": Sequence[str],
+        "owners": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAddonVersionsRequestRequestTypeDef = TypedDict(
     "DescribeAddonVersionsRequestRequestTypeDef",
     {
@@ -645,14 +647,36 @@
         "code": NodegroupIssueCodeType,
         "message": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
+_RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
+    "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
+    "_OptionalListAddonsRequestListAddonsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAddonsRequestListAddonsPaginateTypeDef(
+    _RequiredListAddonsRequestListAddonsPaginateTypeDef,
+    _OptionalListAddonsRequestListAddonsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAddonsRequestRequestTypeDef = TypedDict(
     "_RequiredListAddonsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListAddonsRequestRequestTypeDef = TypedDict(
@@ -667,24 +691,73 @@
 
 class ListAddonsRequestRequestTypeDef(
     _RequiredListAddonsRequestRequestTypeDef, _OptionalListAddonsRequestRequestTypeDef
 ):
     pass
 
 
+ListAddonsResponseTypeDef = TypedDict(
+    "ListAddonsResponseTypeDef",
+    {
+        "addons": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "include": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "include": Sequence[str],
     },
     total=False,
 )
 
+ListClustersResponseTypeDef = TypedDict(
+    "ListClustersResponseTypeDef",
+    {
+        "clusters": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(
+    _RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+    _OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFargateProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListFargateProfilesRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListFargateProfilesRequestRequestTypeDef = TypedDict(
@@ -700,14 +773,45 @@
 class ListFargateProfilesRequestRequestTypeDef(
     _RequiredListFargateProfilesRequestRequestTypeDef,
     _OptionalListFargateProfilesRequestRequestTypeDef,
 ):
     pass
 
 
+ListFargateProfilesResponseTypeDef = TypedDict(
+    "ListFargateProfilesResponseTypeDef",
+    {
+        "fargateProfileNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(
+    _RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+    _OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListIdentityProviderConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityProviderConfigsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListIdentityProviderConfigsRequestRequestTypeDef = TypedDict(
@@ -723,14 +827,36 @@
 class ListIdentityProviderConfigsRequestRequestTypeDef(
     _RequiredListIdentityProviderConfigsRequestRequestTypeDef,
     _OptionalListIdentityProviderConfigsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
+    "_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
+    "_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListNodegroupsRequestListNodegroupsPaginateTypeDef(
+    _RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef,
+    _OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListNodegroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListNodegroupsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListNodegroupsRequestRequestTypeDef = TypedDict(
@@ -745,21 +871,62 @@
 
 class ListNodegroupsRequestRequestTypeDef(
     _RequiredListNodegroupsRequestRequestTypeDef, _OptionalListNodegroupsRequestRequestTypeDef
 ):
     pass
 
 
+ListNodegroupsResponseTypeDef = TypedDict(
+    "ListNodegroupsResponseTypeDef",
+    {
+        "nodegroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
+    "_RequiredListUpdatesRequestListUpdatesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
+    "_OptionalListUpdatesRequestListUpdatesPaginateTypeDef",
+    {
+        "nodegroupName": str,
+        "addonName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListUpdatesRequestListUpdatesPaginateTypeDef(
+    _RequiredListUpdatesRequestListUpdatesPaginateTypeDef,
+    _OptionalListUpdatesRequestListUpdatesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListUpdatesRequestRequestTypeDef = TypedDict(
     "_RequiredListUpdatesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListUpdatesRequestRequestTypeDef = TypedDict(
@@ -776,23 +943,53 @@
 
 class ListUpdatesRequestRequestTypeDef(
     _RequiredListUpdatesRequestRequestTypeDef, _OptionalListUpdatesRequestRequestTypeDef
 ):
     pass
 
 
+ListUpdatesResponseTypeDef = TypedDict(
+    "ListUpdatesResponseTypeDef",
+    {
+        "updateIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LogSetupTypeDef = TypedDict(
     "LogSetupTypeDef",
     {
         "types": Sequence[LogTypeType],
         "enabled": bool,
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
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -887,77 +1084,14 @@
         "architecture": List[str],
         "compatibilities": List[CompatibilityTypeDef],
         "requiresConfiguration": bool,
     },
     total=False,
 )
 
-DescribeAddonConfigurationResponseTypeDef = TypedDict(
-    "DescribeAddonConfigurationResponseTypeDef",
-    {
-        "addonName": str,
-        "addonVersion": str,
-        "configurationSchema": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAddonsResponseTypeDef = TypedDict(
-    "ListAddonsResponseTypeDef",
-    {
-        "addons": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListClustersResponseTypeDef = TypedDict(
-    "ListClustersResponseTypeDef",
-    {
-        "clusters": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListFargateProfilesResponseTypeDef = TypedDict(
-    "ListFargateProfilesResponseTypeDef",
-    {
-        "fargateProfileNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListNodegroupsResponseTypeDef = TypedDict(
-    "ListNodegroupsResponseTypeDef",
-    {
-        "nodegroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListUpdatesResponseTypeDef = TypedDict(
-    "ListUpdatesResponseTypeDef",
-    {
-        "updateIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredAssociateIdentityProviderConfigRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateIdentityProviderConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "oidc": OidcIdentityProviderConfigRequestTypeDef,
     },
 )
@@ -1356,148 +1490,14 @@
 class DescribeNodegroupRequestNodegroupDeletedWaitTypeDef(
     _RequiredDescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
     _OptionalDescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
 ):
     pass
 
 
-DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = TypedDict(
-    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
-    {
-        "kubernetesVersion": str,
-        "addonName": str,
-        "types": Sequence[str],
-        "publishers": Sequence[str],
-        "owners": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
-    "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
-    "_OptionalListAddonsRequestListAddonsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAddonsRequestListAddonsPaginateTypeDef(
-    _RequiredListAddonsRequestListAddonsPaginateTypeDef,
-    _OptionalListAddonsRequestListAddonsPaginateTypeDef,
-):
-    pass
-
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "include": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(
-    _RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-    _OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(
-    _RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-    _OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
-    "_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
-    "_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListNodegroupsRequestListNodegroupsPaginateTypeDef(
-    _RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef,
-    _OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
-    "_RequiredListUpdatesRequestListUpdatesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
-    "_OptionalListUpdatesRequestListUpdatesPaginateTypeDef",
-    {
-        "nodegroupName": str,
-        "addonName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListUpdatesRequestListUpdatesPaginateTypeDef(
-    _RequiredListUpdatesRequestListUpdatesPaginateTypeDef,
-    _OptionalListUpdatesRequestListUpdatesPaginateTypeDef,
-):
-    pass
-
-
 DescribeIdentityProviderConfigRequestRequestTypeDef = TypedDict(
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "identityProviderConfig": IdentityProviderConfigTypeDef,
     },
 )
@@ -1526,15 +1526,15 @@
 
 
 ListIdentityProviderConfigsResponseTypeDef = TypedDict(
     "ListIdentityProviderConfigsResponseTypeDef",
     {
         "identityProviderConfigs": List[IdentityProviderConfigTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "resources": Sequence[str],
@@ -1622,31 +1622,31 @@
     total=False,
 )
 
 CreateFargateProfileResponseTypeDef = TypedDict(
     "CreateFargateProfileResponseTypeDef",
     {
         "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteFargateProfileResponseTypeDef = TypedDict(
     "DeleteFargateProfileResponseTypeDef",
     {
         "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFargateProfileResponseTypeDef = TypedDict(
     "DescribeFargateProfileResponseTypeDef",
     {
         "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateNodegroupConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupConfigRequestRequestTypeDef",
     {
         "clusterName": str,
@@ -1696,15 +1696,15 @@
     pass
 
 
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
         "identityProviderConfig": IdentityProviderConfigResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NodegroupTypeDef = TypedDict(
     "NodegroupTypeDef",
     {
         "nodegroupName": str,
@@ -1814,172 +1814,172 @@
     pass
 
 
 AssociateEncryptionConfigResponseTypeDef = TypedDict(
     "AssociateEncryptionConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateIdentityProviderConfigResponseTypeDef = TypedDict(
     "AssociateIdentityProviderConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUpdateResponseTypeDef = TypedDict(
     "DescribeUpdateResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateIdentityProviderConfigResponseTypeDef = TypedDict(
     "DisassociateIdentityProviderConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAddonResponseTypeDef = TypedDict(
     "UpdateAddonResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterConfigResponseTypeDef = TypedDict(
     "UpdateClusterConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterVersionResponseTypeDef = TypedDict(
     "UpdateClusterVersionResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNodegroupConfigResponseTypeDef = TypedDict(
     "UpdateNodegroupConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNodegroupVersionResponseTypeDef = TypedDict(
     "UpdateNodegroupVersionResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAddonResponseTypeDef = TypedDict(
     "CreateAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAddonResponseTypeDef = TypedDict(
     "DeleteAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAddonResponseTypeDef = TypedDict(
     "DescribeAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAddonVersionsResponseTypeDef = TypedDict(
     "DescribeAddonVersionsResponseTypeDef",
     {
         "addons": List[AddonInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateNodegroupResponseTypeDef = TypedDict(
     "CreateNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteNodegroupResponseTypeDef = TypedDict(
     "DeleteNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeNodegroupResponseTypeDef = TypedDict(
     "DescribeNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeregisterClusterResponseTypeDef = TypedDict(
     "DeregisterClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterClusterResponseTypeDef = TypedDict(
     "RegisterClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/type_defs.pyi` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddonIssueTypeDef",
     "MarketplaceInformationTypeDef",
     "CompatibilityTypeDef",
-    "ResponseMetadataTypeDef",
     "OidcIdentityProviderConfigRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "CertificateTypeDef",
     "ClusterIssueTypeDef",
     "ConnectorConfigResponseTypeDef",
     "KubernetesNetworkConfigResponseTypeDef",
     "VpcConfigResponseTypeDef",
@@ -68,51 +67,59 @@
     "TaintTypeDef",
     "DeleteAddonRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteFargateProfileRequestRequestTypeDef",
     "DeleteNodegroupRequestRequestTypeDef",
     "DeregisterClusterRequestRequestTypeDef",
     "DescribeAddonConfigurationRequestRequestTypeDef",
+    "DescribeAddonConfigurationResponseTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAddonRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
     "DescribeAddonVersionsRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
     "ProviderTypeDef",
     "ErrorDetailTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
+    "ListAddonsRequestListAddonsPaginateTypeDef",
     "ListAddonsRequestRequestTypeDef",
+    "ListAddonsResponseTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListClustersResponseTypeDef",
+    "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
     "ListFargateProfilesRequestRequestTypeDef",
+    "ListFargateProfilesResponseTypeDef",
+    "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
     "ListIdentityProviderConfigsRequestRequestTypeDef",
+    "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
     "ListNodegroupsRequestRequestTypeDef",
+    "ListNodegroupsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "ListUpdatesRequestRequestTypeDef",
+    "ListUpdatesResponseTypeDef",
     "LogSetupTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddonRequestRequestTypeDef",
     "UpdateClusterVersionRequestRequestTypeDef",
     "UpdateLabelsPayloadTypeDef",
     "UpdateParamTypeDef",
     "AddonHealthTypeDef",
     "AddonVersionInfoTypeDef",
-    "DescribeAddonConfigurationResponseTypeDef",
-    "ListAddonsResponseTypeDef",
-    "ListClustersResponseTypeDef",
-    "ListFargateProfilesResponseTypeDef",
-    "ListNodegroupsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUpdatesResponseTypeDef",
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
     "CreateFargateProfileRequestRequestTypeDef",
@@ -124,21 +131,14 @@
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef",
     "DescribeNodegroupRequestNodegroupActiveWaitTypeDef",
     "DescribeNodegroupRequestNodegroupDeletedWaitTypeDef",
-    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
-    "ListAddonsRequestListAddonsPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
     "ListIdentityProviderConfigsResponseTypeDef",
     "EncryptionConfigTypeDef",
     "IdentityProviderConfigResponseTypeDef",
     "IdentityTypeDef",
     "NodegroupHealthTypeDef",
@@ -204,25 +204,14 @@
         "clusterVersion": str,
         "platformVersions": List[str],
         "defaultVersion": bool,
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
 _RequiredOidcIdentityProviderConfigRequestTypeDef = TypedDict(
     "_RequiredOidcIdentityProviderConfigRequestTypeDef",
     {
         "identityProviderConfigName": str,
         "issuerUrl": str,
         "clientId": str,
     },
@@ -488,14 +477,24 @@
     "DescribeAddonConfigurationRequestRequestTypeDef",
     {
         "addonName": str,
         "addonVersion": str,
     },
 )
 
+DescribeAddonConfigurationResponseTypeDef = TypedDict(
+    "DescribeAddonConfigurationResponseTypeDef",
+    {
+        "addonName": str,
+        "addonVersion": str,
+        "configurationSchema": str,
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
@@ -505,20 +504,23 @@
     "DescribeAddonRequestRequestTypeDef",
     {
         "clusterName": str,
         "addonName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = TypedDict(
+    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "kubernetesVersion": str,
+        "addonName": str,
+        "types": Sequence[str],
+        "publishers": Sequence[str],
+        "owners": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAddonVersionsRequestRequestTypeDef = TypedDict(
     "DescribeAddonVersionsRequestRequestTypeDef",
     {
@@ -636,14 +638,34 @@
         "code": NodegroupIssueCodeType,
         "message": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
+_RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
+    "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
+    "_OptionalListAddonsRequestListAddonsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAddonsRequestListAddonsPaginateTypeDef(
+    _RequiredListAddonsRequestListAddonsPaginateTypeDef,
+    _OptionalListAddonsRequestListAddonsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAddonsRequestRequestTypeDef = TypedDict(
     "_RequiredListAddonsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListAddonsRequestRequestTypeDef = TypedDict(
@@ -656,24 +678,71 @@
 )
 
 class ListAddonsRequestRequestTypeDef(
     _RequiredListAddonsRequestRequestTypeDef, _OptionalListAddonsRequestRequestTypeDef
 ):
     pass
 
+ListAddonsResponseTypeDef = TypedDict(
+    "ListAddonsResponseTypeDef",
+    {
+        "addons": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "include": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "include": Sequence[str],
     },
     total=False,
 )
 
+ListClustersResponseTypeDef = TypedDict(
+    "ListClustersResponseTypeDef",
+    {
+        "clusters": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(
+    _RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+    _OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+):
+    pass
+
 _RequiredListFargateProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListFargateProfilesRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListFargateProfilesRequestRequestTypeDef = TypedDict(
@@ -687,14 +756,43 @@
 
 class ListFargateProfilesRequestRequestTypeDef(
     _RequiredListFargateProfilesRequestRequestTypeDef,
     _OptionalListFargateProfilesRequestRequestTypeDef,
 ):
     pass
 
+ListFargateProfilesResponseTypeDef = TypedDict(
+    "ListFargateProfilesResponseTypeDef",
+    {
+        "fargateProfileNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(
+    _RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+    _OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+):
+    pass
+
 _RequiredListIdentityProviderConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityProviderConfigsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListIdentityProviderConfigsRequestRequestTypeDef = TypedDict(
@@ -708,14 +806,34 @@
 
 class ListIdentityProviderConfigsRequestRequestTypeDef(
     _RequiredListIdentityProviderConfigsRequestRequestTypeDef,
     _OptionalListIdentityProviderConfigsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
+    "_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
+    "_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListNodegroupsRequestListNodegroupsPaginateTypeDef(
+    _RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef,
+    _OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef,
+):
+    pass
+
 _RequiredListNodegroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListNodegroupsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListNodegroupsRequestRequestTypeDef = TypedDict(
@@ -728,21 +846,60 @@
 )
 
 class ListNodegroupsRequestRequestTypeDef(
     _RequiredListNodegroupsRequestRequestTypeDef, _OptionalListNodegroupsRequestRequestTypeDef
 ):
     pass
 
+ListNodegroupsResponseTypeDef = TypedDict(
+    "ListNodegroupsResponseTypeDef",
+    {
+        "nodegroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
+    "_RequiredListUpdatesRequestListUpdatesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
+    "_OptionalListUpdatesRequestListUpdatesPaginateTypeDef",
+    {
+        "nodegroupName": str,
+        "addonName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListUpdatesRequestListUpdatesPaginateTypeDef(
+    _RequiredListUpdatesRequestListUpdatesPaginateTypeDef,
+    _OptionalListUpdatesRequestListUpdatesPaginateTypeDef,
+):
+    pass
+
 _RequiredListUpdatesRequestRequestTypeDef = TypedDict(
     "_RequiredListUpdatesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListUpdatesRequestRequestTypeDef = TypedDict(
@@ -757,23 +914,53 @@
 )
 
 class ListUpdatesRequestRequestTypeDef(
     _RequiredListUpdatesRequestRequestTypeDef, _OptionalListUpdatesRequestRequestTypeDef
 ):
     pass
 
+ListUpdatesResponseTypeDef = TypedDict(
+    "ListUpdatesResponseTypeDef",
+    {
+        "updateIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LogSetupTypeDef = TypedDict(
     "LogSetupTypeDef",
     {
         "types": Sequence[LogTypeType],
         "enabled": bool,
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
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -864,77 +1051,14 @@
         "architecture": List[str],
         "compatibilities": List[CompatibilityTypeDef],
         "requiresConfiguration": bool,
     },
     total=False,
 )
 
-DescribeAddonConfigurationResponseTypeDef = TypedDict(
-    "DescribeAddonConfigurationResponseTypeDef",
-    {
-        "addonName": str,
-        "addonVersion": str,
-        "configurationSchema": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAddonsResponseTypeDef = TypedDict(
-    "ListAddonsResponseTypeDef",
-    {
-        "addons": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListClustersResponseTypeDef = TypedDict(
-    "ListClustersResponseTypeDef",
-    {
-        "clusters": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListFargateProfilesResponseTypeDef = TypedDict(
-    "ListFargateProfilesResponseTypeDef",
-    {
-        "fargateProfileNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListNodegroupsResponseTypeDef = TypedDict(
-    "ListNodegroupsResponseTypeDef",
-    {
-        "nodegroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListUpdatesResponseTypeDef = TypedDict(
-    "ListUpdatesResponseTypeDef",
-    {
-        "updateIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredAssociateIdentityProviderConfigRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateIdentityProviderConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "oidc": OidcIdentityProviderConfigRequestTypeDef,
     },
 )
@@ -1303,138 +1427,14 @@
 
 class DescribeNodegroupRequestNodegroupDeletedWaitTypeDef(
     _RequiredDescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
     _OptionalDescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
 ):
     pass
 
-DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = TypedDict(
-    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
-    {
-        "kubernetesVersion": str,
-        "addonName": str,
-        "types": Sequence[str],
-        "publishers": Sequence[str],
-        "owners": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
-    "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
-    "_OptionalListAddonsRequestListAddonsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAddonsRequestListAddonsPaginateTypeDef(
-    _RequiredListAddonsRequestListAddonsPaginateTypeDef,
-    _OptionalListAddonsRequestListAddonsPaginateTypeDef,
-):
-    pass
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "include": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(
-    _RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-    _OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-):
-    pass
-
-_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(
-    _RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-    _OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-):
-    pass
-
-_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
-    "_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
-    "_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListNodegroupsRequestListNodegroupsPaginateTypeDef(
-    _RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef,
-    _OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef,
-):
-    pass
-
-_RequiredListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
-    "_RequiredListUpdatesRequestListUpdatesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
-    "_OptionalListUpdatesRequestListUpdatesPaginateTypeDef",
-    {
-        "nodegroupName": str,
-        "addonName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListUpdatesRequestListUpdatesPaginateTypeDef(
-    _RequiredListUpdatesRequestListUpdatesPaginateTypeDef,
-    _OptionalListUpdatesRequestListUpdatesPaginateTypeDef,
-):
-    pass
-
 DescribeIdentityProviderConfigRequestRequestTypeDef = TypedDict(
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "identityProviderConfig": IdentityProviderConfigTypeDef,
     },
 )
@@ -1461,15 +1461,15 @@
     pass
 
 ListIdentityProviderConfigsResponseTypeDef = TypedDict(
     "ListIdentityProviderConfigsResponseTypeDef",
     {
         "identityProviderConfigs": List[IdentityProviderConfigTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "resources": Sequence[str],
@@ -1557,31 +1557,31 @@
     total=False,
 )
 
 CreateFargateProfileResponseTypeDef = TypedDict(
     "CreateFargateProfileResponseTypeDef",
     {
         "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteFargateProfileResponseTypeDef = TypedDict(
     "DeleteFargateProfileResponseTypeDef",
     {
         "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFargateProfileResponseTypeDef = TypedDict(
     "DescribeFargateProfileResponseTypeDef",
     {
         "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateNodegroupConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupConfigRequestRequestTypeDef",
     {
         "clusterName": str,
@@ -1627,15 +1627,15 @@
 ):
     pass
 
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
         "identityProviderConfig": IdentityProviderConfigResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NodegroupTypeDef = TypedDict(
     "NodegroupTypeDef",
     {
         "nodegroupName": str,
@@ -1741,172 +1741,172 @@
 ):
     pass
 
 AssociateEncryptionConfigResponseTypeDef = TypedDict(
     "AssociateEncryptionConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateIdentityProviderConfigResponseTypeDef = TypedDict(
     "AssociateIdentityProviderConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUpdateResponseTypeDef = TypedDict(
     "DescribeUpdateResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateIdentityProviderConfigResponseTypeDef = TypedDict(
     "DisassociateIdentityProviderConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAddonResponseTypeDef = TypedDict(
     "UpdateAddonResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterConfigResponseTypeDef = TypedDict(
     "UpdateClusterConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterVersionResponseTypeDef = TypedDict(
     "UpdateClusterVersionResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNodegroupConfigResponseTypeDef = TypedDict(
     "UpdateNodegroupConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNodegroupVersionResponseTypeDef = TypedDict(
     "UpdateNodegroupVersionResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAddonResponseTypeDef = TypedDict(
     "CreateAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAddonResponseTypeDef = TypedDict(
     "DeleteAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAddonResponseTypeDef = TypedDict(
     "DescribeAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAddonVersionsResponseTypeDef = TypedDict(
     "DescribeAddonVersionsResponseTypeDef",
     {
         "addons": List[AddonInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateNodegroupResponseTypeDef = TypedDict(
     "CreateNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteNodegroupResponseTypeDef = TypedDict(
     "DeleteNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeNodegroupResponseTypeDef = TypedDict(
     "DescribeNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeregisterClusterResponseTypeDef = TypedDict(
     "DeregisterClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterClusterResponseTypeDef = TypedDict(
     "RegisterClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/waiter.py` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks/waiter.pyi` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks.egg-info/PKG-INFO` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-eks
-Version: 1.26.31
-Summary: Type annotations for boto3.EKS 1.26.31 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.EKS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-eks"></a>
 
 # mypy-boto3-eks
 
 [![PyPI - mypy-boto3-eks](https://img.shields.io/pypi/v/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-eks?color=blue)](https://pypistats.org/packages/mypy-boto3-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EKS 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[boto3.EKS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [mypy-boto3-eks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -414,15 +414,14 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_eks.type_defs import (
     AddonIssueTypeDef,
     MarketplaceInformationTypeDef,
     CompatibilityTypeDef,
-    ResponseMetadataTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     AutoScalingGroupTypeDef,
     CertificateTypeDef,
     ClusterIssueTypeDef,
     ConnectorConfigResponseTypeDef,
     KubernetesNetworkConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
@@ -440,51 +439,59 @@
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteFargateProfileRequestRequestTypeDef,
     DeleteNodegroupRequestRequestTypeDef,
     DeregisterClusterRequestRequestTypeDef,
     DescribeAddonConfigurationRequestRequestTypeDef,
+    DescribeAddonConfigurationResponseTypeDef,
     WaiterConfigTypeDef,
     DescribeAddonRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
     DescribeAddonVersionsRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
+    ListAddonsRequestListAddonsPaginateTypeDef,
     ListAddonsRequestRequestTypeDef,
+    ListAddonsResponseTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListClustersResponseTypeDef,
+    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
+    ListFargateProfilesResponseTypeDef,
+    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
+    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListNodegroupsRequestRequestTypeDef,
+    ListNodegroupsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUpdatesRequestListUpdatesPaginateTypeDef,
     ListUpdatesRequestRequestTypeDef,
+    ListUpdatesResponseTypeDef,
     LogSetupTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddonRequestRequestTypeDef,
     UpdateClusterVersionRequestRequestTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateParamTypeDef,
     AddonHealthTypeDef,
     AddonVersionInfoTypeDef,
-    DescribeAddonConfigurationResponseTypeDef,
-    ListAddonsResponseTypeDef,
-    ListClustersResponseTypeDef,
-    ListFargateProfilesResponseTypeDef,
-    ListNodegroupsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
     CreateFargateProfileRequestRequestTypeDef,
@@ -496,21 +503,14 @@
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     DescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     DescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
-    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
-    ListAddonsRequestListAddonsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
-    ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     EncryptionConfigTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
@@ -559,42 +559,42 @@
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

### Comparing `mypy-boto3-eks-1.26.31/mypy_boto3_eks.egg-info/SOURCES.txt` & `mypy-boto3-eks-1.27.0/mypy_boto3_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.26.31/setup.py` & `mypy-boto3-eks-1.27.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-eks.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-eks",
-    version="1.26.31",
+    version="1.27.0",
     packages=["mypy_boto3_eks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EKS 1.26.31 service generated with mypy-boto3-builder 7.12.0"
+        "Type annotations for boto3.EKS 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/",
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


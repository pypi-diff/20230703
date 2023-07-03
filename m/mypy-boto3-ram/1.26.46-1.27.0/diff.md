# Comparing `tmp/mypy-boto3-ram-1.26.46.tar.gz` & `tmp/mypy-boto3-ram-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ram-1.26.46.tar", last modified: Mon Jan  9 20:27:39 2023, max compression
+gzip compressed data, was "mypy-boto3-ram-1.27.0.tar", last modified: Mon Jul  3 19:51:17 2023, max compression
```

## Comparing `mypy-boto3-ram-1.26.46.tar` & `mypy-boto3-ram-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.372431 mypy-boto3-ram-1.26.46/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16555 2023-01-09 20:27:39.372431 mypy-boto3-ram-1.26.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.372431 mypy-boto3-ram-1.26.46/mypy_boto3_ram/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24209 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30603 2023-01-09 20:27:29.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30556 2023-01-09 20:27:29.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.372431 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16555 2023-01-09 20:27:39.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-09 20:27:39.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-09 20:27:39.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-09 20:27:39.000000 mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 20:27:39.372431 mypy-boto3-ram-1.26.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-09 20:27:28.000000 mypy-boto3-ram-1.26.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.763845 mypy-boto3-ram-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:45:41.000000 mypy-boto3-ram-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-07-03 19:51:17.759845 mypy-boto3-ram-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-07-03 19:45:41.000000 mypy-boto3-ram-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.751845 mypy-boto3-ram-1.27.0/mypy_boto3_ram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-03 19:45:41.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-03 19:45:41.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:45:41.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31754 2023-07-03 19:45:41.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31707 2023-07-03 19:45:41.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-03 19:45:42.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-07-03 19:45:42.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-07-03 19:45:42.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-07-03 19:45:42.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:45:41.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41071 2023-07-03 19:45:42.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41006 2023-07-03 19:45:42.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:45:41.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.759845 mypy-boto3-ram-1.27.0/mypy_boto3_ram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-07-03 19:51:17.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:17.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:17.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:17.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:17.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:17.000000 mypy-boto3-ram-1.27.0/mypy_boto3_ram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:17.763845 mypy-boto3-ram-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:45:41.000000 mypy-boto3-ram-1.27.0/setup.py
```

### Comparing `mypy-boto3-ram-1.26.46/LICENSE` & `mypy-boto3-ram-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-ram-1.26.46/PKG-INFO` & `mypy-boto3-ram-1.27.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-ram
-Version: 1.26.46
-Summary: Type annotations for boto3.RAM 1.26.46 service generated with mypy-boto3-builder 7.12.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ram type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-ram"></a>
 
 # mypy-boto3-ram
 
 [![PyPI - mypy-boto3-ram](https://img.shields.io/pypi/v/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ram?color=blue)](https://pypistats.org/packages/mypy-boto3-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RAM 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[boto3.RAM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ram docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,14 +289,19 @@
 from mypy_boto3_ram.literals import (
     GetResourcePoliciesPaginatorName,
     GetResourceShareAssociationsPaginatorName,
     GetResourceShareInvitationsPaginatorName,
     GetResourceSharesPaginatorName,
     ListPrincipalsPaginatorName,
     ListResourcesPaginatorName,
+    PermissionFeatureSetType,
+    PermissionStatusType,
+    PermissionTypeFilterType,
+    PermissionTypeType,
+    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceRegionScopeType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareFeatureSetType,
     ResourceShareInvitationStatusType,
@@ -352,75 +325,95 @@
 
 `mypy_boto3_ram.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ram.type_defs import (
     AcceptResourceShareInvitationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AssociateResourceSharePermissionRequestRequestTypeDef,
+    AssociateResourceSharePermissionResponseTypeDef,
     AssociateResourceShareRequestRequestTypeDef,
     ResourceShareAssociationTypeDef,
+    AssociatedPermissionTypeDef,
     TagTypeDef,
+    CreatePermissionVersionRequestRequestTypeDef,
+    DeletePermissionRequestRequestTypeDef,
+    DeletePermissionResponseTypeDef,
+    DeletePermissionVersionRequestRequestTypeDef,
+    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareRequestRequestTypeDef,
+    DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionRequestRequestTypeDef,
+    DisassociateResourceSharePermissionResponseTypeDef,
     DisassociateResourceShareRequestRequestTypeDef,
+    EnableSharingWithAwsOrganizationResponseTypeDef,
     GetPermissionRequestRequestTypeDef,
-    ResourceSharePermissionDetailTypeDef,
-    PaginatorConfigTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
+    GetResourcePoliciesResponseTypeDef,
+    GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
     GetResourceShareAssociationsRequestRequestTypeDef,
+    GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
     GetResourceShareInvitationsRequestRequestTypeDef,
     TagFilterTypeDef,
     ListPendingInvitationResourcesRequestRequestTypeDef,
     ResourceTypeDef,
+    ListPermissionAssociationsRequestRequestTypeDef,
     ListPermissionVersionsRequestRequestTypeDef,
-    ResourceSharePermissionSummaryTypeDef,
     ListPermissionsRequestRequestTypeDef,
+    ListPrincipalsRequestListPrincipalsPaginateTypeDef,
     ListPrincipalsRequestRequestTypeDef,
     PrincipalTypeDef,
+    ListReplacePermissionAssociationsWorkRequestRequestTypeDef,
+    ReplacePermissionAssociationsWorkTypeDef,
     ListResourceSharePermissionsRequestRequestTypeDef,
     ListResourceTypesRequestRequestTypeDef,
     ServiceNameAndResourceTypeTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    PromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef,
+    PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     RejectResourceShareInvitationRequestRequestTypeDef,
+    ReplacePermissionAssociationsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    SetDefaultPermissionVersionRequestRequestTypeDef,
+    SetDefaultPermissionVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateResourceShareRequestRequestTypeDef,
-    AssociateResourceSharePermissionResponseTypeDef,
-    DeleteResourceShareResponseTypeDef,
-    DisassociateResourceSharePermissionResponseTypeDef,
-    EnableSharingWithAwsOrganizationResponseTypeDef,
-    GetResourcePoliciesResponseTypeDef,
-    PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     ResourceShareInvitationTypeDef,
+    ListPermissionAssociationsResponseTypeDef,
+    CreatePermissionRequestRequestTypeDef,
     CreateResourceShareRequestRequestTypeDef,
+    ResourceSharePermissionDetailTypeDef,
+    ResourceSharePermissionSummaryTypeDef,
     ResourceShareTypeDef,
     TagResourceRequestRequestTypeDef,
-    GetPermissionResponseTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
-    GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
-    ListPrincipalsRequestListPrincipalsPaginateTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     GetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     GetResourceSharesRequestRequestTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
     ListResourcesResponseTypeDef,
-    ListPermissionVersionsResponseTypeDef,
-    ListPermissionsResponseTypeDef,
-    ListResourceSharePermissionsResponseTypeDef,
     ListPrincipalsResponseTypeDef,
+    ListReplacePermissionAssociationsWorkResponseTypeDef,
+    ReplacePermissionAssociationsResponseTypeDef,
     ListResourceTypesResponseTypeDef,
     AcceptResourceShareInvitationResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
+    CreatePermissionVersionResponseTypeDef,
+    GetPermissionResponseTypeDef,
+    CreatePermissionResponseTypeDef,
+    ListPermissionVersionsResponseTypeDef,
+    ListPermissionsResponseTypeDef,
+    ListResourceSharePermissionsResponseTypeDef,
+    PromotePermissionCreatedFromPolicyResponseTypeDef,
     CreateResourceShareResponseTypeDef,
     GetResourceSharesResponseTypeDef,
     UpdateResourceShareResponseTypeDef,
 )
 
 
 def get_structure() -> AcceptResourceShareInvitationRequestRequestTypeDef:
@@ -430,42 +423,42 @@
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

### Comparing `mypy-boto3-ram-1.26.46/README.md` & `mypy-boto3-ram-1.27.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-ram
+Version: 1.27.0
+Summary: Type annotations for boto3.RAM 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 ram type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-ram"></a>
 
 # mypy-boto3-ram
 
 [![PyPI - mypy-boto3-ram](https://img.shields.io/pypi/v/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ram?color=blue)](https://pypistats.org/packages/mypy-boto3-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RAM 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[boto3.RAM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ram docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,14 +321,19 @@
 from mypy_boto3_ram.literals import (
     GetResourcePoliciesPaginatorName,
     GetResourceShareAssociationsPaginatorName,
     GetResourceShareInvitationsPaginatorName,
     GetResourceSharesPaginatorName,
     ListPrincipalsPaginatorName,
     ListResourcesPaginatorName,
+    PermissionFeatureSetType,
+    PermissionStatusType,
+    PermissionTypeFilterType,
+    PermissionTypeType,
+    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceRegionScopeType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareFeatureSetType,
     ResourceShareInvitationStatusType,
@@ -320,75 +357,95 @@
 
 `mypy_boto3_ram.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ram.type_defs import (
     AcceptResourceShareInvitationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AssociateResourceSharePermissionRequestRequestTypeDef,
+    AssociateResourceSharePermissionResponseTypeDef,
     AssociateResourceShareRequestRequestTypeDef,
     ResourceShareAssociationTypeDef,
+    AssociatedPermissionTypeDef,
     TagTypeDef,
+    CreatePermissionVersionRequestRequestTypeDef,
+    DeletePermissionRequestRequestTypeDef,
+    DeletePermissionResponseTypeDef,
+    DeletePermissionVersionRequestRequestTypeDef,
+    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareRequestRequestTypeDef,
+    DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionRequestRequestTypeDef,
+    DisassociateResourceSharePermissionResponseTypeDef,
     DisassociateResourceShareRequestRequestTypeDef,
+    EnableSharingWithAwsOrganizationResponseTypeDef,
     GetPermissionRequestRequestTypeDef,
-    ResourceSharePermissionDetailTypeDef,
-    PaginatorConfigTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
+    GetResourcePoliciesResponseTypeDef,
+    GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
     GetResourceShareAssociationsRequestRequestTypeDef,
+    GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
     GetResourceShareInvitationsRequestRequestTypeDef,
     TagFilterTypeDef,
     ListPendingInvitationResourcesRequestRequestTypeDef,
     ResourceTypeDef,
+    ListPermissionAssociationsRequestRequestTypeDef,
     ListPermissionVersionsRequestRequestTypeDef,
-    ResourceSharePermissionSummaryTypeDef,
     ListPermissionsRequestRequestTypeDef,
+    ListPrincipalsRequestListPrincipalsPaginateTypeDef,
     ListPrincipalsRequestRequestTypeDef,
     PrincipalTypeDef,
+    ListReplacePermissionAssociationsWorkRequestRequestTypeDef,
+    ReplacePermissionAssociationsWorkTypeDef,
     ListResourceSharePermissionsRequestRequestTypeDef,
     ListResourceTypesRequestRequestTypeDef,
     ServiceNameAndResourceTypeTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    PromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef,
+    PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     RejectResourceShareInvitationRequestRequestTypeDef,
+    ReplacePermissionAssociationsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    SetDefaultPermissionVersionRequestRequestTypeDef,
+    SetDefaultPermissionVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateResourceShareRequestRequestTypeDef,
-    AssociateResourceSharePermissionResponseTypeDef,
-    DeleteResourceShareResponseTypeDef,
-    DisassociateResourceSharePermissionResponseTypeDef,
-    EnableSharingWithAwsOrganizationResponseTypeDef,
-    GetResourcePoliciesResponseTypeDef,
-    PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     ResourceShareInvitationTypeDef,
+    ListPermissionAssociationsResponseTypeDef,
+    CreatePermissionRequestRequestTypeDef,
     CreateResourceShareRequestRequestTypeDef,
+    ResourceSharePermissionDetailTypeDef,
+    ResourceSharePermissionSummaryTypeDef,
     ResourceShareTypeDef,
     TagResourceRequestRequestTypeDef,
-    GetPermissionResponseTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
-    GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
-    ListPrincipalsRequestListPrincipalsPaginateTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     GetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     GetResourceSharesRequestRequestTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
     ListResourcesResponseTypeDef,
-    ListPermissionVersionsResponseTypeDef,
-    ListPermissionsResponseTypeDef,
-    ListResourceSharePermissionsResponseTypeDef,
     ListPrincipalsResponseTypeDef,
+    ListReplacePermissionAssociationsWorkResponseTypeDef,
+    ReplacePermissionAssociationsResponseTypeDef,
     ListResourceTypesResponseTypeDef,
     AcceptResourceShareInvitationResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
+    CreatePermissionVersionResponseTypeDef,
+    GetPermissionResponseTypeDef,
+    CreatePermissionResponseTypeDef,
+    ListPermissionVersionsResponseTypeDef,
+    ListPermissionsResponseTypeDef,
+    ListResourceSharePermissionsResponseTypeDef,
+    PromotePermissionCreatedFromPolicyResponseTypeDef,
     CreateResourceShareResponseTypeDef,
     GetResourceSharesResponseTypeDef,
     UpdateResourceShareResponseTypeDef,
 )
 
 
 def get_structure() -> AcceptResourceShareInvitationRequestRequestTypeDef:
@@ -398,42 +455,42 @@
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

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram/__init__.py` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram/__init__.pyi` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram/__main__.py` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RAM 1.26.46\nVersion:         1.26.46\nBuilder version:"
-        " 7.12.2\nDocs:           "
+        "Type annotations for boto3.RAM 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.46")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram/client.py` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram/client.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    PermissionFeatureSetType,
+    PermissionTypeFilterType,
+    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareStatusType,
 )
 from .paginator import (
@@ -33,80 +36,91 @@
     ListPrincipalsPaginator,
     ListResourcesPaginator,
 )
 from .type_defs import (
     AcceptResourceShareInvitationResponseTypeDef,
     AssociateResourceSharePermissionResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
+    CreatePermissionResponseTypeDef,
+    CreatePermissionVersionResponseTypeDef,
     CreateResourceShareResponseTypeDef,
+    DeletePermissionResponseTypeDef,
+    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     EnableSharingWithAwsOrganizationResponseTypeDef,
     GetPermissionResponseTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     GetResourceSharesResponseTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
+    ListPermissionAssociationsResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListPermissionVersionsResponseTypeDef,
     ListPrincipalsResponseTypeDef,
+    ListReplacePermissionAssociationsWorkResponseTypeDef,
     ListResourceSharePermissionsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListResourceTypesResponseTypeDef,
+    PromotePermissionCreatedFromPolicyResponseTypeDef,
     PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
+    ReplacePermissionAssociationsResponseTypeDef,
+    SetDefaultPermissionVersionResponseTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
     UpdateResourceShareResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("RAMClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     InvalidClientTokenException: Type[BotocoreClientError]
     InvalidMaxResultsException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
+    InvalidPolicyException: Type[BotocoreClientError]
     InvalidResourceTypeException: Type[BotocoreClientError]
     InvalidStateTransitionException: Type[BotocoreClientError]
     MalformedArnException: Type[BotocoreClientError]
+    MalformedPolicyTemplateException: Type[BotocoreClientError]
     MissingRequiredParameterException: Type[BotocoreClientError]
     OperationNotPermittedException: Type[BotocoreClientError]
+    PermissionAlreadyExistsException: Type[BotocoreClientError]
+    PermissionLimitExceededException: Type[BotocoreClientError]
+    PermissionVersionsLimitExceededException: Type[BotocoreClientError]
     ResourceArnNotFoundException: Type[BotocoreClientError]
     ResourceShareInvitationAlreadyAcceptedException: Type[BotocoreClientError]
     ResourceShareInvitationAlreadyRejectedException: Type[BotocoreClientError]
     ResourceShareInvitationArnNotFoundException: Type[BotocoreClientError]
     ResourceShareInvitationExpiredException: Type[BotocoreClientError]
     ResourceShareLimitExceededException: Type[BotocoreClientError]
     ServerInternalException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     TagLimitExceededException: Type[BotocoreClientError]
     TagPolicyViolationException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnknownResourceException: Type[BotocoreClientError]
-
+    UnmatchedPolicyPermissionException: Type[BotocoreClientError]
 
 class RAMClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/)
     """
 
@@ -116,41 +130,38 @@
     def exceptions(self) -> Exceptions:
         """
         RAMClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#exceptions)
         """
-
     def accept_resource_share_invitation(
         self, *, resourceShareInvitationArn: str, clientToken: str = ...
     ) -> AcceptResourceShareInvitationResponseTypeDef:
         """
         Accepts an invitation to a resource share from another Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.accept_resource_share_invitation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#accept_resource_share_invitation)
         """
-
     def associate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         clientToken: str = ...
     ) -> AssociateResourceShareResponseTypeDef:
         """
         Adds the specified list of principals and list of resources to a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#associate_resource_share)
         """
-
     def associate_resource_share_permission(
         self,
         *,
         resourceShareArn: str,
         permissionArn: str,
         replace: bool = ...,
         clientToken: str = ...,
@@ -159,31 +170,53 @@
         """
         Adds or replaces the RAM permission for a resource type included in a resource
         share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#associate_resource_share_permission)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#close)
         """
+    def create_permission(
+        self,
+        *,
+        name: str,
+        resourceType: str,
+        policyTemplate: str,
+        clientToken: str = ...,
+        tags: Sequence[TagTypeDef] = ...
+    ) -> CreatePermissionResponseTypeDef:
+        """
+        Creates a customer managed permission for a specified resource type that you can
+        attach to resource shares.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_permission)
+        """
+    def create_permission_version(
+        self, *, permissionArn: str, policyTemplate: str, clientToken: str = ...
+    ) -> CreatePermissionVersionResponseTypeDef:
+        """
+        Creates a new version of the specified customer managed permission.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_permission_version)
+        """
     def create_resource_share(
         self,
         *,
         name: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
@@ -193,85 +226,97 @@
     ) -> CreateResourceShareResponseTypeDef:
         """
         Creates a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_resource_share)
         """
+    def delete_permission(
+        self, *, permissionArn: str, clientToken: str = ...
+    ) -> DeletePermissionResponseTypeDef:
+        """
+        Deletes the specified customer managed permission in the Amazon Web Services
+        Region in which you call this operation.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_permission)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#delete_permission)
+        """
+    def delete_permission_version(
+        self, *, permissionArn: str, permissionVersion: int, clientToken: str = ...
+    ) -> DeletePermissionVersionResponseTypeDef:
+        """
+        Deletes one version of a customer managed permission.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_permission_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#delete_permission_version)
+        """
     def delete_resource_share(
         self, *, resourceShareArn: str, clientToken: str = ...
     ) -> DeleteResourceShareResponseTypeDef:
         """
         Deletes the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#delete_resource_share)
         """
-
     def disassociate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         clientToken: str = ...
     ) -> DisassociateResourceShareResponseTypeDef:
         """
-        Disassociates the specified principals or resources from the specified resource
-        share.
+        Removes the specified principals or resources from participating in the
+        specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#disassociate_resource_share)
         """
-
     def disassociate_resource_share_permission(
         self, *, resourceShareArn: str, permissionArn: str, clientToken: str = ...
     ) -> DisassociateResourceSharePermissionResponseTypeDef:
         """
-        Disassociates an RAM permission from a resource share.
+        Removes a managed permission from a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#disassociate_resource_share_permission)
         """
-
     def enable_sharing_with_aws_organization(
         self,
     ) -> EnableSharingWithAwsOrganizationResponseTypeDef:
         """
         Enables resource sharing within your organization in Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.enable_sharing_with_aws_organization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#enable_sharing_with_aws_organization)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#generate_presigned_url)
         """
-
     def get_permission(
         self, *, permissionArn: str, permissionVersion: int = ...
     ) -> GetPermissionResponseTypeDef:
         """
-        Gets the contents of an RAM permission in JSON format.
+        Retrieves the contents of a managed permission in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_permission)
         """
-
     def get_resource_policies(
         self,
         *,
         resourceArns: Sequence[str],
         principal: str = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -279,69 +324,66 @@
         """
         Retrieves the resource policies for the specified resources that you own and
         have shared.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_resource_policies)
         """
-
     def get_resource_share_associations(
         self,
         *,
         associationType: ResourceShareAssociationTypeType,
         resourceShareArns: Sequence[str] = ...,
         resourceArn: str = ...,
         principal: str = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetResourceShareAssociationsResponseTypeDef:
         """
-        Retrieves the resource and principal associations for resource shares that you
-        own.
+        Retrieves the lists of resources and principals that associated for resource
+        shares that you own.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_resource_share_associations)
         """
-
     def get_resource_share_invitations(
         self,
         *,
         resourceShareInvitationArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetResourceShareInvitationsResponseTypeDef:
         """
         Retrieves details about invitations that you have received for resource shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_invitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_resource_share_invitations)
         """
-
     def get_resource_shares(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        permissionArn: str = ...
+        permissionArn: str = ...,
+        permissionVersion: int = ...
     ) -> GetResourceSharesResponseTypeDef:
         """
         Retrieves details about the resource shares that you own or that are shared with
         you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_resource_shares)
         """
-
     def list_pending_invitation_resources(
         self,
         *,
         resourceShareInvitationArn: str,
         nextToken: str = ...,
         maxResults: int = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...
@@ -349,36 +391,57 @@
         """
         Lists the resources in a resource share that is shared with you but for which
         the invitation is still `PENDING`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_pending_invitation_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_pending_invitation_resources)
         """
+    def list_permission_associations(
+        self,
+        *,
+        permissionArn: str = ...,
+        permissionVersion: int = ...,
+        associationStatus: ResourceShareAssociationStatusType = ...,
+        resourceType: str = ...,
+        featureSet: PermissionFeatureSetType = ...,
+        defaultVersion: bool = ...,
+        nextToken: str = ...,
+        maxResults: int = ...
+    ) -> ListPermissionAssociationsResponseTypeDef:
+        """
+        Lists information about the managed permission and its associations to any
+        resource shares that use this managed permission.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_permission_associations)
+        """
     def list_permission_versions(
         self, *, permissionArn: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListPermissionVersionsResponseTypeDef:
         """
         Lists the available versions of the specified RAM permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_permission_versions)
         """
-
     def list_permissions(
-        self, *, resourceType: str = ..., nextToken: str = ..., maxResults: int = ...
+        self,
+        *,
+        resourceType: str = ...,
+        nextToken: str = ...,
+        maxResults: int = ...,
+        permissionType: PermissionTypeFilterType = ...
     ) -> ListPermissionsResponseTypeDef:
         """
         Retrieves a list of available RAM permissions that you can use for the supported
         resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_permissions)
         """
-
     def list_principals(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceArn: str = ...,
         principals: Sequence[str] = ...,
         resourceType: str = ...,
@@ -389,39 +452,51 @@
         """
         Lists the principals that you are sharing resources with or that are sharing
         resources with you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_principals)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_principals)
         """
+    def list_replace_permission_associations_work(
+        self,
+        *,
+        workIds: Sequence[str] = ...,
+        status: ReplacePermissionAssociationsWorkStatusType = ...,
+        nextToken: str = ...,
+        maxResults: int = ...
+    ) -> ListReplacePermissionAssociationsWorkResponseTypeDef:
+        """
+        Retrieves the current status of the asynchronous tasks performed by RAM when you
+        perform the  ReplacePermissionAssociationsWork operation.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_replace_permission_associations_work)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_replace_permission_associations_work)
+        """
     def list_resource_share_permissions(
         self, *, resourceShareArn: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListResourceSharePermissionsResponseTypeDef:
         """
         Lists the RAM permissions that are associated with a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resource_share_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_resource_share_permissions)
         """
-
     def list_resource_types(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...
     ) -> ListResourceTypesResponseTypeDef:
         """
         Lists the resource types that can be shared by RAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resource_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_resource_types)
         """
-
     def list_resources(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         principal: str = ...,
         resourceType: str = ...,
         resourceArns: Sequence[str] = ...,
@@ -433,110 +508,144 @@
         """
         Lists the resources that you added to a resource share or the resources that are
         shared with you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_resources)
         """
+    def promote_permission_created_from_policy(
+        self, *, permissionArn: str, name: str, clientToken: str = ...
+    ) -> PromotePermissionCreatedFromPolicyResponseTypeDef:
+        """
+        When you attach a resource-based policy to a resource, RAM automatically creates
+        a resource share of `featureSet`= `CREATED_FROM_POLICY` with a managed
+        permission that has the same IAM permissions as the original resource-based
+        policy.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.promote_permission_created_from_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#promote_permission_created_from_policy)
+        """
     def promote_resource_share_created_from_policy(
         self, *, resourceShareArn: str
     ) -> PromoteResourceShareCreatedFromPolicyResponseTypeDef:
         """
-        When you attach a resource-based permission policy to a resource, it
-        automatically creates a resource share.
+        When you attach a resource-based policy to a resource, RAM automatically creates
+        a resource share of `featureSet`= `CREATED_FROM_POLICY` with a managed
+        permission that has the same IAM permissions as the original resource-based
+        policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.promote_resource_share_created_from_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#promote_resource_share_created_from_policy)
         """
-
     def reject_resource_share_invitation(
         self, *, resourceShareInvitationArn: str, clientToken: str = ...
     ) -> RejectResourceShareInvitationResponseTypeDef:
         """
         Rejects an invitation to a resource share from another Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.reject_resource_share_invitation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#reject_resource_share_invitation)
         """
+    def replace_permission_associations(
+        self,
+        *,
+        fromPermissionArn: str,
+        toPermissionArn: str,
+        fromPermissionVersion: int = ...,
+        clientToken: str = ...
+    ) -> ReplacePermissionAssociationsResponseTypeDef:
+        """
+        Updates all resource shares that use a managed permission to a different managed
+        permission.
 
-    def tag_resource(self, *, resourceShareArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.replace_permission_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#replace_permission_associations)
+        """
+    def set_default_permission_version(
+        self, *, permissionArn: str, permissionVersion: int, clientToken: str = ...
+    ) -> SetDefaultPermissionVersionResponseTypeDef:
         """
-        Adds the specified tag keys and values to the specified resource share.
+        Designates the specified version number as the default version for the specified
+        customer managed permission.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.set_default_permission_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#set_default_permission_version)
+        """
+    def tag_resource(
+        self, *, tags: Sequence[TagTypeDef], resourceShareArn: str = ..., resourceArn: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Adds the specified tag keys and values to a resource share or managed
+        permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#tag_resource)
         """
-
-    def untag_resource(self, *, resourceShareArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
+    def untag_resource(
+        self, *, tagKeys: Sequence[str], resourceShareArn: str = ..., resourceArn: str = ...
+    ) -> Dict[str, Any]:
         """
-        Removes the specified tag key and value pairs from the specified resource share.
+        Removes the specified tag key and value pairs from the specified resource share
+        or managed permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#untag_resource)
         """
-
     def update_resource_share(
         self,
         *,
         resourceShareArn: str,
         name: str = ...,
         allowExternalPrincipals: bool = ...,
         clientToken: str = ...
     ) -> UpdateResourceShareResponseTypeDef:
         """
         Modifies some of the properties of the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.update_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#update_resource_share)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_policies"]
     ) -> GetResourcePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_share_associations"]
     ) -> GetResourceShareAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_share_invitations"]
     ) -> GetResourceShareInvitationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_shares"]
     ) -> GetResourceSharesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_principals"]) -> ListPrincipalsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_resources"]) -> ListResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram/client.pyi` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    PermissionFeatureSetType,
+    PermissionTypeFilterType,
+    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareStatusType,
 )
 from .paginator import (
@@ -33,76 +36,95 @@
     ListPrincipalsPaginator,
     ListResourcesPaginator,
 )
 from .type_defs import (
     AcceptResourceShareInvitationResponseTypeDef,
     AssociateResourceSharePermissionResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
+    CreatePermissionResponseTypeDef,
+    CreatePermissionVersionResponseTypeDef,
     CreateResourceShareResponseTypeDef,
+    DeletePermissionResponseTypeDef,
+    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     EnableSharingWithAwsOrganizationResponseTypeDef,
     GetPermissionResponseTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     GetResourceSharesResponseTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
+    ListPermissionAssociationsResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListPermissionVersionsResponseTypeDef,
     ListPrincipalsResponseTypeDef,
+    ListReplacePermissionAssociationsWorkResponseTypeDef,
     ListResourceSharePermissionsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListResourceTypesResponseTypeDef,
+    PromotePermissionCreatedFromPolicyResponseTypeDef,
     PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
+    ReplacePermissionAssociationsResponseTypeDef,
+    SetDefaultPermissionVersionResponseTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
     UpdateResourceShareResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("RAMClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     InvalidClientTokenException: Type[BotocoreClientError]
     InvalidMaxResultsException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
+    InvalidPolicyException: Type[BotocoreClientError]
     InvalidResourceTypeException: Type[BotocoreClientError]
     InvalidStateTransitionException: Type[BotocoreClientError]
     MalformedArnException: Type[BotocoreClientError]
+    MalformedPolicyTemplateException: Type[BotocoreClientError]
     MissingRequiredParameterException: Type[BotocoreClientError]
     OperationNotPermittedException: Type[BotocoreClientError]
+    PermissionAlreadyExistsException: Type[BotocoreClientError]
+    PermissionLimitExceededException: Type[BotocoreClientError]
+    PermissionVersionsLimitExceededException: Type[BotocoreClientError]
     ResourceArnNotFoundException: Type[BotocoreClientError]
     ResourceShareInvitationAlreadyAcceptedException: Type[BotocoreClientError]
     ResourceShareInvitationAlreadyRejectedException: Type[BotocoreClientError]
     ResourceShareInvitationArnNotFoundException: Type[BotocoreClientError]
     ResourceShareInvitationExpiredException: Type[BotocoreClientError]
     ResourceShareLimitExceededException: Type[BotocoreClientError]
     ServerInternalException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     TagLimitExceededException: Type[BotocoreClientError]
     TagPolicyViolationException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnknownResourceException: Type[BotocoreClientError]
+    UnmatchedPolicyPermissionException: Type[BotocoreClientError]
+
 
 class RAMClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/)
     """
 
@@ -112,38 +134,41 @@
     def exceptions(self) -> Exceptions:
         """
         RAMClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#exceptions)
         """
+
     def accept_resource_share_invitation(
         self, *, resourceShareInvitationArn: str, clientToken: str = ...
     ) -> AcceptResourceShareInvitationResponseTypeDef:
         """
         Accepts an invitation to a resource share from another Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.accept_resource_share_invitation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#accept_resource_share_invitation)
         """
+
     def associate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         clientToken: str = ...
     ) -> AssociateResourceShareResponseTypeDef:
         """
         Adds the specified list of principals and list of resources to a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#associate_resource_share)
         """
+
     def associate_resource_share_permission(
         self,
         *,
         resourceShareArn: str,
         permissionArn: str,
         replace: bool = ...,
         clientToken: str = ...,
@@ -152,28 +177,58 @@
         """
         Adds or replaces the RAM permission for a resource type included in a resource
         share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#associate_resource_share_permission)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#close)
         """
+
+    def create_permission(
+        self,
+        *,
+        name: str,
+        resourceType: str,
+        policyTemplate: str,
+        clientToken: str = ...,
+        tags: Sequence[TagTypeDef] = ...
+    ) -> CreatePermissionResponseTypeDef:
+        """
+        Creates a customer managed permission for a specified resource type that you can
+        attach to resource shares.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_permission)
+        """
+
+    def create_permission_version(
+        self, *, permissionArn: str, policyTemplate: str, clientToken: str = ...
+    ) -> CreatePermissionVersionResponseTypeDef:
+        """
+        Creates a new version of the specified customer managed permission.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_permission_version)
+        """
+
     def create_resource_share(
         self,
         *,
         name: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
@@ -183,78 +238,106 @@
     ) -> CreateResourceShareResponseTypeDef:
         """
         Creates a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_resource_share)
         """
+
+    def delete_permission(
+        self, *, permissionArn: str, clientToken: str = ...
+    ) -> DeletePermissionResponseTypeDef:
+        """
+        Deletes the specified customer managed permission in the Amazon Web Services
+        Region in which you call this operation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_permission)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#delete_permission)
+        """
+
+    def delete_permission_version(
+        self, *, permissionArn: str, permissionVersion: int, clientToken: str = ...
+    ) -> DeletePermissionVersionResponseTypeDef:
+        """
+        Deletes one version of a customer managed permission.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_permission_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#delete_permission_version)
+        """
+
     def delete_resource_share(
         self, *, resourceShareArn: str, clientToken: str = ...
     ) -> DeleteResourceShareResponseTypeDef:
         """
         Deletes the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#delete_resource_share)
         """
+
     def disassociate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         clientToken: str = ...
     ) -> DisassociateResourceShareResponseTypeDef:
         """
-        Disassociates the specified principals or resources from the specified resource
-        share.
+        Removes the specified principals or resources from participating in the
+        specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#disassociate_resource_share)
         """
+
     def disassociate_resource_share_permission(
         self, *, resourceShareArn: str, permissionArn: str, clientToken: str = ...
     ) -> DisassociateResourceSharePermissionResponseTypeDef:
         """
-        Disassociates an RAM permission from a resource share.
+        Removes a managed permission from a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#disassociate_resource_share_permission)
         """
+
     def enable_sharing_with_aws_organization(
         self,
     ) -> EnableSharingWithAwsOrganizationResponseTypeDef:
         """
         Enables resource sharing within your organization in Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.enable_sharing_with_aws_organization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#enable_sharing_with_aws_organization)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#generate_presigned_url)
         """
+
     def get_permission(
         self, *, permissionArn: str, permissionVersion: int = ...
     ) -> GetPermissionResponseTypeDef:
         """
-        Gets the contents of an RAM permission in JSON format.
+        Retrieves the contents of a managed permission in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_permission)
         """
+
     def get_resource_policies(
         self,
         *,
         resourceArns: Sequence[str],
         principal: str = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -262,65 +345,70 @@
         """
         Retrieves the resource policies for the specified resources that you own and
         have shared.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_resource_policies)
         """
+
     def get_resource_share_associations(
         self,
         *,
         associationType: ResourceShareAssociationTypeType,
         resourceShareArns: Sequence[str] = ...,
         resourceArn: str = ...,
         principal: str = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetResourceShareAssociationsResponseTypeDef:
         """
-        Retrieves the resource and principal associations for resource shares that you
-        own.
+        Retrieves the lists of resources and principals that associated for resource
+        shares that you own.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_resource_share_associations)
         """
+
     def get_resource_share_invitations(
         self,
         *,
         resourceShareInvitationArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetResourceShareInvitationsResponseTypeDef:
         """
         Retrieves details about invitations that you have received for resource shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_invitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_resource_share_invitations)
         """
+
     def get_resource_shares(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        permissionArn: str = ...
+        permissionArn: str = ...,
+        permissionVersion: int = ...
     ) -> GetResourceSharesResponseTypeDef:
         """
         Retrieves details about the resource shares that you own or that are shared with
         you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_resource_shares)
         """
+
     def list_pending_invitation_resources(
         self,
         *,
         resourceShareInvitationArn: str,
         nextToken: str = ...,
         maxResults: int = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...
@@ -328,33 +416,61 @@
         """
         Lists the resources in a resource share that is shared with you but for which
         the invitation is still `PENDING`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_pending_invitation_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_pending_invitation_resources)
         """
+
+    def list_permission_associations(
+        self,
+        *,
+        permissionArn: str = ...,
+        permissionVersion: int = ...,
+        associationStatus: ResourceShareAssociationStatusType = ...,
+        resourceType: str = ...,
+        featureSet: PermissionFeatureSetType = ...,
+        defaultVersion: bool = ...,
+        nextToken: str = ...,
+        maxResults: int = ...
+    ) -> ListPermissionAssociationsResponseTypeDef:
+        """
+        Lists information about the managed permission and its associations to any
+        resource shares that use this managed permission.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_permission_associations)
+        """
+
     def list_permission_versions(
         self, *, permissionArn: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListPermissionVersionsResponseTypeDef:
         """
         Lists the available versions of the specified RAM permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_permission_versions)
         """
+
     def list_permissions(
-        self, *, resourceType: str = ..., nextToken: str = ..., maxResults: int = ...
+        self,
+        *,
+        resourceType: str = ...,
+        nextToken: str = ...,
+        maxResults: int = ...,
+        permissionType: PermissionTypeFilterType = ...
     ) -> ListPermissionsResponseTypeDef:
         """
         Retrieves a list of available RAM permissions that you can use for the supported
         resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_permissions)
         """
+
     def list_principals(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceArn: str = ...,
         principals: Sequence[str] = ...,
         resourceType: str = ...,
@@ -365,36 +481,55 @@
         """
         Lists the principals that you are sharing resources with or that are sharing
         resources with you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_principals)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_principals)
         """
+
+    def list_replace_permission_associations_work(
+        self,
+        *,
+        workIds: Sequence[str] = ...,
+        status: ReplacePermissionAssociationsWorkStatusType = ...,
+        nextToken: str = ...,
+        maxResults: int = ...
+    ) -> ListReplacePermissionAssociationsWorkResponseTypeDef:
+        """
+        Retrieves the current status of the asynchronous tasks performed by RAM when you
+        perform the  ReplacePermissionAssociationsWork operation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_replace_permission_associations_work)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_replace_permission_associations_work)
+        """
+
     def list_resource_share_permissions(
         self, *, resourceShareArn: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListResourceSharePermissionsResponseTypeDef:
         """
         Lists the RAM permissions that are associated with a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resource_share_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_resource_share_permissions)
         """
+
     def list_resource_types(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...
     ) -> ListResourceTypesResponseTypeDef:
         """
         Lists the resource types that can be shared by RAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resource_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_resource_types)
         """
+
     def list_resources(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         principal: str = ...,
         resourceType: str = ...,
         resourceArns: Sequence[str] = ...,
@@ -406,99 +541,158 @@
         """
         Lists the resources that you added to a resource share or the resources that are
         shared with you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#list_resources)
         """
+
+    def promote_permission_created_from_policy(
+        self, *, permissionArn: str, name: str, clientToken: str = ...
+    ) -> PromotePermissionCreatedFromPolicyResponseTypeDef:
+        """
+        When you attach a resource-based policy to a resource, RAM automatically creates
+        a resource share of `featureSet`= `CREATED_FROM_POLICY` with a managed
+        permission that has the same IAM permissions as the original resource-based
+        policy.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.promote_permission_created_from_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#promote_permission_created_from_policy)
+        """
+
     def promote_resource_share_created_from_policy(
         self, *, resourceShareArn: str
     ) -> PromoteResourceShareCreatedFromPolicyResponseTypeDef:
         """
-        When you attach a resource-based permission policy to a resource, it
-        automatically creates a resource share.
+        When you attach a resource-based policy to a resource, RAM automatically creates
+        a resource share of `featureSet`= `CREATED_FROM_POLICY` with a managed
+        permission that has the same IAM permissions as the original resource-based
+        policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.promote_resource_share_created_from_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#promote_resource_share_created_from_policy)
         """
+
     def reject_resource_share_invitation(
         self, *, resourceShareInvitationArn: str, clientToken: str = ...
     ) -> RejectResourceShareInvitationResponseTypeDef:
         """
         Rejects an invitation to a resource share from another Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.reject_resource_share_invitation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#reject_resource_share_invitation)
         """
-    def tag_resource(self, *, resourceShareArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
+
+    def replace_permission_associations(
+        self,
+        *,
+        fromPermissionArn: str,
+        toPermissionArn: str,
+        fromPermissionVersion: int = ...,
+        clientToken: str = ...
+    ) -> ReplacePermissionAssociationsResponseTypeDef:
+        """
+        Updates all resource shares that use a managed permission to a different managed
+        permission.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.replace_permission_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#replace_permission_associations)
+        """
+
+    def set_default_permission_version(
+        self, *, permissionArn: str, permissionVersion: int, clientToken: str = ...
+    ) -> SetDefaultPermissionVersionResponseTypeDef:
+        """
+        Designates the specified version number as the default version for the specified
+        customer managed permission.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.set_default_permission_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#set_default_permission_version)
+        """
+
+    def tag_resource(
+        self, *, tags: Sequence[TagTypeDef], resourceShareArn: str = ..., resourceArn: str = ...
+    ) -> Dict[str, Any]:
         """
-        Adds the specified tag keys and values to the specified resource share.
+        Adds the specified tag keys and values to a resource share or managed
+        permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#tag_resource)
         """
-    def untag_resource(self, *, resourceShareArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
+
+    def untag_resource(
+        self, *, tagKeys: Sequence[str], resourceShareArn: str = ..., resourceArn: str = ...
+    ) -> Dict[str, Any]:
         """
-        Removes the specified tag key and value pairs from the specified resource share.
+        Removes the specified tag key and value pairs from the specified resource share
+        or managed permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#untag_resource)
         """
+
     def update_resource_share(
         self,
         *,
         resourceShareArn: str,
         name: str = ...,
         allowExternalPrincipals: bool = ...,
         clientToken: str = ...
     ) -> UpdateResourceShareResponseTypeDef:
         """
         Modifies some of the properties of the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.update_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#update_resource_share)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_policies"]
     ) -> GetResourcePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_share_associations"]
     ) -> GetResourceShareAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_share_invitations"]
     ) -> GetResourceShareInvitationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_shares"]
     ) -> GetResourceSharesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_principals"]) -> ListPrincipalsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_resources"]) -> ListResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram/literals.py` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 __all__ = (
     "GetResourcePoliciesPaginatorName",
     "GetResourceShareAssociationsPaginatorName",
     "GetResourceShareInvitationsPaginatorName",
     "GetResourceSharesPaginatorName",
     "ListPrincipalsPaginatorName",
     "ListResourcesPaginatorName",
+    "PermissionFeatureSetType",
+    "PermissionStatusType",
+    "PermissionTypeFilterType",
+    "PermissionTypeType",
+    "ReplacePermissionAssociationsWorkStatusType",
     "ResourceOwnerType",
     "ResourceRegionScopeFilterType",
     "ResourceRegionScopeType",
     "ResourceShareAssociationStatusType",
     "ResourceShareAssociationTypeType",
     "ResourceShareFeatureSetType",
     "ResourceShareInvitationStatusType",
@@ -45,14 +50,19 @@
 
 GetResourcePoliciesPaginatorName = Literal["get_resource_policies"]
 GetResourceShareAssociationsPaginatorName = Literal["get_resource_share_associations"]
 GetResourceShareInvitationsPaginatorName = Literal["get_resource_share_invitations"]
 GetResourceSharesPaginatorName = Literal["get_resource_shares"]
 ListPrincipalsPaginatorName = Literal["list_principals"]
 ListResourcesPaginatorName = Literal["list_resources"]
+PermissionFeatureSetType = Literal["CREATED_FROM_POLICY", "PROMOTING_TO_STANDARD", "STANDARD"]
+PermissionStatusType = Literal["ATTACHABLE", "DELETED", "DELETING", "UNATTACHABLE"]
+PermissionTypeFilterType = Literal["ALL", "AWS_MANAGED", "CUSTOMER_MANAGED"]
+PermissionTypeType = Literal["AWS_MANAGED", "CUSTOMER_MANAGED"]
+ReplacePermissionAssociationsWorkStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS"]
 ResourceOwnerType = Literal["OTHER-ACCOUNTS", "SELF"]
 ResourceRegionScopeFilterType = Literal["ALL", "GLOBAL", "REGIONAL"]
 ResourceRegionScopeType = Literal["GLOBAL", "REGIONAL"]
 ResourceShareAssociationStatusType = Literal[
     "ASSOCIATED", "ASSOCIATING", "DISASSOCIATED", "DISASSOCIATING", "FAILED"
 ]
 ResourceShareAssociationTypeType = Literal["PRINCIPAL", "RESOURCE"]
@@ -74,14 +84,15 @@
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
@@ -102,31 +113,34 @@
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
@@ -205,14 +219,15 @@
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
@@ -223,14 +238,15 @@
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
@@ -266,14 +282,15 @@
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
@@ -292,16 +309,19 @@
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
@@ -381,18 +401,21 @@
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
@@ -429,14 +452,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram/literals.pyi` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 __all__ = (
     "GetResourcePoliciesPaginatorName",
     "GetResourceShareAssociationsPaginatorName",
     "GetResourceShareInvitationsPaginatorName",
     "GetResourceSharesPaginatorName",
     "ListPrincipalsPaginatorName",
     "ListResourcesPaginatorName",
+    "PermissionFeatureSetType",
+    "PermissionStatusType",
+    "PermissionTypeFilterType",
+    "PermissionTypeType",
+    "ReplacePermissionAssociationsWorkStatusType",
     "ResourceOwnerType",
     "ResourceRegionScopeFilterType",
     "ResourceRegionScopeType",
     "ResourceShareAssociationStatusType",
     "ResourceShareAssociationTypeType",
     "ResourceShareFeatureSetType",
     "ResourceShareInvitationStatusType",
@@ -43,14 +48,19 @@
 
 GetResourcePoliciesPaginatorName = Literal["get_resource_policies"]
 GetResourceShareAssociationsPaginatorName = Literal["get_resource_share_associations"]
 GetResourceShareInvitationsPaginatorName = Literal["get_resource_share_invitations"]
 GetResourceSharesPaginatorName = Literal["get_resource_shares"]
 ListPrincipalsPaginatorName = Literal["list_principals"]
 ListResourcesPaginatorName = Literal["list_resources"]
+PermissionFeatureSetType = Literal["CREATED_FROM_POLICY", "PROMOTING_TO_STANDARD", "STANDARD"]
+PermissionStatusType = Literal["ATTACHABLE", "DELETED", "DELETING", "UNATTACHABLE"]
+PermissionTypeFilterType = Literal["ALL", "AWS_MANAGED", "CUSTOMER_MANAGED"]
+PermissionTypeType = Literal["AWS_MANAGED", "CUSTOMER_MANAGED"]
+ReplacePermissionAssociationsWorkStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS"]
 ResourceOwnerType = Literal["OTHER-ACCOUNTS", "SELF"]
 ResourceRegionScopeFilterType = Literal["ALL", "GLOBAL", "REGIONAL"]
 ResourceRegionScopeType = Literal["GLOBAL", "REGIONAL"]
 ResourceShareAssociationStatusType = Literal[
     "ASSOCIATED", "ASSOCIATING", "DISASSOCIATED", "DISASSOCIATING", "FAILED"
 ]
 ResourceShareAssociationTypeType = Literal["PRINCIPAL", "RESOURCE"]
@@ -72,14 +82,15 @@
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
@@ -100,31 +111,34 @@
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
@@ -203,14 +217,15 @@
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
@@ -221,14 +236,15 @@
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
@@ -264,14 +280,15 @@
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
@@ -290,16 +307,19 @@
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
@@ -379,18 +399,21 @@
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
@@ -427,14 +450,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram/paginator.py` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceArns: Sequence[str],
         principal: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourcepoliciespaginator)
         """
 
 
@@ -100,15 +100,15 @@
         self,
         *,
         associationType: ResourceShareAssociationTypeType,
         resourceShareArns: Sequence[str] = ...,
         resourceArn: str = ...,
         principal: str = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourceShareAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShareAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourceshareassociationspaginator)
         """
 
 
@@ -119,15 +119,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceShareInvitationArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourceShareInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShareInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourceshareinvitationspaginator)
         """
 
 
@@ -142,15 +142,16 @@
         *,
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         permissionArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        permissionVersion: int = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourceSharesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourcesharespaginator)
         """
 
 
@@ -164,15 +165,15 @@
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceArn: str = ...,
         principals: Sequence[str] = ...,
         resourceType: str = ...,
         resourceShareArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.ListPrincipals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#listprincipalspaginator)
         """
 
 
@@ -187,13 +188,13 @@
         *,
         resourceOwner: ResourceOwnerType,
         principal: str = ...,
         resourceType: str = ...,
         resourceArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#listresourcespaginator)
         """
```

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram/paginator.pyi` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceArns: Sequence[str],
         principal: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourcepoliciespaginator)
         """
 
 class GetResourceShareAssociationsPaginator(Paginator):
@@ -96,15 +96,15 @@
         self,
         *,
         associationType: ResourceShareAssociationTypeType,
         resourceShareArns: Sequence[str] = ...,
         resourceArn: str = ...,
         principal: str = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourceShareAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShareAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourceshareassociationspaginator)
         """
 
 class GetResourceShareInvitationsPaginator(Paginator):
@@ -114,15 +114,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceShareInvitationArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourceShareInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShareInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourceshareinvitationspaginator)
         """
 
 class GetResourceSharesPaginator(Paginator):
@@ -136,15 +136,16 @@
         *,
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         permissionArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        permissionVersion: int = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourceSharesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourcesharespaginator)
         """
 
 class ListPrincipalsPaginator(Paginator):
@@ -157,15 +158,15 @@
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceArn: str = ...,
         principals: Sequence[str] = ...,
         resourceType: str = ...,
         resourceShareArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.ListPrincipals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#listprincipalspaginator)
         """
 
 class ListResourcesPaginator(Paginator):
@@ -179,13 +180,13 @@
         *,
         resourceOwner: ResourceOwnerType,
         principal: str = ...,
         resourceType: str = ...,
         resourceArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#listresourcespaginator)
         """
```

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram/type_defs.py` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram/type_defs.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,19 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
+    PermissionFeatureSetType,
+    PermissionStatusType,
+    PermissionTypeFilterType,
+    PermissionTypeType,
+    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceRegionScopeType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareFeatureSetType,
     ResourceShareInvitationStatusType,
@@ -31,75 +36,95 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptResourceShareInvitationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AssociateResourceSharePermissionRequestRequestTypeDef",
+    "AssociateResourceSharePermissionResponseTypeDef",
     "AssociateResourceShareRequestRequestTypeDef",
     "ResourceShareAssociationTypeDef",
+    "AssociatedPermissionTypeDef",
     "TagTypeDef",
+    "CreatePermissionVersionRequestRequestTypeDef",
+    "DeletePermissionRequestRequestTypeDef",
+    "DeletePermissionResponseTypeDef",
+    "DeletePermissionVersionRequestRequestTypeDef",
+    "DeletePermissionVersionResponseTypeDef",
     "DeleteResourceShareRequestRequestTypeDef",
+    "DeleteResourceShareResponseTypeDef",
     "DisassociateResourceSharePermissionRequestRequestTypeDef",
+    "DisassociateResourceSharePermissionResponseTypeDef",
     "DisassociateResourceShareRequestRequestTypeDef",
+    "EnableSharingWithAwsOrganizationResponseTypeDef",
     "GetPermissionRequestRequestTypeDef",
-    "ResourceSharePermissionDetailTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
+    "GetResourcePoliciesResponseTypeDef",
+    "GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
     "GetResourceShareAssociationsRequestRequestTypeDef",
+    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
     "GetResourceShareInvitationsRequestRequestTypeDef",
     "TagFilterTypeDef",
     "ListPendingInvitationResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
+    "ListPermissionAssociationsRequestRequestTypeDef",
     "ListPermissionVersionsRequestRequestTypeDef",
-    "ResourceSharePermissionSummaryTypeDef",
     "ListPermissionsRequestRequestTypeDef",
+    "ListPrincipalsRequestListPrincipalsPaginateTypeDef",
     "ListPrincipalsRequestRequestTypeDef",
     "PrincipalTypeDef",
+    "ListReplacePermissionAssociationsWorkRequestRequestTypeDef",
+    "ReplacePermissionAssociationsWorkTypeDef",
     "ListResourceSharePermissionsRequestRequestTypeDef",
     "ListResourceTypesRequestRequestTypeDef",
     "ServiceNameAndResourceTypeTypeDef",
+    "ListResourcesRequestListResourcesPaginateTypeDef",
     "ListResourcesRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "PromotePermissionCreatedFromPolicyRequestRequestTypeDef",
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
+    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
     "RejectResourceShareInvitationRequestRequestTypeDef",
+    "ReplacePermissionAssociationsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "SetDefaultPermissionVersionRequestRequestTypeDef",
+    "SetDefaultPermissionVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateResourceShareRequestRequestTypeDef",
-    "AssociateResourceSharePermissionResponseTypeDef",
-    "DeleteResourceShareResponseTypeDef",
-    "DisassociateResourceSharePermissionResponseTypeDef",
-    "EnableSharingWithAwsOrganizationResponseTypeDef",
-    "GetResourcePoliciesResponseTypeDef",
-    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
     "AssociateResourceShareResponseTypeDef",
     "DisassociateResourceShareResponseTypeDef",
     "GetResourceShareAssociationsResponseTypeDef",
     "ResourceShareInvitationTypeDef",
+    "ListPermissionAssociationsResponseTypeDef",
+    "CreatePermissionRequestRequestTypeDef",
     "CreateResourceShareRequestRequestTypeDef",
+    "ResourceSharePermissionDetailTypeDef",
+    "ResourceSharePermissionSummaryTypeDef",
     "ResourceShareTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "GetPermissionResponseTypeDef",
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    "GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
-    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
-    "ListPrincipalsRequestListPrincipalsPaginateTypeDef",
-    "ListResourcesRequestListResourcesPaginateTypeDef",
     "GetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     "GetResourceSharesRequestRequestTypeDef",
     "ListPendingInvitationResourcesResponseTypeDef",
     "ListResourcesResponseTypeDef",
-    "ListPermissionVersionsResponseTypeDef",
-    "ListPermissionsResponseTypeDef",
-    "ListResourceSharePermissionsResponseTypeDef",
     "ListPrincipalsResponseTypeDef",
+    "ListReplacePermissionAssociationsWorkResponseTypeDef",
+    "ReplacePermissionAssociationsResponseTypeDef",
     "ListResourceTypesResponseTypeDef",
     "AcceptResourceShareInvitationResponseTypeDef",
     "GetResourceShareInvitationsResponseTypeDef",
     "RejectResourceShareInvitationResponseTypeDef",
+    "CreatePermissionVersionResponseTypeDef",
+    "GetPermissionResponseTypeDef",
+    "CreatePermissionResponseTypeDef",
+    "ListPermissionVersionsResponseTypeDef",
+    "ListPermissionsResponseTypeDef",
+    "ListResourceSharePermissionsResponseTypeDef",
+    "PromotePermissionCreatedFromPolicyResponseTypeDef",
     "CreateResourceShareResponseTypeDef",
     "GetResourceSharesResponseTypeDef",
     "UpdateResourceShareResponseTypeDef",
 )
 
 _RequiredAcceptResourceShareInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptResourceShareInvitationRequestRequestTypeDef",
@@ -119,25 +144,14 @@
 class AcceptResourceShareInvitationRequestRequestTypeDef(
     _RequiredAcceptResourceShareInvitationRequestRequestTypeDef,
     _OptionalAcceptResourceShareInvitationRequestRequestTypeDef,
 ):
     pass
 
 
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
 _RequiredAssociateResourceSharePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateResourceSharePermissionRequestRequestTypeDef",
     {
         "resourceShareArn": str,
         "permissionArn": str,
     },
 )
@@ -155,14 +169,23 @@
 class AssociateResourceSharePermissionRequestRequestTypeDef(
     _RequiredAssociateResourceSharePermissionRequestRequestTypeDef,
     _OptionalAssociateResourceSharePermissionRequestRequestTypeDef,
 ):
     pass
 
 
+AssociateResourceSharePermissionResponseTypeDef = TypedDict(
+    "AssociateResourceSharePermissionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAssociateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalAssociateResourceShareRequestRequestTypeDef = TypedDict(
@@ -195,23 +218,125 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "external": bool,
     },
     total=False,
 )
 
+AssociatedPermissionTypeDef = TypedDict(
+    "AssociatedPermissionTypeDef",
+    {
+        "arn": str,
+        "permissionVersion": str,
+        "defaultVersion": bool,
+        "resourceType": str,
+        "status": str,
+        "featureSet": PermissionFeatureSetType,
+        "lastUpdatedTime": datetime,
+        "resourceShareArn": str,
+    },
+    total=False,
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
+_RequiredCreatePermissionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePermissionVersionRequestRequestTypeDef",
+    {
+        "permissionArn": str,
+        "policyTemplate": str,
+    },
+)
+_OptionalCreatePermissionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePermissionVersionRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class CreatePermissionVersionRequestRequestTypeDef(
+    _RequiredCreatePermissionVersionRequestRequestTypeDef,
+    _OptionalCreatePermissionVersionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDeletePermissionRequestRequestTypeDef = TypedDict(
+    "_RequiredDeletePermissionRequestRequestTypeDef",
+    {
+        "permissionArn": str,
+    },
+)
+_OptionalDeletePermissionRequestRequestTypeDef = TypedDict(
+    "_OptionalDeletePermissionRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class DeletePermissionRequestRequestTypeDef(
+    _RequiredDeletePermissionRequestRequestTypeDef, _OptionalDeletePermissionRequestRequestTypeDef
+):
+    pass
+
+
+DeletePermissionResponseTypeDef = TypedDict(
+    "DeletePermissionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "permissionStatus": PermissionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDeletePermissionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredDeletePermissionVersionRequestRequestTypeDef",
+    {
+        "permissionArn": str,
+        "permissionVersion": int,
+    },
+)
+_OptionalDeletePermissionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalDeletePermissionVersionRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class DeletePermissionVersionRequestRequestTypeDef(
+    _RequiredDeletePermissionVersionRequestRequestTypeDef,
+    _OptionalDeletePermissionVersionRequestRequestTypeDef,
+):
+    pass
+
+
+DeletePermissionVersionResponseTypeDef = TypedDict(
+    "DeletePermissionVersionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "permissionStatus": PermissionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalDeleteResourceShareRequestRequestTypeDef = TypedDict(
@@ -226,14 +351,23 @@
 class DeleteResourceShareRequestRequestTypeDef(
     _RequiredDeleteResourceShareRequestRequestTypeDef,
     _OptionalDeleteResourceShareRequestRequestTypeDef,
 ):
     pass
 
 
+DeleteResourceShareResponseTypeDef = TypedDict(
+    "DeleteResourceShareResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDisassociateResourceSharePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateResourceSharePermissionRequestRequestTypeDef",
     {
         "resourceShareArn": str,
         "permissionArn": str,
     },
 )
@@ -249,14 +383,23 @@
 class DisassociateResourceSharePermissionRequestRequestTypeDef(
     _RequiredDisassociateResourceSharePermissionRequestRequestTypeDef,
     _OptionalDisassociateResourceSharePermissionRequestRequestTypeDef,
 ):
     pass
 
 
+DisassociateResourceSharePermissionResponseTypeDef = TypedDict(
+    "DisassociateResourceSharePermissionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDisassociateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalDisassociateResourceShareRequestRequestTypeDef = TypedDict(
@@ -273,14 +416,22 @@
 class DisassociateResourceShareRequestRequestTypeDef(
     _RequiredDisassociateResourceShareRequestRequestTypeDef,
     _OptionalDisassociateResourceShareRequestRequestTypeDef,
 ):
     pass
 
 
+EnableSharingWithAwsOrganizationResponseTypeDef = TypedDict(
+    "EnableSharingWithAwsOrganizationResponseTypeDef",
+    {
+        "returnValue": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredGetPermissionRequestRequestTypeDef",
     {
         "permissionArn": str,
     },
 )
 _OptionalGetPermissionRequestRequestTypeDef = TypedDict(
@@ -294,40 +445,37 @@
 
 class GetPermissionRequestRequestTypeDef(
     _RequiredGetPermissionRequestRequestTypeDef, _OptionalGetPermissionRequestRequestTypeDef
 ):
     pass
 
 
-ResourceSharePermissionDetailTypeDef = TypedDict(
-    "ResourceSharePermissionDetailTypeDef",
+_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "permission": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
+        "resourceArns": Sequence[str],
     },
-    total=False,
 )
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "principal": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "resourceArns": Sequence[str],
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -344,14 +492,49 @@
 class GetResourcePoliciesRequestRequestTypeDef(
     _RequiredGetResourcePoliciesRequestRequestTypeDef,
     _OptionalGetResourcePoliciesRequestRequestTypeDef,
 ):
     pass
 
 
+GetResourcePoliciesResponseTypeDef = TypedDict(
+    "GetResourcePoliciesResponseTypeDef",
+    {
+        "policies": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
+    {
+        "associationType": ResourceShareAssociationTypeType,
+    },
+)
+_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
+    {
+        "resourceShareArns": Sequence[str],
+        "resourceArn": str,
+        "principal": str,
+        "associationStatus": ResourceShareAssociationStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef(
+    _RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
+    _OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetResourceShareAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceShareAssociationsRequestRequestTypeDef",
     {
         "associationType": ResourceShareAssociationTypeType,
     },
 )
 _OptionalGetResourceShareAssociationsRequestRequestTypeDef = TypedDict(
@@ -371,14 +554,24 @@
 class GetResourceShareAssociationsRequestRequestTypeDef(
     _RequiredGetResourceShareAssociationsRequestRequestTypeDef,
     _OptionalGetResourceShareAssociationsRequestRequestTypeDef,
 ):
     pass
 
 
+GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef = TypedDict(
+    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
+    {
+        "resourceShareInvitationArns": Sequence[str],
+        "resourceShareArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetResourceShareInvitationsRequestRequestTypeDef = TypedDict(
     "GetResourceShareInvitationsRequestRequestTypeDef",
     {
         "resourceShareInvitationArns": Sequence[str],
         "resourceShareArns": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -431,14 +624,29 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "resourceRegionScope": ResourceRegionScopeType,
     },
     total=False,
 )
 
+ListPermissionAssociationsRequestRequestTypeDef = TypedDict(
+    "ListPermissionAssociationsRequestRequestTypeDef",
+    {
+        "permissionArn": str,
+        "permissionVersion": int,
+        "associationStatus": ResourceShareAssociationStatusType,
+        "resourceType": str,
+        "featureSet": PermissionFeatureSetType,
+        "defaultVersion": bool,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
 _RequiredListPermissionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionVersionsRequestRequestTypeDef",
     {
         "permissionArn": str,
     },
 )
 _OptionalListPermissionVersionsRequestRequestTypeDef = TypedDict(
@@ -454,40 +662,51 @@
 class ListPermissionVersionsRequestRequestTypeDef(
     _RequiredListPermissionVersionsRequestRequestTypeDef,
     _OptionalListPermissionVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-ResourceSharePermissionSummaryTypeDef = TypedDict(
-    "ResourceSharePermissionSummaryTypeDef",
+ListPermissionsRequestRequestTypeDef = TypedDict(
+    "ListPermissionsRequestRequestTypeDef",
     {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
         "resourceType": str,
-        "status": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
+        "nextToken": str,
+        "maxResults": int,
+        "permissionType": PermissionTypeFilterType,
     },
     total=False,
 )
 
-ListPermissionsRequestRequestTypeDef = TypedDict(
-    "ListPermissionsRequestRequestTypeDef",
+_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef",
     {
+        "resourceOwner": ResourceOwnerType,
+    },
+)
+_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "principals": Sequence[str],
         "resourceType": str,
-        "nextToken": str,
-        "maxResults": int,
+        "resourceShareArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListPrincipalsRequestListPrincipalsPaginateTypeDef(
+    _RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef,
+    _OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalsRequestRequestTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
     },
 )
 _OptionalListPrincipalsRequestRequestTypeDef = TypedDict(
@@ -518,14 +737,41 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "external": bool,
     },
     total=False,
 )
 
+ListReplacePermissionAssociationsWorkRequestRequestTypeDef = TypedDict(
+    "ListReplacePermissionAssociationsWorkRequestRequestTypeDef",
+    {
+        "workIds": Sequence[str],
+        "status": ReplacePermissionAssociationsWorkStatusType,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+ReplacePermissionAssociationsWorkTypeDef = TypedDict(
+    "ReplacePermissionAssociationsWorkTypeDef",
+    {
+        "id": str,
+        "fromPermissionArn": str,
+        "fromPermissionVersion": str,
+        "toPermissionArn": str,
+        "toPermissionVersion": str,
+        "status": ReplacePermissionAssociationsWorkStatusType,
+        "statusMessage": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredListResourceSharePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceSharePermissionsRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalListResourceSharePermissionsRequestRequestTypeDef = TypedDict(
@@ -561,14 +807,41 @@
         "resourceType": str,
         "serviceName": str,
         "resourceRegionScope": ResourceRegionScopeType,
     },
     total=False,
 )
 
+_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "resourceOwner": ResourceOwnerType,
+    },
+)
+_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "principal": str,
+        "resourceType": str,
+        "resourceArns": Sequence[str],
+        "resourceShareArns": Sequence[str],
+        "resourceRegionScope": ResourceRegionScopeFilterType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListResourcesRequestListResourcesPaginateTypeDef(
+    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
+    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -588,21 +861,62 @@
 
 class ListResourcesRequestRequestTypeDef(
     _RequiredListResourcesRequestRequestTypeDef, _OptionalListResourcesRequestRequestTypeDef
 ):
     pass
 
 
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
+_RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef",
+    {
+        "permissionArn": str,
+        "name": str,
+    },
+)
+_OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class PromotePermissionCreatedFromPolicyRequestRequestTypeDef(
+    _RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef,
+    _OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef,
+):
+    pass
+
+
 PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef = TypedDict(
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 
+PromoteResourceShareCreatedFromPolicyResponseTypeDef = TypedDict(
+    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
+    {
+        "returnValue": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRejectResourceShareInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredRejectResourceShareInvitationRequestRequestTypeDef",
     {
         "resourceShareInvitationArn": str,
     },
 )
 _OptionalRejectResourceShareInvitationRequestRequestTypeDef = TypedDict(
@@ -617,122 +931,151 @@
 class RejectResourceShareInvitationRequestRequestTypeDef(
     _RequiredRejectResourceShareInvitationRequestRequestTypeDef,
     _OptionalRejectResourceShareInvitationRequestRequestTypeDef,
 ):
     pass
 
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceShareArn": str,
-        "tagKeys": Sequence[str],
-    },
-)
-
-_RequiredUpdateResourceShareRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateResourceShareRequestRequestTypeDef",
+_RequiredReplacePermissionAssociationsRequestRequestTypeDef = TypedDict(
+    "_RequiredReplacePermissionAssociationsRequestRequestTypeDef",
     {
-        "resourceShareArn": str,
+        "fromPermissionArn": str,
+        "toPermissionArn": str,
     },
 )
-_OptionalUpdateResourceShareRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateResourceShareRequestRequestTypeDef",
+_OptionalReplacePermissionAssociationsRequestRequestTypeDef = TypedDict(
+    "_OptionalReplacePermissionAssociationsRequestRequestTypeDef",
     {
-        "name": str,
-        "allowExternalPrincipals": bool,
+        "fromPermissionVersion": int,
         "clientToken": str,
     },
     total=False,
 )
 
 
-class UpdateResourceShareRequestRequestTypeDef(
-    _RequiredUpdateResourceShareRequestRequestTypeDef,
-    _OptionalUpdateResourceShareRequestRequestTypeDef,
+class ReplacePermissionAssociationsRequestRequestTypeDef(
+    _RequiredReplacePermissionAssociationsRequestRequestTypeDef,
+    _OptionalReplacePermissionAssociationsRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateResourceSharePermissionResponseTypeDef = TypedDict(
-    "AssociateResourceSharePermissionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "returnValue": bool,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-DeleteResourceShareResponseTypeDef = TypedDict(
-    "DeleteResourceShareResponseTypeDef",
+_RequiredSetDefaultPermissionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredSetDefaultPermissionVersionRequestRequestTypeDef",
+    {
+        "permissionArn": str,
+        "permissionVersion": int,
+    },
+)
+_OptionalSetDefaultPermissionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalSetDefaultPermissionVersionRequestRequestTypeDef",
     {
-        "returnValue": bool,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-DisassociateResourceSharePermissionResponseTypeDef = TypedDict(
-    "DisassociateResourceSharePermissionResponseTypeDef",
+
+class SetDefaultPermissionVersionRequestRequestTypeDef(
+    _RequiredSetDefaultPermissionVersionRequestRequestTypeDef,
+    _OptionalSetDefaultPermissionVersionRequestRequestTypeDef,
+):
+    pass
+
+
+SetDefaultPermissionVersionResponseTypeDef = TypedDict(
+    "SetDefaultPermissionVersionResponseTypeDef",
     {
         "returnValue": bool,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EnableSharingWithAwsOrganizationResponseTypeDef = TypedDict(
-    "EnableSharingWithAwsOrganizationResponseTypeDef",
+_RequiredUntagResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredUntagResourceRequestRequestTypeDef",
     {
-        "returnValue": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tagKeys": Sequence[str],
     },
 )
-
-GetResourcePoliciesResponseTypeDef = TypedDict(
-    "GetResourcePoliciesResponseTypeDef",
+_OptionalUntagResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalUntagResourceRequestRequestTypeDef",
     {
-        "policies": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceShareArn": str,
+        "resourceArn": str,
     },
+    total=False,
 )
 
-PromoteResourceShareCreatedFromPolicyResponseTypeDef = TypedDict(
-    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
+
+class UntagResourceRequestRequestTypeDef(
+    _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateResourceShareRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateResourceShareRequestRequestTypeDef",
     {
-        "returnValue": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceShareArn": str,
+    },
+)
+_OptionalUpdateResourceShareRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateResourceShareRequestRequestTypeDef",
+    {
+        "name": str,
+        "allowExternalPrincipals": bool,
+        "clientToken": str,
     },
+    total=False,
 )
 
+
+class UpdateResourceShareRequestRequestTypeDef(
+    _RequiredUpdateResourceShareRequestRequestTypeDef,
+    _OptionalUpdateResourceShareRequestRequestTypeDef,
+):
+    pass
+
+
 AssociateResourceShareResponseTypeDef = TypedDict(
     "AssociateResourceShareResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateResourceShareResponseTypeDef = TypedDict(
     "DisassociateResourceShareResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceShareAssociationsResponseTypeDef = TypedDict(
     "GetResourceShareAssociationsResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceShareInvitationTypeDef = TypedDict(
     "ResourceShareInvitationTypeDef",
     {
         "resourceShareInvitationArn": str,
@@ -744,14 +1087,47 @@
         "status": ResourceShareInvitationStatusType,
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "receiverArn": str,
     },
     total=False,
 )
 
+ListPermissionAssociationsResponseTypeDef = TypedDict(
+    "ListPermissionAssociationsResponseTypeDef",
+    {
+        "permissions": List[AssociatedPermissionTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreatePermissionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePermissionRequestRequestTypeDef",
+    {
+        "name": str,
+        "resourceType": str,
+        "policyTemplate": str,
+    },
+)
+_OptionalCreatePermissionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePermissionRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreatePermissionRequestRequestTypeDef(
+    _RequiredCreatePermissionRequestRequestTypeDef, _OptionalCreatePermissionRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceShareRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateResourceShareRequestRequestTypeDef = TypedDict(
@@ -771,155 +1147,88 @@
 class CreateResourceShareRequestRequestTypeDef(
     _RequiredCreateResourceShareRequestRequestTypeDef,
     _OptionalCreateResourceShareRequestRequestTypeDef,
 ):
     pass
 
 
-ResourceShareTypeDef = TypedDict(
-    "ResourceShareTypeDef",
+ResourceSharePermissionDetailTypeDef = TypedDict(
+    "ResourceSharePermissionDetailTypeDef",
     {
-        "resourceShareArn": str,
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
         "name": str,
-        "owningAccountId": str,
-        "allowExternalPrincipals": bool,
-        "status": ResourceShareStatusType,
-        "statusMessage": str,
-        "tags": List[TagTypeDef],
+        "resourceType": str,
+        "permission": str,
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
-        "featureSet": ResourceShareFeatureSetType,
-    },
-    total=False,
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceShareArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
-GetPermissionResponseTypeDef = TypedDict(
-    "GetPermissionResponseTypeDef",
-    {
-        "permission": ResourceSharePermissionDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "resourceArns": Sequence[str],
-    },
-)
-_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "principal": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "isResourceTypeDefault": bool,
+        "permissionType": PermissionTypeType,
+        "featureSet": PermissionFeatureSetType,
+        "status": PermissionStatusType,
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
-class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
-    {
-        "associationType": ResourceShareAssociationTypeType,
-    },
-)
-_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
+ResourceSharePermissionSummaryTypeDef = TypedDict(
+    "ResourceSharePermissionSummaryTypeDef",
     {
-        "resourceShareArns": Sequence[str],
-        "resourceArn": str,
-        "principal": str,
-        "associationStatus": ResourceShareAssociationStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "status": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+        "permissionType": PermissionTypeType,
+        "featureSet": PermissionFeatureSetType,
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
-class GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef(
-    _RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
-    _OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
-):
-    pass
-
-
-GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef = TypedDict(
-    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
+ResourceShareTypeDef = TypedDict(
+    "ResourceShareTypeDef",
     {
-        "resourceShareInvitationArns": Sequence[str],
-        "resourceShareArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "resourceShareArn": str,
+        "name": str,
+        "owningAccountId": str,
+        "allowExternalPrincipals": bool,
+        "status": ResourceShareStatusType,
+        "statusMessage": str,
+        "tags": List[TagTypeDef],
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "featureSet": ResourceShareFeatureSetType,
     },
     total=False,
 )
 
-_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef",
+_RequiredTagResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredTagResourceRequestRequestTypeDef",
     {
-        "resourceOwner": ResourceOwnerType,
+        "tags": Sequence[TagTypeDef],
     },
 )
-_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef",
+_OptionalTagResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalTagResourceRequestRequestTypeDef",
     {
+        "resourceShareArn": str,
         "resourceArn": str,
-        "principals": Sequence[str],
-        "resourceType": str,
-        "resourceShareArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPrincipalsRequestListPrincipalsPaginateTypeDef(
-    _RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef,
-    _OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "resourceOwner": ResourceOwnerType,
-    },
-)
-_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "principal": str,
-        "resourceType": str,
-        "resourceArns": Sequence[str],
-        "resourceShareArns": Sequence[str],
-        "resourceRegionScope": ResourceRegionScopeFilterType,
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListResourcesRequestListResourcesPaginateTypeDef(
-    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
-    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
+class TagResourceRequestRequestTypeDef(
+    _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
 
 _RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef = TypedDict(
     "_RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     {
@@ -930,15 +1239,16 @@
     "_OptionalGetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     {
         "resourceShareArns": Sequence[str],
         "resourceShareStatus": ResourceShareStatusType,
         "name": str,
         "tagFilters": Sequence[TagFilterTypeDef],
         "permissionArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "permissionVersion": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class GetResourceSharesRequestGetResourceSharesPaginateTypeDef(
     _RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef,
@@ -959,14 +1269,15 @@
         "resourceShareArns": Sequence[str],
         "resourceShareStatus": ResourceShareStatusType,
         "name": str,
         "tagFilters": Sequence[TagFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
         "permissionArn": str,
+        "permissionVersion": int,
     },
     total=False,
 )
 
 
 class GetResourceSharesRequestRequestTypeDef(
     _RequiredGetResourceSharesRequestRequestTypeDef, _OptionalGetResourceSharesRequestRequestTypeDef
@@ -975,118 +1286,171 @@
 
 
 ListPendingInvitationResourcesResponseTypeDef = TypedDict(
     "ListPendingInvitationResourcesResponseTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPermissionVersionsResponseTypeDef = TypedDict(
-    "ListPermissionVersionsResponseTypeDef",
-    {
-        "permissions": List[ResourceSharePermissionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPermissionsResponseTypeDef = TypedDict(
-    "ListPermissionsResponseTypeDef",
+ListPrincipalsResponseTypeDef = TypedDict(
+    "ListPrincipalsResponseTypeDef",
     {
-        "permissions": List[ResourceSharePermissionSummaryTypeDef],
+        "principals": List[PrincipalTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListResourceSharePermissionsResponseTypeDef = TypedDict(
-    "ListResourceSharePermissionsResponseTypeDef",
+ListReplacePermissionAssociationsWorkResponseTypeDef = TypedDict(
+    "ListReplacePermissionAssociationsWorkResponseTypeDef",
     {
-        "permissions": List[ResourceSharePermissionSummaryTypeDef],
+        "replacePermissionAssociationsWorks": List[ReplacePermissionAssociationsWorkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPrincipalsResponseTypeDef = TypedDict(
-    "ListPrincipalsResponseTypeDef",
+ReplacePermissionAssociationsResponseTypeDef = TypedDict(
+    "ReplacePermissionAssociationsResponseTypeDef",
     {
-        "principals": List[PrincipalTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "replacePermissionAssociationsWork": ReplacePermissionAssociationsWorkTypeDef,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceTypesResponseTypeDef = TypedDict(
     "ListResourceTypesResponseTypeDef",
     {
         "resourceTypes": List[ServiceNameAndResourceTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AcceptResourceShareInvitationResponseTypeDef = TypedDict(
     "AcceptResourceShareInvitationResponseTypeDef",
     {
         "resourceShareInvitation": ResourceShareInvitationTypeDef,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceShareInvitationsResponseTypeDef = TypedDict(
     "GetResourceShareInvitationsResponseTypeDef",
     {
         "resourceShareInvitations": List[ResourceShareInvitationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RejectResourceShareInvitationResponseTypeDef = TypedDict(
     "RejectResourceShareInvitationResponseTypeDef",
     {
         "resourceShareInvitation": ResourceShareInvitationTypeDef,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePermissionVersionResponseTypeDef = TypedDict(
+    "CreatePermissionVersionResponseTypeDef",
+    {
+        "permission": ResourceSharePermissionDetailTypeDef,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetPermissionResponseTypeDef = TypedDict(
+    "GetPermissionResponseTypeDef",
+    {
+        "permission": ResourceSharePermissionDetailTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePermissionResponseTypeDef = TypedDict(
+    "CreatePermissionResponseTypeDef",
+    {
+        "permission": ResourceSharePermissionSummaryTypeDef,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPermissionVersionsResponseTypeDef = TypedDict(
+    "ListPermissionVersionsResponseTypeDef",
+    {
+        "permissions": List[ResourceSharePermissionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPermissionsResponseTypeDef = TypedDict(
+    "ListPermissionsResponseTypeDef",
+    {
+        "permissions": List[ResourceSharePermissionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListResourceSharePermissionsResponseTypeDef = TypedDict(
+    "ListResourceSharePermissionsResponseTypeDef",
+    {
+        "permissions": List[ResourceSharePermissionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PromotePermissionCreatedFromPolicyResponseTypeDef = TypedDict(
+    "PromotePermissionCreatedFromPolicyResponseTypeDef",
+    {
+        "permission": ResourceSharePermissionSummaryTypeDef,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateResourceShareResponseTypeDef = TypedDict(
     "CreateResourceShareResponseTypeDef",
     {
         "resourceShare": ResourceShareTypeDef,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceSharesResponseTypeDef = TypedDict(
     "GetResourceSharesResponseTypeDef",
     {
         "resourceShares": List[ResourceShareTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateResourceShareResponseTypeDef = TypedDict(
     "UpdateResourceShareResponseTypeDef",
     {
         "resourceShare": ResourceShareTypeDef,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram/type_defs.pyi` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram/type_defs.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -12,14 +12,19 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
+    PermissionFeatureSetType,
+    PermissionStatusType,
+    PermissionTypeFilterType,
+    PermissionTypeType,
+    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceRegionScopeType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareFeatureSetType,
     ResourceShareInvitationStatusType,
@@ -30,75 +35,95 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptResourceShareInvitationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AssociateResourceSharePermissionRequestRequestTypeDef",
+    "AssociateResourceSharePermissionResponseTypeDef",
     "AssociateResourceShareRequestRequestTypeDef",
     "ResourceShareAssociationTypeDef",
+    "AssociatedPermissionTypeDef",
     "TagTypeDef",
+    "CreatePermissionVersionRequestRequestTypeDef",
+    "DeletePermissionRequestRequestTypeDef",
+    "DeletePermissionResponseTypeDef",
+    "DeletePermissionVersionRequestRequestTypeDef",
+    "DeletePermissionVersionResponseTypeDef",
     "DeleteResourceShareRequestRequestTypeDef",
+    "DeleteResourceShareResponseTypeDef",
     "DisassociateResourceSharePermissionRequestRequestTypeDef",
+    "DisassociateResourceSharePermissionResponseTypeDef",
     "DisassociateResourceShareRequestRequestTypeDef",
+    "EnableSharingWithAwsOrganizationResponseTypeDef",
     "GetPermissionRequestRequestTypeDef",
-    "ResourceSharePermissionDetailTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
+    "GetResourcePoliciesResponseTypeDef",
+    "GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
     "GetResourceShareAssociationsRequestRequestTypeDef",
+    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
     "GetResourceShareInvitationsRequestRequestTypeDef",
     "TagFilterTypeDef",
     "ListPendingInvitationResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
+    "ListPermissionAssociationsRequestRequestTypeDef",
     "ListPermissionVersionsRequestRequestTypeDef",
-    "ResourceSharePermissionSummaryTypeDef",
     "ListPermissionsRequestRequestTypeDef",
+    "ListPrincipalsRequestListPrincipalsPaginateTypeDef",
     "ListPrincipalsRequestRequestTypeDef",
     "PrincipalTypeDef",
+    "ListReplacePermissionAssociationsWorkRequestRequestTypeDef",
+    "ReplacePermissionAssociationsWorkTypeDef",
     "ListResourceSharePermissionsRequestRequestTypeDef",
     "ListResourceTypesRequestRequestTypeDef",
     "ServiceNameAndResourceTypeTypeDef",
+    "ListResourcesRequestListResourcesPaginateTypeDef",
     "ListResourcesRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "PromotePermissionCreatedFromPolicyRequestRequestTypeDef",
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
+    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
     "RejectResourceShareInvitationRequestRequestTypeDef",
+    "ReplacePermissionAssociationsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "SetDefaultPermissionVersionRequestRequestTypeDef",
+    "SetDefaultPermissionVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateResourceShareRequestRequestTypeDef",
-    "AssociateResourceSharePermissionResponseTypeDef",
-    "DeleteResourceShareResponseTypeDef",
-    "DisassociateResourceSharePermissionResponseTypeDef",
-    "EnableSharingWithAwsOrganizationResponseTypeDef",
-    "GetResourcePoliciesResponseTypeDef",
-    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
     "AssociateResourceShareResponseTypeDef",
     "DisassociateResourceShareResponseTypeDef",
     "GetResourceShareAssociationsResponseTypeDef",
     "ResourceShareInvitationTypeDef",
+    "ListPermissionAssociationsResponseTypeDef",
+    "CreatePermissionRequestRequestTypeDef",
     "CreateResourceShareRequestRequestTypeDef",
+    "ResourceSharePermissionDetailTypeDef",
+    "ResourceSharePermissionSummaryTypeDef",
     "ResourceShareTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "GetPermissionResponseTypeDef",
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    "GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
-    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
-    "ListPrincipalsRequestListPrincipalsPaginateTypeDef",
-    "ListResourcesRequestListResourcesPaginateTypeDef",
     "GetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     "GetResourceSharesRequestRequestTypeDef",
     "ListPendingInvitationResourcesResponseTypeDef",
     "ListResourcesResponseTypeDef",
-    "ListPermissionVersionsResponseTypeDef",
-    "ListPermissionsResponseTypeDef",
-    "ListResourceSharePermissionsResponseTypeDef",
     "ListPrincipalsResponseTypeDef",
+    "ListReplacePermissionAssociationsWorkResponseTypeDef",
+    "ReplacePermissionAssociationsResponseTypeDef",
     "ListResourceTypesResponseTypeDef",
     "AcceptResourceShareInvitationResponseTypeDef",
     "GetResourceShareInvitationsResponseTypeDef",
     "RejectResourceShareInvitationResponseTypeDef",
+    "CreatePermissionVersionResponseTypeDef",
+    "GetPermissionResponseTypeDef",
+    "CreatePermissionResponseTypeDef",
+    "ListPermissionVersionsResponseTypeDef",
+    "ListPermissionsResponseTypeDef",
+    "ListResourceSharePermissionsResponseTypeDef",
+    "PromotePermissionCreatedFromPolicyResponseTypeDef",
     "CreateResourceShareResponseTypeDef",
     "GetResourceSharesResponseTypeDef",
     "UpdateResourceShareResponseTypeDef",
 )
 
 _RequiredAcceptResourceShareInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptResourceShareInvitationRequestRequestTypeDef",
@@ -116,25 +141,14 @@
 
 class AcceptResourceShareInvitationRequestRequestTypeDef(
     _RequiredAcceptResourceShareInvitationRequestRequestTypeDef,
     _OptionalAcceptResourceShareInvitationRequestRequestTypeDef,
 ):
     pass
 
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
 _RequiredAssociateResourceSharePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateResourceSharePermissionRequestRequestTypeDef",
     {
         "resourceShareArn": str,
         "permissionArn": str,
     },
 )
@@ -150,14 +164,23 @@
 
 class AssociateResourceSharePermissionRequestRequestTypeDef(
     _RequiredAssociateResourceSharePermissionRequestRequestTypeDef,
     _OptionalAssociateResourceSharePermissionRequestRequestTypeDef,
 ):
     pass
 
+AssociateResourceSharePermissionResponseTypeDef = TypedDict(
+    "AssociateResourceSharePermissionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAssociateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalAssociateResourceShareRequestRequestTypeDef = TypedDict(
@@ -188,23 +211,119 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "external": bool,
     },
     total=False,
 )
 
+AssociatedPermissionTypeDef = TypedDict(
+    "AssociatedPermissionTypeDef",
+    {
+        "arn": str,
+        "permissionVersion": str,
+        "defaultVersion": bool,
+        "resourceType": str,
+        "status": str,
+        "featureSet": PermissionFeatureSetType,
+        "lastUpdatedTime": datetime,
+        "resourceShareArn": str,
+    },
+    total=False,
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
+_RequiredCreatePermissionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePermissionVersionRequestRequestTypeDef",
+    {
+        "permissionArn": str,
+        "policyTemplate": str,
+    },
+)
+_OptionalCreatePermissionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePermissionVersionRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class CreatePermissionVersionRequestRequestTypeDef(
+    _RequiredCreatePermissionVersionRequestRequestTypeDef,
+    _OptionalCreatePermissionVersionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDeletePermissionRequestRequestTypeDef = TypedDict(
+    "_RequiredDeletePermissionRequestRequestTypeDef",
+    {
+        "permissionArn": str,
+    },
+)
+_OptionalDeletePermissionRequestRequestTypeDef = TypedDict(
+    "_OptionalDeletePermissionRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class DeletePermissionRequestRequestTypeDef(
+    _RequiredDeletePermissionRequestRequestTypeDef, _OptionalDeletePermissionRequestRequestTypeDef
+):
+    pass
+
+DeletePermissionResponseTypeDef = TypedDict(
+    "DeletePermissionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "permissionStatus": PermissionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDeletePermissionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredDeletePermissionVersionRequestRequestTypeDef",
+    {
+        "permissionArn": str,
+        "permissionVersion": int,
+    },
+)
+_OptionalDeletePermissionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalDeletePermissionVersionRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class DeletePermissionVersionRequestRequestTypeDef(
+    _RequiredDeletePermissionVersionRequestRequestTypeDef,
+    _OptionalDeletePermissionVersionRequestRequestTypeDef,
+):
+    pass
+
+DeletePermissionVersionResponseTypeDef = TypedDict(
+    "DeletePermissionVersionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "permissionStatus": PermissionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalDeleteResourceShareRequestRequestTypeDef = TypedDict(
@@ -217,14 +336,23 @@
 
 class DeleteResourceShareRequestRequestTypeDef(
     _RequiredDeleteResourceShareRequestRequestTypeDef,
     _OptionalDeleteResourceShareRequestRequestTypeDef,
 ):
     pass
 
+DeleteResourceShareResponseTypeDef = TypedDict(
+    "DeleteResourceShareResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDisassociateResourceSharePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateResourceSharePermissionRequestRequestTypeDef",
     {
         "resourceShareArn": str,
         "permissionArn": str,
     },
 )
@@ -238,14 +366,23 @@
 
 class DisassociateResourceSharePermissionRequestRequestTypeDef(
     _RequiredDisassociateResourceSharePermissionRequestRequestTypeDef,
     _OptionalDisassociateResourceSharePermissionRequestRequestTypeDef,
 ):
     pass
 
+DisassociateResourceSharePermissionResponseTypeDef = TypedDict(
+    "DisassociateResourceSharePermissionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDisassociateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalDisassociateResourceShareRequestRequestTypeDef = TypedDict(
@@ -260,14 +397,22 @@
 
 class DisassociateResourceShareRequestRequestTypeDef(
     _RequiredDisassociateResourceShareRequestRequestTypeDef,
     _OptionalDisassociateResourceShareRequestRequestTypeDef,
 ):
     pass
 
+EnableSharingWithAwsOrganizationResponseTypeDef = TypedDict(
+    "EnableSharingWithAwsOrganizationResponseTypeDef",
+    {
+        "returnValue": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredGetPermissionRequestRequestTypeDef",
     {
         "permissionArn": str,
     },
 )
 _OptionalGetPermissionRequestRequestTypeDef = TypedDict(
@@ -279,40 +424,35 @@
 )
 
 class GetPermissionRequestRequestTypeDef(
     _RequiredGetPermissionRequestRequestTypeDef, _OptionalGetPermissionRequestRequestTypeDef
 ):
     pass
 
-ResourceSharePermissionDetailTypeDef = TypedDict(
-    "ResourceSharePermissionDetailTypeDef",
+_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "permission": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
+        "resourceArns": Sequence[str],
     },
-    total=False,
 )
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "principal": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "resourceArns": Sequence[str],
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -327,14 +467,47 @@
 
 class GetResourcePoliciesRequestRequestTypeDef(
     _RequiredGetResourcePoliciesRequestRequestTypeDef,
     _OptionalGetResourcePoliciesRequestRequestTypeDef,
 ):
     pass
 
+GetResourcePoliciesResponseTypeDef = TypedDict(
+    "GetResourcePoliciesResponseTypeDef",
+    {
+        "policies": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
+    {
+        "associationType": ResourceShareAssociationTypeType,
+    },
+)
+_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
+    {
+        "resourceShareArns": Sequence[str],
+        "resourceArn": str,
+        "principal": str,
+        "associationStatus": ResourceShareAssociationStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef(
+    _RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
+    _OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetResourceShareAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceShareAssociationsRequestRequestTypeDef",
     {
         "associationType": ResourceShareAssociationTypeType,
     },
 )
 _OptionalGetResourceShareAssociationsRequestRequestTypeDef = TypedDict(
@@ -352,14 +525,24 @@
 
 class GetResourceShareAssociationsRequestRequestTypeDef(
     _RequiredGetResourceShareAssociationsRequestRequestTypeDef,
     _OptionalGetResourceShareAssociationsRequestRequestTypeDef,
 ):
     pass
 
+GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef = TypedDict(
+    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
+    {
+        "resourceShareInvitationArns": Sequence[str],
+        "resourceShareArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetResourceShareInvitationsRequestRequestTypeDef = TypedDict(
     "GetResourceShareInvitationsRequestRequestTypeDef",
     {
         "resourceShareInvitationArns": Sequence[str],
         "resourceShareArns": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -410,14 +593,29 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "resourceRegionScope": ResourceRegionScopeType,
     },
     total=False,
 )
 
+ListPermissionAssociationsRequestRequestTypeDef = TypedDict(
+    "ListPermissionAssociationsRequestRequestTypeDef",
+    {
+        "permissionArn": str,
+        "permissionVersion": int,
+        "associationStatus": ResourceShareAssociationStatusType,
+        "resourceType": str,
+        "featureSet": PermissionFeatureSetType,
+        "defaultVersion": bool,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
 _RequiredListPermissionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionVersionsRequestRequestTypeDef",
     {
         "permissionArn": str,
     },
 )
 _OptionalListPermissionVersionsRequestRequestTypeDef = TypedDict(
@@ -431,40 +629,49 @@
 
 class ListPermissionVersionsRequestRequestTypeDef(
     _RequiredListPermissionVersionsRequestRequestTypeDef,
     _OptionalListPermissionVersionsRequestRequestTypeDef,
 ):
     pass
 
-ResourceSharePermissionSummaryTypeDef = TypedDict(
-    "ResourceSharePermissionSummaryTypeDef",
+ListPermissionsRequestRequestTypeDef = TypedDict(
+    "ListPermissionsRequestRequestTypeDef",
     {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
         "resourceType": str,
-        "status": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
+        "nextToken": str,
+        "maxResults": int,
+        "permissionType": PermissionTypeFilterType,
     },
     total=False,
 )
 
-ListPermissionsRequestRequestTypeDef = TypedDict(
-    "ListPermissionsRequestRequestTypeDef",
+_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef",
+    {
+        "resourceOwner": ResourceOwnerType,
+    },
+)
+_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef",
     {
+        "resourceArn": str,
+        "principals": Sequence[str],
         "resourceType": str,
-        "nextToken": str,
-        "maxResults": int,
+        "resourceShareArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListPrincipalsRequestListPrincipalsPaginateTypeDef(
+    _RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef,
+    _OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef,
+):
+    pass
+
 _RequiredListPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalsRequestRequestTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
     },
 )
 _OptionalListPrincipalsRequestRequestTypeDef = TypedDict(
@@ -493,14 +700,41 @@
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
         "external": bool,
     },
     total=False,
 )
 
+ListReplacePermissionAssociationsWorkRequestRequestTypeDef = TypedDict(
+    "ListReplacePermissionAssociationsWorkRequestRequestTypeDef",
+    {
+        "workIds": Sequence[str],
+        "status": ReplacePermissionAssociationsWorkStatusType,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+ReplacePermissionAssociationsWorkTypeDef = TypedDict(
+    "ReplacePermissionAssociationsWorkTypeDef",
+    {
+        "id": str,
+        "fromPermissionArn": str,
+        "fromPermissionVersion": str,
+        "toPermissionArn": str,
+        "toPermissionVersion": str,
+        "status": ReplacePermissionAssociationsWorkStatusType,
+        "statusMessage": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredListResourceSharePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceSharePermissionsRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalListResourceSharePermissionsRequestRequestTypeDef = TypedDict(
@@ -534,14 +768,39 @@
         "resourceType": str,
         "serviceName": str,
         "resourceRegionScope": ResourceRegionScopeType,
     },
     total=False,
 )
 
+_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "resourceOwner": ResourceOwnerType,
+    },
+)
+_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "principal": str,
+        "resourceType": str,
+        "resourceArns": Sequence[str],
+        "resourceShareArns": Sequence[str],
+        "resourceRegionScope": ResourceRegionScopeFilterType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListResourcesRequestListResourcesPaginateTypeDef(
+    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
+    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -559,21 +818,60 @@
 )
 
 class ListResourcesRequestRequestTypeDef(
     _RequiredListResourcesRequestRequestTypeDef, _OptionalListResourcesRequestRequestTypeDef
 ):
     pass
 
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
+_RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef",
+    {
+        "permissionArn": str,
+        "name": str,
+    },
+)
+_OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class PromotePermissionCreatedFromPolicyRequestRequestTypeDef(
+    _RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef,
+    _OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef,
+):
+    pass
+
 PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef = TypedDict(
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 
+PromoteResourceShareCreatedFromPolicyResponseTypeDef = TypedDict(
+    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
+    {
+        "returnValue": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRejectResourceShareInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredRejectResourceShareInvitationRequestRequestTypeDef",
     {
         "resourceShareInvitationArn": str,
     },
 )
 _OptionalRejectResourceShareInvitationRequestRequestTypeDef = TypedDict(
@@ -586,120 +884,143 @@
 
 class RejectResourceShareInvitationRequestRequestTypeDef(
     _RequiredRejectResourceShareInvitationRequestRequestTypeDef,
     _OptionalRejectResourceShareInvitationRequestRequestTypeDef,
 ):
     pass
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceShareArn": str,
-        "tagKeys": Sequence[str],
-    },
-)
-
-_RequiredUpdateResourceShareRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateResourceShareRequestRequestTypeDef",
+_RequiredReplacePermissionAssociationsRequestRequestTypeDef = TypedDict(
+    "_RequiredReplacePermissionAssociationsRequestRequestTypeDef",
     {
-        "resourceShareArn": str,
+        "fromPermissionArn": str,
+        "toPermissionArn": str,
     },
 )
-_OptionalUpdateResourceShareRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateResourceShareRequestRequestTypeDef",
+_OptionalReplacePermissionAssociationsRequestRequestTypeDef = TypedDict(
+    "_OptionalReplacePermissionAssociationsRequestRequestTypeDef",
     {
-        "name": str,
-        "allowExternalPrincipals": bool,
+        "fromPermissionVersion": int,
         "clientToken": str,
     },
     total=False,
 )
 
-class UpdateResourceShareRequestRequestTypeDef(
-    _RequiredUpdateResourceShareRequestRequestTypeDef,
-    _OptionalUpdateResourceShareRequestRequestTypeDef,
+class ReplacePermissionAssociationsRequestRequestTypeDef(
+    _RequiredReplacePermissionAssociationsRequestRequestTypeDef,
+    _OptionalReplacePermissionAssociationsRequestRequestTypeDef,
 ):
     pass
 
-AssociateResourceSharePermissionResponseTypeDef = TypedDict(
-    "AssociateResourceSharePermissionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "returnValue": bool,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-DeleteResourceShareResponseTypeDef = TypedDict(
-    "DeleteResourceShareResponseTypeDef",
+_RequiredSetDefaultPermissionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredSetDefaultPermissionVersionRequestRequestTypeDef",
+    {
+        "permissionArn": str,
+        "permissionVersion": int,
+    },
+)
+_OptionalSetDefaultPermissionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalSetDefaultPermissionVersionRequestRequestTypeDef",
     {
-        "returnValue": bool,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-DisassociateResourceSharePermissionResponseTypeDef = TypedDict(
-    "DisassociateResourceSharePermissionResponseTypeDef",
+class SetDefaultPermissionVersionRequestRequestTypeDef(
+    _RequiredSetDefaultPermissionVersionRequestRequestTypeDef,
+    _OptionalSetDefaultPermissionVersionRequestRequestTypeDef,
+):
+    pass
+
+SetDefaultPermissionVersionResponseTypeDef = TypedDict(
+    "SetDefaultPermissionVersionResponseTypeDef",
     {
         "returnValue": bool,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EnableSharingWithAwsOrganizationResponseTypeDef = TypedDict(
-    "EnableSharingWithAwsOrganizationResponseTypeDef",
+_RequiredUntagResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredUntagResourceRequestRequestTypeDef",
     {
-        "returnValue": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tagKeys": Sequence[str],
     },
 )
-
-GetResourcePoliciesResponseTypeDef = TypedDict(
-    "GetResourcePoliciesResponseTypeDef",
+_OptionalUntagResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalUntagResourceRequestRequestTypeDef",
     {
-        "policies": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceShareArn": str,
+        "resourceArn": str,
     },
+    total=False,
 )
 
-PromoteResourceShareCreatedFromPolicyResponseTypeDef = TypedDict(
-    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
+class UntagResourceRequestRequestTypeDef(
+    _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateResourceShareRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateResourceShareRequestRequestTypeDef",
     {
-        "returnValue": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceShareArn": str,
     },
 )
+_OptionalUpdateResourceShareRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateResourceShareRequestRequestTypeDef",
+    {
+        "name": str,
+        "allowExternalPrincipals": bool,
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class UpdateResourceShareRequestRequestTypeDef(
+    _RequiredUpdateResourceShareRequestRequestTypeDef,
+    _OptionalUpdateResourceShareRequestRequestTypeDef,
+):
+    pass
 
 AssociateResourceShareResponseTypeDef = TypedDict(
     "AssociateResourceShareResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateResourceShareResponseTypeDef = TypedDict(
     "DisassociateResourceShareResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceShareAssociationsResponseTypeDef = TypedDict(
     "GetResourceShareAssociationsResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceShareInvitationTypeDef = TypedDict(
     "ResourceShareInvitationTypeDef",
     {
         "resourceShareInvitationArn": str,
@@ -711,14 +1032,45 @@
         "status": ResourceShareInvitationStatusType,
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "receiverArn": str,
     },
     total=False,
 )
 
+ListPermissionAssociationsResponseTypeDef = TypedDict(
+    "ListPermissionAssociationsResponseTypeDef",
+    {
+        "permissions": List[AssociatedPermissionTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreatePermissionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePermissionRequestRequestTypeDef",
+    {
+        "name": str,
+        "resourceType": str,
+        "policyTemplate": str,
+    },
+)
+_OptionalCreatePermissionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePermissionRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreatePermissionRequestRequestTypeDef(
+    _RequiredCreatePermissionRequestRequestTypeDef, _OptionalCreatePermissionRequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceShareRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateResourceShareRequestRequestTypeDef = TypedDict(
@@ -736,148 +1088,87 @@
 
 class CreateResourceShareRequestRequestTypeDef(
     _RequiredCreateResourceShareRequestRequestTypeDef,
     _OptionalCreateResourceShareRequestRequestTypeDef,
 ):
     pass
 
-ResourceShareTypeDef = TypedDict(
-    "ResourceShareTypeDef",
+ResourceSharePermissionDetailTypeDef = TypedDict(
+    "ResourceSharePermissionDetailTypeDef",
     {
-        "resourceShareArn": str,
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
         "name": str,
-        "owningAccountId": str,
-        "allowExternalPrincipals": bool,
-        "status": ResourceShareStatusType,
-        "statusMessage": str,
-        "tags": List[TagTypeDef],
+        "resourceType": str,
+        "permission": str,
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
-        "featureSet": ResourceShareFeatureSetType,
-    },
-    total=False,
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceShareArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
-GetPermissionResponseTypeDef = TypedDict(
-    "GetPermissionResponseTypeDef",
-    {
-        "permission": ResourceSharePermissionDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "resourceArns": Sequence[str],
-    },
-)
-_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "principal": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "isResourceTypeDefault": bool,
+        "permissionType": PermissionTypeType,
+        "featureSet": PermissionFeatureSetType,
+        "status": PermissionStatusType,
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
-class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
-_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
-    {
-        "associationType": ResourceShareAssociationTypeType,
-    },
-)
-_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
+ResourceSharePermissionSummaryTypeDef = TypedDict(
+    "ResourceSharePermissionSummaryTypeDef",
     {
-        "resourceShareArns": Sequence[str],
-        "resourceArn": str,
-        "principal": str,
-        "associationStatus": ResourceShareAssociationStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "status": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+        "permissionType": PermissionTypeType,
+        "featureSet": PermissionFeatureSetType,
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
-class GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef(
-    _RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
-    _OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
-):
-    pass
-
-GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef = TypedDict(
-    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
+ResourceShareTypeDef = TypedDict(
+    "ResourceShareTypeDef",
     {
-        "resourceShareInvitationArns": Sequence[str],
-        "resourceShareArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "resourceShareArn": str,
+        "name": str,
+        "owningAccountId": str,
+        "allowExternalPrincipals": bool,
+        "status": ResourceShareStatusType,
+        "statusMessage": str,
+        "tags": List[TagTypeDef],
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "featureSet": ResourceShareFeatureSetType,
     },
     total=False,
 )
 
-_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef",
+_RequiredTagResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredTagResourceRequestRequestTypeDef",
     {
-        "resourceOwner": ResourceOwnerType,
+        "tags": Sequence[TagTypeDef],
     },
 )
-_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef",
+_OptionalTagResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalTagResourceRequestRequestTypeDef",
     {
+        "resourceShareArn": str,
         "resourceArn": str,
-        "principals": Sequence[str],
-        "resourceType": str,
-        "resourceShareArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPrincipalsRequestListPrincipalsPaginateTypeDef(
-    _RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef,
-    _OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef,
-):
-    pass
-
-_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "resourceOwner": ResourceOwnerType,
-    },
-)
-_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "principal": str,
-        "resourceType": str,
-        "resourceArns": Sequence[str],
-        "resourceShareArns": Sequence[str],
-        "resourceRegionScope": ResourceRegionScopeFilterType,
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListResourcesRequestListResourcesPaginateTypeDef(
-    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
-    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
+class TagResourceRequestRequestTypeDef(
+    _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
 _RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef = TypedDict(
     "_RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
@@ -887,15 +1178,16 @@
     "_OptionalGetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     {
         "resourceShareArns": Sequence[str],
         "resourceShareStatus": ResourceShareStatusType,
         "name": str,
         "tagFilters": Sequence[TagFilterTypeDef],
         "permissionArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "permissionVersion": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class GetResourceSharesRequestGetResourceSharesPaginateTypeDef(
     _RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     _OptionalGetResourceSharesRequestGetResourceSharesPaginateTypeDef,
@@ -914,132 +1206,186 @@
         "resourceShareArns": Sequence[str],
         "resourceShareStatus": ResourceShareStatusType,
         "name": str,
         "tagFilters": Sequence[TagFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
         "permissionArn": str,
+        "permissionVersion": int,
     },
     total=False,
 )
 
 class GetResourceSharesRequestRequestTypeDef(
     _RequiredGetResourceSharesRequestRequestTypeDef, _OptionalGetResourceSharesRequestRequestTypeDef
 ):
     pass
 
 ListPendingInvitationResourcesResponseTypeDef = TypedDict(
     "ListPendingInvitationResourcesResponseTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPermissionVersionsResponseTypeDef = TypedDict(
-    "ListPermissionVersionsResponseTypeDef",
-    {
-        "permissions": List[ResourceSharePermissionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPermissionsResponseTypeDef = TypedDict(
-    "ListPermissionsResponseTypeDef",
+ListPrincipalsResponseTypeDef = TypedDict(
+    "ListPrincipalsResponseTypeDef",
     {
-        "permissions": List[ResourceSharePermissionSummaryTypeDef],
+        "principals": List[PrincipalTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListResourceSharePermissionsResponseTypeDef = TypedDict(
-    "ListResourceSharePermissionsResponseTypeDef",
+ListReplacePermissionAssociationsWorkResponseTypeDef = TypedDict(
+    "ListReplacePermissionAssociationsWorkResponseTypeDef",
     {
-        "permissions": List[ResourceSharePermissionSummaryTypeDef],
+        "replacePermissionAssociationsWorks": List[ReplacePermissionAssociationsWorkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPrincipalsResponseTypeDef = TypedDict(
-    "ListPrincipalsResponseTypeDef",
+ReplacePermissionAssociationsResponseTypeDef = TypedDict(
+    "ReplacePermissionAssociationsResponseTypeDef",
     {
-        "principals": List[PrincipalTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "replacePermissionAssociationsWork": ReplacePermissionAssociationsWorkTypeDef,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceTypesResponseTypeDef = TypedDict(
     "ListResourceTypesResponseTypeDef",
     {
         "resourceTypes": List[ServiceNameAndResourceTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AcceptResourceShareInvitationResponseTypeDef = TypedDict(
     "AcceptResourceShareInvitationResponseTypeDef",
     {
         "resourceShareInvitation": ResourceShareInvitationTypeDef,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceShareInvitationsResponseTypeDef = TypedDict(
     "GetResourceShareInvitationsResponseTypeDef",
     {
         "resourceShareInvitations": List[ResourceShareInvitationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RejectResourceShareInvitationResponseTypeDef = TypedDict(
     "RejectResourceShareInvitationResponseTypeDef",
     {
         "resourceShareInvitation": ResourceShareInvitationTypeDef,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePermissionVersionResponseTypeDef = TypedDict(
+    "CreatePermissionVersionResponseTypeDef",
+    {
+        "permission": ResourceSharePermissionDetailTypeDef,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetPermissionResponseTypeDef = TypedDict(
+    "GetPermissionResponseTypeDef",
+    {
+        "permission": ResourceSharePermissionDetailTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePermissionResponseTypeDef = TypedDict(
+    "CreatePermissionResponseTypeDef",
+    {
+        "permission": ResourceSharePermissionSummaryTypeDef,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPermissionVersionsResponseTypeDef = TypedDict(
+    "ListPermissionVersionsResponseTypeDef",
+    {
+        "permissions": List[ResourceSharePermissionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPermissionsResponseTypeDef = TypedDict(
+    "ListPermissionsResponseTypeDef",
+    {
+        "permissions": List[ResourceSharePermissionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListResourceSharePermissionsResponseTypeDef = TypedDict(
+    "ListResourceSharePermissionsResponseTypeDef",
+    {
+        "permissions": List[ResourceSharePermissionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PromotePermissionCreatedFromPolicyResponseTypeDef = TypedDict(
+    "PromotePermissionCreatedFromPolicyResponseTypeDef",
+    {
+        "permission": ResourceSharePermissionSummaryTypeDef,
+        "clientToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateResourceShareResponseTypeDef = TypedDict(
     "CreateResourceShareResponseTypeDef",
     {
         "resourceShare": ResourceShareTypeDef,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceSharesResponseTypeDef = TypedDict(
     "GetResourceSharesResponseTypeDef",
     {
         "resourceShares": List[ResourceShareTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateResourceShareResponseTypeDef = TypedDict(
     "UpdateResourceShareResponseTypeDef",
     {
         "resourceShare": ResourceShareTypeDef,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/PKG-INFO` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ram
-Version: 1.26.46
-Summary: Type annotations for boto3.RAM 1.26.46 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.RAM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ram"></a>
 
 # mypy-boto3-ram
 
 [![PyPI - mypy-boto3-ram](https://img.shields.io/pypi/v/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ram?color=blue)](https://pypistats.org/packages/mypy-boto3-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RAM 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[boto3.RAM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ram docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,14 +321,19 @@
 from mypy_boto3_ram.literals import (
     GetResourcePoliciesPaginatorName,
     GetResourceShareAssociationsPaginatorName,
     GetResourceShareInvitationsPaginatorName,
     GetResourceSharesPaginatorName,
     ListPrincipalsPaginatorName,
     ListResourcesPaginatorName,
+    PermissionFeatureSetType,
+    PermissionStatusType,
+    PermissionTypeFilterType,
+    PermissionTypeType,
+    ReplacePermissionAssociationsWorkStatusType,
     ResourceOwnerType,
     ResourceRegionScopeFilterType,
     ResourceRegionScopeType,
     ResourceShareAssociationStatusType,
     ResourceShareAssociationTypeType,
     ResourceShareFeatureSetType,
     ResourceShareInvitationStatusType,
@@ -352,75 +357,95 @@
 
 `mypy_boto3_ram.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ram.type_defs import (
     AcceptResourceShareInvitationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AssociateResourceSharePermissionRequestRequestTypeDef,
+    AssociateResourceSharePermissionResponseTypeDef,
     AssociateResourceShareRequestRequestTypeDef,
     ResourceShareAssociationTypeDef,
+    AssociatedPermissionTypeDef,
     TagTypeDef,
+    CreatePermissionVersionRequestRequestTypeDef,
+    DeletePermissionRequestRequestTypeDef,
+    DeletePermissionResponseTypeDef,
+    DeletePermissionVersionRequestRequestTypeDef,
+    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareRequestRequestTypeDef,
+    DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionRequestRequestTypeDef,
+    DisassociateResourceSharePermissionResponseTypeDef,
     DisassociateResourceShareRequestRequestTypeDef,
+    EnableSharingWithAwsOrganizationResponseTypeDef,
     GetPermissionRequestRequestTypeDef,
-    ResourceSharePermissionDetailTypeDef,
-    PaginatorConfigTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
+    GetResourcePoliciesResponseTypeDef,
+    GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
     GetResourceShareAssociationsRequestRequestTypeDef,
+    GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
     GetResourceShareInvitationsRequestRequestTypeDef,
     TagFilterTypeDef,
     ListPendingInvitationResourcesRequestRequestTypeDef,
     ResourceTypeDef,
+    ListPermissionAssociationsRequestRequestTypeDef,
     ListPermissionVersionsRequestRequestTypeDef,
-    ResourceSharePermissionSummaryTypeDef,
     ListPermissionsRequestRequestTypeDef,
+    ListPrincipalsRequestListPrincipalsPaginateTypeDef,
     ListPrincipalsRequestRequestTypeDef,
     PrincipalTypeDef,
+    ListReplacePermissionAssociationsWorkRequestRequestTypeDef,
+    ReplacePermissionAssociationsWorkTypeDef,
     ListResourceSharePermissionsRequestRequestTypeDef,
     ListResourceTypesRequestRequestTypeDef,
     ServiceNameAndResourceTypeTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    PromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef,
+    PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     RejectResourceShareInvitationRequestRequestTypeDef,
+    ReplacePermissionAssociationsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    SetDefaultPermissionVersionRequestRequestTypeDef,
+    SetDefaultPermissionVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateResourceShareRequestRequestTypeDef,
-    AssociateResourceSharePermissionResponseTypeDef,
-    DeleteResourceShareResponseTypeDef,
-    DisassociateResourceSharePermissionResponseTypeDef,
-    EnableSharingWithAwsOrganizationResponseTypeDef,
-    GetResourcePoliciesResponseTypeDef,
-    PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     ResourceShareInvitationTypeDef,
+    ListPermissionAssociationsResponseTypeDef,
+    CreatePermissionRequestRequestTypeDef,
     CreateResourceShareRequestRequestTypeDef,
+    ResourceSharePermissionDetailTypeDef,
+    ResourceSharePermissionSummaryTypeDef,
     ResourceShareTypeDef,
     TagResourceRequestRequestTypeDef,
-    GetPermissionResponseTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
-    GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
-    ListPrincipalsRequestListPrincipalsPaginateTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     GetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     GetResourceSharesRequestRequestTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
     ListResourcesResponseTypeDef,
-    ListPermissionVersionsResponseTypeDef,
-    ListPermissionsResponseTypeDef,
-    ListResourceSharePermissionsResponseTypeDef,
     ListPrincipalsResponseTypeDef,
+    ListReplacePermissionAssociationsWorkResponseTypeDef,
+    ReplacePermissionAssociationsResponseTypeDef,
     ListResourceTypesResponseTypeDef,
     AcceptResourceShareInvitationResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
+    CreatePermissionVersionResponseTypeDef,
+    GetPermissionResponseTypeDef,
+    CreatePermissionResponseTypeDef,
+    ListPermissionVersionsResponseTypeDef,
+    ListPermissionsResponseTypeDef,
+    ListResourceSharePermissionsResponseTypeDef,
+    PromotePermissionCreatedFromPolicyResponseTypeDef,
     CreateResourceShareResponseTypeDef,
     GetResourceSharesResponseTypeDef,
     UpdateResourceShareResponseTypeDef,
 )
 
 
 def get_structure() -> AcceptResourceShareInvitationRequestRequestTypeDef:
@@ -430,42 +455,42 @@
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

### Comparing `mypy-boto3-ram-1.26.46/mypy_boto3_ram.egg-info/SOURCES.txt` & `mypy-boto3-ram-1.27.0/mypy_boto3_ram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.26.46/setup.py` & `mypy-boto3-ram-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-ram.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ram",
-    version="1.26.46",
+    version="1.27.0",
     packages=["mypy_boto3_ram"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RAM 1.26.46 service generated with mypy-boto3-builder 7.12.2"
+        "Type annotations for boto3.RAM 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/",
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


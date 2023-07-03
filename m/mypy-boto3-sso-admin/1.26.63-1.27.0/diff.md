# Comparing `tmp/mypy-boto3-sso-admin-1.26.63.tar.gz` & `tmp/mypy-boto3-sso-admin-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sso-admin-1.26.63.tar", last modified: Thu Feb  2 20:49:29 2023, max compression
+gzip compressed data, was "mypy-boto3-sso-admin-1.27.0.tar", last modified: Mon Jul  3 19:51:31 2023, max compression
```

## Comparing `mypy-boto3-sso-admin-1.26.63.tar` & `mypy-boto3-sso-admin-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:49:29.754340 mypy-boto3-sso-admin-1.26.63/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-02-02 20:49:29.754340 mypy-boto3-sso-admin-1.26.63/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18891 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:49:29.754340 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34842 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34787 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-02-02 20:49:16.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39766 2023-02-02 20:49:16.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39717 2023-02-02 20:49:16.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:49:29.754340 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-02-02 20:49:29.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-02-02 20:49:29.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 20:49:29.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 20:49:29.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-02 20:49:29.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-02 20:49:29.000000 mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 20:49:29.754340 mypy-boto3-sso-admin-1.26.63/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-02-02 20:49:15.000000 mypy-boto3-sso-admin-1.26.63/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:31.036057 mypy-boto3-sso-admin-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-07-03 19:51:31.036057 mypy-boto3-sso-admin-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18871 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:31.036057 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34841 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34786 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-07-03 19:48:45.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39832 2023-07-03 19:48:45.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39783 2023-07-03 19:48:45.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:31.036057 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-07-03 19:51:30.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:51:30.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:30.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:30.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:30.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:51:30.000000 mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:31.036057 mypy-boto3-sso-admin-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-03 19:48:44.000000 mypy-boto3-sso-admin-1.27.0/setup.py
```

### Comparing `mypy-boto3-sso-admin-1.26.63/LICENSE` & `mypy-boto3-sso-admin-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-sso-admin-1.26.63/PKG-INFO` & `mypy-boto3-sso-admin-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-admin
-Version: 1.26.63
-Summary: Type annotations for boto3.SSOAdmin 1.26.63 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.SSOAdmin 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sso-admin"></a>
 
 # mypy-boto3-sso-admin
 
 [![PyPI - mypy-boto3-sso-admin](https://img.shields.io/pypi/v/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso-admin?color=blue)](https://pypistats.org/packages/mypy-boto3-sso-admin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOAdmin 1.26.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
+[boto3.SSOAdmin 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
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
 [mypy-boto3-sso-admin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -384,15 +384,14 @@
     AccountAssignmentOperationStatusMetadataTypeDef,
     AccountAssignmentOperationStatusTypeDef,
     AccountAssignmentTypeDef,
     CustomerManagedPolicyReferenceTypeDef,
     AttachManagedPolicyToPermissionSetRequestRequestTypeDef,
     AttachedManagedPolicyTypeDef,
     CreateAccountAssignmentRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     PermissionSetTypeDef,
     DeleteAccountAssignmentRequestRequestTypeDef,
     DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef,
     DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DeletePermissionSetRequestRequestTypeDef,
     DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef,
@@ -400,70 +399,71 @@
     DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DescribePermissionSetProvisioningStatusRequestRequestTypeDef,
     PermissionSetProvisioningStatusTypeDef,
     DescribePermissionSetRequestRequestTypeDef,
     DetachManagedPolicyFromPermissionSetRequestRequestTypeDef,
     GetInlinePolicyForPermissionSetRequestRequestTypeDef,
+    GetInlinePolicyForPermissionSetResponseTypeDef,
     GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef,
     InstanceMetadataTypeDef,
     OperationStatusFilterTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
     ListAccountAssignmentsRequestRequestTypeDef,
+    ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
     ListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
+    ListAccountsForProvisionedPermissionSetResponseTypeDef,
+    ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
+    ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
     ListManagedPoliciesInPermissionSetRequestRequestTypeDef,
     PermissionSetProvisioningStatusMetadataTypeDef,
+    ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
     ListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
+    ListPermissionSetsProvisionedToAccountResponseTypeDef,
+    ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
     ListPermissionSetsRequestRequestTypeDef,
+    ListPermissionSetsResponseTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ProvisionPermissionSetRequestRequestTypeDef,
     PutInlinePolicyToPermissionSetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePermissionSetRequestRequestTypeDef,
     AccessControlAttributeTypeDef,
-    AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
-    DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef,
-    PermissionsBoundaryTypeDef,
+    ListAccountAssignmentCreationStatusResponseTypeDef,
+    ListAccountAssignmentDeletionStatusResponseTypeDef,
     CreateAccountAssignmentResponseTypeDef,
     DeleteAccountAssignmentResponseTypeDef,
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
-    GetInlinePolicyForPermissionSetResponseTypeDef,
-    ListAccountAssignmentCreationStatusResponseTypeDef,
-    ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
-    ListAccountsForProvisionedPermissionSetResponseTypeDef,
+    AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
+    DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
+    PermissionsBoundaryTypeDef,
     ListManagedPoliciesInPermissionSetResponseTypeDef,
-    ListPermissionSetsProvisionedToAccountResponseTypeDef,
-    ListPermissionSetsResponseTypeDef,
     CreatePermissionSetRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreatePermissionSetResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     ProvisionPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
-    ListAccountAssignmentCreationStatusRequestRequestTypeDef,
-    ListAccountAssignmentDeletionStatusRequestRequestTypeDef,
-    ListPermissionSetProvisioningStatusRequestRequestTypeDef,
     ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+    ListAccountAssignmentCreationStatusRequestRequestTypeDef,
     ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
-    ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
-    ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
-    ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
-    ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+    ListAccountAssignmentDeletionStatusRequestRequestTypeDef,
     ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
-    ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
-    ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListPermissionSetProvisioningStatusRequestRequestTypeDef,
     ListPermissionSetProvisioningStatusResponseTypeDef,
     InstanceAccessControlAttributeConfigurationTypeDef,
     GetPermissionsBoundaryForPermissionSetResponseTypeDef,
     PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef,
     CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
     UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
@@ -477,42 +477,42 @@
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

### Comparing `mypy-boto3-sso-admin-1.26.63/README.md` & `mypy-boto3-sso-admin-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sso-admin"></a>
 
 # mypy-boto3-sso-admin
 
 [![PyPI - mypy-boto3-sso-admin](https://img.shields.io/pypi/v/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso-admin?color=blue)](https://pypistats.org/packages/mypy-boto3-sso-admin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOAdmin 1.26.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
+[boto3.SSOAdmin 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
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
 [mypy-boto3-sso-admin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,15 +352,14 @@
     AccountAssignmentOperationStatusMetadataTypeDef,
     AccountAssignmentOperationStatusTypeDef,
     AccountAssignmentTypeDef,
     CustomerManagedPolicyReferenceTypeDef,
     AttachManagedPolicyToPermissionSetRequestRequestTypeDef,
     AttachedManagedPolicyTypeDef,
     CreateAccountAssignmentRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     PermissionSetTypeDef,
     DeleteAccountAssignmentRequestRequestTypeDef,
     DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef,
     DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DeletePermissionSetRequestRequestTypeDef,
     DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef,
@@ -368,70 +367,71 @@
     DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DescribePermissionSetProvisioningStatusRequestRequestTypeDef,
     PermissionSetProvisioningStatusTypeDef,
     DescribePermissionSetRequestRequestTypeDef,
     DetachManagedPolicyFromPermissionSetRequestRequestTypeDef,
     GetInlinePolicyForPermissionSetRequestRequestTypeDef,
+    GetInlinePolicyForPermissionSetResponseTypeDef,
     GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef,
     InstanceMetadataTypeDef,
     OperationStatusFilterTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
     ListAccountAssignmentsRequestRequestTypeDef,
+    ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
     ListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
+    ListAccountsForProvisionedPermissionSetResponseTypeDef,
+    ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
+    ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
     ListManagedPoliciesInPermissionSetRequestRequestTypeDef,
     PermissionSetProvisioningStatusMetadataTypeDef,
+    ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
     ListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
+    ListPermissionSetsProvisionedToAccountResponseTypeDef,
+    ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
     ListPermissionSetsRequestRequestTypeDef,
+    ListPermissionSetsResponseTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ProvisionPermissionSetRequestRequestTypeDef,
     PutInlinePolicyToPermissionSetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePermissionSetRequestRequestTypeDef,
     AccessControlAttributeTypeDef,
-    AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
-    DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef,
-    PermissionsBoundaryTypeDef,
+    ListAccountAssignmentCreationStatusResponseTypeDef,
+    ListAccountAssignmentDeletionStatusResponseTypeDef,
     CreateAccountAssignmentResponseTypeDef,
     DeleteAccountAssignmentResponseTypeDef,
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
-    GetInlinePolicyForPermissionSetResponseTypeDef,
-    ListAccountAssignmentCreationStatusResponseTypeDef,
-    ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
-    ListAccountsForProvisionedPermissionSetResponseTypeDef,
+    AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
+    DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
+    PermissionsBoundaryTypeDef,
     ListManagedPoliciesInPermissionSetResponseTypeDef,
-    ListPermissionSetsProvisionedToAccountResponseTypeDef,
-    ListPermissionSetsResponseTypeDef,
     CreatePermissionSetRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreatePermissionSetResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     ProvisionPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
-    ListAccountAssignmentCreationStatusRequestRequestTypeDef,
-    ListAccountAssignmentDeletionStatusRequestRequestTypeDef,
-    ListPermissionSetProvisioningStatusRequestRequestTypeDef,
     ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+    ListAccountAssignmentCreationStatusRequestRequestTypeDef,
     ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
-    ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
-    ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
-    ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
-    ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+    ListAccountAssignmentDeletionStatusRequestRequestTypeDef,
     ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
-    ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
-    ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListPermissionSetProvisioningStatusRequestRequestTypeDef,
     ListPermissionSetProvisioningStatusResponseTypeDef,
     InstanceAccessControlAttributeConfigurationTypeDef,
     GetPermissionsBoundaryForPermissionSetResponseTypeDef,
     PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef,
     CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
     UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
@@ -445,42 +445,42 @@
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

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/__init__.py` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/__init__.pyi` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/__main__.py` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSOAdmin 1.26.63\nVersion:         1.26.63\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.SSOAdmin 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.63")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/client.py` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/client/#list_permission_set_provisioning_status)
         """
 
     def list_permission_sets(
         self, *, InstanceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPermissionSetsResponseTypeDef:
         """
-        Lists the  PermissionSet s in an IAM Identity Center instance.
+        Lists the  PermissionSets in an IAM Identity Center instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_permission_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/client/#list_permission_sets)
         """
 
     def list_permission_sets_provisioned_to_account(
         self,
```

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/client.pyi` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -451,15 +451,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_permission_set_provisioning_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/client/#list_permission_set_provisioning_status)
         """
     def list_permission_sets(
         self, *, InstanceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPermissionSetsResponseTypeDef:
         """
-        Lists the  PermissionSet s in an IAM Identity Center instance.
+        Lists the  PermissionSets in an IAM Identity Center instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.list_permission_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/client/#list_permission_sets)
         """
     def list_permission_sets_provisioned_to_account(
         self,
         *,
```

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/literals.py` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
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
@@ -137,14 +138,15 @@
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
@@ -223,14 +225,15 @@
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
@@ -241,14 +244,15 @@
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
@@ -284,14 +288,15 @@
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
@@ -310,16 +315,19 @@
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
@@ -399,18 +407,21 @@
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

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/literals.pyi` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
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
@@ -135,14 +136,15 @@
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
@@ -221,14 +223,15 @@
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
@@ -239,14 +242,15 @@
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
@@ -282,14 +286,15 @@
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
@@ -308,16 +313,19 @@
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
@@ -397,18 +405,21 @@
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

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/paginator.py` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountAssignmentCreationStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentCreationStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountassignmentcreationstatuspaginator)
         """
 
 
@@ -111,15 +111,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountAssignmentDeletionStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentDeletionStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountassignmentdeletionstatuspaginator)
         """
 
 
@@ -131,15 +131,15 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         AccountId: str,
         PermissionSetArn: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountAssignmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountassignmentspaginator)
         """
 
 
@@ -151,15 +151,15 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         ProvisioningStatus: ProvisioningStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountsForProvisionedPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountsForProvisionedPermissionSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountsforprovisionedpermissionsetpaginator)
         """
 
 
@@ -170,30 +170,30 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListCustomerManagedPolicyReferencesInPermissionSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listcustomermanagedpolicyreferencesinpermissionsetpaginator)
         """
 
 
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listinstancespaginator)
         """
 
 
@@ -204,15 +204,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListManagedPoliciesInPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListManagedPoliciesInPermissionSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listmanagedpoliciesinpermissionsetpaginator)
         """
 
 
@@ -223,30 +223,30 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPermissionSetProvisioningStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetProvisioningStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetprovisioningstatuspaginator)
         """
 
 
 class ListPermissionSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetspaginator)
     """
 
     def paginate(
-        self, *, InstanceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InstanceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPermissionSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetspaginator)
         """
 
 
@@ -258,28 +258,32 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         AccountId: str,
         ProvisioningStatus: ProvisioningStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPermissionSetsProvisionedToAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetsProvisionedToAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetsprovisionedtoaccountpaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, InstanceArn: str, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        InstanceArn: str,
+        ResourceArn: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/paginator.pyi` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountAssignmentCreationStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentCreationStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountassignmentcreationstatuspaginator)
         """
 
 class ListAccountAssignmentDeletionStatusPaginator(Paginator):
@@ -107,15 +107,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountAssignmentDeletionStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentDeletionStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountassignmentdeletionstatuspaginator)
         """
 
 class ListAccountAssignmentsPaginator(Paginator):
@@ -126,15 +126,15 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         AccountId: str,
         PermissionSetArn: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountAssignmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountassignmentspaginator)
         """
 
 class ListAccountsForProvisionedPermissionSetPaginator(Paginator):
@@ -145,15 +145,15 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         ProvisioningStatus: ProvisioningStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountsForProvisionedPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountsForProvisionedPermissionSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountsforprovisionedpermissionsetpaginator)
         """
 
 class ListCustomerManagedPolicyReferencesInPermissionSetPaginator(Paginator):
@@ -163,29 +163,29 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListCustomerManagedPolicyReferencesInPermissionSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listcustomermanagedpolicyreferencesinpermissionsetpaginator)
         """
 
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listinstancespaginator)
         """
 
 class ListManagedPoliciesInPermissionSetPaginator(Paginator):
@@ -195,15 +195,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListManagedPoliciesInPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListManagedPoliciesInPermissionSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listmanagedpoliciesinpermissionsetpaginator)
         """
 
 class ListPermissionSetProvisioningStatusPaginator(Paginator):
@@ -213,29 +213,29 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPermissionSetProvisioningStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetProvisioningStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetprovisioningstatuspaginator)
         """
 
 class ListPermissionSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetspaginator)
     """
 
     def paginate(
-        self, *, InstanceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InstanceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPermissionSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetspaginator)
         """
 
 class ListPermissionSetsProvisionedToAccountPaginator(Paginator):
@@ -246,27 +246,31 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         AccountId: str,
         ProvisioningStatus: ProvisioningStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPermissionSetsProvisionedToAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetsProvisionedToAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetsprovisionedtoaccountpaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, InstanceArn: str, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        InstanceArn: str,
+        ResourceArn: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/type_defs.py` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     "AccountAssignmentOperationStatusMetadataTypeDef",
     "AccountAssignmentOperationStatusTypeDef",
     "AccountAssignmentTypeDef",
     "CustomerManagedPolicyReferenceTypeDef",
     "AttachManagedPolicyToPermissionSetRequestRequestTypeDef",
     "AttachedManagedPolicyTypeDef",
     "CreateAccountAssignmentRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "PermissionSetTypeDef",
     "DeleteAccountAssignmentRequestRequestTypeDef",
     "DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef",
     "DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "DeletePermissionSetRequestRequestTypeDef",
     "DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef",
@@ -54,70 +53,71 @@
     "DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef",
     "DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "DescribePermissionSetProvisioningStatusRequestRequestTypeDef",
     "PermissionSetProvisioningStatusTypeDef",
     "DescribePermissionSetRequestRequestTypeDef",
     "DetachManagedPolicyFromPermissionSetRequestRequestTypeDef",
     "GetInlinePolicyForPermissionSetRequestRequestTypeDef",
+    "GetInlinePolicyForPermissionSetResponseTypeDef",
     "GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef",
     "InstanceMetadataTypeDef",
     "OperationStatusFilterTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
     "ListAccountAssignmentsRequestRequestTypeDef",
+    "ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
     "ListAccountsForProvisionedPermissionSetRequestRequestTypeDef",
+    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
+    "ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
     "ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
+    "ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
     "ListManagedPoliciesInPermissionSetRequestRequestTypeDef",
     "PermissionSetProvisioningStatusMetadataTypeDef",
+    "ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
     "ListPermissionSetsProvisionedToAccountRequestRequestTypeDef",
+    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
+    "ListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
     "ListPermissionSetsRequestRequestTypeDef",
+    "ListPermissionSetsResponseTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ProvisionPermissionSetRequestRequestTypeDef",
     "PutInlinePolicyToPermissionSetRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePermissionSetRequestRequestTypeDef",
     "AccessControlAttributeTypeDef",
-    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
-    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
-    "PermissionsBoundaryTypeDef",
+    "ListAccountAssignmentCreationStatusResponseTypeDef",
+    "ListAccountAssignmentDeletionStatusResponseTypeDef",
     "CreateAccountAssignmentResponseTypeDef",
     "DeleteAccountAssignmentResponseTypeDef",
     "DescribeAccountAssignmentCreationStatusResponseTypeDef",
     "DescribeAccountAssignmentDeletionStatusResponseTypeDef",
-    "GetInlinePolicyForPermissionSetResponseTypeDef",
-    "ListAccountAssignmentCreationStatusResponseTypeDef",
-    "ListAccountAssignmentDeletionStatusResponseTypeDef",
     "ListAccountAssignmentsResponseTypeDef",
-    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
+    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
+    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
     "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
+    "PermissionsBoundaryTypeDef",
     "ListManagedPoliciesInPermissionSetResponseTypeDef",
-    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
-    "ListPermissionSetsResponseTypeDef",
     "CreatePermissionSetRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreatePermissionSetResponseTypeDef",
     "DescribePermissionSetResponseTypeDef",
     "DescribePermissionSetProvisioningStatusResponseTypeDef",
     "ProvisionPermissionSetResponseTypeDef",
     "ListInstancesResponseTypeDef",
-    "ListAccountAssignmentCreationStatusRequestRequestTypeDef",
-    "ListAccountAssignmentDeletionStatusRequestRequestTypeDef",
-    "ListPermissionSetProvisioningStatusRequestRequestTypeDef",
     "ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
+    "ListAccountAssignmentCreationStatusRequestRequestTypeDef",
     "ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
-    "ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
-    "ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
-    "ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
-    "ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+    "ListAccountAssignmentDeletionStatusRequestRequestTypeDef",
     "ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
-    "ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
-    "ListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListPermissionSetProvisioningStatusRequestRequestTypeDef",
     "ListPermissionSetProvisioningStatusResponseTypeDef",
     "InstanceAccessControlAttributeConfigurationTypeDef",
     "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
     "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
@@ -214,25 +214,14 @@
         "TargetType": Literal["AWS_ACCOUNT"],
         "PermissionSetArn": str,
         "PrincipalType": PrincipalTypeType,
         "PrincipalId": str,
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -358,14 +347,22 @@
     "GetInlinePolicyForPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
 
+GetInlinePolicyForPermissionSetResponseTypeDef = TypedDict(
+    "GetInlinePolicyForPermissionSetResponseTypeDef",
+    {
+        "InlinePolicy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef = TypedDict(
     "GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -383,24 +380,38 @@
     "OperationStatusFilterTypeDef",
     {
         "Status": StatusValuesType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "InstanceArn": str,
+        "AccountId": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef(
+    _RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+    _OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAccountAssignmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountAssignmentsRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "AccountId": str,
         "PermissionSetArn": str,
     },
@@ -418,14 +429,38 @@
 class ListAccountAssignmentsRequestRequestTypeDef(
     _RequiredListAccountAssignmentsRequestRequestTypeDef,
     _OptionalListAccountAssignmentsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
+    "_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
+    "_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
+    {
+        "ProvisioningStatus": ProvisioningStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef(
+    _RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
+    _OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAccountsForProvisionedPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountsForProvisionedPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -443,14 +478,46 @@
 class ListAccountsForProvisionedPermissionSetRequestRequestTypeDef(
     _RequiredListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
     _OptionalListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
 ):
     pass
 
 
+ListAccountsForProvisionedPermissionSetResponseTypeDef = TypedDict(
+    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
+    {
+        "AccountIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
+    "_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
+    "_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef(
+    _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
+    _OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -467,23 +534,54 @@
 class ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef(
     _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
     _OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
 ):
     pass
 
 
+ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "ListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInstancesRequestRequestTypeDef = TypedDict(
     "ListInstancesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
+    "_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
+    "_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef(
+    _RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+    _OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListManagedPoliciesInPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedPoliciesInPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -510,14 +608,38 @@
         "Status": StatusValuesType,
         "RequestId": str,
         "CreatedDate": datetime,
     },
     total=False,
 )
 
+_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
+    "_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "AccountId": str,
+    },
+)
+_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
+    "_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
+    {
+        "ProvisioningStatus": ProvisioningStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef(
+    _RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
+    _OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPermissionSetsProvisionedToAccountRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionSetsProvisionedToAccountRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "AccountId": str,
     },
 )
@@ -535,14 +657,45 @@
 class ListPermissionSetsProvisionedToAccountRequestRequestTypeDef(
     _RequiredListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
     _OptionalListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
 ):
     pass
 
 
+ListPermissionSetsProvisionedToAccountResponseTypeDef = TypedDict(
+    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
+    {
+        "NextToken": str,
+        "PermissionSets": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
+    "_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
+    {
+        "InstanceArn": str,
+    },
+)
+_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
+    "_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPermissionSetsRequestListPermissionSetsPaginateTypeDef(
+    _RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
+    _OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPermissionSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionSetsRequestRequestTypeDef",
     {
         "InstanceArn": str,
     },
 )
 _OptionalListPermissionSetsRequestRequestTypeDef = TypedDict(
@@ -558,14 +711,46 @@
 class ListPermissionSetsRequestRequestTypeDef(
     _RequiredListPermissionSetsRequestRequestTypeDef,
     _OptionalListPermissionSetsRequestRequestTypeDef,
 ):
     pass
 
 
+ListPermissionSetsResponseTypeDef = TypedDict(
+    "ListPermissionSetsResponseTypeDef",
+    {
+        "PermissionSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "ResourceArn": str,
     },
 )
@@ -581,14 +766,24 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
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
 _RequiredProvisionPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
         "TargetType": ProvisionTargetTypeType,
     },
@@ -614,14 +809,25 @@
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
         "InlinePolicy": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
@@ -656,150 +862,115 @@
     "AccessControlAttributeTypeDef",
     {
         "Key": str,
         "Value": AccessControlAttributeValueTypeDef,
     },
 )
 
-AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef = TypedDict(
-    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
-    {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
-    },
-)
-
-DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef = TypedDict(
-    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
+ListAccountAssignmentCreationStatusResponseTypeDef = TypedDict(
+    "ListAccountAssignmentCreationStatusResponseTypeDef",
     {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
+        "AccountAssignmentsCreationStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PermissionsBoundaryTypeDef = TypedDict(
-    "PermissionsBoundaryTypeDef",
+ListAccountAssignmentDeletionStatusResponseTypeDef = TypedDict(
+    "ListAccountAssignmentDeletionStatusResponseTypeDef",
     {
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
-        "ManagedPolicyArn": str,
+        "AccountAssignmentsDeletionStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 CreateAccountAssignmentResponseTypeDef = TypedDict(
     "CreateAccountAssignmentResponseTypeDef",
     {
         "AccountAssignmentCreationStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAccountAssignmentResponseTypeDef = TypedDict(
     "DeleteAccountAssignmentResponseTypeDef",
     {
         "AccountAssignmentDeletionStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccountAssignmentCreationStatusResponseTypeDef = TypedDict(
     "DescribeAccountAssignmentCreationStatusResponseTypeDef",
     {
         "AccountAssignmentCreationStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccountAssignmentDeletionStatusResponseTypeDef = TypedDict(
     "DescribeAccountAssignmentDeletionStatusResponseTypeDef",
     {
         "AccountAssignmentDeletionStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetInlinePolicyForPermissionSetResponseTypeDef = TypedDict(
-    "GetInlinePolicyForPermissionSetResponseTypeDef",
-    {
-        "InlinePolicy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAccountAssignmentCreationStatusResponseTypeDef = TypedDict(
-    "ListAccountAssignmentCreationStatusResponseTypeDef",
-    {
-        "AccountAssignmentsCreationStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAccountAssignmentDeletionStatusResponseTypeDef = TypedDict(
-    "ListAccountAssignmentDeletionStatusResponseTypeDef",
-    {
-        "AccountAssignmentsDeletionStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccountAssignmentsResponseTypeDef = TypedDict(
     "ListAccountAssignmentsResponseTypeDef",
     {
         "AccountAssignments": List[AccountAssignmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAccountsForProvisionedPermissionSetResponseTypeDef = TypedDict(
-    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
+AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef = TypedDict(
+    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
     {
-        "AccountIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
     },
 )
 
-ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef = TypedDict(
-    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
+DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef = TypedDict(
+    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
     {
-        "CustomerManagedPolicyReferences": List[CustomerManagedPolicyReferenceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
     },
 )
 
-ListManagedPoliciesInPermissionSetResponseTypeDef = TypedDict(
-    "ListManagedPoliciesInPermissionSetResponseTypeDef",
+ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef = TypedDict(
+    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
     {
-        "AttachedManagedPolicies": List[AttachedManagedPolicyTypeDef],
+        "CustomerManagedPolicyReferences": List[CustomerManagedPolicyReferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPermissionSetsProvisionedToAccountResponseTypeDef = TypedDict(
-    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
+PermissionsBoundaryTypeDef = TypedDict(
+    "PermissionsBoundaryTypeDef",
     {
-        "NextToken": str,
-        "PermissionSets": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
+        "ManagedPolicyArn": str,
     },
+    total=False,
 )
 
-ListPermissionSetsResponseTypeDef = TypedDict(
-    "ListPermissionSetsResponseTypeDef",
+ListManagedPoliciesInPermissionSetResponseTypeDef = TypedDict(
+    "ListManagedPoliciesInPermissionSetResponseTypeDef",
     {
-        "PermissionSets": List[str],
+        "AttachedManagedPolicies": List[AttachedManagedPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePermissionSetRequestRequestTypeDef",
     {
         "Name": str,
@@ -826,15 +997,15 @@
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
@@ -843,384 +1014,213 @@
     },
 )
 
 CreatePermissionSetResponseTypeDef = TypedDict(
     "CreatePermissionSetResponseTypeDef",
     {
         "PermissionSet": PermissionSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePermissionSetResponseTypeDef = TypedDict(
     "DescribePermissionSetResponseTypeDef",
     {
         "PermissionSet": PermissionSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePermissionSetProvisioningStatusResponseTypeDef = TypedDict(
     "DescribePermissionSetProvisioningStatusResponseTypeDef",
     {
         "PermissionSetProvisioningStatus": PermissionSetProvisioningStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProvisionPermissionSetResponseTypeDef = TypedDict(
     "ProvisionPermissionSetResponseTypeDef",
     {
         "PermissionSetProvisioningStatus": PermissionSetProvisioningStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "Instances": List[InstanceMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef",
-    {
-        "InstanceArn": str,
-    },
-)
-_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-        "Filter": OperationStatusFilterTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListAccountAssignmentCreationStatusRequestRequestTypeDef(
-    _RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef,
-    _OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef",
+_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
     {
         "InstanceArn": str,
     },
 )
-_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef",
+_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
         "Filter": OperationStatusFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class ListAccountAssignmentDeletionStatusRequestRequestTypeDef(
-    _RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef,
-    _OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef,
+class ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef(
+    _RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+    _OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef",
+_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef",
     {
         "InstanceArn": str,
     },
 )
-_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef",
+_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filter": OperationStatusFilterTypeDef,
     },
     total=False,
 )
 
 
-class ListPermissionSetProvisioningStatusRequestRequestTypeDef(
-    _RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef,
-    _OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
-    {
-        "InstanceArn": str,
-    },
-)
-_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
-    {
-        "Filter": OperationStatusFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef(
-    _RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
-    _OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+class ListAccountAssignmentCreationStatusRequestRequestTypeDef(
+    _RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef,
+    _OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef,
 ):
     pass
 
 
 _RequiredListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef = TypedDict(
     "_RequiredListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
     {
         "InstanceArn": str,
     },
 )
 _OptionalListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef = TypedDict(
     "_OptionalListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
     {
         "Filter": OperationStatusFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef(
     _RequiredListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
     _OptionalListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "AccountId": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef(
-    _RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
-    _OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
-    "_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
-    "_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
-    {
-        "ProvisioningStatus": ProvisioningStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef(
-    _RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
-    _OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
-    "_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
-    "_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef(
-    _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
-    _OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
-):
-    pass
-
-
-ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "ListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
-    "_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef",
     {
         "InstanceArn": str,
-        "PermissionSetArn": str,
     },
 )
-_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
-    "_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "Filter": OperationStatusFilterTypeDef,
     },
     total=False,
 )
 
 
-class ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef(
-    _RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
-    _OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+class ListAccountAssignmentDeletionStatusRequestRequestTypeDef(
+    _RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef,
+    _OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef,
 ):
     pass
 
 
 _RequiredListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef = TypedDict(
     "_RequiredListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     {
         "InstanceArn": str,
     },
 )
 _OptionalListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef = TypedDict(
     "_OptionalListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     {
         "Filter": OperationStatusFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef(
     _RequiredListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
     _OptionalListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
-    "_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "AccountId": str,
-    },
-)
-_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
-    "_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
-    {
-        "ProvisioningStatus": ProvisioningStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef(
-    _RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
-    _OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
-    "_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
-    {
-        "InstanceArn": str,
-    },
-)
-_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
-    "_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPermissionSetsRequestListPermissionSetsPaginateTypeDef(
-    _RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
-    _OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef",
     {
         "InstanceArn": str,
-        "ResourceArn": str,
     },
 )
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "Filter": OperationStatusFilterTypeDef,
     },
     total=False,
 )
 
 
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+class ListPermissionSetProvisioningStatusRequestRequestTypeDef(
+    _RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef,
+    _OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef,
 ):
     pass
 
 
 ListPermissionSetProvisioningStatusResponseTypeDef = TypedDict(
     "ListPermissionSetProvisioningStatusResponseTypeDef",
     {
         "PermissionSetsProvisioningStatus": List[PermissionSetProvisioningStatusMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceAccessControlAttributeConfigurationTypeDef = TypedDict(
     "InstanceAccessControlAttributeConfigurationTypeDef",
     {
         "AccessControlAttributes": Sequence[AccessControlAttributeTypeDef],
     },
 )
 
 GetPermissionsBoundaryForPermissionSetResponseTypeDef = TypedDict(
     "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     {
         "PermissionsBoundary": PermissionsBoundaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef = TypedDict(
     "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
@@ -1243,15 +1243,15 @@
     "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     {
         "Status": InstanceAccessControlAttributeConfigurationStatusType,
         "StatusReason": str,
         "InstanceAccessControlAttributeConfiguration": (
             InstanceAccessControlAttributeConfigurationTypeDef
         ),
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     {
         "InstanceArn": str,
```

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin/type_defs.pyi` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     "AccountAssignmentOperationStatusMetadataTypeDef",
     "AccountAssignmentOperationStatusTypeDef",
     "AccountAssignmentTypeDef",
     "CustomerManagedPolicyReferenceTypeDef",
     "AttachManagedPolicyToPermissionSetRequestRequestTypeDef",
     "AttachedManagedPolicyTypeDef",
     "CreateAccountAssignmentRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "PermissionSetTypeDef",
     "DeleteAccountAssignmentRequestRequestTypeDef",
     "DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef",
     "DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "DeletePermissionSetRequestRequestTypeDef",
     "DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef",
@@ -53,70 +52,71 @@
     "DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef",
     "DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "DescribePermissionSetProvisioningStatusRequestRequestTypeDef",
     "PermissionSetProvisioningStatusTypeDef",
     "DescribePermissionSetRequestRequestTypeDef",
     "DetachManagedPolicyFromPermissionSetRequestRequestTypeDef",
     "GetInlinePolicyForPermissionSetRequestRequestTypeDef",
+    "GetInlinePolicyForPermissionSetResponseTypeDef",
     "GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef",
     "InstanceMetadataTypeDef",
     "OperationStatusFilterTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
     "ListAccountAssignmentsRequestRequestTypeDef",
+    "ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
     "ListAccountsForProvisionedPermissionSetRequestRequestTypeDef",
+    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
+    "ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
     "ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
+    "ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
     "ListManagedPoliciesInPermissionSetRequestRequestTypeDef",
     "PermissionSetProvisioningStatusMetadataTypeDef",
+    "ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
     "ListPermissionSetsProvisionedToAccountRequestRequestTypeDef",
+    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
+    "ListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
     "ListPermissionSetsRequestRequestTypeDef",
+    "ListPermissionSetsResponseTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ProvisionPermissionSetRequestRequestTypeDef",
     "PutInlinePolicyToPermissionSetRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePermissionSetRequestRequestTypeDef",
     "AccessControlAttributeTypeDef",
-    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
-    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
-    "PermissionsBoundaryTypeDef",
+    "ListAccountAssignmentCreationStatusResponseTypeDef",
+    "ListAccountAssignmentDeletionStatusResponseTypeDef",
     "CreateAccountAssignmentResponseTypeDef",
     "DeleteAccountAssignmentResponseTypeDef",
     "DescribeAccountAssignmentCreationStatusResponseTypeDef",
     "DescribeAccountAssignmentDeletionStatusResponseTypeDef",
-    "GetInlinePolicyForPermissionSetResponseTypeDef",
-    "ListAccountAssignmentCreationStatusResponseTypeDef",
-    "ListAccountAssignmentDeletionStatusResponseTypeDef",
     "ListAccountAssignmentsResponseTypeDef",
-    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
+    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
+    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
     "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
+    "PermissionsBoundaryTypeDef",
     "ListManagedPoliciesInPermissionSetResponseTypeDef",
-    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
-    "ListPermissionSetsResponseTypeDef",
     "CreatePermissionSetRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreatePermissionSetResponseTypeDef",
     "DescribePermissionSetResponseTypeDef",
     "DescribePermissionSetProvisioningStatusResponseTypeDef",
     "ProvisionPermissionSetResponseTypeDef",
     "ListInstancesResponseTypeDef",
-    "ListAccountAssignmentCreationStatusRequestRequestTypeDef",
-    "ListAccountAssignmentDeletionStatusRequestRequestTypeDef",
-    "ListPermissionSetProvisioningStatusRequestRequestTypeDef",
     "ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
+    "ListAccountAssignmentCreationStatusRequestRequestTypeDef",
     "ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
-    "ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
-    "ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
-    "ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
-    "ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+    "ListAccountAssignmentDeletionStatusRequestRequestTypeDef",
     "ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
-    "ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
-    "ListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListPermissionSetProvisioningStatusRequestRequestTypeDef",
     "ListPermissionSetProvisioningStatusResponseTypeDef",
     "InstanceAccessControlAttributeConfigurationTypeDef",
     "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
     "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
@@ -211,25 +211,14 @@
         "TargetType": Literal["AWS_ACCOUNT"],
         "PermissionSetArn": str,
         "PrincipalType": PrincipalTypeType,
         "PrincipalId": str,
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -355,14 +344,22 @@
     "GetInlinePolicyForPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
 
+GetInlinePolicyForPermissionSetResponseTypeDef = TypedDict(
+    "GetInlinePolicyForPermissionSetResponseTypeDef",
+    {
+        "InlinePolicy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef = TypedDict(
     "GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -380,24 +377,36 @@
     "OperationStatusFilterTypeDef",
     {
         "Status": StatusValuesType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "InstanceArn": str,
+        "AccountId": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef(
+    _RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+    _OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAccountAssignmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountAssignmentsRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "AccountId": str,
         "PermissionSetArn": str,
     },
@@ -413,14 +422,36 @@
 
 class ListAccountAssignmentsRequestRequestTypeDef(
     _RequiredListAccountAssignmentsRequestRequestTypeDef,
     _OptionalListAccountAssignmentsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
+    "_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
+    "_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
+    {
+        "ProvisioningStatus": ProvisioningStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef(
+    _RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
+    _OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
+):
+    pass
+
 _RequiredListAccountsForProvisionedPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountsForProvisionedPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -436,14 +467,44 @@
 
 class ListAccountsForProvisionedPermissionSetRequestRequestTypeDef(
     _RequiredListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
     _OptionalListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
 ):
     pass
 
+ListAccountsForProvisionedPermissionSetResponseTypeDef = TypedDict(
+    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
+    {
+        "AccountIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
+    "_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
+    "_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef(
+    _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
+    _OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
+):
+    pass
+
 _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -458,23 +519,52 @@
 
 class ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef(
     _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
     _OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
 ):
     pass
 
+ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "ListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInstancesRequestRequestTypeDef = TypedDict(
     "ListInstancesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
+    "_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
+    "_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef(
+    _RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+    _OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+):
+    pass
+
 _RequiredListManagedPoliciesInPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedPoliciesInPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -499,14 +589,36 @@
         "Status": StatusValuesType,
         "RequestId": str,
         "CreatedDate": datetime,
     },
     total=False,
 )
 
+_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
+    "_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "AccountId": str,
+    },
+)
+_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
+    "_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
+    {
+        "ProvisioningStatus": ProvisioningStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef(
+    _RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
+    _OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
+):
+    pass
+
 _RequiredListPermissionSetsProvisionedToAccountRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionSetsProvisionedToAccountRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "AccountId": str,
     },
 )
@@ -522,14 +634,43 @@
 
 class ListPermissionSetsProvisionedToAccountRequestRequestTypeDef(
     _RequiredListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
     _OptionalListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
 ):
     pass
 
+ListPermissionSetsProvisionedToAccountResponseTypeDef = TypedDict(
+    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
+    {
+        "NextToken": str,
+        "PermissionSets": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
+    "_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
+    {
+        "InstanceArn": str,
+    },
+)
+_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
+    "_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPermissionSetsRequestListPermissionSetsPaginateTypeDef(
+    _RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
+    _OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListPermissionSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionSetsRequestRequestTypeDef",
     {
         "InstanceArn": str,
     },
 )
 _OptionalListPermissionSetsRequestRequestTypeDef = TypedDict(
@@ -543,14 +684,44 @@
 
 class ListPermissionSetsRequestRequestTypeDef(
     _RequiredListPermissionSetsRequestRequestTypeDef,
     _OptionalListPermissionSetsRequestRequestTypeDef,
 ):
     pass
 
+ListPermissionSetsResponseTypeDef = TypedDict(
+    "ListPermissionSetsResponseTypeDef",
+    {
+        "PermissionSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "ResourceArn": str,
     },
 )
@@ -564,14 +735,24 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
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
 _RequiredProvisionPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
         "TargetType": ProvisionTargetTypeType,
     },
@@ -595,14 +776,25 @@
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
         "InlinePolicy": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
@@ -635,150 +827,115 @@
     "AccessControlAttributeTypeDef",
     {
         "Key": str,
         "Value": AccessControlAttributeValueTypeDef,
     },
 )
 
-AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef = TypedDict(
-    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
-    {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
-    },
-)
-
-DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef = TypedDict(
-    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
+ListAccountAssignmentCreationStatusResponseTypeDef = TypedDict(
+    "ListAccountAssignmentCreationStatusResponseTypeDef",
     {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
+        "AccountAssignmentsCreationStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PermissionsBoundaryTypeDef = TypedDict(
-    "PermissionsBoundaryTypeDef",
+ListAccountAssignmentDeletionStatusResponseTypeDef = TypedDict(
+    "ListAccountAssignmentDeletionStatusResponseTypeDef",
     {
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
-        "ManagedPolicyArn": str,
+        "AccountAssignmentsDeletionStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 CreateAccountAssignmentResponseTypeDef = TypedDict(
     "CreateAccountAssignmentResponseTypeDef",
     {
         "AccountAssignmentCreationStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAccountAssignmentResponseTypeDef = TypedDict(
     "DeleteAccountAssignmentResponseTypeDef",
     {
         "AccountAssignmentDeletionStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccountAssignmentCreationStatusResponseTypeDef = TypedDict(
     "DescribeAccountAssignmentCreationStatusResponseTypeDef",
     {
         "AccountAssignmentCreationStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccountAssignmentDeletionStatusResponseTypeDef = TypedDict(
     "DescribeAccountAssignmentDeletionStatusResponseTypeDef",
     {
         "AccountAssignmentDeletionStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetInlinePolicyForPermissionSetResponseTypeDef = TypedDict(
-    "GetInlinePolicyForPermissionSetResponseTypeDef",
-    {
-        "InlinePolicy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAccountAssignmentCreationStatusResponseTypeDef = TypedDict(
-    "ListAccountAssignmentCreationStatusResponseTypeDef",
-    {
-        "AccountAssignmentsCreationStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAccountAssignmentDeletionStatusResponseTypeDef = TypedDict(
-    "ListAccountAssignmentDeletionStatusResponseTypeDef",
-    {
-        "AccountAssignmentsDeletionStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccountAssignmentsResponseTypeDef = TypedDict(
     "ListAccountAssignmentsResponseTypeDef",
     {
         "AccountAssignments": List[AccountAssignmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAccountsForProvisionedPermissionSetResponseTypeDef = TypedDict(
-    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
+AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef = TypedDict(
+    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
     {
-        "AccountIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
     },
 )
 
-ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef = TypedDict(
-    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
+DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef = TypedDict(
+    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
     {
-        "CustomerManagedPolicyReferences": List[CustomerManagedPolicyReferenceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
     },
 )
 
-ListManagedPoliciesInPermissionSetResponseTypeDef = TypedDict(
-    "ListManagedPoliciesInPermissionSetResponseTypeDef",
+ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef = TypedDict(
+    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
     {
-        "AttachedManagedPolicies": List[AttachedManagedPolicyTypeDef],
+        "CustomerManagedPolicyReferences": List[CustomerManagedPolicyReferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPermissionSetsProvisionedToAccountResponseTypeDef = TypedDict(
-    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
+PermissionsBoundaryTypeDef = TypedDict(
+    "PermissionsBoundaryTypeDef",
     {
-        "NextToken": str,
-        "PermissionSets": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
+        "ManagedPolicyArn": str,
     },
+    total=False,
 )
 
-ListPermissionSetsResponseTypeDef = TypedDict(
-    "ListPermissionSetsResponseTypeDef",
+ListManagedPoliciesInPermissionSetResponseTypeDef = TypedDict(
+    "ListManagedPoliciesInPermissionSetResponseTypeDef",
     {
-        "PermissionSets": List[str],
+        "AttachedManagedPolicies": List[AttachedManagedPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePermissionSetRequestRequestTypeDef",
     {
         "Name": str,
@@ -803,15 +960,15 @@
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
@@ -820,358 +977,201 @@
     },
 )
 
 CreatePermissionSetResponseTypeDef = TypedDict(
     "CreatePermissionSetResponseTypeDef",
     {
         "PermissionSet": PermissionSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePermissionSetResponseTypeDef = TypedDict(
     "DescribePermissionSetResponseTypeDef",
     {
         "PermissionSet": PermissionSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePermissionSetProvisioningStatusResponseTypeDef = TypedDict(
     "DescribePermissionSetProvisioningStatusResponseTypeDef",
     {
         "PermissionSetProvisioningStatus": PermissionSetProvisioningStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProvisionPermissionSetResponseTypeDef = TypedDict(
     "ProvisionPermissionSetResponseTypeDef",
     {
         "PermissionSetProvisioningStatus": PermissionSetProvisioningStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "Instances": List[InstanceMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef",
-    {
-        "InstanceArn": str,
-    },
-)
-_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-        "Filter": OperationStatusFilterTypeDef,
-    },
-    total=False,
-)
-
-class ListAccountAssignmentCreationStatusRequestRequestTypeDef(
-    _RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef,
-    _OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef,
-):
-    pass
-
-_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef",
+_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
     {
         "InstanceArn": str,
     },
 )
-_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef",
+_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
         "Filter": OperationStatusFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class ListAccountAssignmentDeletionStatusRequestRequestTypeDef(
-    _RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef,
-    _OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef,
+class ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef(
+    _RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+    _OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
 ):
     pass
 
-_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef",
+_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef",
     {
         "InstanceArn": str,
     },
 )
-_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef",
+_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filter": OperationStatusFilterTypeDef,
     },
     total=False,
 )
 
-class ListPermissionSetProvisioningStatusRequestRequestTypeDef(
-    _RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef,
-    _OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef,
-):
-    pass
-
-_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
-    {
-        "InstanceArn": str,
-    },
-)
-_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
-    {
-        "Filter": OperationStatusFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef(
-    _RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
-    _OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+class ListAccountAssignmentCreationStatusRequestRequestTypeDef(
+    _RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef,
+    _OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef,
 ):
     pass
 
 _RequiredListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef = TypedDict(
     "_RequiredListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
     {
         "InstanceArn": str,
     },
 )
 _OptionalListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef = TypedDict(
     "_OptionalListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
     {
         "Filter": OperationStatusFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef(
     _RequiredListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
     _OptionalListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
 ):
     pass
 
-_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "AccountId": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef(
-    _RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
-    _OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
-):
-    pass
-
-_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
-    "_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
-    "_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
-    {
-        "ProvisioningStatus": ProvisioningStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef(
-    _RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
-    _OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
-):
-    pass
-
-_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
-    "_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
-    "_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef(
-    _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
-    _OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
-):
-    pass
-
-ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "ListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
-    "_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef",
     {
         "InstanceArn": str,
-        "PermissionSetArn": str,
     },
 )
-_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
-    "_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "Filter": OperationStatusFilterTypeDef,
     },
     total=False,
 )
 
-class ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef(
-    _RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
-    _OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+class ListAccountAssignmentDeletionStatusRequestRequestTypeDef(
+    _RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef,
+    _OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef,
 ):
     pass
 
 _RequiredListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef = TypedDict(
     "_RequiredListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     {
         "InstanceArn": str,
     },
 )
 _OptionalListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef = TypedDict(
     "_OptionalListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     {
         "Filter": OperationStatusFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef(
     _RequiredListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
     _OptionalListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
 ):
     pass
 
-_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
-    "_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "AccountId": str,
-    },
-)
-_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
-    "_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
-    {
-        "ProvisioningStatus": ProvisioningStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef(
-    _RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
-    _OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
-):
-    pass
-
-_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
-    "_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
-    {
-        "InstanceArn": str,
-    },
-)
-_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
-    "_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPermissionSetsRequestListPermissionSetsPaginateTypeDef(
-    _RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
-    _OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
-):
-    pass
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef",
     {
         "InstanceArn": str,
-        "ResourceArn": str,
     },
 )
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "Filter": OperationStatusFilterTypeDef,
     },
     total=False,
 )
 
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+class ListPermissionSetProvisioningStatusRequestRequestTypeDef(
+    _RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef,
+    _OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef,
 ):
     pass
 
 ListPermissionSetProvisioningStatusResponseTypeDef = TypedDict(
     "ListPermissionSetProvisioningStatusResponseTypeDef",
     {
         "PermissionSetsProvisioningStatus": List[PermissionSetProvisioningStatusMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceAccessControlAttributeConfigurationTypeDef = TypedDict(
     "InstanceAccessControlAttributeConfigurationTypeDef",
     {
         "AccessControlAttributes": Sequence[AccessControlAttributeTypeDef],
     },
 )
 
 GetPermissionsBoundaryForPermissionSetResponseTypeDef = TypedDict(
     "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     {
         "PermissionsBoundary": PermissionsBoundaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef = TypedDict(
     "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
@@ -1194,15 +1194,15 @@
     "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     {
         "Status": InstanceAccessControlAttributeConfigurationStatusType,
         "StatusReason": str,
         "InstanceAccessControlAttributeConfiguration": (
             InstanceAccessControlAttributeConfigurationTypeDef
         ),
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     {
         "InstanceArn": str,
```

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin.egg-info/PKG-INFO` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-admin
-Version: 1.26.63
-Summary: Type annotations for boto3.SSOAdmin 1.26.63 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.SSOAdmin 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sso-admin"></a>
 
 # mypy-boto3-sso-admin
 
 [![PyPI - mypy-boto3-sso-admin](https://img.shields.io/pypi/v/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso-admin?color=blue)](https://pypistats.org/packages/mypy-boto3-sso-admin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOAdmin 1.26.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
+[boto3.SSOAdmin 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
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
 [mypy-boto3-sso-admin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -384,15 +384,14 @@
     AccountAssignmentOperationStatusMetadataTypeDef,
     AccountAssignmentOperationStatusTypeDef,
     AccountAssignmentTypeDef,
     CustomerManagedPolicyReferenceTypeDef,
     AttachManagedPolicyToPermissionSetRequestRequestTypeDef,
     AttachedManagedPolicyTypeDef,
     CreateAccountAssignmentRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     PermissionSetTypeDef,
     DeleteAccountAssignmentRequestRequestTypeDef,
     DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef,
     DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DeletePermissionSetRequestRequestTypeDef,
     DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef,
@@ -400,70 +399,71 @@
     DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DescribePermissionSetProvisioningStatusRequestRequestTypeDef,
     PermissionSetProvisioningStatusTypeDef,
     DescribePermissionSetRequestRequestTypeDef,
     DetachManagedPolicyFromPermissionSetRequestRequestTypeDef,
     GetInlinePolicyForPermissionSetRequestRequestTypeDef,
+    GetInlinePolicyForPermissionSetResponseTypeDef,
     GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef,
     InstanceMetadataTypeDef,
     OperationStatusFilterTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
     ListAccountAssignmentsRequestRequestTypeDef,
+    ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
     ListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
+    ListAccountsForProvisionedPermissionSetResponseTypeDef,
+    ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
+    ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
     ListManagedPoliciesInPermissionSetRequestRequestTypeDef,
     PermissionSetProvisioningStatusMetadataTypeDef,
+    ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
     ListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
+    ListPermissionSetsProvisionedToAccountResponseTypeDef,
+    ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
     ListPermissionSetsRequestRequestTypeDef,
+    ListPermissionSetsResponseTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ProvisionPermissionSetRequestRequestTypeDef,
     PutInlinePolicyToPermissionSetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePermissionSetRequestRequestTypeDef,
     AccessControlAttributeTypeDef,
-    AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
-    DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef,
-    PermissionsBoundaryTypeDef,
+    ListAccountAssignmentCreationStatusResponseTypeDef,
+    ListAccountAssignmentDeletionStatusResponseTypeDef,
     CreateAccountAssignmentResponseTypeDef,
     DeleteAccountAssignmentResponseTypeDef,
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
-    GetInlinePolicyForPermissionSetResponseTypeDef,
-    ListAccountAssignmentCreationStatusResponseTypeDef,
-    ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
-    ListAccountsForProvisionedPermissionSetResponseTypeDef,
+    AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
+    DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
+    PermissionsBoundaryTypeDef,
     ListManagedPoliciesInPermissionSetResponseTypeDef,
-    ListPermissionSetsProvisionedToAccountResponseTypeDef,
-    ListPermissionSetsResponseTypeDef,
     CreatePermissionSetRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreatePermissionSetResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     ProvisionPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
-    ListAccountAssignmentCreationStatusRequestRequestTypeDef,
-    ListAccountAssignmentDeletionStatusRequestRequestTypeDef,
-    ListPermissionSetProvisioningStatusRequestRequestTypeDef,
     ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+    ListAccountAssignmentCreationStatusRequestRequestTypeDef,
     ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
-    ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
-    ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
-    ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
-    ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+    ListAccountAssignmentDeletionStatusRequestRequestTypeDef,
     ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
-    ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
-    ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListPermissionSetProvisioningStatusRequestRequestTypeDef,
     ListPermissionSetProvisioningStatusResponseTypeDef,
     InstanceAccessControlAttributeConfigurationTypeDef,
     GetPermissionsBoundaryForPermissionSetResponseTypeDef,
     PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef,
     CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
     UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
@@ -477,42 +477,42 @@
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

### Comparing `mypy-boto3-sso-admin-1.26.63/mypy_boto3_sso_admin.egg-info/SOURCES.txt` & `mypy-boto3-sso-admin-1.27.0/mypy_boto3_sso_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.26.63/setup.py` & `mypy-boto3-sso-admin-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-sso-admin.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sso-admin",
-    version="1.26.63",
+    version="1.27.0",
     packages=["mypy_boto3_sso_admin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSOAdmin 1.26.63 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.SSOAdmin 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/",
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


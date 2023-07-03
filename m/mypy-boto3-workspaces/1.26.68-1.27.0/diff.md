# Comparing `tmp/mypy-boto3-workspaces-1.26.68.tar.gz` & `tmp/mypy-boto3-workspaces-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-1.26.68.tar", last modified: Thu Feb  9 20:26:51 2023, max compression
+gzip compressed data, was "mypy-boto3-workspaces-1.27.0.tar", last modified: Mon Jul  3 19:51:37 2023, max compression
```

## Comparing `mypy-boto3-workspaces-1.26.68.tar` & `mypy-boto3-workspaces-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:51.606842 mypy-boto3-workspaces-1.26.68/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22019 2023-02-09 20:26:51.606842 mypy-boto3-workspaces-1.26.68/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:51.606842 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48049 2023-02-09 20:26:38.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47969 2023-02-09 20:26:38.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-02-09 20:26:38.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13037 2023-02-09 20:26:38.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-02-09 20:26:38.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-02-09 20:26:38.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53904 2023-02-09 20:26:40.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53863 2023-02-09 20:26:39.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:51.606842 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22019 2023-02-09 20:26:51.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-09 20:26:51.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:51.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:51.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 20:26:51.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 20:26:51.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 20:26:51.606842 mypy-boto3-workspaces-1.26.68/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:37.492166 mypy-boto3-workspaces-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:54.000000 mypy-boto3-workspaces-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21998 2023-07-03 19:51:37.492166 mypy-boto3-workspaces-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-03 19:49:54.000000 mypy-boto3-workspaces-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:37.492166 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-03 19:49:54.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-03 19:49:54.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:49:54.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48055 2023-07-03 19:49:54.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47975 2023-07-03 19:49:54.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-07-03 19:49:55.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13274 2023-07-03 19:49:55.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-07-03 19:49:55.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-07-03 19:49:55.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:54.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53990 2023-07-03 19:49:56.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53949 2023-07-03 19:49:55.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:54.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:37.492166 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21998 2023-07-03 19:51:37.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:51:37.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:37.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:37.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:37.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:51:37.000000 mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:37.492166 mypy-boto3-workspaces-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:49:54.000000 mypy-boto3-workspaces-1.27.0/setup.py
```

### Comparing `mypy-boto3-workspaces-1.26.68/LICENSE` & `mypy-boto3-workspaces-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-workspaces-1.26.68/PKG-INFO` & `mypy-boto3-workspaces-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces
-Version: 1.26.68
-Summary: Type annotations for boto3.WorkSpaces 1.26.68 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.WorkSpaces 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-workspaces"></a>
 
 # mypy-boto3-workspaces
 
 [![PyPI - mypy-boto3-workspaces](https://img.shields.io/pypi/v/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
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
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,97 +390,105 @@
 `mypy_boto3_workspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateConnectionAliasResultTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ClientPropertiesTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
+    CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
+    CreateConnectClientAddInResultTypeDef,
+    CreateConnectionAliasResultTypeDef,
+    CreateIpGroupResultTypeDef,
     PendingCreateStandbyWorkspacesRequestTypeDef,
+    CreateUpdatedWorkspaceImageResultTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
     DefaultClientBrandingAttributesTypeDef,
     DefaultImportClientBrandingAttributesTypeDef,
     DefaultWorkspaceCreationPropertiesTypeDef,
     DeleteClientBrandingRequestRequestTypeDef,
     DeleteConnectClientAddInRequestRequestTypeDef,
     DeleteConnectionAliasRequestRequestTypeDef,
     DeleteIpGroupRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteWorkspaceBundleRequestRequestTypeDef,
     DeleteWorkspaceImageRequestRequestTypeDef,
     DeregisterWorkspaceDirectoryRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
     DescribeAccountModificationsRequestRequestTypeDef,
+    DescribeAccountResultTypeDef,
     DescribeClientBrandingRequestRequestTypeDef,
     IosClientBrandingAttributesTypeDef,
     DescribeClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsRequestRequestTypeDef,
     DescribeConnectionAliasPermissionsRequestRequestTypeDef,
     DescribeConnectionAliasesRequestRequestTypeDef,
+    DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeIpGroupsRequestRequestTypeDef,
     DescribeTagsRequestRequestTypeDef,
+    DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
     DescribeWorkspaceBundlesRequestRequestTypeDef,
+    DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestRequestTypeDef,
     DescribeWorkspaceImagePermissionsRequestRequestTypeDef,
     ImagePermissionTypeDef,
+    DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
     DescribeWorkspaceImagesRequestRequestTypeDef,
     DescribeWorkspaceSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
+    DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
     DescribeWorkspacesConnectionStatusRequestRequestTypeDef,
     WorkspaceConnectionStatusTypeDef,
+    DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
     DescribeWorkspacesRequestRequestTypeDef,
     DisassociateConnectionAliasRequestRequestTypeDef,
     DisassociateIpGroupsRequestRequestTypeDef,
     FailedWorkspaceChangeRequestTypeDef,
     IosImportClientBrandingAttributesTypeDef,
+    ImportWorkspaceImageResultTypeDef,
+    ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     ListAvailableManagementCidrRangesRequestRequestTypeDef,
+    ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceRequestRequestTypeDef,
+    MigrateWorkspaceResultTypeDef,
     ModificationStateTypeDef,
     ModifyAccountRequestRequestTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
     RelatedWorkspacePropertiesTypeDef,
+    ResponseMetadataTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
     UpdateWorkspaceBundleRequestRequestTypeDef,
     UpdateWorkspaceImagePermissionRequestRequestTypeDef,
-    AssociateConnectionAliasResultTypeDef,
-    CopyWorkspaceImageResultTypeDef,
-    CreateConnectClientAddInResultTypeDef,
-    CreateConnectionAliasResultTypeDef,
-    CreateIpGroupResultTypeDef,
-    CreateUpdatedWorkspaceImageResultTypeDef,
     DescribeAccountModificationsResultTypeDef,
-    DescribeAccountResultTypeDef,
-    ImportWorkspaceImageResultTypeDef,
-    ListAvailableManagementCidrRangesResultTypeDef,
-    MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
     WorkspacesIpGroupTypeDef,
     ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
@@ -496,22 +504,14 @@
     DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
     StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
     WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
-    DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
-    DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
-    DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
-    DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
-    DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
-    DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
-    DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
-    ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     DescribeClientBrandingResultTypeDef,
     ImportClientBrandingResultTypeDef,
     DescribeWorkspaceImagePermissionsResultTypeDef,
     DescribeWorkspaceSnapshotsResultTypeDef,
     DescribeWorkspacesConnectionStatusResultTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildWorkspacesResultTypeDef,
@@ -557,42 +557,42 @@
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

### Comparing `mypy-boto3-workspaces-1.26.68/README.md` & `mypy-boto3-workspaces-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-workspaces"></a>
 
 # mypy-boto3-workspaces
 
 [![PyPI - mypy-boto3-workspaces](https://img.shields.io/pypi/v/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
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
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,97 +358,105 @@
 `mypy_boto3_workspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateConnectionAliasResultTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ClientPropertiesTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
+    CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
+    CreateConnectClientAddInResultTypeDef,
+    CreateConnectionAliasResultTypeDef,
+    CreateIpGroupResultTypeDef,
     PendingCreateStandbyWorkspacesRequestTypeDef,
+    CreateUpdatedWorkspaceImageResultTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
     DefaultClientBrandingAttributesTypeDef,
     DefaultImportClientBrandingAttributesTypeDef,
     DefaultWorkspaceCreationPropertiesTypeDef,
     DeleteClientBrandingRequestRequestTypeDef,
     DeleteConnectClientAddInRequestRequestTypeDef,
     DeleteConnectionAliasRequestRequestTypeDef,
     DeleteIpGroupRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteWorkspaceBundleRequestRequestTypeDef,
     DeleteWorkspaceImageRequestRequestTypeDef,
     DeregisterWorkspaceDirectoryRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
     DescribeAccountModificationsRequestRequestTypeDef,
+    DescribeAccountResultTypeDef,
     DescribeClientBrandingRequestRequestTypeDef,
     IosClientBrandingAttributesTypeDef,
     DescribeClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsRequestRequestTypeDef,
     DescribeConnectionAliasPermissionsRequestRequestTypeDef,
     DescribeConnectionAliasesRequestRequestTypeDef,
+    DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeIpGroupsRequestRequestTypeDef,
     DescribeTagsRequestRequestTypeDef,
+    DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
     DescribeWorkspaceBundlesRequestRequestTypeDef,
+    DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestRequestTypeDef,
     DescribeWorkspaceImagePermissionsRequestRequestTypeDef,
     ImagePermissionTypeDef,
+    DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
     DescribeWorkspaceImagesRequestRequestTypeDef,
     DescribeWorkspaceSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
+    DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
     DescribeWorkspacesConnectionStatusRequestRequestTypeDef,
     WorkspaceConnectionStatusTypeDef,
+    DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
     DescribeWorkspacesRequestRequestTypeDef,
     DisassociateConnectionAliasRequestRequestTypeDef,
     DisassociateIpGroupsRequestRequestTypeDef,
     FailedWorkspaceChangeRequestTypeDef,
     IosImportClientBrandingAttributesTypeDef,
+    ImportWorkspaceImageResultTypeDef,
+    ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     ListAvailableManagementCidrRangesRequestRequestTypeDef,
+    ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceRequestRequestTypeDef,
+    MigrateWorkspaceResultTypeDef,
     ModificationStateTypeDef,
     ModifyAccountRequestRequestTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
     RelatedWorkspacePropertiesTypeDef,
+    ResponseMetadataTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
     UpdateWorkspaceBundleRequestRequestTypeDef,
     UpdateWorkspaceImagePermissionRequestRequestTypeDef,
-    AssociateConnectionAliasResultTypeDef,
-    CopyWorkspaceImageResultTypeDef,
-    CreateConnectClientAddInResultTypeDef,
-    CreateConnectionAliasResultTypeDef,
-    CreateIpGroupResultTypeDef,
-    CreateUpdatedWorkspaceImageResultTypeDef,
     DescribeAccountModificationsResultTypeDef,
-    DescribeAccountResultTypeDef,
-    ImportWorkspaceImageResultTypeDef,
-    ListAvailableManagementCidrRangesResultTypeDef,
-    MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
     WorkspacesIpGroupTypeDef,
     ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
@@ -464,22 +472,14 @@
     DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
     StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
     WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
-    DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
-    DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
-    DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
-    DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
-    DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
-    DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
-    DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
-    ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     DescribeClientBrandingResultTypeDef,
     ImportClientBrandingResultTypeDef,
     DescribeWorkspaceImagePermissionsResultTypeDef,
     DescribeWorkspaceSnapshotsResultTypeDef,
     DescribeWorkspacesConnectionStatusResultTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildWorkspacesResultTypeDef,
@@ -525,42 +525,42 @@
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

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/__init__.py` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/__init__.pyi` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/__main__.py` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkSpaces 1.26.68\nVersion:         1.26.68\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.WorkSpaces 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.68")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/client.py` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,16 +613,16 @@
         IngestionProcess: WorkspaceImageIngestionProcessType,
         ImageName: str,
         ImageDescription: str,
         Tags: Sequence[TagTypeDef] = ...,
         Applications: Sequence[ApplicationType] = ...
     ) -> ImportWorkspaceImageResultTypeDef:
         """
-        Imports the specified Windows 10 Bring Your Own License (BYOL) image into Amazon
-        WorkSpaces.
+        Imports the specified Windows 10 or 11 Bring Your Own License (BYOL) image into
+        Amazon WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.import_workspace_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#import_workspace_image)
         """
 
     def list_available_management_cidr_ranges(
         self, *, ManagementCidrRangeConstraint: str, MaxResults: int = ..., NextToken: str = ...
```

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/client.pyi` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -565,16 +565,16 @@
         IngestionProcess: WorkspaceImageIngestionProcessType,
         ImageName: str,
         ImageDescription: str,
         Tags: Sequence[TagTypeDef] = ...,
         Applications: Sequence[ApplicationType] = ...
     ) -> ImportWorkspaceImageResultTypeDef:
         """
-        Imports the specified Windows 10 Bring Your Own License (BYOL) image into Amazon
-        WorkSpaces.
+        Imports the specified Windows 10 or 11 Bring Your Own License (BYOL) image into
+        Amazon WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.import_workspace_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#import_workspace_image)
         """
     def list_available_management_cidr_ranges(
         self, *, ManagementCidrRangeConstraint: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAvailableManagementCidrRangesResultTypeDef:
```

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/literals.py` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,15 @@
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
@@ -224,14 +225,15 @@
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
@@ -310,14 +312,15 @@
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
@@ -328,14 +331,15 @@
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
@@ -371,14 +375,15 @@
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
@@ -397,16 +402,19 @@
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
@@ -486,18 +494,21 @@
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

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/literals.pyi` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,15 @@
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
@@ -222,14 +223,15 @@
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
@@ -308,14 +310,15 @@
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
@@ -326,14 +329,15 @@
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
@@ -369,14 +373,15 @@
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
@@ -395,16 +400,19 @@
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
@@ -484,18 +492,21 @@
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

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/paginator.py` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,30 +75,30 @@
 class DescribeAccountModificationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeAccountModifications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeaccountmodificationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccountModificationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeAccountModifications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeaccountmodificationspaginator)
         """
 
 
 class DescribeIpGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeIpGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeipgroupspaginator)
     """
 
     def paginate(
-        self, *, GroupIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GroupIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeIpGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeIpGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeipgroupspaginator)
         """
 
 
@@ -109,15 +109,15 @@
     """
 
     def paginate(
         self,
         *,
         BundleIds: Sequence[str] = ...,
         Owner: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeWorkspaceBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacebundlespaginator)
         """
 
 
@@ -128,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryIds: Sequence[str] = ...,
         Limit: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeWorkspaceDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceDirectories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacedirectoriespaginator)
         """
 
 
@@ -147,15 +147,15 @@
     """
 
     def paginate(
         self,
         *,
         ImageIds: Sequence[str] = ...,
         ImageType: ImageTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeWorkspaceImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspaceimagespaginator)
         """
 
 
@@ -168,43 +168,46 @@
     def paginate(
         self,
         *,
         WorkspaceIds: Sequence[str] = ...,
         DirectoryId: str = ...,
         UserName: str = ...,
         BundleId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeWorkspacesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacespaginator)
         """
 
 
 class DescribeWorkspacesConnectionStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspacesConnectionStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacesconnectionstatuspaginator)
     """
 
     def paginate(
-        self, *, WorkspaceIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, WorkspaceIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeWorkspacesConnectionStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspacesConnectionStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacesconnectionstatuspaginator)
         """
 
 
 class ListAvailableManagementCidrRangesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.ListAvailableManagementCidrRanges)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#listavailablemanagementcidrrangespaginator)
     """
 
     def paginate(
-        self, *, ManagementCidrRangeConstraint: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        ManagementCidrRangeConstraint: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAvailableManagementCidrRangesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.ListAvailableManagementCidrRanges.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#listavailablemanagementcidrrangespaginator)
         """
```

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/paginator.pyi` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -72,29 +72,29 @@
 class DescribeAccountModificationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeAccountModifications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeaccountmodificationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccountModificationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeAccountModifications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeaccountmodificationspaginator)
         """
 
 class DescribeIpGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeIpGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeipgroupspaginator)
     """
 
     def paginate(
-        self, *, GroupIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GroupIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeIpGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeIpGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeipgroupspaginator)
         """
 
 class DescribeWorkspaceBundlesPaginator(Paginator):
@@ -104,15 +104,15 @@
     """
 
     def paginate(
         self,
         *,
         BundleIds: Sequence[str] = ...,
         Owner: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeWorkspaceBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacebundlespaginator)
         """
 
 class DescribeWorkspaceDirectoriesPaginator(Paginator):
@@ -122,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryIds: Sequence[str] = ...,
         Limit: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeWorkspaceDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceDirectories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacedirectoriespaginator)
         """
 
 class DescribeWorkspaceImagesPaginator(Paginator):
@@ -140,15 +140,15 @@
     """
 
     def paginate(
         self,
         *,
         ImageIds: Sequence[str] = ...,
         ImageType: ImageTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeWorkspaceImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspaceimagespaginator)
         """
 
 class DescribeWorkspacesPaginator(Paginator):
@@ -160,41 +160,44 @@
     def paginate(
         self,
         *,
         WorkspaceIds: Sequence[str] = ...,
         DirectoryId: str = ...,
         UserName: str = ...,
         BundleId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeWorkspacesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacespaginator)
         """
 
 class DescribeWorkspacesConnectionStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspacesConnectionStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacesconnectionstatuspaginator)
     """
 
     def paginate(
-        self, *, WorkspaceIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, WorkspaceIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeWorkspacesConnectionStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspacesConnectionStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacesconnectionstatuspaginator)
         """
 
 class ListAvailableManagementCidrRangesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.ListAvailableManagementCidrRanges)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#listavailablemanagementcidrrangespaginator)
     """
 
     def paginate(
-        self, *, ManagementCidrRangeConstraint: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        ManagementCidrRangeConstraint: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAvailableManagementCidrRangesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.ListAvailableManagementCidrRanges.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#listavailablemanagementcidrrangespaginator)
         """
```

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/type_defs.py` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,97 +60,105 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountModificationTypeDef",
     "AssociateConnectionAliasRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateConnectionAliasResultTypeDef",
     "AssociateIpGroupsRequestRequestTypeDef",
     "IpRuleItemTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
     "ClientPropertiesTypeDef",
     "ComputeTypeTypeDef",
     "ConnectClientAddInTypeDef",
     "ConnectionAliasAssociationTypeDef",
     "ConnectionAliasPermissionTypeDef",
     "TagTypeDef",
+    "CopyWorkspaceImageResultTypeDef",
     "CreateConnectClientAddInRequestRequestTypeDef",
+    "CreateConnectClientAddInResultTypeDef",
+    "CreateConnectionAliasResultTypeDef",
+    "CreateIpGroupResultTypeDef",
     "PendingCreateStandbyWorkspacesRequestTypeDef",
+    "CreateUpdatedWorkspaceImageResultTypeDef",
     "RootStorageTypeDef",
     "UserStorageTypeDef",
     "OperatingSystemTypeDef",
     "DefaultClientBrandingAttributesTypeDef",
     "DefaultImportClientBrandingAttributesTypeDef",
     "DefaultWorkspaceCreationPropertiesTypeDef",
     "DeleteClientBrandingRequestRequestTypeDef",
     "DeleteConnectClientAddInRequestRequestTypeDef",
     "DeleteConnectionAliasRequestRequestTypeDef",
     "DeleteIpGroupRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteWorkspaceBundleRequestRequestTypeDef",
     "DeleteWorkspaceImageRequestRequestTypeDef",
     "DeregisterWorkspaceDirectoryRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
     "DescribeAccountModificationsRequestRequestTypeDef",
+    "DescribeAccountResultTypeDef",
     "DescribeClientBrandingRequestRequestTypeDef",
     "IosClientBrandingAttributesTypeDef",
     "DescribeClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsRequestRequestTypeDef",
     "DescribeConnectionAliasPermissionsRequestRequestTypeDef",
     "DescribeConnectionAliasesRequestRequestTypeDef",
+    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
     "DescribeIpGroupsRequestRequestTypeDef",
     "DescribeTagsRequestRequestTypeDef",
+    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
+    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
     "DescribeWorkspaceDirectoriesRequestRequestTypeDef",
     "DescribeWorkspaceImagePermissionsRequestRequestTypeDef",
     "ImagePermissionTypeDef",
+    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     "DescribeWorkspaceSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
+    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     "WorkspaceConnectionStatusTypeDef",
+    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
     "DescribeWorkspacesRequestRequestTypeDef",
     "DisassociateConnectionAliasRequestRequestTypeDef",
     "DisassociateIpGroupsRequestRequestTypeDef",
     "FailedWorkspaceChangeRequestTypeDef",
     "IosImportClientBrandingAttributesTypeDef",
+    "ImportWorkspaceImageResultTypeDef",
+    "ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
     "ListAvailableManagementCidrRangesRequestRequestTypeDef",
+    "ListAvailableManagementCidrRangesResultTypeDef",
     "MigrateWorkspaceRequestRequestTypeDef",
+    "MigrateWorkspaceResultTypeDef",
     "ModificationStateTypeDef",
     "ModifyAccountRequestRequestTypeDef",
     "SamlPropertiesTypeDef",
     "SelfservicePermissionsTypeDef",
     "WorkspaceAccessPropertiesTypeDef",
     "WorkspaceCreationPropertiesTypeDef",
     "WorkspacePropertiesTypeDef",
     "ModifyWorkspaceStateRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "RebootRequestTypeDef",
     "RebuildRequestTypeDef",
     "RelatedWorkspacePropertiesTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreWorkspaceRequestRequestTypeDef",
     "RevokeIpRulesRequestRequestTypeDef",
     "StartRequestTypeDef",
     "StopRequestTypeDef",
     "TerminateRequestTypeDef",
     "UpdateConnectClientAddInRequestRequestTypeDef",
     "UpdateResultTypeDef",
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     "UpdateWorkspaceImagePermissionRequestRequestTypeDef",
-    "AssociateConnectionAliasResultTypeDef",
-    "CopyWorkspaceImageResultTypeDef",
-    "CreateConnectClientAddInResultTypeDef",
-    "CreateConnectionAliasResultTypeDef",
-    "CreateIpGroupResultTypeDef",
-    "CreateUpdatedWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsResultTypeDef",
-    "DescribeAccountResultTypeDef",
-    "ImportWorkspaceImageResultTypeDef",
-    "ListAvailableManagementCidrRangesResultTypeDef",
-    "MigrateWorkspaceResultTypeDef",
     "AuthorizeIpRulesRequestRequestTypeDef",
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
     "WorkspacesIpGroupTypeDef",
     "ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     "ClientPropertiesResultTypeDef",
     "ModifyClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsResultTypeDef",
@@ -166,22 +174,14 @@
     "DescribeTagsResultTypeDef",
     "ImportWorkspaceImageRequestRequestTypeDef",
     "RegisterWorkspaceDirectoryRequestRequestTypeDef",
     "StandbyWorkspaceTypeDef",
     "CreateWorkspaceBundleRequestRequestTypeDef",
     "WorkspaceBundleTypeDef",
     "CreateWorkspaceImageResultTypeDef",
-    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
-    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
-    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
-    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
-    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
-    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
-    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
-    "ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
     "DescribeClientBrandingResultTypeDef",
     "ImportClientBrandingResultTypeDef",
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     "DescribeWorkspaceSnapshotsResultTypeDef",
     "DescribeWorkspacesConnectionStatusResultTypeDef",
     "RebootWorkspacesResultTypeDef",
     "RebuildWorkspacesResultTypeDef",
@@ -236,22 +236,19 @@
     "AssociateConnectionAliasRequestRequestTypeDef",
     {
         "AliasId": str,
         "ResourceId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateConnectionAliasResultTypeDef = TypedDict(
+    "AssociateConnectionAliasResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ConnectionIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateIpGroupsRequestRequestTypeDef = TypedDict(
     "AssociateIpGroupsRequestRequestTypeDef",
     {
         "DirectoryId": str,
@@ -339,34 +336,74 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
+CopyWorkspaceImageResultTypeDef = TypedDict(
+    "CopyWorkspaceImageResultTypeDef",
+    {
+        "ImageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateConnectClientAddInRequestRequestTypeDef = TypedDict(
     "CreateConnectClientAddInRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
 )
 
+CreateConnectClientAddInResultTypeDef = TypedDict(
+    "CreateConnectClientAddInResultTypeDef",
+    {
+        "AddInId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateConnectionAliasResultTypeDef = TypedDict(
+    "CreateConnectionAliasResultTypeDef",
+    {
+        "AliasId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateIpGroupResultTypeDef = TypedDict(
+    "CreateIpGroupResultTypeDef",
+    {
+        "GroupId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PendingCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     {
         "UserName": str,
         "DirectoryId": str,
         "State": WorkspaceStateType,
         "WorkspaceId": str,
     },
     total=False,
 )
 
+CreateUpdatedWorkspaceImageResultTypeDef = TypedDict(
+    "CreateUpdatedWorkspaceImageResultTypeDef",
+    {
+        "ImageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RootStorageTypeDef = TypedDict(
     "RootStorageTypeDef",
     {
         "Capacity": str,
     },
     total=False,
 )
@@ -480,32 +517,39 @@
 DeregisterWorkspaceDirectoryRequestRequestTypeDef = TypedDict(
     "DeregisterWorkspaceDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef = TypedDict(
+    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAccountModificationsRequestRequestTypeDef = TypedDict(
     "DescribeAccountModificationsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeAccountResultTypeDef = TypedDict(
+    "DescribeAccountResultTypeDef",
+    {
+        "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
+        "DedicatedTenancyManagementCidrRange": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeClientBrandingRequestRequestTypeDef = TypedDict(
     "DescribeClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
@@ -583,14 +627,23 @@
         "ResourceId": str,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef = TypedDict(
+    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
+    {
+        "GroupIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeIpGroupsRequestRequestTypeDef = TypedDict(
     "DescribeIpGroupsRequestRequestTypeDef",
     {
         "GroupIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -600,24 +653,44 @@
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
+DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef = TypedDict(
+    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
+    {
+        "BundleIds": Sequence[str],
+        "Owner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeWorkspaceBundlesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     {
         "BundleIds": Sequence[str],
         "Owner": str,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef = TypedDict(
+    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
+    {
+        "DirectoryIds": Sequence[str],
+        "Limit": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeWorkspaceDirectoriesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceDirectoriesRequestRequestTypeDef",
     {
         "DirectoryIds": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -651,14 +724,24 @@
     "ImagePermissionTypeDef",
     {
         "SharedAccountId": str,
     },
     total=False,
 )
 
+DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef = TypedDict(
+    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
+    {
+        "ImageIds": Sequence[str],
+        "ImageType": ImageTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeWorkspaceImagesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     {
         "ImageIds": Sequence[str],
         "ImageType": ImageTypeType,
         "NextToken": str,
         "MaxResults": int,
@@ -677,14 +760,23 @@
     "SnapshotTypeDef",
     {
         "SnapshotTime": datetime,
     },
     total=False,
 )
 
+DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef = TypedDict(
+    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
+    {
+        "WorkspaceIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeWorkspacesConnectionStatusRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "NextToken": str,
     },
     total=False,
@@ -697,14 +789,26 @@
         "ConnectionState": ConnectionStateType,
         "ConnectionStateCheckTimestamp": datetime,
         "LastKnownUserConnectionTimestamp": datetime,
     },
     total=False,
 )
 
+DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef = TypedDict(
+    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
+    {
+        "WorkspaceIds": Sequence[str],
+        "DirectoryId": str,
+        "UserName": str,
+        "BundleId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeWorkspacesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "DirectoryId": str,
         "UserName": str,
         "BundleId": str,
@@ -749,14 +853,44 @@
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Mapping[str, str],
     },
     total=False,
 )
 
+ImportWorkspaceImageResultTypeDef = TypedDict(
+    "ImportWorkspaceImageResultTypeDef",
+    {
+        "ImageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
+    "_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
+    {
+        "ManagementCidrRangeConstraint": str,
+    },
+)
+_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
+    "_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef(
+    _RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
+    _OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableManagementCidrRangesRequestRequestTypeDef",
     {
         "ManagementCidrRangeConstraint": str,
     },
 )
 _OptionalListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
@@ -772,22 +906,40 @@
 class ListAvailableManagementCidrRangesRequestRequestTypeDef(
     _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef,
     _OptionalListAvailableManagementCidrRangesRequestRequestTypeDef,
 ):
     pass
 
 
+ListAvailableManagementCidrRangesResultTypeDef = TypedDict(
+    "ListAvailableManagementCidrRangesResultTypeDef",
+    {
+        "ManagementCidrRanges": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MigrateWorkspaceRequestRequestTypeDef = TypedDict(
     "MigrateWorkspaceRequestRequestTypeDef",
     {
         "SourceWorkspaceId": str,
         "BundleId": str,
     },
 )
 
+MigrateWorkspaceResultTypeDef = TypedDict(
+    "MigrateWorkspaceResultTypeDef",
+    {
+        "SourceWorkspaceId": str,
+        "TargetWorkspaceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ModificationStateTypeDef = TypedDict(
     "ModificationStateTypeDef",
     {
         "Resource": ModificationResourceEnumType,
         "State": ModificationStateEnumType,
     },
     total=False,
@@ -869,14 +1021,24 @@
     "ModifyWorkspaceStateRequestRequestTypeDef",
     {
         "WorkspaceId": str,
         "WorkspaceState": TargetWorkspaceStateType,
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
 RebootRequestTypeDef = TypedDict(
     "RebootRequestTypeDef",
     {
         "WorkspaceId": str,
     },
 )
 
@@ -894,14 +1056,25 @@
         "Region": str,
         "State": WorkspaceStateType,
         "Type": StandbyWorkspaceRelationshipTypeType,
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
 RestoreWorkspaceRequestRequestTypeDef = TypedDict(
     "RestoreWorkspaceRequestRequestTypeDef",
     {
         "WorkspaceId": str,
     },
 )
 
@@ -983,103 +1156,20 @@
     {
         "ImageId": str,
         "AllowCopyImage": bool,
         "SharedAccountId": str,
     },
 )
 
-AssociateConnectionAliasResultTypeDef = TypedDict(
-    "AssociateConnectionAliasResultTypeDef",
-    {
-        "ConnectionIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CopyWorkspaceImageResultTypeDef = TypedDict(
-    "CopyWorkspaceImageResultTypeDef",
-    {
-        "ImageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateConnectClientAddInResultTypeDef = TypedDict(
-    "CreateConnectClientAddInResultTypeDef",
-    {
-        "AddInId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateConnectionAliasResultTypeDef = TypedDict(
-    "CreateConnectionAliasResultTypeDef",
-    {
-        "AliasId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIpGroupResultTypeDef = TypedDict(
-    "CreateIpGroupResultTypeDef",
-    {
-        "GroupId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUpdatedWorkspaceImageResultTypeDef = TypedDict(
-    "CreateUpdatedWorkspaceImageResultTypeDef",
-    {
-        "ImageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAccountModificationsResultTypeDef = TypedDict(
     "DescribeAccountModificationsResultTypeDef",
     {
         "AccountModifications": List[AccountModificationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountResultTypeDef = TypedDict(
-    "DescribeAccountResultTypeDef",
-    {
-        "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
-        "DedicatedTenancyManagementCidrRange": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportWorkspaceImageResultTypeDef = TypedDict(
-    "ImportWorkspaceImageResultTypeDef",
-    {
-        "ImageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAvailableManagementCidrRangesResultTypeDef = TypedDict(
-    "ListAvailableManagementCidrRangesResultTypeDef",
-    {
-        "ManagementCidrRanges": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MigrateWorkspaceResultTypeDef = TypedDict(
-    "MigrateWorkspaceResultTypeDef",
-    {
-        "SourceWorkspaceId": str,
-        "TargetWorkspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthorizeIpRulesRequestRequestTypeDef = TypedDict(
     "AuthorizeIpRulesRequestRequestTypeDef",
     {
         "GroupId": str,
@@ -1149,15 +1239,15 @@
 )
 
 DescribeConnectClientAddInsResultTypeDef = TypedDict(
     "DescribeConnectClientAddInsResultTypeDef",
     {
         "AddIns": List[ConnectClientAddInTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConnectionAliasTypeDef = TypedDict(
     "ConnectionAliasTypeDef",
     {
         "ConnectionString": str,
@@ -1171,15 +1261,15 @@
 
 DescribeConnectionAliasPermissionsResultTypeDef = TypedDict(
     "DescribeConnectionAliasPermissionsResultTypeDef",
     {
         "AliasId": str,
         "ConnectionAliasPermissions": List[ConnectionAliasPermissionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConnectionAliasPermissionRequestRequestTypeDef = TypedDict(
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
     {
         "AliasId": str,
@@ -1313,15 +1403,15 @@
     pass
 
 
 DescribeTagsResultTypeDef = TypedDict(
     "DescribeTagsResultTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportWorkspaceImageRequestRequestTypeDef = TypedDict(
     "_RequiredImportWorkspaceImageRequestRequestTypeDef",
     {
         "Ec2ImageId": str,
@@ -1447,199 +1537,109 @@
         "Name": str,
         "Description": str,
         "OperatingSystem": OperatingSystemTypeDef,
         "State": WorkspaceImageStateType,
         "RequiredTenancy": WorkspaceImageRequiredTenancyType,
         "Created": datetime,
         "OwnerAccountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef = TypedDict(
-    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef = TypedDict(
-    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
-    {
-        "GroupIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef = TypedDict(
-    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
-    {
-        "BundleIds": Sequence[str],
-        "Owner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef = TypedDict(
-    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
-    {
-        "DirectoryIds": Sequence[str],
-        "Limit": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef = TypedDict(
-    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
-    {
-        "ImageIds": Sequence[str],
-        "ImageType": ImageTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef = TypedDict(
-    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
-    {
-        "WorkspaceIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef = TypedDict(
-    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
-    {
-        "WorkspaceIds": Sequence[str],
-        "DirectoryId": str,
-        "UserName": str,
-        "BundleId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
-    "_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
-    {
-        "ManagementCidrRangeConstraint": str,
-    },
-)
-_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
-    "_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef(
-    _RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
-    _OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
-):
-    pass
-
-
 DescribeClientBrandingResultTypeDef = TypedDict(
     "DescribeClientBrandingResultTypeDef",
     {
         "DeviceTypeWindows": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeOsx": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeAndroid": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeIos": IosClientBrandingAttributesTypeDef,
         "DeviceTypeLinux": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeWeb": DefaultClientBrandingAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportClientBrandingResultTypeDef = TypedDict(
     "ImportClientBrandingResultTypeDef",
     {
         "DeviceTypeWindows": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeOsx": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeAndroid": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeIos": IosClientBrandingAttributesTypeDef,
         "DeviceTypeLinux": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeWeb": DefaultClientBrandingAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspaceImagePermissionsResultTypeDef = TypedDict(
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     {
         "ImageId": str,
         "ImagePermissions": List[ImagePermissionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspaceSnapshotsResultTypeDef = TypedDict(
     "DescribeWorkspaceSnapshotsResultTypeDef",
     {
         "RebuildSnapshots": List[SnapshotTypeDef],
         "RestoreSnapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspacesConnectionStatusResultTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusResultTypeDef",
     {
         "WorkspacesConnectionStatus": List[WorkspaceConnectionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootWorkspacesResultTypeDef = TypedDict(
     "RebootWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebuildWorkspacesResultTypeDef = TypedDict(
     "RebuildWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartWorkspacesResultTypeDef = TypedDict(
     "StartWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopWorkspacesResultTypeDef = TypedDict(
     "StopWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TerminateWorkspacesResultTypeDef = TypedDict(
     "TerminateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportClientBrandingRequestRequestTypeDef = TypedDict(
     "_RequiredImportClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
@@ -1848,32 +1848,32 @@
 )
 
 DescribeIpGroupsResultTypeDef = TypedDict(
     "DescribeIpGroupsResultTypeDef",
     {
         "Result": List[WorkspacesIpGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClientPropertiesResultTypeDef = TypedDict(
     "DescribeClientPropertiesResultTypeDef",
     {
         "ClientPropertiesList": List[ClientPropertiesResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectionAliasesResultTypeDef = TypedDict(
     "DescribeConnectionAliasesResultTypeDef",
     {
         "ConnectionAliases": List[ConnectionAliasTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
     "CreateStandbyWorkspacesRequestRequestTypeDef",
     {
         "PrimaryRegion": str,
@@ -1891,33 +1891,33 @@
     total=False,
 )
 
 CreateWorkspaceBundleResultTypeDef = TypedDict(
     "CreateWorkspaceBundleResultTypeDef",
     {
         "WorkspaceBundle": WorkspaceBundleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspaceBundlesResultTypeDef = TypedDict(
     "DescribeWorkspaceBundlesResultTypeDef",
     {
         "Bundles": List[WorkspaceBundleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspaceDirectoriesResultTypeDef = TypedDict(
     "DescribeWorkspaceDirectoriesResultTypeDef",
     {
         "Directories": List[WorkspaceDirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateWorkspacesRequestRequestTypeDef = TypedDict(
     "CreateWorkspacesRequestRequestTypeDef",
     {
         "Workspaces": Sequence[WorkspaceRequestTypeDef],
@@ -1935,37 +1935,37 @@
 )
 
 DescribeWorkspacesResultTypeDef = TypedDict(
     "DescribeWorkspacesResultTypeDef",
     {
         "Workspaces": List[WorkspaceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspaceImagesResultTypeDef = TypedDict(
     "DescribeWorkspaceImagesResultTypeDef",
     {
         "Images": List[WorkspaceImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStandbyWorkspacesResultTypeDef = TypedDict(
     "CreateStandbyWorkspacesResultTypeDef",
     {
         "FailedStandbyRequests": List[FailedCreateStandbyWorkspacesRequestTypeDef],
         "PendingStandbyRequests": List[PendingCreateStandbyWorkspacesRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateWorkspacesResultTypeDef = TypedDict(
     "CreateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedCreateWorkspaceRequestTypeDef],
         "PendingRequests": List[WorkspaceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/type_defs.pyi` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,97 +59,105 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountModificationTypeDef",
     "AssociateConnectionAliasRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateConnectionAliasResultTypeDef",
     "AssociateIpGroupsRequestRequestTypeDef",
     "IpRuleItemTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
     "ClientPropertiesTypeDef",
     "ComputeTypeTypeDef",
     "ConnectClientAddInTypeDef",
     "ConnectionAliasAssociationTypeDef",
     "ConnectionAliasPermissionTypeDef",
     "TagTypeDef",
+    "CopyWorkspaceImageResultTypeDef",
     "CreateConnectClientAddInRequestRequestTypeDef",
+    "CreateConnectClientAddInResultTypeDef",
+    "CreateConnectionAliasResultTypeDef",
+    "CreateIpGroupResultTypeDef",
     "PendingCreateStandbyWorkspacesRequestTypeDef",
+    "CreateUpdatedWorkspaceImageResultTypeDef",
     "RootStorageTypeDef",
     "UserStorageTypeDef",
     "OperatingSystemTypeDef",
     "DefaultClientBrandingAttributesTypeDef",
     "DefaultImportClientBrandingAttributesTypeDef",
     "DefaultWorkspaceCreationPropertiesTypeDef",
     "DeleteClientBrandingRequestRequestTypeDef",
     "DeleteConnectClientAddInRequestRequestTypeDef",
     "DeleteConnectionAliasRequestRequestTypeDef",
     "DeleteIpGroupRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteWorkspaceBundleRequestRequestTypeDef",
     "DeleteWorkspaceImageRequestRequestTypeDef",
     "DeregisterWorkspaceDirectoryRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
     "DescribeAccountModificationsRequestRequestTypeDef",
+    "DescribeAccountResultTypeDef",
     "DescribeClientBrandingRequestRequestTypeDef",
     "IosClientBrandingAttributesTypeDef",
     "DescribeClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsRequestRequestTypeDef",
     "DescribeConnectionAliasPermissionsRequestRequestTypeDef",
     "DescribeConnectionAliasesRequestRequestTypeDef",
+    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
     "DescribeIpGroupsRequestRequestTypeDef",
     "DescribeTagsRequestRequestTypeDef",
+    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
+    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
     "DescribeWorkspaceDirectoriesRequestRequestTypeDef",
     "DescribeWorkspaceImagePermissionsRequestRequestTypeDef",
     "ImagePermissionTypeDef",
+    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     "DescribeWorkspaceSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
+    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     "WorkspaceConnectionStatusTypeDef",
+    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
     "DescribeWorkspacesRequestRequestTypeDef",
     "DisassociateConnectionAliasRequestRequestTypeDef",
     "DisassociateIpGroupsRequestRequestTypeDef",
     "FailedWorkspaceChangeRequestTypeDef",
     "IosImportClientBrandingAttributesTypeDef",
+    "ImportWorkspaceImageResultTypeDef",
+    "ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
     "ListAvailableManagementCidrRangesRequestRequestTypeDef",
+    "ListAvailableManagementCidrRangesResultTypeDef",
     "MigrateWorkspaceRequestRequestTypeDef",
+    "MigrateWorkspaceResultTypeDef",
     "ModificationStateTypeDef",
     "ModifyAccountRequestRequestTypeDef",
     "SamlPropertiesTypeDef",
     "SelfservicePermissionsTypeDef",
     "WorkspaceAccessPropertiesTypeDef",
     "WorkspaceCreationPropertiesTypeDef",
     "WorkspacePropertiesTypeDef",
     "ModifyWorkspaceStateRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "RebootRequestTypeDef",
     "RebuildRequestTypeDef",
     "RelatedWorkspacePropertiesTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreWorkspaceRequestRequestTypeDef",
     "RevokeIpRulesRequestRequestTypeDef",
     "StartRequestTypeDef",
     "StopRequestTypeDef",
     "TerminateRequestTypeDef",
     "UpdateConnectClientAddInRequestRequestTypeDef",
     "UpdateResultTypeDef",
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     "UpdateWorkspaceImagePermissionRequestRequestTypeDef",
-    "AssociateConnectionAliasResultTypeDef",
-    "CopyWorkspaceImageResultTypeDef",
-    "CreateConnectClientAddInResultTypeDef",
-    "CreateConnectionAliasResultTypeDef",
-    "CreateIpGroupResultTypeDef",
-    "CreateUpdatedWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsResultTypeDef",
-    "DescribeAccountResultTypeDef",
-    "ImportWorkspaceImageResultTypeDef",
-    "ListAvailableManagementCidrRangesResultTypeDef",
-    "MigrateWorkspaceResultTypeDef",
     "AuthorizeIpRulesRequestRequestTypeDef",
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
     "WorkspacesIpGroupTypeDef",
     "ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     "ClientPropertiesResultTypeDef",
     "ModifyClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsResultTypeDef",
@@ -165,22 +173,14 @@
     "DescribeTagsResultTypeDef",
     "ImportWorkspaceImageRequestRequestTypeDef",
     "RegisterWorkspaceDirectoryRequestRequestTypeDef",
     "StandbyWorkspaceTypeDef",
     "CreateWorkspaceBundleRequestRequestTypeDef",
     "WorkspaceBundleTypeDef",
     "CreateWorkspaceImageResultTypeDef",
-    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
-    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
-    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
-    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
-    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
-    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
-    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
-    "ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
     "DescribeClientBrandingResultTypeDef",
     "ImportClientBrandingResultTypeDef",
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     "DescribeWorkspaceSnapshotsResultTypeDef",
     "DescribeWorkspacesConnectionStatusResultTypeDef",
     "RebootWorkspacesResultTypeDef",
     "RebuildWorkspacesResultTypeDef",
@@ -235,22 +235,19 @@
     "AssociateConnectionAliasRequestRequestTypeDef",
     {
         "AliasId": str,
         "ResourceId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateConnectionAliasResultTypeDef = TypedDict(
+    "AssociateConnectionAliasResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ConnectionIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateIpGroupsRequestRequestTypeDef = TypedDict(
     "AssociateIpGroupsRequestRequestTypeDef",
     {
         "DirectoryId": str,
@@ -336,34 +333,74 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+CopyWorkspaceImageResultTypeDef = TypedDict(
+    "CopyWorkspaceImageResultTypeDef",
+    {
+        "ImageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateConnectClientAddInRequestRequestTypeDef = TypedDict(
     "CreateConnectClientAddInRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
 )
 
+CreateConnectClientAddInResultTypeDef = TypedDict(
+    "CreateConnectClientAddInResultTypeDef",
+    {
+        "AddInId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateConnectionAliasResultTypeDef = TypedDict(
+    "CreateConnectionAliasResultTypeDef",
+    {
+        "AliasId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateIpGroupResultTypeDef = TypedDict(
+    "CreateIpGroupResultTypeDef",
+    {
+        "GroupId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PendingCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     {
         "UserName": str,
         "DirectoryId": str,
         "State": WorkspaceStateType,
         "WorkspaceId": str,
     },
     total=False,
 )
 
+CreateUpdatedWorkspaceImageResultTypeDef = TypedDict(
+    "CreateUpdatedWorkspaceImageResultTypeDef",
+    {
+        "ImageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RootStorageTypeDef = TypedDict(
     "RootStorageTypeDef",
     {
         "Capacity": str,
     },
     total=False,
 )
@@ -477,32 +514,39 @@
 DeregisterWorkspaceDirectoryRequestRequestTypeDef = TypedDict(
     "DeregisterWorkspaceDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef = TypedDict(
+    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAccountModificationsRequestRequestTypeDef = TypedDict(
     "DescribeAccountModificationsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeAccountResultTypeDef = TypedDict(
+    "DescribeAccountResultTypeDef",
+    {
+        "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
+        "DedicatedTenancyManagementCidrRange": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeClientBrandingRequestRequestTypeDef = TypedDict(
     "DescribeClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
@@ -576,14 +620,23 @@
         "ResourceId": str,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef = TypedDict(
+    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
+    {
+        "GroupIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeIpGroupsRequestRequestTypeDef = TypedDict(
     "DescribeIpGroupsRequestRequestTypeDef",
     {
         "GroupIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -593,24 +646,44 @@
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
+DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef = TypedDict(
+    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
+    {
+        "BundleIds": Sequence[str],
+        "Owner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeWorkspaceBundlesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     {
         "BundleIds": Sequence[str],
         "Owner": str,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef = TypedDict(
+    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
+    {
+        "DirectoryIds": Sequence[str],
+        "Limit": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeWorkspaceDirectoriesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceDirectoriesRequestRequestTypeDef",
     {
         "DirectoryIds": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -642,14 +715,24 @@
     "ImagePermissionTypeDef",
     {
         "SharedAccountId": str,
     },
     total=False,
 )
 
+DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef = TypedDict(
+    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
+    {
+        "ImageIds": Sequence[str],
+        "ImageType": ImageTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeWorkspaceImagesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     {
         "ImageIds": Sequence[str],
         "ImageType": ImageTypeType,
         "NextToken": str,
         "MaxResults": int,
@@ -668,14 +751,23 @@
     "SnapshotTypeDef",
     {
         "SnapshotTime": datetime,
     },
     total=False,
 )
 
+DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef = TypedDict(
+    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
+    {
+        "WorkspaceIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeWorkspacesConnectionStatusRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "NextToken": str,
     },
     total=False,
@@ -688,14 +780,26 @@
         "ConnectionState": ConnectionStateType,
         "ConnectionStateCheckTimestamp": datetime,
         "LastKnownUserConnectionTimestamp": datetime,
     },
     total=False,
 )
 
+DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef = TypedDict(
+    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
+    {
+        "WorkspaceIds": Sequence[str],
+        "DirectoryId": str,
+        "UserName": str,
+        "BundleId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeWorkspacesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "DirectoryId": str,
         "UserName": str,
         "BundleId": str,
@@ -740,14 +844,42 @@
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Mapping[str, str],
     },
     total=False,
 )
 
+ImportWorkspaceImageResultTypeDef = TypedDict(
+    "ImportWorkspaceImageResultTypeDef",
+    {
+        "ImageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
+    "_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
+    {
+        "ManagementCidrRangeConstraint": str,
+    },
+)
+_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
+    "_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef(
+    _RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
+    _OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
+):
+    pass
+
 _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableManagementCidrRangesRequestRequestTypeDef",
     {
         "ManagementCidrRangeConstraint": str,
     },
 )
 _OptionalListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
@@ -761,22 +893,40 @@
 
 class ListAvailableManagementCidrRangesRequestRequestTypeDef(
     _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef,
     _OptionalListAvailableManagementCidrRangesRequestRequestTypeDef,
 ):
     pass
 
+ListAvailableManagementCidrRangesResultTypeDef = TypedDict(
+    "ListAvailableManagementCidrRangesResultTypeDef",
+    {
+        "ManagementCidrRanges": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MigrateWorkspaceRequestRequestTypeDef = TypedDict(
     "MigrateWorkspaceRequestRequestTypeDef",
     {
         "SourceWorkspaceId": str,
         "BundleId": str,
     },
 )
 
+MigrateWorkspaceResultTypeDef = TypedDict(
+    "MigrateWorkspaceResultTypeDef",
+    {
+        "SourceWorkspaceId": str,
+        "TargetWorkspaceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ModificationStateTypeDef = TypedDict(
     "ModificationStateTypeDef",
     {
         "Resource": ModificationResourceEnumType,
         "State": ModificationStateEnumType,
     },
     total=False,
@@ -858,14 +1008,24 @@
     "ModifyWorkspaceStateRequestRequestTypeDef",
     {
         "WorkspaceId": str,
         "WorkspaceState": TargetWorkspaceStateType,
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
 RebootRequestTypeDef = TypedDict(
     "RebootRequestTypeDef",
     {
         "WorkspaceId": str,
     },
 )
 
@@ -883,14 +1043,25 @@
         "Region": str,
         "State": WorkspaceStateType,
         "Type": StandbyWorkspaceRelationshipTypeType,
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
 RestoreWorkspaceRequestRequestTypeDef = TypedDict(
     "RestoreWorkspaceRequestRequestTypeDef",
     {
         "WorkspaceId": str,
     },
 )
 
@@ -970,103 +1141,20 @@
     {
         "ImageId": str,
         "AllowCopyImage": bool,
         "SharedAccountId": str,
     },
 )
 
-AssociateConnectionAliasResultTypeDef = TypedDict(
-    "AssociateConnectionAliasResultTypeDef",
-    {
-        "ConnectionIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CopyWorkspaceImageResultTypeDef = TypedDict(
-    "CopyWorkspaceImageResultTypeDef",
-    {
-        "ImageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateConnectClientAddInResultTypeDef = TypedDict(
-    "CreateConnectClientAddInResultTypeDef",
-    {
-        "AddInId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateConnectionAliasResultTypeDef = TypedDict(
-    "CreateConnectionAliasResultTypeDef",
-    {
-        "AliasId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIpGroupResultTypeDef = TypedDict(
-    "CreateIpGroupResultTypeDef",
-    {
-        "GroupId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUpdatedWorkspaceImageResultTypeDef = TypedDict(
-    "CreateUpdatedWorkspaceImageResultTypeDef",
-    {
-        "ImageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAccountModificationsResultTypeDef = TypedDict(
     "DescribeAccountModificationsResultTypeDef",
     {
         "AccountModifications": List[AccountModificationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountResultTypeDef = TypedDict(
-    "DescribeAccountResultTypeDef",
-    {
-        "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
-        "DedicatedTenancyManagementCidrRange": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportWorkspaceImageResultTypeDef = TypedDict(
-    "ImportWorkspaceImageResultTypeDef",
-    {
-        "ImageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAvailableManagementCidrRangesResultTypeDef = TypedDict(
-    "ListAvailableManagementCidrRangesResultTypeDef",
-    {
-        "ManagementCidrRanges": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MigrateWorkspaceResultTypeDef = TypedDict(
-    "MigrateWorkspaceResultTypeDef",
-    {
-        "SourceWorkspaceId": str,
-        "TargetWorkspaceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthorizeIpRulesRequestRequestTypeDef = TypedDict(
     "AuthorizeIpRulesRequestRequestTypeDef",
     {
         "GroupId": str,
@@ -1134,15 +1222,15 @@
 )
 
 DescribeConnectClientAddInsResultTypeDef = TypedDict(
     "DescribeConnectClientAddInsResultTypeDef",
     {
         "AddIns": List[ConnectClientAddInTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConnectionAliasTypeDef = TypedDict(
     "ConnectionAliasTypeDef",
     {
         "ConnectionString": str,
@@ -1156,15 +1244,15 @@
 
 DescribeConnectionAliasPermissionsResultTypeDef = TypedDict(
     "DescribeConnectionAliasPermissionsResultTypeDef",
     {
         "AliasId": str,
         "ConnectionAliasPermissions": List[ConnectionAliasPermissionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConnectionAliasPermissionRequestRequestTypeDef = TypedDict(
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
     {
         "AliasId": str,
@@ -1288,15 +1376,15 @@
 ):
     pass
 
 DescribeTagsResultTypeDef = TypedDict(
     "DescribeTagsResultTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportWorkspaceImageRequestRequestTypeDef = TypedDict(
     "_RequiredImportWorkspaceImageRequestRequestTypeDef",
     {
         "Ec2ImageId": str,
@@ -1414,197 +1502,109 @@
         "Name": str,
         "Description": str,
         "OperatingSystem": OperatingSystemTypeDef,
         "State": WorkspaceImageStateType,
         "RequiredTenancy": WorkspaceImageRequiredTenancyType,
         "Created": datetime,
         "OwnerAccountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef = TypedDict(
-    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef = TypedDict(
-    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
-    {
-        "GroupIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef = TypedDict(
-    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
-    {
-        "BundleIds": Sequence[str],
-        "Owner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef = TypedDict(
-    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
-    {
-        "DirectoryIds": Sequence[str],
-        "Limit": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef = TypedDict(
-    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
-    {
-        "ImageIds": Sequence[str],
-        "ImageType": ImageTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef = TypedDict(
-    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
-    {
-        "WorkspaceIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef = TypedDict(
-    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
-    {
-        "WorkspaceIds": Sequence[str],
-        "DirectoryId": str,
-        "UserName": str,
-        "BundleId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
-    "_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
-    {
-        "ManagementCidrRangeConstraint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
-    "_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef(
-    _RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
-    _OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
-):
-    pass
 
 DescribeClientBrandingResultTypeDef = TypedDict(
     "DescribeClientBrandingResultTypeDef",
     {
         "DeviceTypeWindows": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeOsx": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeAndroid": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeIos": IosClientBrandingAttributesTypeDef,
         "DeviceTypeLinux": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeWeb": DefaultClientBrandingAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportClientBrandingResultTypeDef = TypedDict(
     "ImportClientBrandingResultTypeDef",
     {
         "DeviceTypeWindows": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeOsx": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeAndroid": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeIos": IosClientBrandingAttributesTypeDef,
         "DeviceTypeLinux": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeWeb": DefaultClientBrandingAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspaceImagePermissionsResultTypeDef = TypedDict(
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     {
         "ImageId": str,
         "ImagePermissions": List[ImagePermissionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspaceSnapshotsResultTypeDef = TypedDict(
     "DescribeWorkspaceSnapshotsResultTypeDef",
     {
         "RebuildSnapshots": List[SnapshotTypeDef],
         "RestoreSnapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspacesConnectionStatusResultTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusResultTypeDef",
     {
         "WorkspacesConnectionStatus": List[WorkspaceConnectionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootWorkspacesResultTypeDef = TypedDict(
     "RebootWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebuildWorkspacesResultTypeDef = TypedDict(
     "RebuildWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartWorkspacesResultTypeDef = TypedDict(
     "StartWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopWorkspacesResultTypeDef = TypedDict(
     "StopWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TerminateWorkspacesResultTypeDef = TypedDict(
     "TerminateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportClientBrandingRequestRequestTypeDef = TypedDict(
     "_RequiredImportClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
@@ -1807,32 +1807,32 @@
 )
 
 DescribeIpGroupsResultTypeDef = TypedDict(
     "DescribeIpGroupsResultTypeDef",
     {
         "Result": List[WorkspacesIpGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClientPropertiesResultTypeDef = TypedDict(
     "DescribeClientPropertiesResultTypeDef",
     {
         "ClientPropertiesList": List[ClientPropertiesResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectionAliasesResultTypeDef = TypedDict(
     "DescribeConnectionAliasesResultTypeDef",
     {
         "ConnectionAliases": List[ConnectionAliasTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
     "CreateStandbyWorkspacesRequestRequestTypeDef",
     {
         "PrimaryRegion": str,
@@ -1850,33 +1850,33 @@
     total=False,
 )
 
 CreateWorkspaceBundleResultTypeDef = TypedDict(
     "CreateWorkspaceBundleResultTypeDef",
     {
         "WorkspaceBundle": WorkspaceBundleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspaceBundlesResultTypeDef = TypedDict(
     "DescribeWorkspaceBundlesResultTypeDef",
     {
         "Bundles": List[WorkspaceBundleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspaceDirectoriesResultTypeDef = TypedDict(
     "DescribeWorkspaceDirectoriesResultTypeDef",
     {
         "Directories": List[WorkspaceDirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateWorkspacesRequestRequestTypeDef = TypedDict(
     "CreateWorkspacesRequestRequestTypeDef",
     {
         "Workspaces": Sequence[WorkspaceRequestTypeDef],
@@ -1894,37 +1894,37 @@
 )
 
 DescribeWorkspacesResultTypeDef = TypedDict(
     "DescribeWorkspacesResultTypeDef",
     {
         "Workspaces": List[WorkspaceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspaceImagesResultTypeDef = TypedDict(
     "DescribeWorkspaceImagesResultTypeDef",
     {
         "Images": List[WorkspaceImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStandbyWorkspacesResultTypeDef = TypedDict(
     "CreateStandbyWorkspacesResultTypeDef",
     {
         "FailedStandbyRequests": List[FailedCreateStandbyWorkspacesRequestTypeDef],
         "PendingStandbyRequests": List[PendingCreateStandbyWorkspacesRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateWorkspacesResultTypeDef = TypedDict(
     "CreateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedCreateWorkspaceRequestTypeDef],
         "PendingRequests": List[WorkspaceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/PKG-INFO` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces
-Version: 1.26.68
-Summary: Type annotations for boto3.WorkSpaces 1.26.68 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.WorkSpaces 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-workspaces"></a>
 
 # mypy-boto3-workspaces
 
 [![PyPI - mypy-boto3-workspaces](https://img.shields.io/pypi/v/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
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
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,97 +390,105 @@
 `mypy_boto3_workspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateConnectionAliasResultTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ClientPropertiesTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
+    CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
+    CreateConnectClientAddInResultTypeDef,
+    CreateConnectionAliasResultTypeDef,
+    CreateIpGroupResultTypeDef,
     PendingCreateStandbyWorkspacesRequestTypeDef,
+    CreateUpdatedWorkspaceImageResultTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
     DefaultClientBrandingAttributesTypeDef,
     DefaultImportClientBrandingAttributesTypeDef,
     DefaultWorkspaceCreationPropertiesTypeDef,
     DeleteClientBrandingRequestRequestTypeDef,
     DeleteConnectClientAddInRequestRequestTypeDef,
     DeleteConnectionAliasRequestRequestTypeDef,
     DeleteIpGroupRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteWorkspaceBundleRequestRequestTypeDef,
     DeleteWorkspaceImageRequestRequestTypeDef,
     DeregisterWorkspaceDirectoryRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
     DescribeAccountModificationsRequestRequestTypeDef,
+    DescribeAccountResultTypeDef,
     DescribeClientBrandingRequestRequestTypeDef,
     IosClientBrandingAttributesTypeDef,
     DescribeClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsRequestRequestTypeDef,
     DescribeConnectionAliasPermissionsRequestRequestTypeDef,
     DescribeConnectionAliasesRequestRequestTypeDef,
+    DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeIpGroupsRequestRequestTypeDef,
     DescribeTagsRequestRequestTypeDef,
+    DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
     DescribeWorkspaceBundlesRequestRequestTypeDef,
+    DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestRequestTypeDef,
     DescribeWorkspaceImagePermissionsRequestRequestTypeDef,
     ImagePermissionTypeDef,
+    DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
     DescribeWorkspaceImagesRequestRequestTypeDef,
     DescribeWorkspaceSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
+    DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
     DescribeWorkspacesConnectionStatusRequestRequestTypeDef,
     WorkspaceConnectionStatusTypeDef,
+    DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
     DescribeWorkspacesRequestRequestTypeDef,
     DisassociateConnectionAliasRequestRequestTypeDef,
     DisassociateIpGroupsRequestRequestTypeDef,
     FailedWorkspaceChangeRequestTypeDef,
     IosImportClientBrandingAttributesTypeDef,
+    ImportWorkspaceImageResultTypeDef,
+    ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     ListAvailableManagementCidrRangesRequestRequestTypeDef,
+    ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceRequestRequestTypeDef,
+    MigrateWorkspaceResultTypeDef,
     ModificationStateTypeDef,
     ModifyAccountRequestRequestTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
     RelatedWorkspacePropertiesTypeDef,
+    ResponseMetadataTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
     UpdateWorkspaceBundleRequestRequestTypeDef,
     UpdateWorkspaceImagePermissionRequestRequestTypeDef,
-    AssociateConnectionAliasResultTypeDef,
-    CopyWorkspaceImageResultTypeDef,
-    CreateConnectClientAddInResultTypeDef,
-    CreateConnectionAliasResultTypeDef,
-    CreateIpGroupResultTypeDef,
-    CreateUpdatedWorkspaceImageResultTypeDef,
     DescribeAccountModificationsResultTypeDef,
-    DescribeAccountResultTypeDef,
-    ImportWorkspaceImageResultTypeDef,
-    ListAvailableManagementCidrRangesResultTypeDef,
-    MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
     WorkspacesIpGroupTypeDef,
     ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
@@ -496,22 +504,14 @@
     DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
     StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
     WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
-    DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
-    DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
-    DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
-    DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
-    DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
-    DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
-    DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
-    ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     DescribeClientBrandingResultTypeDef,
     ImportClientBrandingResultTypeDef,
     DescribeWorkspaceImagePermissionsResultTypeDef,
     DescribeWorkspaceSnapshotsResultTypeDef,
     DescribeWorkspacesConnectionStatusResultTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildWorkspacesResultTypeDef,
@@ -557,42 +557,42 @@
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

### Comparing `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/SOURCES.txt` & `mypy-boto3-workspaces-1.27.0/mypy_boto3_workspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.26.68/setup.py` & `mypy-boto3-workspaces-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-workspaces.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workspaces",
-    version="1.26.68",
+    version="1.27.0",
     packages=["mypy_boto3_workspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkSpaces 1.26.68 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.WorkSpaces 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/",
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


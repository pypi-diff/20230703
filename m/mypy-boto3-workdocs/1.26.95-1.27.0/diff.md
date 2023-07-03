# Comparing `tmp/mypy-boto3-workdocs-1.26.95.tar.gz` & `tmp/mypy-boto3-workdocs-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workdocs-1.26.95.tar", last modified: Mon Mar 20 19:32:46 2023, max compression
+gzip compressed data, was "mypy-boto3-workdocs-1.27.0.tar", last modified: Mon Jul  3 19:51:36 2023, max compression
```

## Comparing `mypy-boto3-workdocs-1.26.95.tar` & `mypy-boto3-workdocs-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:46.551025 mypy-boto3-workdocs-1.26.95/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-03-20 19:32:46.547025 mypy-boto3-workdocs-1.26.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:46.547025 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38652 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38591 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-03-20 19:32:34.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13859 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50540 2023-03-20 19:32:35.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50449 2023-03-20 19:32:34.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:46.547025 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-03-20 19:32:46.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-20 19:32:46.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:32:46.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:32:46.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-20 19:32:46.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-20 19:32:46.000000 mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 19:32:46.551025 mypy-boto3-workdocs-1.26.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-20 19:32:33.000000 mypy-boto3-workdocs-1.26.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:36.704152 mypy-boto3-workdocs-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-03 19:51:36.704152 mypy-boto3-workdocs-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:36.704152 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38652 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38591 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-07-03 19:49:46.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13800 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50612 2023-07-03 19:49:46.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50521 2023-07-03 19:49:46.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:36.704152 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-03 19:51:36.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:51:36.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:36.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:36.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:36.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:36.000000 mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:36.704152 mypy-boto3-workdocs-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:49:45.000000 mypy-boto3-workdocs-1.27.0/setup.py
```

### Comparing `mypy-boto3-workdocs-1.26.95/LICENSE` & `mypy-boto3-workdocs-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-workdocs-1.26.95/PKG-INFO` & `mypy-boto3-workdocs-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workdocs
-Version: 1.26.95
-Summary: Type annotations for boto3.WorkDocs 1.26.95 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.WorkDocs 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-workdocs"></a>
 
 # mypy-boto3-workdocs
 
 [![PyPI - mypy-boto3-workdocs](https://img.shields.io/pypi/v/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workdocs?color=blue)](https://pypistats.org/packages/mypy-boto3-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkDocs 1.26.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[boto3.WorkDocs 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workdocs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -397,15 +397,14 @@
 `mypy_boto3_workdocs.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workdocs.type_defs import (
     AbortDocumentVersionUploadRequestRequestTypeDef,
     ActivateUserRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UserMetadataTypeDef,
     NotificationOptionsTypeDef,
     SharePrincipalTypeDef,
     ShareResultTypeDef,
     CreateCommentRequestRequestTypeDef,
     CreateCustomMetadataRequestRequestTypeDef,
     CreateFolderRequestRequestTypeDef,
@@ -421,67 +420,68 @@
     DeleteDocumentRequestRequestTypeDef,
     DeleteDocumentVersionRequestRequestTypeDef,
     DeleteFolderContentsRequestRequestTypeDef,
     DeleteFolderRequestRequestTypeDef,
     DeleteLabelsRequestRequestTypeDef,
     DeleteNotificationSubscriptionRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
     DescribeActivitiesRequestRequestTypeDef,
+    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
     DescribeCommentsRequestRequestTypeDef,
+    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeDocumentVersionsRequestRequestTypeDef,
     DocumentVersionMetadataTypeDef,
+    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeFolderContentsRequestRequestTypeDef,
+    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeGroupsRequestRequestTypeDef,
     GroupMetadataTypeDef,
+    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestRequestTypeDef,
+    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
     DescribeResourcePermissionsRequestRequestTypeDef,
+    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
     DescribeRootFoldersRequestRequestTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     LongRangeTypeTypeDef,
     SearchPrincipalTypeTypeDef,
     GetCurrentUserRequestRequestTypeDef,
     GetDocumentPathRequestRequestTypeDef,
     GetDocumentRequestRequestTypeDef,
     GetDocumentVersionRequestRequestTypeDef,
     GetFolderPathRequestRequestTypeDef,
     GetFolderRequestRequestTypeDef,
     GetResourcesRequestRequestTypeDef,
     InitiateDocumentVersionUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
+    PaginatorConfigTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
+    ResponseMetadataTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     UpdateDocumentVersionRequestRequestTypeDef,
     UpdateFolderRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ResourceMetadataTypeDef,
     AddResourcePermissionsRequestRequestTypeDef,
     AddResourcePermissionsResponseTypeDef,
     CreateFolderResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserStorageMetadataTypeDef,
-    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
-    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeDocumentVersionsResponseTypeDef,
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
     FiltersTypeDef,
     PrincipalTypeDef,
@@ -519,42 +519,42 @@
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

### Comparing `mypy-boto3-workdocs-1.26.95/README.md` & `mypy-boto3-workdocs-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-workdocs"></a>
 
 # mypy-boto3-workdocs
 
 [![PyPI - mypy-boto3-workdocs](https://img.shields.io/pypi/v/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workdocs?color=blue)](https://pypistats.org/packages/mypy-boto3-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkDocs 1.26.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[boto3.WorkDocs 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workdocs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,15 +365,14 @@
 `mypy_boto3_workdocs.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workdocs.type_defs import (
     AbortDocumentVersionUploadRequestRequestTypeDef,
     ActivateUserRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UserMetadataTypeDef,
     NotificationOptionsTypeDef,
     SharePrincipalTypeDef,
     ShareResultTypeDef,
     CreateCommentRequestRequestTypeDef,
     CreateCustomMetadataRequestRequestTypeDef,
     CreateFolderRequestRequestTypeDef,
@@ -389,67 +388,68 @@
     DeleteDocumentRequestRequestTypeDef,
     DeleteDocumentVersionRequestRequestTypeDef,
     DeleteFolderContentsRequestRequestTypeDef,
     DeleteFolderRequestRequestTypeDef,
     DeleteLabelsRequestRequestTypeDef,
     DeleteNotificationSubscriptionRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
     DescribeActivitiesRequestRequestTypeDef,
+    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
     DescribeCommentsRequestRequestTypeDef,
+    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeDocumentVersionsRequestRequestTypeDef,
     DocumentVersionMetadataTypeDef,
+    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeFolderContentsRequestRequestTypeDef,
+    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeGroupsRequestRequestTypeDef,
     GroupMetadataTypeDef,
+    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestRequestTypeDef,
+    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
     DescribeResourcePermissionsRequestRequestTypeDef,
+    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
     DescribeRootFoldersRequestRequestTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     LongRangeTypeTypeDef,
     SearchPrincipalTypeTypeDef,
     GetCurrentUserRequestRequestTypeDef,
     GetDocumentPathRequestRequestTypeDef,
     GetDocumentRequestRequestTypeDef,
     GetDocumentVersionRequestRequestTypeDef,
     GetFolderPathRequestRequestTypeDef,
     GetFolderRequestRequestTypeDef,
     GetResourcesRequestRequestTypeDef,
     InitiateDocumentVersionUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
+    PaginatorConfigTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
+    ResponseMetadataTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     UpdateDocumentVersionRequestRequestTypeDef,
     UpdateFolderRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ResourceMetadataTypeDef,
     AddResourcePermissionsRequestRequestTypeDef,
     AddResourcePermissionsResponseTypeDef,
     CreateFolderResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserStorageMetadataTypeDef,
-    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
-    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeDocumentVersionsResponseTypeDef,
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
     FiltersTypeDef,
     PrincipalTypeDef,
@@ -487,42 +487,42 @@
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

### Comparing `mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/__init__.py` & `mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/__init__.pyi` & `mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/client.py` & `mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/client.pyi` & `mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/literals.py` & `mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,15 @@
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
@@ -259,14 +260,15 @@
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
@@ -364,14 +366,15 @@
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
@@ -407,14 +410,15 @@
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
@@ -433,16 +437,19 @@
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
@@ -526,15 +533,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
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

### Comparing `mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/literals.pyi` & `mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,15 @@
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
@@ -257,14 +258,15 @@
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
@@ -362,14 +364,15 @@
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
@@ -405,14 +408,15 @@
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
@@ -431,16 +435,19 @@
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
@@ -524,15 +531,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
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

### Comparing `mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/paginator.py` & `mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeactivitiespaginator)
         """
 
 
@@ -130,15 +130,15 @@
 
     def paginate(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeCommentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeComments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describecommentspaginator)
         """
 
 
@@ -151,15 +151,15 @@
     def paginate(
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Include: str = ...,
         Fields: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDocumentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeDocumentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describedocumentversionspaginator)
         """
 
 
@@ -174,15 +174,15 @@
         *,
         FolderId: str,
         AuthenticationToken: str = ...,
         Sort: ResourceSortTypeType = ...,
         Order: OrderTypeType = ...,
         Type: FolderContentTypeType = ...,
         Include: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeFolderContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeFolderContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describefoldercontentspaginator)
         """
 
 
@@ -194,30 +194,30 @@
 
     def paginate(
         self,
         *,
         SearchQuery: str,
         AuthenticationToken: str = ...,
         OrganizationId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describegroupspaginator)
         """
 
 
 class DescribeNotificationSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describenotificationsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeNotificationSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describenotificationsubscriptionspaginator)
         """
 
 
@@ -229,30 +229,30 @@
 
     def paginate(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         PrincipalId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeResourcePermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeResourcePermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeresourcepermissionspaginator)
         """
 
 
 class DescribeRootFoldersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describerootfolderspaginator)
     """
 
     def paginate(
-        self, *, AuthenticationToken: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AuthenticationToken: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRootFoldersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describerootfolderspaginator)
         """
 
 
@@ -269,15 +269,15 @@
         OrganizationId: str = ...,
         UserIds: str = ...,
         Query: str = ...,
         Include: UserFilterTypeType = ...,
         Order: OrderTypeType = ...,
         Sort: UserSortTypeType = ...,
         Fields: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeuserspaginator)
         """
 
 
@@ -293,13 +293,13 @@
         AuthenticationToken: str = ...,
         QueryText: str = ...,
         QueryScopes: Sequence[SearchQueryScopeTypeType] = ...,
         OrganizationId: str = ...,
         AdditionalResponseFields: Sequence[Literal["WEBURL"]] = ...,
         Filters: FiltersTypeDef = ...,
         OrderBy: Sequence[SearchSortResultTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.SearchResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#searchresourcespaginator)
         """
```

### Comparing `mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/paginator.pyi` & `mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/paginator.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeactivitiespaginator)
         """
 
 class DescribeCommentsPaginator(Paginator):
@@ -125,15 +125,15 @@
 
     def paginate(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeCommentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeComments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describecommentspaginator)
         """
 
 class DescribeDocumentVersionsPaginator(Paginator):
@@ -145,15 +145,15 @@
     def paginate(
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Include: str = ...,
         Fields: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDocumentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeDocumentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describedocumentversionspaginator)
         """
 
 class DescribeFolderContentsPaginator(Paginator):
@@ -167,15 +167,15 @@
         *,
         FolderId: str,
         AuthenticationToken: str = ...,
         Sort: ResourceSortTypeType = ...,
         Order: OrderTypeType = ...,
         Type: FolderContentTypeType = ...,
         Include: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeFolderContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeFolderContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describefoldercontentspaginator)
         """
 
 class DescribeGroupsPaginator(Paginator):
@@ -186,29 +186,29 @@
 
     def paginate(
         self,
         *,
         SearchQuery: str,
         AuthenticationToken: str = ...,
         OrganizationId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describegroupspaginator)
         """
 
 class DescribeNotificationSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describenotificationsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeNotificationSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describenotificationsubscriptionspaginator)
         """
 
 class DescribeResourcePermissionsPaginator(Paginator):
@@ -219,29 +219,29 @@
 
     def paginate(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         PrincipalId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeResourcePermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeResourcePermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeresourcepermissionspaginator)
         """
 
 class DescribeRootFoldersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describerootfolderspaginator)
     """
 
     def paginate(
-        self, *, AuthenticationToken: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AuthenticationToken: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRootFoldersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describerootfolderspaginator)
         """
 
 class DescribeUsersPaginator(Paginator):
@@ -257,15 +257,15 @@
         OrganizationId: str = ...,
         UserIds: str = ...,
         Query: str = ...,
         Include: UserFilterTypeType = ...,
         Order: OrderTypeType = ...,
         Sort: UserSortTypeType = ...,
         Fields: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeuserspaginator)
         """
 
 class SearchResourcesPaginator(Paginator):
@@ -280,13 +280,13 @@
         AuthenticationToken: str = ...,
         QueryText: str = ...,
         QueryScopes: Sequence[SearchQueryScopeTypeType] = ...,
         OrganizationId: str = ...,
         AdditionalResponseFields: Sequence[Literal["WEBURL"]] = ...,
         Filters: FiltersTypeDef = ...,
         OrderBy: Sequence[SearchSortResultTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.SearchResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#searchresourcespaginator)
         """
```

### Comparing `mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/type_defs.py` & `mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AbortDocumentVersionUploadRequestRequestTypeDef",
     "ActivateUserRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UserMetadataTypeDef",
     "NotificationOptionsTypeDef",
     "SharePrincipalTypeDef",
     "ShareResultTypeDef",
     "CreateCommentRequestRequestTypeDef",
     "CreateCustomMetadataRequestRequestTypeDef",
     "CreateFolderRequestRequestTypeDef",
@@ -83,67 +82,68 @@
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteDocumentVersionRequestRequestTypeDef",
     "DeleteFolderContentsRequestRequestTypeDef",
     "DeleteFolderRequestRequestTypeDef",
     "DeleteLabelsRequestRequestTypeDef",
     "DeleteNotificationSubscriptionRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     "DescribeActivitiesRequestRequestTypeDef",
+    "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
     "DescribeCommentsRequestRequestTypeDef",
+    "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
     "DescribeDocumentVersionsRequestRequestTypeDef",
     "DocumentVersionMetadataTypeDef",
+    "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
     "DescribeFolderContentsRequestRequestTypeDef",
+    "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
     "DescribeGroupsRequestRequestTypeDef",
     "GroupMetadataTypeDef",
+    "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
     "DescribeNotificationSubscriptionsRequestRequestTypeDef",
+    "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
     "DescribeResourcePermissionsRequestRequestTypeDef",
+    "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
     "DescribeRootFoldersRequestRequestTypeDef",
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "LongRangeTypeTypeDef",
     "SearchPrincipalTypeTypeDef",
     "GetCurrentUserRequestRequestTypeDef",
     "GetDocumentPathRequestRequestTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "GetDocumentVersionRequestRequestTypeDef",
     "GetFolderPathRequestRequestTypeDef",
     "GetFolderRequestRequestTypeDef",
     "GetResourcesRequestRequestTypeDef",
     "InitiateDocumentVersionUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
+    "PaginatorConfigTypeDef",
     "PermissionInfoTypeDef",
     "RemoveAllResourcePermissionsRequestRequestTypeDef",
     "RemoveResourcePermissionRequestRequestTypeDef",
     "ResourcePathComponentTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreDocumentVersionsRequestRequestTypeDef",
     "SearchSortResultTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
     "UpdateDocumentVersionRequestRequestTypeDef",
     "UpdateFolderRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ResourceMetadataTypeDef",
     "AddResourcePermissionsRequestRequestTypeDef",
     "AddResourcePermissionsResponseTypeDef",
     "CreateFolderResponseTypeDef",
     "DescribeRootFoldersResponseTypeDef",
     "GetFolderResponseTypeDef",
     "CreateNotificationSubscriptionResponseTypeDef",
     "DescribeNotificationSubscriptionsResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UserStorageMetadataTypeDef",
-    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
-    "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
-    "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeDocumentVersionsResponseTypeDef",
     "DocumentMetadataTypeDef",
     "GetDocumentVersionResponseTypeDef",
     "DescribeGroupsResponseTypeDef",
     "ParticipantsTypeDef",
     "FiltersTypeDef",
     "PrincipalTypeDef",
@@ -213,25 +213,14 @@
 
 class ActivateUserRequestRequestTypeDef(
     _RequiredActivateUserRequestRequestTypeDef, _OptionalActivateUserRequestRequestTypeDef
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
 UserMetadataTypeDef = TypedDict(
     "UserMetadataTypeDef",
     {
         "Id": str,
         "Username": str,
         "GivenName": str,
         "Surname": str,
@@ -627,20 +616,26 @@
 
 class DeleteUserRequestRequestTypeDef(
     _RequiredDeleteUserRequestRequestTypeDef, _OptionalDeleteUserRequestRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
+    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "AuthenticationToken": str,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "OrganizationId": str,
+        "ActivityTypes": str,
+        "ResourceId": str,
+        "UserId": str,
+        "IncludeIndirectActivities": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeActivitiesRequestRequestTypeDef = TypedDict(
     "DescribeActivitiesRequestRequestTypeDef",
     {
@@ -654,14 +649,38 @@
         "IncludeIndirectActivities": bool,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    {
+        "DocumentId": str,
+        "VersionId": str,
+    },
+)
+_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeCommentsRequestDescribeCommentsPaginateTypeDef(
+    _RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    _OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeCommentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommentsRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
     },
 )
@@ -678,14 +697,39 @@
 
 class DescribeCommentsRequestRequestTypeDef(
     _RequiredDescribeCommentsRequestRequestTypeDef, _OptionalDescribeCommentsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    {
+        "DocumentId": str,
+    },
+)
+_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Include": str,
+        "Fields": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef(
+    _RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+    _OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentVersionsRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalDescribeDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -724,14 +768,41 @@
         "CreatorId": str,
         "Thumbnail": Dict[DocumentThumbnailTypeType, str],
         "Source": Dict[DocumentSourceTypeType, str],
     },
     total=False,
 )
 
+_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    {
+        "FolderId": str,
+    },
+)
+_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Sort": ResourceSortTypeType,
+        "Order": OrderTypeType,
+        "Type": FolderContentTypeType,
+        "Include": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef(
+    _RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+    _OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeFolderContentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFolderContentsRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalDescribeFolderContentsRequestRequestTypeDef = TypedDict(
@@ -752,14 +823,38 @@
 class DescribeFolderContentsRequestRequestTypeDef(
     _RequiredDescribeFolderContentsRequestRequestTypeDef,
     _OptionalDescribeFolderContentsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    {
+        "SearchQuery": str,
+    },
+)
+_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "OrganizationId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeGroupsRequestDescribeGroupsPaginateTypeDef(
+    _RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+    _OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeGroupsRequestRequestTypeDef",
     {
         "SearchQuery": str,
     },
 )
 _OptionalDescribeGroupsRequestRequestTypeDef = TypedDict(
@@ -785,14 +880,36 @@
     {
         "Id": str,
         "Name": str,
     },
     total=False,
 )
 
+_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef(
+    _RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+    _OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalDescribeNotificationSubscriptionsRequestRequestTypeDef = TypedDict(
@@ -808,14 +925,38 @@
 class DescribeNotificationSubscriptionsRequestRequestTypeDef(
     _RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef,
     _OptionalDescribeNotificationSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "PrincipalId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef(
+    _RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+    _OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeResourcePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourcePermissionsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalDescribeResourcePermissionsRequestRequestTypeDef = TypedDict(
@@ -833,14 +974,36 @@
 class DescribeResourcePermissionsRequestRequestTypeDef(
     _RequiredDescribeResourcePermissionsRequestRequestTypeDef,
     _OptionalDescribeResourcePermissionsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+    },
+)
+_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef(
+    _RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+    _OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeRootFoldersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRootFoldersRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
 )
 _OptionalDescribeRootFoldersRequestRequestTypeDef = TypedDict(
@@ -856,14 +1019,30 @@
 class DescribeRootFoldersRequestRequestTypeDef(
     _RequiredDescribeRootFoldersRequestRequestTypeDef,
     _OptionalDescribeRootFoldersRequestRequestTypeDef,
 ):
     pass
 
 
+DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "OrganizationId": str,
+        "UserIds": str,
+        "Query": str,
+        "Include": UserFilterTypeType,
+        "Order": OrderTypeType,
+        "Sort": UserSortTypeType,
+        "Fields": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeUsersRequestRequestTypeDef = TypedDict(
     "DescribeUsersRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
         "OrganizationId": str,
         "UserIds": str,
         "Query": str,
@@ -873,14 +1052,21 @@
         "Marker": str,
         "Limit": int,
         "Fields": str,
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
 LongRangeTypeTypeDef = TypedDict(
     "LongRangeTypeTypeDef",
     {
         "StartValue": int,
         "EndValue": int,
     },
     total=False,
@@ -1063,14 +1249,24 @@
     {
         "UploadUrl": str,
         "SignedHeaders": Dict[str, str],
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
 PermissionInfoTypeDef = TypedDict(
     "PermissionInfoTypeDef",
     {
         "Role": RoleTypeType,
         "Type": RolePermissionTypeType,
     },
     total=False,
@@ -1127,14 +1323,25 @@
     {
         "Id": str,
         "Name": str,
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
 _RequiredRestoreDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreDocumentVersionsRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalRestoreDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -1230,21 +1437,14 @@
 
 class UpdateFolderRequestRequestTypeDef(
     _RequiredUpdateFolderRequestRequestTypeDef, _OptionalUpdateFolderRequestRequestTypeDef
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ResourceMetadataTypeDef = TypedDict(
     "ResourceMetadataTypeDef",
     {
         "Type": ResourceTypeType,
         "Name": str,
         "OriginalName": str,
         "Id": str,
@@ -1279,58 +1479,58 @@
     pass
 
 
 AddResourcePermissionsResponseTypeDef = TypedDict(
     "AddResourcePermissionsResponseTypeDef",
     {
         "ShareResults": List[ShareResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFolderResponseTypeDef = TypedDict(
     "CreateFolderResponseTypeDef",
     {
         "Metadata": FolderMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRootFoldersResponseTypeDef = TypedDict(
     "DescribeRootFoldersResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFolderResponseTypeDef = TypedDict(
     "GetFolderResponseTypeDef",
     {
         "Metadata": FolderMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateNotificationSubscriptionResponseTypeDef = TypedDict(
     "CreateNotificationSubscriptionResponseTypeDef",
     {
         "Subscription": SubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeNotificationSubscriptionsResponseTypeDef = TypedDict(
     "DescribeNotificationSubscriptionsResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "Username": str,
@@ -1391,220 +1591,20 @@
     {
         "StorageUtilizedInBytes": int,
         "StorageRule": StorageRuleTypeTypeDef,
     },
     total=False,
 )
 
-DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
-    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "OrganizationId": str,
-        "ActivityTypes": str,
-        "ResourceId": str,
-        "UserId": str,
-        "IncludeIndirectActivities": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
-    {
-        "DocumentId": str,
-        "VersionId": str,
-    },
-)
-_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeCommentsRequestDescribeCommentsPaginateTypeDef(
-    _RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-    _OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    {
-        "DocumentId": str,
-    },
-)
-_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Include": str,
-        "Fields": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef(
-    _RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-    _OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    {
-        "FolderId": str,
-    },
-)
-_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Sort": ResourceSortTypeType,
-        "Order": OrderTypeType,
-        "Type": FolderContentTypeType,
-        "Include": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef(
-    _RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-    _OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    {
-        "SearchQuery": str,
-    },
-)
-_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "OrganizationId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeGroupsRequestDescribeGroupsPaginateTypeDef(
-    _RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-    _OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef(
-    _RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-    _OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "PrincipalId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef(
-    _RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-    _OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-    },
-)
-_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef(
-    _RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-    _OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-):
-    pass
-
-
-DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "OrganizationId": str,
-        "UserIds": str,
-        "Query": str,
-        "Include": UserFilterTypeType,
-        "Order": OrderTypeType,
-        "Sort": UserSortTypeType,
-        "Fields": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeDocumentVersionsResponseTypeDef = TypedDict(
     "DescribeDocumentVersionsResponseTypeDef",
     {
         "DocumentVersions": List[DocumentVersionMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DocumentMetadataTypeDef = TypedDict(
     "DocumentMetadataTypeDef",
     {
         "Id": str,
@@ -1620,24 +1620,24 @@
 )
 
 GetDocumentVersionResponseTypeDef = TypedDict(
     "GetDocumentVersionResponseTypeDef",
     {
         "Metadata": DocumentVersionMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGroupsResponseTypeDef = TypedDict(
     "DescribeGroupsResponseTypeDef",
     {
         "Groups": List[GroupMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ParticipantsTypeDef = TypedDict(
     "ParticipantsTypeDef",
     {
         "Users": List[UserMetadataTypeDef],
@@ -1705,43 +1705,43 @@
 
 DescribeFolderContentsResponseTypeDef = TypedDict(
     "DescribeFolderContentsResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDocumentResponseTypeDef = TypedDict(
     "GetDocumentResponseTypeDef",
     {
         "Metadata": DocumentMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourcesResponseTypeDef = TypedDict(
     "GetResourcesResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InitiateDocumentVersionUploadResponseTypeDef = TypedDict(
     "InitiateDocumentVersionUploadResponseTypeDef",
     {
         "Metadata": DocumentMetadataTypeDef,
         "UploadMetadata": UploadMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchResourcesRequestRequestTypeDef = TypedDict(
     "SearchResourcesRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
@@ -1763,49 +1763,49 @@
         "AuthenticationToken": str,
         "QueryText": str,
         "QueryScopes": Sequence[SearchQueryScopeTypeType],
         "OrganizationId": str,
         "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
         "Filters": FiltersTypeDef,
         "OrderBy": Sequence[SearchSortResultTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeResourcePermissionsResponseTypeDef = TypedDict(
     "DescribeResourcePermissionsResponseTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDocumentPathResponseTypeDef = TypedDict(
     "GetDocumentPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFolderPathResponseTypeDef = TypedDict(
     "GetFolderPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActivateUserResponseTypeDef = TypedDict(
     "ActivateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CommentMetadataTypeDef = TypedDict(
     "CommentMetadataTypeDef",
     {
         "CommentId": str,
@@ -1844,41 +1844,41 @@
     pass
 
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUsersResponseTypeDef = TypedDict(
     "DescribeUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "TotalNumberOfUsers": int,
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCurrentUserResponseTypeDef = TypedDict(
     "GetCurrentUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActivityTypeDef = TypedDict(
     "ActivityTypeDef",
     {
         "Type": ActivityTypeType,
@@ -1907,37 +1907,37 @@
     total=False,
 )
 
 CreateCommentResponseTypeDef = TypedDict(
     "CreateCommentResponseTypeDef",
     {
         "Comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCommentsResponseTypeDef = TypedDict(
     "DescribeCommentsResponseTypeDef",
     {
         "Comments": List[CommentTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeActivitiesResponseTypeDef = TypedDict(
     "DescribeActivitiesResponseTypeDef",
     {
         "UserActivities": List[ActivityTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchResourcesResponseTypeDef = TypedDict(
     "SearchResourcesResponseTypeDef",
     {
         "Items": List[ResponseItemTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs/type_defs.pyi` & `mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbortDocumentVersionUploadRequestRequestTypeDef",
     "ActivateUserRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UserMetadataTypeDef",
     "NotificationOptionsTypeDef",
     "SharePrincipalTypeDef",
     "ShareResultTypeDef",
     "CreateCommentRequestRequestTypeDef",
     "CreateCustomMetadataRequestRequestTypeDef",
     "CreateFolderRequestRequestTypeDef",
@@ -82,67 +81,68 @@
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteDocumentVersionRequestRequestTypeDef",
     "DeleteFolderContentsRequestRequestTypeDef",
     "DeleteFolderRequestRequestTypeDef",
     "DeleteLabelsRequestRequestTypeDef",
     "DeleteNotificationSubscriptionRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     "DescribeActivitiesRequestRequestTypeDef",
+    "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
     "DescribeCommentsRequestRequestTypeDef",
+    "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
     "DescribeDocumentVersionsRequestRequestTypeDef",
     "DocumentVersionMetadataTypeDef",
+    "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
     "DescribeFolderContentsRequestRequestTypeDef",
+    "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
     "DescribeGroupsRequestRequestTypeDef",
     "GroupMetadataTypeDef",
+    "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
     "DescribeNotificationSubscriptionsRequestRequestTypeDef",
+    "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
     "DescribeResourcePermissionsRequestRequestTypeDef",
+    "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
     "DescribeRootFoldersRequestRequestTypeDef",
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "LongRangeTypeTypeDef",
     "SearchPrincipalTypeTypeDef",
     "GetCurrentUserRequestRequestTypeDef",
     "GetDocumentPathRequestRequestTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "GetDocumentVersionRequestRequestTypeDef",
     "GetFolderPathRequestRequestTypeDef",
     "GetFolderRequestRequestTypeDef",
     "GetResourcesRequestRequestTypeDef",
     "InitiateDocumentVersionUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
+    "PaginatorConfigTypeDef",
     "PermissionInfoTypeDef",
     "RemoveAllResourcePermissionsRequestRequestTypeDef",
     "RemoveResourcePermissionRequestRequestTypeDef",
     "ResourcePathComponentTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreDocumentVersionsRequestRequestTypeDef",
     "SearchSortResultTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
     "UpdateDocumentVersionRequestRequestTypeDef",
     "UpdateFolderRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ResourceMetadataTypeDef",
     "AddResourcePermissionsRequestRequestTypeDef",
     "AddResourcePermissionsResponseTypeDef",
     "CreateFolderResponseTypeDef",
     "DescribeRootFoldersResponseTypeDef",
     "GetFolderResponseTypeDef",
     "CreateNotificationSubscriptionResponseTypeDef",
     "DescribeNotificationSubscriptionsResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UserStorageMetadataTypeDef",
-    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
-    "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
-    "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeDocumentVersionsResponseTypeDef",
     "DocumentMetadataTypeDef",
     "GetDocumentVersionResponseTypeDef",
     "DescribeGroupsResponseTypeDef",
     "ParticipantsTypeDef",
     "FiltersTypeDef",
     "PrincipalTypeDef",
@@ -208,25 +208,14 @@
 )
 
 class ActivateUserRequestRequestTypeDef(
     _RequiredActivateUserRequestRequestTypeDef, _OptionalActivateUserRequestRequestTypeDef
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
 UserMetadataTypeDef = TypedDict(
     "UserMetadataTypeDef",
     {
         "Id": str,
         "Username": str,
         "GivenName": str,
         "Surname": str,
@@ -596,20 +585,26 @@
 )
 
 class DeleteUserRequestRequestTypeDef(
     _RequiredDeleteUserRequestRequestTypeDef, _OptionalDeleteUserRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
+    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "AuthenticationToken": str,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "OrganizationId": str,
+        "ActivityTypes": str,
+        "ResourceId": str,
+        "UserId": str,
+        "IncludeIndirectActivities": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeActivitiesRequestRequestTypeDef = TypedDict(
     "DescribeActivitiesRequestRequestTypeDef",
     {
@@ -623,14 +618,36 @@
         "IncludeIndirectActivities": bool,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    {
+        "DocumentId": str,
+        "VersionId": str,
+    },
+)
+_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeCommentsRequestDescribeCommentsPaginateTypeDef(
+    _RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    _OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeCommentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommentsRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
     },
 )
@@ -645,14 +662,37 @@
 )
 
 class DescribeCommentsRequestRequestTypeDef(
     _RequiredDescribeCommentsRequestRequestTypeDef, _OptionalDescribeCommentsRequestRequestTypeDef
 ):
     pass
 
+_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    {
+        "DocumentId": str,
+    },
+)
+_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Include": str,
+        "Fields": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef(
+    _RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+    _OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentVersionsRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalDescribeDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -689,14 +729,39 @@
         "CreatorId": str,
         "Thumbnail": Dict[DocumentThumbnailTypeType, str],
         "Source": Dict[DocumentSourceTypeType, str],
     },
     total=False,
 )
 
+_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    {
+        "FolderId": str,
+    },
+)
+_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Sort": ResourceSortTypeType,
+        "Order": OrderTypeType,
+        "Type": FolderContentTypeType,
+        "Include": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef(
+    _RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+    _OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeFolderContentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFolderContentsRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalDescribeFolderContentsRequestRequestTypeDef = TypedDict(
@@ -715,14 +780,36 @@
 
 class DescribeFolderContentsRequestRequestTypeDef(
     _RequiredDescribeFolderContentsRequestRequestTypeDef,
     _OptionalDescribeFolderContentsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    {
+        "SearchQuery": str,
+    },
+)
+_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "OrganizationId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeGroupsRequestDescribeGroupsPaginateTypeDef(
+    _RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+    _OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeGroupsRequestRequestTypeDef",
     {
         "SearchQuery": str,
     },
 )
 _OptionalDescribeGroupsRequestRequestTypeDef = TypedDict(
@@ -746,14 +833,34 @@
     {
         "Id": str,
         "Name": str,
     },
     total=False,
 )
 
+_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef(
+    _RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+    _OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalDescribeNotificationSubscriptionsRequestRequestTypeDef = TypedDict(
@@ -767,14 +874,36 @@
 
 class DescribeNotificationSubscriptionsRequestRequestTypeDef(
     _RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef,
     _OptionalDescribeNotificationSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "PrincipalId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef(
+    _RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+    _OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeResourcePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourcePermissionsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalDescribeResourcePermissionsRequestRequestTypeDef = TypedDict(
@@ -790,14 +919,34 @@
 
 class DescribeResourcePermissionsRequestRequestTypeDef(
     _RequiredDescribeResourcePermissionsRequestRequestTypeDef,
     _OptionalDescribeResourcePermissionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+    },
+)
+_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef(
+    _RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+    _OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeRootFoldersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRootFoldersRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
 )
 _OptionalDescribeRootFoldersRequestRequestTypeDef = TypedDict(
@@ -811,14 +960,30 @@
 
 class DescribeRootFoldersRequestRequestTypeDef(
     _RequiredDescribeRootFoldersRequestRequestTypeDef,
     _OptionalDescribeRootFoldersRequestRequestTypeDef,
 ):
     pass
 
+DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "OrganizationId": str,
+        "UserIds": str,
+        "Query": str,
+        "Include": UserFilterTypeType,
+        "Order": OrderTypeType,
+        "Sort": UserSortTypeType,
+        "Fields": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeUsersRequestRequestTypeDef = TypedDict(
     "DescribeUsersRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
         "OrganizationId": str,
         "UserIds": str,
         "Query": str,
@@ -828,14 +993,21 @@
         "Marker": str,
         "Limit": int,
         "Fields": str,
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
 LongRangeTypeTypeDef = TypedDict(
     "LongRangeTypeTypeDef",
     {
         "StartValue": int,
         "EndValue": int,
     },
     total=False,
@@ -1006,14 +1178,24 @@
     {
         "UploadUrl": str,
         "SignedHeaders": Dict[str, str],
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
 PermissionInfoTypeDef = TypedDict(
     "PermissionInfoTypeDef",
     {
         "Role": RoleTypeType,
         "Type": RolePermissionTypeType,
     },
     total=False,
@@ -1066,14 +1248,25 @@
     {
         "Id": str,
         "Name": str,
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
 _RequiredRestoreDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreDocumentVersionsRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalRestoreDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -1161,21 +1354,14 @@
 )
 
 class UpdateFolderRequestRequestTypeDef(
     _RequiredUpdateFolderRequestRequestTypeDef, _OptionalUpdateFolderRequestRequestTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ResourceMetadataTypeDef = TypedDict(
     "ResourceMetadataTypeDef",
     {
         "Type": ResourceTypeType,
         "Name": str,
         "OriginalName": str,
         "Id": str,
@@ -1208,58 +1394,58 @@
 ):
     pass
 
 AddResourcePermissionsResponseTypeDef = TypedDict(
     "AddResourcePermissionsResponseTypeDef",
     {
         "ShareResults": List[ShareResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFolderResponseTypeDef = TypedDict(
     "CreateFolderResponseTypeDef",
     {
         "Metadata": FolderMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRootFoldersResponseTypeDef = TypedDict(
     "DescribeRootFoldersResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFolderResponseTypeDef = TypedDict(
     "GetFolderResponseTypeDef",
     {
         "Metadata": FolderMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateNotificationSubscriptionResponseTypeDef = TypedDict(
     "CreateNotificationSubscriptionResponseTypeDef",
     {
         "Subscription": SubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeNotificationSubscriptionsResponseTypeDef = TypedDict(
     "DescribeNotificationSubscriptionsResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "Username": str,
@@ -1316,206 +1502,20 @@
     {
         "StorageUtilizedInBytes": int,
         "StorageRule": StorageRuleTypeTypeDef,
     },
     total=False,
 )
 
-DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
-    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "OrganizationId": str,
-        "ActivityTypes": str,
-        "ResourceId": str,
-        "UserId": str,
-        "IncludeIndirectActivities": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
-    {
-        "DocumentId": str,
-        "VersionId": str,
-    },
-)
-_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeCommentsRequestDescribeCommentsPaginateTypeDef(
-    _RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-    _OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    {
-        "DocumentId": str,
-    },
-)
-_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Include": str,
-        "Fields": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef(
-    _RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-    _OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    {
-        "FolderId": str,
-    },
-)
-_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Sort": ResourceSortTypeType,
-        "Order": OrderTypeType,
-        "Type": FolderContentTypeType,
-        "Include": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef(
-    _RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-    _OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    {
-        "SearchQuery": str,
-    },
-)
-_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "OrganizationId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeGroupsRequestDescribeGroupsPaginateTypeDef(
-    _RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-    _OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef(
-    _RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-    _OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "PrincipalId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef(
-    _RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-    _OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-    },
-)
-_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef(
-    _RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-    _OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-):
-    pass
-
-DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "OrganizationId": str,
-        "UserIds": str,
-        "Query": str,
-        "Include": UserFilterTypeType,
-        "Order": OrderTypeType,
-        "Sort": UserSortTypeType,
-        "Fields": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeDocumentVersionsResponseTypeDef = TypedDict(
     "DescribeDocumentVersionsResponseTypeDef",
     {
         "DocumentVersions": List[DocumentVersionMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DocumentMetadataTypeDef = TypedDict(
     "DocumentMetadataTypeDef",
     {
         "Id": str,
@@ -1531,24 +1531,24 @@
 )
 
 GetDocumentVersionResponseTypeDef = TypedDict(
     "GetDocumentVersionResponseTypeDef",
     {
         "Metadata": DocumentVersionMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGroupsResponseTypeDef = TypedDict(
     "DescribeGroupsResponseTypeDef",
     {
         "Groups": List[GroupMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ParticipantsTypeDef = TypedDict(
     "ParticipantsTypeDef",
     {
         "Users": List[UserMetadataTypeDef],
@@ -1616,43 +1616,43 @@
 
 DescribeFolderContentsResponseTypeDef = TypedDict(
     "DescribeFolderContentsResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDocumentResponseTypeDef = TypedDict(
     "GetDocumentResponseTypeDef",
     {
         "Metadata": DocumentMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourcesResponseTypeDef = TypedDict(
     "GetResourcesResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InitiateDocumentVersionUploadResponseTypeDef = TypedDict(
     "InitiateDocumentVersionUploadResponseTypeDef",
     {
         "Metadata": DocumentMetadataTypeDef,
         "UploadMetadata": UploadMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchResourcesRequestRequestTypeDef = TypedDict(
     "SearchResourcesRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
@@ -1674,49 +1674,49 @@
         "AuthenticationToken": str,
         "QueryText": str,
         "QueryScopes": Sequence[SearchQueryScopeTypeType],
         "OrganizationId": str,
         "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
         "Filters": FiltersTypeDef,
         "OrderBy": Sequence[SearchSortResultTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeResourcePermissionsResponseTypeDef = TypedDict(
     "DescribeResourcePermissionsResponseTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDocumentPathResponseTypeDef = TypedDict(
     "GetDocumentPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFolderPathResponseTypeDef = TypedDict(
     "GetFolderPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActivateUserResponseTypeDef = TypedDict(
     "ActivateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CommentMetadataTypeDef = TypedDict(
     "CommentMetadataTypeDef",
     {
         "CommentId": str,
@@ -1753,41 +1753,41 @@
 class CommentTypeDef(_RequiredCommentTypeDef, _OptionalCommentTypeDef):
     pass
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUsersResponseTypeDef = TypedDict(
     "DescribeUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "TotalNumberOfUsers": int,
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCurrentUserResponseTypeDef = TypedDict(
     "GetCurrentUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActivityTypeDef = TypedDict(
     "ActivityTypeDef",
     {
         "Type": ActivityTypeType,
@@ -1816,37 +1816,37 @@
     total=False,
 )
 
 CreateCommentResponseTypeDef = TypedDict(
     "CreateCommentResponseTypeDef",
     {
         "Comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCommentsResponseTypeDef = TypedDict(
     "DescribeCommentsResponseTypeDef",
     {
         "Comments": List[CommentTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeActivitiesResponseTypeDef = TypedDict(
     "DescribeActivitiesResponseTypeDef",
     {
         "UserActivities": List[ActivityTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchResourcesResponseTypeDef = TypedDict(
     "SearchResourcesResponseTypeDef",
     {
         "Items": List[ResponseItemTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs.egg-info/PKG-INFO` & `mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workdocs
-Version: 1.26.95
-Summary: Type annotations for boto3.WorkDocs 1.26.95 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.WorkDocs 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-workdocs"></a>
 
 # mypy-boto3-workdocs
 
 [![PyPI - mypy-boto3-workdocs](https://img.shields.io/pypi/v/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workdocs?color=blue)](https://pypistats.org/packages/mypy-boto3-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkDocs 1.26.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[boto3.WorkDocs 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workdocs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -397,15 +397,14 @@
 `mypy_boto3_workdocs.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workdocs.type_defs import (
     AbortDocumentVersionUploadRequestRequestTypeDef,
     ActivateUserRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UserMetadataTypeDef,
     NotificationOptionsTypeDef,
     SharePrincipalTypeDef,
     ShareResultTypeDef,
     CreateCommentRequestRequestTypeDef,
     CreateCustomMetadataRequestRequestTypeDef,
     CreateFolderRequestRequestTypeDef,
@@ -421,67 +420,68 @@
     DeleteDocumentRequestRequestTypeDef,
     DeleteDocumentVersionRequestRequestTypeDef,
     DeleteFolderContentsRequestRequestTypeDef,
     DeleteFolderRequestRequestTypeDef,
     DeleteLabelsRequestRequestTypeDef,
     DeleteNotificationSubscriptionRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
     DescribeActivitiesRequestRequestTypeDef,
+    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
     DescribeCommentsRequestRequestTypeDef,
+    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeDocumentVersionsRequestRequestTypeDef,
     DocumentVersionMetadataTypeDef,
+    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeFolderContentsRequestRequestTypeDef,
+    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeGroupsRequestRequestTypeDef,
     GroupMetadataTypeDef,
+    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestRequestTypeDef,
+    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
     DescribeResourcePermissionsRequestRequestTypeDef,
+    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
     DescribeRootFoldersRequestRequestTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     LongRangeTypeTypeDef,
     SearchPrincipalTypeTypeDef,
     GetCurrentUserRequestRequestTypeDef,
     GetDocumentPathRequestRequestTypeDef,
     GetDocumentRequestRequestTypeDef,
     GetDocumentVersionRequestRequestTypeDef,
     GetFolderPathRequestRequestTypeDef,
     GetFolderRequestRequestTypeDef,
     GetResourcesRequestRequestTypeDef,
     InitiateDocumentVersionUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
+    PaginatorConfigTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
+    ResponseMetadataTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     UpdateDocumentVersionRequestRequestTypeDef,
     UpdateFolderRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ResourceMetadataTypeDef,
     AddResourcePermissionsRequestRequestTypeDef,
     AddResourcePermissionsResponseTypeDef,
     CreateFolderResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserStorageMetadataTypeDef,
-    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
-    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeDocumentVersionsResponseTypeDef,
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
     FiltersTypeDef,
     PrincipalTypeDef,
@@ -519,42 +519,42 @@
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

### Comparing `mypy-boto3-workdocs-1.26.95/mypy_boto3_workdocs.egg-info/SOURCES.txt` & `mypy-boto3-workdocs-1.27.0/mypy_boto3_workdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.26.95/setup.py` & `mypy-boto3-workdocs-1.27.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-workdocs.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workdocs",
-    version="1.26.95",
+    version="1.27.0",
     packages=["mypy_boto3_workdocs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkDocs 1.26.95 service generated with mypy-boto3-builder"
-        " 7.13.0"
+        "Type annotations for boto3.WorkDocs 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/",
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


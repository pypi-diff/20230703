# Comparing `tmp/mypy-boto3-codestar-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-codestar-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codestar-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:15 2022, max compression
+gzip compressed data, was "mypy-boto3-codestar-1.27.0.tar", last modified: Mon Jul  3 19:50:34 2023, max compression
```

## Comparing `mypy-boto3-codestar-1.26.0.post1.tar` & `mypy-boto3-codestar-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:15.744818 mypy-boto3-codestar-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:59.000000 mypy-boto3-codestar-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14896 2022-11-01 21:43:15.744818 mypy-boto3-codestar-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13451 2022-11-01 21:31:59.000000 mypy-boto3-codestar-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:15.744818 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-11-01 21:31:59.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-11-01 21:31:59.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-01 21:31:59.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15728 2022-11-01 21:31:59.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    15699 2022-11-01 21:31:59.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7625 2022-11-01 21:32:00.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7623 2022-11-01 21:32:00.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4923 2022-11-01 21:32:00.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4917 2022-11-01 21:32:00.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:59.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    17970 2022-11-01 21:32:00.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    17938 2022-11-01 21:32:00.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:59.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:15.744818 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14896 2022-11-01 21:43:15.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-11-01 21:43:15.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:15.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:15.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:15.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-01 21:43:15.000000 mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:15.744818 mypy-boto3-codestar-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2022-11-01 21:31:58.000000 mypy-boto3-codestar-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.047026 mypy-boto3-codestar-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-07-03 19:50:34.043026 mypy-boto3-codestar-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.043026 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15728 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18008 2023-07-03 19:34:29.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17976 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:28.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.043026 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-07-03 19:50:33.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:50:33.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:33.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:33.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:33.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:50:33.000000 mypy-boto3-codestar-1.27.0/mypy_boto3_codestar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:34.047026 mypy-boto3-codestar-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:34:27.000000 mypy-boto3-codestar-1.27.0/setup.py
```

### Comparing `mypy-boto3-codestar-1.26.0.post1/LICENSE` & `mypy-boto3-codestar-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-codestar-1.26.0.post1/PKG-INFO` & `mypy-boto3-codestar-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeStar 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeStar 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/
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
 
 <a id="mypy-boto3-codestar"></a>
 
 # mypy-boto3-codestar
 
 [![PyPI - mypy-boto3-codestar](https://img.shields.io/pypi/v/mypy-boto3-codestar.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codestar?color=blue)](https://pypistats.org/packages/mypy-boto3-codestar)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStar 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
+[boto3.CodeStar 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
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
 [mypy-boto3-codestar docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,58 +330,58 @@
 
 `mypy_boto3_codestar.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar.type_defs import (
     AssociateTeamMemberRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateTeamMemberResultTypeDef,
     CodeCommitCodeDestinationTypeDef,
     GitHubCodeDestinationTypeDef,
     S3LocationTypeDef,
+    CreateProjectResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
+    CreateUserProfileResultTypeDef,
     DeleteProjectRequestRequestTypeDef,
+    DeleteProjectResultTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
+    DeleteUserProfileResultTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ProjectStatusTypeDef,
     DescribeUserProfileRequestRequestTypeDef,
+    DescribeUserProfileResultTypeDef,
     DisassociateTeamMemberRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForProjectRequestRequestTypeDef,
+    ListTagsForProjectResultTypeDef,
+    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
     ListTeamMembersRequestRequestTypeDef,
     TeamMemberTypeDef,
+    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListUserProfilesRequestRequestTypeDef,
     UserProfileSummaryTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagProjectRequestRequestTypeDef,
+    TagProjectResultTypeDef,
     UntagProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     UpdateTeamMemberRequestRequestTypeDef,
-    UpdateUserProfileRequestRequestTypeDef,
-    AssociateTeamMemberResultTypeDef,
-    CreateProjectResultTypeDef,
-    CreateUserProfileResultTypeDef,
-    DeleteProjectResultTypeDef,
-    DeleteUserProfileResultTypeDef,
-    DescribeUserProfileResultTypeDef,
-    ListTagsForProjectResultTypeDef,
-    TagProjectResultTypeDef,
     UpdateTeamMemberResultTypeDef,
+    UpdateUserProfileRequestRequestTypeDef,
     UpdateUserProfileResultTypeDef,
     CodeDestinationTypeDef,
     CodeSourceTypeDef,
     ToolchainSourceTypeDef,
     DescribeProjectResultTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
-    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
-    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListProjectsResultTypeDef,
     ListResourcesResultTypeDef,
     ListTeamMembersResultTypeDef,
     ListUserProfilesResultTypeDef,
     CodeTypeDef,
     ToolchainTypeDef,
     CreateProjectRequestRequestTypeDef,
@@ -394,42 +395,42 @@
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

### Comparing `mypy-boto3-codestar-1.26.0.post1/README.md` & `mypy-boto3-codestar-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codestar"></a>
 
 # mypy-boto3-codestar
 
 [![PyPI - mypy-boto3-codestar](https://img.shields.io/pypi/v/mypy-boto3-codestar.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codestar?color=blue)](https://pypistats.org/packages/mypy-boto3-codestar)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStar 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
+[boto3.CodeStar 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
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
 [mypy-boto3-codestar docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,58 +298,58 @@
 
 `mypy_boto3_codestar.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar.type_defs import (
     AssociateTeamMemberRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateTeamMemberResultTypeDef,
     CodeCommitCodeDestinationTypeDef,
     GitHubCodeDestinationTypeDef,
     S3LocationTypeDef,
+    CreateProjectResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
+    CreateUserProfileResultTypeDef,
     DeleteProjectRequestRequestTypeDef,
+    DeleteProjectResultTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
+    DeleteUserProfileResultTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ProjectStatusTypeDef,
     DescribeUserProfileRequestRequestTypeDef,
+    DescribeUserProfileResultTypeDef,
     DisassociateTeamMemberRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForProjectRequestRequestTypeDef,
+    ListTagsForProjectResultTypeDef,
+    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
     ListTeamMembersRequestRequestTypeDef,
     TeamMemberTypeDef,
+    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListUserProfilesRequestRequestTypeDef,
     UserProfileSummaryTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagProjectRequestRequestTypeDef,
+    TagProjectResultTypeDef,
     UntagProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     UpdateTeamMemberRequestRequestTypeDef,
-    UpdateUserProfileRequestRequestTypeDef,
-    AssociateTeamMemberResultTypeDef,
-    CreateProjectResultTypeDef,
-    CreateUserProfileResultTypeDef,
-    DeleteProjectResultTypeDef,
-    DeleteUserProfileResultTypeDef,
-    DescribeUserProfileResultTypeDef,
-    ListTagsForProjectResultTypeDef,
-    TagProjectResultTypeDef,
     UpdateTeamMemberResultTypeDef,
+    UpdateUserProfileRequestRequestTypeDef,
     UpdateUserProfileResultTypeDef,
     CodeDestinationTypeDef,
     CodeSourceTypeDef,
     ToolchainSourceTypeDef,
     DescribeProjectResultTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
-    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
-    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListProjectsResultTypeDef,
     ListResourcesResultTypeDef,
     ListTeamMembersResultTypeDef,
     ListUserProfilesResultTypeDef,
     CodeTypeDef,
     ToolchainTypeDef,
     CreateProjectRequestRequestTypeDef,
@@ -363,42 +363,42 @@
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

### Comparing `mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/__init__.py` & `mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/__init__.pyi` & `mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/client.py` & `mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/client.pyi` & `mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/literals.py` & `mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,23 +48,25 @@
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
@@ -74,30 +76,35 @@
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
@@ -123,14 +130,15 @@
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
@@ -175,51 +183,57 @@
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
@@ -232,14 +246,15 @@
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
@@ -251,28 +266,35 @@
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
@@ -281,14 +303,15 @@
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
@@ -299,55 +322,64 @@
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

### Comparing `mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/literals.pyi` & `mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -46,23 +46,25 @@
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
@@ -72,30 +74,35 @@
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
@@ -121,14 +128,15 @@
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
@@ -173,51 +181,57 @@
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
@@ -230,14 +244,15 @@
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
@@ -249,28 +264,35 @@
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
@@ -279,14 +301,15 @@
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
@@ -297,55 +320,64 @@
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

### Comparing `mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/paginator.py` & `mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,58 +58,58 @@
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listprojectspaginator)
         """
 
 
 class ListResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listresourcespaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listresourcespaginator)
         """
 
 
 class ListTeamMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listteammemberspaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTeamMembersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listteammemberspaginator)
         """
 
 
 class ListUserProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listuserprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUserProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listuserprofilespaginator)
         """
```

### Comparing `mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/paginator.pyi` & `mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,55 +55,55 @@
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listprojectspaginator)
         """
 
 class ListResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listresourcespaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listresourcespaginator)
         """
 
 class ListTeamMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listteammemberspaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTeamMembersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listteammemberspaginator)
         """
 
 class ListUserProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listuserprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUserProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listuserprofilespaginator)
         """
```

### Comparing `mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/type_defs.py` & `mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,58 +19,58 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateTeamMemberRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateTeamMemberResultTypeDef",
     "CodeCommitCodeDestinationTypeDef",
     "GitHubCodeDestinationTypeDef",
     "S3LocationTypeDef",
+    "CreateProjectResultTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
+    "CreateUserProfileResultTypeDef",
     "DeleteProjectRequestRequestTypeDef",
+    "DeleteProjectResultTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
+    "DeleteUserProfileResultTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "ProjectStatusTypeDef",
     "DescribeUserProfileRequestRequestTypeDef",
+    "DescribeUserProfileResultTypeDef",
     "DisassociateTeamMemberRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
+    "ListResourcesRequestListResourcesPaginateTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListTagsForProjectRequestRequestTypeDef",
+    "ListTagsForProjectResultTypeDef",
+    "ListTeamMembersRequestListTeamMembersPaginateTypeDef",
     "ListTeamMembersRequestRequestTypeDef",
     "TeamMemberTypeDef",
+    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
     "ListUserProfilesRequestRequestTypeDef",
     "UserProfileSummaryTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagProjectRequestRequestTypeDef",
+    "TagProjectResultTypeDef",
     "UntagProjectRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "UpdateTeamMemberRequestRequestTypeDef",
-    "UpdateUserProfileRequestRequestTypeDef",
-    "AssociateTeamMemberResultTypeDef",
-    "CreateProjectResultTypeDef",
-    "CreateUserProfileResultTypeDef",
-    "DeleteProjectResultTypeDef",
-    "DeleteUserProfileResultTypeDef",
-    "DescribeUserProfileResultTypeDef",
-    "ListTagsForProjectResultTypeDef",
-    "TagProjectResultTypeDef",
     "UpdateTeamMemberResultTypeDef",
+    "UpdateUserProfileRequestRequestTypeDef",
     "UpdateUserProfileResultTypeDef",
     "CodeDestinationTypeDef",
     "CodeSourceTypeDef",
     "ToolchainSourceTypeDef",
     "DescribeProjectResultTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    "ListResourcesRequestListResourcesPaginateTypeDef",
-    "ListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
     "ListProjectsResultTypeDef",
     "ListResourcesResultTypeDef",
     "ListTeamMembersResultTypeDef",
     "ListUserProfilesResultTypeDef",
     "CodeTypeDef",
     "ToolchainTypeDef",
     "CreateProjectRequestRequestTypeDef",
@@ -97,22 +97,19 @@
 class AssociateTeamMemberRequestRequestTypeDef(
     _RequiredAssociateTeamMemberRequestRequestTypeDef,
     _OptionalAssociateTeamMemberRequestRequestTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateTeamMemberResultTypeDef = TypedDict(
+    "AssociateTeamMemberResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "clientRequestToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CodeCommitCodeDestinationTypeDef = TypedDict(
     "CodeCommitCodeDestinationTypeDef",
     {
         "name": str,
@@ -150,14 +147,25 @@
     {
         "bucketName": str,
         "bucketKey": str,
     },
     total=False,
 )
 
+CreateProjectResultTypeDef = TypedDict(
+    "CreateProjectResultTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "clientRequestToken": str,
+        "projectTemplateId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
         "displayName": str,
         "emailAddress": str,
     },
@@ -173,14 +181,27 @@
 
 class CreateUserProfileRequestRequestTypeDef(
     _RequiredCreateUserProfileRequestRequestTypeDef, _OptionalCreateUserProfileRequestRequestTypeDef
 ):
     pass
 
 
+CreateUserProfileResultTypeDef = TypedDict(
+    "CreateUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "displayName": str,
+        "emailAddress": str,
+        "sshPublicKey": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
@@ -195,21 +216,38 @@
 
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
 
+DeleteProjectResultTypeDef = TypedDict(
+    "DeleteProjectResultTypeDef",
+    {
+        "stackId": str,
+        "projectArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteUserProfileRequestRequestTypeDef = TypedDict(
     "DeleteUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 
+DeleteUserProfileResultTypeDef = TypedDict(
+    "DeleteUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -235,28 +273,39 @@
 DescribeUserProfileRequestRequestTypeDef = TypedDict(
     "DescribeUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 
+DescribeUserProfileResultTypeDef = TypedDict(
+    "DescribeUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "displayName": str,
+        "emailAddress": str,
+        "sshPublicKey": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateTeamMemberRequestRequestTypeDef = TypedDict(
     "DisassociateTeamMemberRequestRequestTypeDef",
     {
         "projectId": str,
         "userArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
@@ -271,14 +320,36 @@
     {
         "projectId": str,
         "projectArn": str,
     },
     total=False,
 )
 
+_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
+    {
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
         "projectId": str,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -323,14 +394,45 @@
 class ListTagsForProjectRequestRequestTypeDef(
     _RequiredListTagsForProjectRequestRequestTypeDef,
     _OptionalListTagsForProjectRequestRequestTypeDef,
 ):
     pass
 
 
+ListTagsForProjectResultTypeDef = TypedDict(
+    "ListTagsForProjectResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
+    "_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
+    "_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTeamMembersRequestListTeamMembersPaginateTypeDef(
+    _RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef,
+    _OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTeamMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListTeamMembersRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListTeamMembersRequestRequestTypeDef = TypedDict(
@@ -365,14 +467,22 @@
 )
 
 
 class TeamMemberTypeDef(_RequiredTeamMemberTypeDef, _OptionalTeamMemberTypeDef):
     pass
 
 
+ListUserProfilesRequestListUserProfilesPaginateTypeDef = TypedDict(
+    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListUserProfilesRequestRequestTypeDef = TypedDict(
     "ListUserProfilesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -385,22 +495,51 @@
         "displayName": str,
         "emailAddress": str,
         "sshPublicKey": str,
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
 TagProjectRequestRequestTypeDef = TypedDict(
     "TagProjectRequestRequestTypeDef",
     {
         "id": str,
         "tags": Mapping[str, str],
     },
 )
 
+TagProjectResultTypeDef = TypedDict(
+    "TagProjectResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagProjectRequestRequestTypeDef = TypedDict(
     "UntagProjectRequestRequestTypeDef",
     {
         "id": str,
         "tags": Sequence[str],
     },
 )
@@ -446,14 +585,24 @@
 
 class UpdateTeamMemberRequestRequestTypeDef(
     _RequiredUpdateTeamMemberRequestRequestTypeDef, _OptionalUpdateTeamMemberRequestRequestTypeDef
 ):
     pass
 
 
+UpdateTeamMemberResultTypeDef = TypedDict(
+    "UpdateTeamMemberResultTypeDef",
+    {
+        "userArn": str,
+        "projectRole": str,
+        "remoteAccessAllowed": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 _OptionalUpdateUserProfileRequestRequestTypeDef = TypedDict(
@@ -469,113 +618,24 @@
 
 class UpdateUserProfileRequestRequestTypeDef(
     _RequiredUpdateUserProfileRequestRequestTypeDef, _OptionalUpdateUserProfileRequestRequestTypeDef
 ):
     pass
 
 
-AssociateTeamMemberResultTypeDef = TypedDict(
-    "AssociateTeamMemberResultTypeDef",
-    {
-        "clientRequestToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProjectResultTypeDef = TypedDict(
-    "CreateProjectResultTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "clientRequestToken": str,
-        "projectTemplateId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserProfileResultTypeDef = TypedDict(
-    "CreateUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "displayName": str,
-        "emailAddress": str,
-        "sshPublicKey": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProjectResultTypeDef = TypedDict(
-    "DeleteProjectResultTypeDef",
-    {
-        "stackId": str,
-        "projectArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteUserProfileResultTypeDef = TypedDict(
-    "DeleteUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeUserProfileResultTypeDef = TypedDict(
-    "DescribeUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "displayName": str,
-        "emailAddress": str,
-        "sshPublicKey": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForProjectResultTypeDef = TypedDict(
-    "ListTagsForProjectResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TagProjectResultTypeDef = TypedDict(
-    "TagProjectResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTeamMemberResultTypeDef = TypedDict(
-    "UpdateTeamMemberResultTypeDef",
-    {
-        "userArn": str,
-        "projectRole": str,
-        "remoteAccessAllowed": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateUserProfileResultTypeDef = TypedDict(
     "UpdateUserProfileResultTypeDef",
     {
         "userArn": str,
         "displayName": str,
         "emailAddress": str,
         "sshPublicKey": str,
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CodeDestinationTypeDef = TypedDict(
     "CodeDestinationTypeDef",
     {
         "codeCommit": CodeCommitCodeDestinationTypeDef,
@@ -606,111 +666,51 @@
         "arn": str,
         "description": str,
         "clientRequestToken": str,
         "createdTimeStamp": datetime,
         "stackId": str,
         "projectTemplateId": str,
         "status": ProjectStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListResourcesRequestListResourcesPaginateTypeDef(
-    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
-    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
-    "_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
-    "_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTeamMembersRequestListTeamMembersPaginateTypeDef(
-    _RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef,
-    _OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef,
-):
-    pass
-
-
-ListUserProfilesRequestListUserProfilesPaginateTypeDef = TypedDict(
-    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListProjectsResultTypeDef = TypedDict(
     "ListProjectsResultTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourcesResultTypeDef = TypedDict(
     "ListResourcesResultTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTeamMembersResultTypeDef = TypedDict(
     "ListTeamMembersResultTypeDef",
     {
         "teamMembers": List[TeamMemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUserProfilesResultTypeDef = TypedDict(
     "ListUserProfilesResultTypeDef",
     {
         "userProfiles": List[UserProfileSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CodeTypeDef = TypedDict(
     "CodeTypeDef",
     {
         "source": CodeSourceTypeDef,
```

### Comparing `mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar/type_defs.pyi` & `mypy-boto3-codestar-1.27.0/mypy_boto3_codestar/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -18,58 +18,58 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateTeamMemberRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateTeamMemberResultTypeDef",
     "CodeCommitCodeDestinationTypeDef",
     "GitHubCodeDestinationTypeDef",
     "S3LocationTypeDef",
+    "CreateProjectResultTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
+    "CreateUserProfileResultTypeDef",
     "DeleteProjectRequestRequestTypeDef",
+    "DeleteProjectResultTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
+    "DeleteUserProfileResultTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "ProjectStatusTypeDef",
     "DescribeUserProfileRequestRequestTypeDef",
+    "DescribeUserProfileResultTypeDef",
     "DisassociateTeamMemberRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
+    "ListResourcesRequestListResourcesPaginateTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListTagsForProjectRequestRequestTypeDef",
+    "ListTagsForProjectResultTypeDef",
+    "ListTeamMembersRequestListTeamMembersPaginateTypeDef",
     "ListTeamMembersRequestRequestTypeDef",
     "TeamMemberTypeDef",
+    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
     "ListUserProfilesRequestRequestTypeDef",
     "UserProfileSummaryTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagProjectRequestRequestTypeDef",
+    "TagProjectResultTypeDef",
     "UntagProjectRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "UpdateTeamMemberRequestRequestTypeDef",
-    "UpdateUserProfileRequestRequestTypeDef",
-    "AssociateTeamMemberResultTypeDef",
-    "CreateProjectResultTypeDef",
-    "CreateUserProfileResultTypeDef",
-    "DeleteProjectResultTypeDef",
-    "DeleteUserProfileResultTypeDef",
-    "DescribeUserProfileResultTypeDef",
-    "ListTagsForProjectResultTypeDef",
-    "TagProjectResultTypeDef",
     "UpdateTeamMemberResultTypeDef",
+    "UpdateUserProfileRequestRequestTypeDef",
     "UpdateUserProfileResultTypeDef",
     "CodeDestinationTypeDef",
     "CodeSourceTypeDef",
     "ToolchainSourceTypeDef",
     "DescribeProjectResultTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    "ListResourcesRequestListResourcesPaginateTypeDef",
-    "ListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
     "ListProjectsResultTypeDef",
     "ListResourcesResultTypeDef",
     "ListTeamMembersResultTypeDef",
     "ListUserProfilesResultTypeDef",
     "CodeTypeDef",
     "ToolchainTypeDef",
     "CreateProjectRequestRequestTypeDef",
@@ -94,22 +94,19 @@
 
 class AssociateTeamMemberRequestRequestTypeDef(
     _RequiredAssociateTeamMemberRequestRequestTypeDef,
     _OptionalAssociateTeamMemberRequestRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateTeamMemberResultTypeDef = TypedDict(
+    "AssociateTeamMemberResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "clientRequestToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CodeCommitCodeDestinationTypeDef = TypedDict(
     "CodeCommitCodeDestinationTypeDef",
     {
         "name": str,
@@ -145,14 +142,25 @@
     {
         "bucketName": str,
         "bucketKey": str,
     },
     total=False,
 )
 
+CreateProjectResultTypeDef = TypedDict(
+    "CreateProjectResultTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "clientRequestToken": str,
+        "projectTemplateId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
         "displayName": str,
         "emailAddress": str,
     },
@@ -166,14 +174,27 @@
 )
 
 class CreateUserProfileRequestRequestTypeDef(
     _RequiredCreateUserProfileRequestRequestTypeDef, _OptionalCreateUserProfileRequestRequestTypeDef
 ):
     pass
 
+CreateUserProfileResultTypeDef = TypedDict(
+    "CreateUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "displayName": str,
+        "emailAddress": str,
+        "sshPublicKey": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
@@ -186,21 +207,38 @@
 )
 
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
+DeleteProjectResultTypeDef = TypedDict(
+    "DeleteProjectResultTypeDef",
+    {
+        "stackId": str,
+        "projectArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteUserProfileRequestRequestTypeDef = TypedDict(
     "DeleteUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 
+DeleteUserProfileResultTypeDef = TypedDict(
+    "DeleteUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -224,28 +262,39 @@
 DescribeUserProfileRequestRequestTypeDef = TypedDict(
     "DescribeUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 
+DescribeUserProfileResultTypeDef = TypedDict(
+    "DescribeUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "displayName": str,
+        "emailAddress": str,
+        "sshPublicKey": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateTeamMemberRequestRequestTypeDef = TypedDict(
     "DisassociateTeamMemberRequestRequestTypeDef",
     {
         "projectId": str,
         "userArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
@@ -260,14 +309,34 @@
     {
         "projectId": str,
         "projectArn": str,
     },
     total=False,
 )
 
+_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
+    {
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
         "projectId": str,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -308,14 +377,43 @@
 
 class ListTagsForProjectRequestRequestTypeDef(
     _RequiredListTagsForProjectRequestRequestTypeDef,
     _OptionalListTagsForProjectRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForProjectResultTypeDef = TypedDict(
+    "ListTagsForProjectResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
+    "_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
+    "_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTeamMembersRequestListTeamMembersPaginateTypeDef(
+    _RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef,
+    _OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef,
+):
+    pass
+
 _RequiredListTeamMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListTeamMembersRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListTeamMembersRequestRequestTypeDef = TypedDict(
@@ -346,14 +444,22 @@
     },
     total=False,
 )
 
 class TeamMemberTypeDef(_RequiredTeamMemberTypeDef, _OptionalTeamMemberTypeDef):
     pass
 
+ListUserProfilesRequestListUserProfilesPaginateTypeDef = TypedDict(
+    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListUserProfilesRequestRequestTypeDef = TypedDict(
     "ListUserProfilesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -366,22 +472,51 @@
         "displayName": str,
         "emailAddress": str,
         "sshPublicKey": str,
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
 TagProjectRequestRequestTypeDef = TypedDict(
     "TagProjectRequestRequestTypeDef",
     {
         "id": str,
         "tags": Mapping[str, str],
     },
 )
 
+TagProjectResultTypeDef = TypedDict(
+    "TagProjectResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagProjectRequestRequestTypeDef = TypedDict(
     "UntagProjectRequestRequestTypeDef",
     {
         "id": str,
         "tags": Sequence[str],
     },
 )
@@ -423,14 +558,24 @@
 )
 
 class UpdateTeamMemberRequestRequestTypeDef(
     _RequiredUpdateTeamMemberRequestRequestTypeDef, _OptionalUpdateTeamMemberRequestRequestTypeDef
 ):
     pass
 
+UpdateTeamMemberResultTypeDef = TypedDict(
+    "UpdateTeamMemberResultTypeDef",
+    {
+        "userArn": str,
+        "projectRole": str,
+        "remoteAccessAllowed": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 _OptionalUpdateUserProfileRequestRequestTypeDef = TypedDict(
@@ -444,113 +589,24 @@
 )
 
 class UpdateUserProfileRequestRequestTypeDef(
     _RequiredUpdateUserProfileRequestRequestTypeDef, _OptionalUpdateUserProfileRequestRequestTypeDef
 ):
     pass
 
-AssociateTeamMemberResultTypeDef = TypedDict(
-    "AssociateTeamMemberResultTypeDef",
-    {
-        "clientRequestToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProjectResultTypeDef = TypedDict(
-    "CreateProjectResultTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "clientRequestToken": str,
-        "projectTemplateId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserProfileResultTypeDef = TypedDict(
-    "CreateUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "displayName": str,
-        "emailAddress": str,
-        "sshPublicKey": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProjectResultTypeDef = TypedDict(
-    "DeleteProjectResultTypeDef",
-    {
-        "stackId": str,
-        "projectArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteUserProfileResultTypeDef = TypedDict(
-    "DeleteUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeUserProfileResultTypeDef = TypedDict(
-    "DescribeUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "displayName": str,
-        "emailAddress": str,
-        "sshPublicKey": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForProjectResultTypeDef = TypedDict(
-    "ListTagsForProjectResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TagProjectResultTypeDef = TypedDict(
-    "TagProjectResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTeamMemberResultTypeDef = TypedDict(
-    "UpdateTeamMemberResultTypeDef",
-    {
-        "userArn": str,
-        "projectRole": str,
-        "remoteAccessAllowed": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateUserProfileResultTypeDef = TypedDict(
     "UpdateUserProfileResultTypeDef",
     {
         "userArn": str,
         "displayName": str,
         "emailAddress": str,
         "sshPublicKey": str,
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CodeDestinationTypeDef = TypedDict(
     "CodeDestinationTypeDef",
     {
         "codeCommit": CodeCommitCodeDestinationTypeDef,
@@ -581,107 +637,51 @@
         "arn": str,
         "description": str,
         "clientRequestToken": str,
         "createdTimeStamp": datetime,
         "stackId": str,
         "projectTemplateId": str,
         "status": ProjectStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListResourcesRequestListResourcesPaginateTypeDef(
-    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
-    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
-):
-    pass
-
-_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
-    "_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
-    "_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTeamMembersRequestListTeamMembersPaginateTypeDef(
-    _RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef,
-    _OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef,
-):
-    pass
-
-ListUserProfilesRequestListUserProfilesPaginateTypeDef = TypedDict(
-    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListProjectsResultTypeDef = TypedDict(
     "ListProjectsResultTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourcesResultTypeDef = TypedDict(
     "ListResourcesResultTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTeamMembersResultTypeDef = TypedDict(
     "ListTeamMembersResultTypeDef",
     {
         "teamMembers": List[TeamMemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUserProfilesResultTypeDef = TypedDict(
     "ListUserProfilesResultTypeDef",
     {
         "userProfiles": List[UserProfileSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CodeTypeDef = TypedDict(
     "CodeTypeDef",
     {
         "source": CodeSourceTypeDef,
```

### Comparing `mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar.egg-info/PKG-INFO` & `mypy-boto3-codestar-1.27.0/mypy_boto3_codestar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeStar 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeStar 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/
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
 
 <a id="mypy-boto3-codestar"></a>
 
 # mypy-boto3-codestar
 
 [![PyPI - mypy-boto3-codestar](https://img.shields.io/pypi/v/mypy-boto3-codestar.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codestar?color=blue)](https://pypistats.org/packages/mypy-boto3-codestar)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStar 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
+[boto3.CodeStar 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
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
 [mypy-boto3-codestar docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,58 +330,58 @@
 
 `mypy_boto3_codestar.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar.type_defs import (
     AssociateTeamMemberRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateTeamMemberResultTypeDef,
     CodeCommitCodeDestinationTypeDef,
     GitHubCodeDestinationTypeDef,
     S3LocationTypeDef,
+    CreateProjectResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
+    CreateUserProfileResultTypeDef,
     DeleteProjectRequestRequestTypeDef,
+    DeleteProjectResultTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
+    DeleteUserProfileResultTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ProjectStatusTypeDef,
     DescribeUserProfileRequestRequestTypeDef,
+    DescribeUserProfileResultTypeDef,
     DisassociateTeamMemberRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForProjectRequestRequestTypeDef,
+    ListTagsForProjectResultTypeDef,
+    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
     ListTeamMembersRequestRequestTypeDef,
     TeamMemberTypeDef,
+    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListUserProfilesRequestRequestTypeDef,
     UserProfileSummaryTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagProjectRequestRequestTypeDef,
+    TagProjectResultTypeDef,
     UntagProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     UpdateTeamMemberRequestRequestTypeDef,
-    UpdateUserProfileRequestRequestTypeDef,
-    AssociateTeamMemberResultTypeDef,
-    CreateProjectResultTypeDef,
-    CreateUserProfileResultTypeDef,
-    DeleteProjectResultTypeDef,
-    DeleteUserProfileResultTypeDef,
-    DescribeUserProfileResultTypeDef,
-    ListTagsForProjectResultTypeDef,
-    TagProjectResultTypeDef,
     UpdateTeamMemberResultTypeDef,
+    UpdateUserProfileRequestRequestTypeDef,
     UpdateUserProfileResultTypeDef,
     CodeDestinationTypeDef,
     CodeSourceTypeDef,
     ToolchainSourceTypeDef,
     DescribeProjectResultTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
-    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
-    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListProjectsResultTypeDef,
     ListResourcesResultTypeDef,
     ListTeamMembersResultTypeDef,
     ListUserProfilesResultTypeDef,
     CodeTypeDef,
     ToolchainTypeDef,
     CreateProjectRequestRequestTypeDef,
@@ -394,42 +395,42 @@
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

### Comparing `mypy-boto3-codestar-1.26.0.post1/mypy_boto3_codestar.egg-info/SOURCES.txt` & `mypy-boto3-codestar-1.27.0/mypy_boto3_codestar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.26.0.post1/setup.py` & `mypy-boto3-codestar-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-codestar.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codestar",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_codestar"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeStar 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.CodeStar 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 codestar type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_codestar": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_codestar": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/",
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


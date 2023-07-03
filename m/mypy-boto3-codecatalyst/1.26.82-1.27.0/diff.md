# Comparing `tmp/mypy-boto3-codecatalyst-1.26.82.tar.gz` & `tmp/mypy-boto3-codecatalyst-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codecatalyst-1.26.82.tar", last modified: Wed Mar  1 20:27:29 2023, max compression
+gzip compressed data, was "mypy-boto3-codecatalyst-1.27.0.tar", last modified: Mon Jul  3 19:50:31 2023, max compression
```

## Comparing `mypy-boto3-codecatalyst-1.26.82.tar` & `mypy-boto3-codecatalyst-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:29.582109 mypy-boto3-codecatalyst-1.26.82/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17229 2023-03-01 20:27:29.582109 mypy-boto3-codecatalyst-1.26.82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:29.582109 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22862 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22823 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32475 2023-03-01 20:27:18.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32416 2023-03-01 20:27:18.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:29.582109 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17229 2023-03-01 20:27:29.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-01 20:27:29.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:27:29.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:27:29.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-01 20:27:29.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-01 20:27:29.000000 mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 20:27:29.582109 mypy-boto3-codecatalyst-1.26.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-01 20:27:17.000000 mypy-boto3-codecatalyst-1.26.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.798985 mypy-boto3-codecatalyst-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-07-03 19:50:31.798985 mypy-boto3-codecatalyst-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16151 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.790985 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24109 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24068 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34764 2023-07-03 19:34:13.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34701 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.798985 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-07-03 19:50:31.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:50:31.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:31.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:31.000000 mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:31.798985 mypy-boto3-codecatalyst-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:34:12.000000 mypy-boto3-codecatalyst-1.27.0/setup.py
```

### Comparing `mypy-boto3-codecatalyst-1.26.82/LICENSE` & `mypy-boto3-codecatalyst-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-codecatalyst-1.26.82/PKG-INFO` & `mypy-boto3-codecatalyst-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecatalyst
-Version: 1.26.82
-Summary: Type annotations for boto3.CodeCatalyst 1.26.82 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeCatalyst 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-codecatalyst"></a>
 
 # mypy-boto3-codecatalyst
 
 [![PyPI - mypy-boto3-codecatalyst](https://img.shields.io/pypi/v/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.26.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,27 +281,31 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_codecatalyst import CodeCatalystClient
 from mypy_boto3_codecatalyst.paginator import (
     ListAccessTokensPaginator,
+    ListDevEnvironmentSessionsPaginator,
     ListDevEnvironmentsPaginator,
     ListEventLogsPaginator,
     ListProjectsPaginator,
     ListSourceRepositoriesPaginator,
     ListSourceRepositoryBranchesPaginator,
     ListSpacesPaginator,
 )
 
 client: CodeCatalystClient = Session().client("codecatalyst")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_access_tokens_paginator: ListAccessTokensPaginator = client.get_paginator("list_access_tokens")
+list_dev_environment_sessions_paginator: ListDevEnvironmentSessionsPaginator = client.get_paginator(
+    "list_dev_environment_sessions"
+)
 list_dev_environments_paginator: ListDevEnvironmentsPaginator = client.get_paginator(
     "list_dev_environments"
 )
 list_event_logs_paginator: ListEventLogsPaginator = client.get_paginator("list_event_logs")
 list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
 list_source_repositories_paginator: ListSourceRepositoriesPaginator = client.get_paginator(
     "list_source_repositories"
@@ -323,14 +327,15 @@
 from mypy_boto3_codecatalyst.literals import (
     ComparisonOperatorType,
     DevEnvironmentSessionTypeType,
     DevEnvironmentStatusType,
     FilterKeyType,
     InstanceTypeType,
     ListAccessTokensPaginatorName,
+    ListDevEnvironmentSessionsPaginatorName,
     ListDevEnvironmentsPaginatorName,
     ListEventLogsPaginatorName,
     ListProjectsPaginatorName,
     ListSourceRepositoriesPaginatorName,
     ListSourceRepositoryBranchesPaginatorName,
     ListSpacesPaginatorName,
     OperationTypeType,
@@ -353,82 +358,86 @@
 `mypy_boto3_codecatalyst.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
     CreateAccessTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAccessTokenResponseTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
+    CreateDevEnvironmentResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
+    CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
+    CreateSourceRepositoryBranchResponseTypeDef,
     DeleteAccessTokenRequestRequestTypeDef,
     DeleteDevEnvironmentRequestRequestTypeDef,
+    DeleteDevEnvironmentResponseTypeDef,
     DevEnvironmentAccessDetailsTypeDef,
     DevEnvironmentRepositorySummaryTypeDef,
     ExecuteCommandSessionConfigurationTypeDef,
+    DevEnvironmentSessionSummaryTypeDef,
     IdeTypeDef,
     PersistentStorageTypeDef,
     EmailAddressTypeDef,
     EventPayloadTypeDef,
     ProjectInformationTypeDef,
     UserIdentityTypeDef,
     FilterTypeDef,
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
+    GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
+    GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSpaceRequestRequestTypeDef,
+    GetSpaceResponseTypeDef,
     GetSubscriptionRequestRequestTypeDef,
+    GetSubscriptionResponseTypeDef,
     GetUserDetailsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
     ListAccessTokensRequestRequestTypeDef,
+    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    ListDevEnvironmentSessionsRequestRequestTypeDef,
+    ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
+    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
+    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
+    ListSpacesRequestListSpacesPaginateTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
-    StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentSessionRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
-    GetProjectResponseTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
-    GetSpaceResponseTypeDef,
-    GetSubscriptionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentRequestRequestTypeDef,
     StopDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentSessionRequestRequestTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     VerifySessionResponseTypeDef,
+    ListAccessTokensResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
+    ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestRequestTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
     ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
+    ListDevEnvironmentsRequestRequestTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
@@ -444,42 +453,42 @@
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

### Comparing `mypy-boto3-codecatalyst-1.26.82/README.md` & `mypy-boto3-codecatalyst-1.27.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codecatalyst"></a>
 
 # mypy-boto3-codecatalyst
 
 [![PyPI - mypy-boto3-codecatalyst](https://img.shields.io/pypi/v/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.26.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -249,27 +249,31 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_codecatalyst import CodeCatalystClient
 from mypy_boto3_codecatalyst.paginator import (
     ListAccessTokensPaginator,
+    ListDevEnvironmentSessionsPaginator,
     ListDevEnvironmentsPaginator,
     ListEventLogsPaginator,
     ListProjectsPaginator,
     ListSourceRepositoriesPaginator,
     ListSourceRepositoryBranchesPaginator,
     ListSpacesPaginator,
 )
 
 client: CodeCatalystClient = Session().client("codecatalyst")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_access_tokens_paginator: ListAccessTokensPaginator = client.get_paginator("list_access_tokens")
+list_dev_environment_sessions_paginator: ListDevEnvironmentSessionsPaginator = client.get_paginator(
+    "list_dev_environment_sessions"
+)
 list_dev_environments_paginator: ListDevEnvironmentsPaginator = client.get_paginator(
     "list_dev_environments"
 )
 list_event_logs_paginator: ListEventLogsPaginator = client.get_paginator("list_event_logs")
 list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
 list_source_repositories_paginator: ListSourceRepositoriesPaginator = client.get_paginator(
     "list_source_repositories"
@@ -291,14 +295,15 @@
 from mypy_boto3_codecatalyst.literals import (
     ComparisonOperatorType,
     DevEnvironmentSessionTypeType,
     DevEnvironmentStatusType,
     FilterKeyType,
     InstanceTypeType,
     ListAccessTokensPaginatorName,
+    ListDevEnvironmentSessionsPaginatorName,
     ListDevEnvironmentsPaginatorName,
     ListEventLogsPaginatorName,
     ListProjectsPaginatorName,
     ListSourceRepositoriesPaginatorName,
     ListSourceRepositoryBranchesPaginatorName,
     ListSpacesPaginatorName,
     OperationTypeType,
@@ -321,82 +326,86 @@
 `mypy_boto3_codecatalyst.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
     CreateAccessTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAccessTokenResponseTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
+    CreateDevEnvironmentResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
+    CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
+    CreateSourceRepositoryBranchResponseTypeDef,
     DeleteAccessTokenRequestRequestTypeDef,
     DeleteDevEnvironmentRequestRequestTypeDef,
+    DeleteDevEnvironmentResponseTypeDef,
     DevEnvironmentAccessDetailsTypeDef,
     DevEnvironmentRepositorySummaryTypeDef,
     ExecuteCommandSessionConfigurationTypeDef,
+    DevEnvironmentSessionSummaryTypeDef,
     IdeTypeDef,
     PersistentStorageTypeDef,
     EmailAddressTypeDef,
     EventPayloadTypeDef,
     ProjectInformationTypeDef,
     UserIdentityTypeDef,
     FilterTypeDef,
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
+    GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
+    GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSpaceRequestRequestTypeDef,
+    GetSpaceResponseTypeDef,
     GetSubscriptionRequestRequestTypeDef,
+    GetSubscriptionResponseTypeDef,
     GetUserDetailsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
     ListAccessTokensRequestRequestTypeDef,
+    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    ListDevEnvironmentSessionsRequestRequestTypeDef,
+    ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
+    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
+    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
+    ListSpacesRequestListSpacesPaginateTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
-    StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentSessionRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
-    GetProjectResponseTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
-    GetSpaceResponseTypeDef,
-    GetSubscriptionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentRequestRequestTypeDef,
     StopDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentSessionRequestRequestTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     VerifySessionResponseTypeDef,
+    ListAccessTokensResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
+    ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestRequestTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
     ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
+    ListDevEnvironmentsRequestRequestTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
@@ -412,42 +421,42 @@
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

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/__init__.py` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -5,52 +5,55 @@
 
     ```python
     from boto3.session import Session
     from mypy_boto3_codecatalyst import (
         Client,
         CodeCatalystClient,
         ListAccessTokensPaginator,
+        ListDevEnvironmentSessionsPaginator,
         ListDevEnvironmentsPaginator,
         ListEventLogsPaginator,
         ListProjectsPaginator,
         ListSourceRepositoriesPaginator,
         ListSourceRepositoryBranchesPaginator,
         ListSpacesPaginator,
     )
 
     session = Session()
     client: CodeCatalystClient = session.client("codecatalyst")
 
     list_access_tokens_paginator: ListAccessTokensPaginator = client.get_paginator("list_access_tokens")
+    list_dev_environment_sessions_paginator: ListDevEnvironmentSessionsPaginator = client.get_paginator("list_dev_environment_sessions")
     list_dev_environments_paginator: ListDevEnvironmentsPaginator = client.get_paginator("list_dev_environments")
     list_event_logs_paginator: ListEventLogsPaginator = client.get_paginator("list_event_logs")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_source_repositories_paginator: ListSourceRepositoriesPaginator = client.get_paginator("list_source_repositories")
     list_source_repository_branches_paginator: ListSourceRepositoryBranchesPaginator = client.get_paginator("list_source_repository_branches")
     list_spaces_paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
     ```
 """
 from .client import CodeCatalystClient
 from .paginator import (
     ListAccessTokensPaginator,
+    ListDevEnvironmentSessionsPaginator,
     ListDevEnvironmentsPaginator,
     ListEventLogsPaginator,
     ListProjectsPaginator,
     ListSourceRepositoriesPaginator,
     ListSourceRepositoryBranchesPaginator,
     ListSpacesPaginator,
 )
 
 Client = CodeCatalystClient
 
-
 __all__ = (
     "Client",
     "CodeCatalystClient",
     "ListAccessTokensPaginator",
+    "ListDevEnvironmentSessionsPaginator",
     "ListDevEnvironmentsPaginator",
     "ListEventLogsPaginator",
     "ListProjectsPaginator",
     "ListSourceRepositoriesPaginator",
     "ListSourceRepositoryBranchesPaginator",
     "ListSpacesPaginator",
 )
```

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/__init__.pyi` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,51 +5,56 @@
 
     ```python
     from boto3.session import Session
     from mypy_boto3_codecatalyst import (
         Client,
         CodeCatalystClient,
         ListAccessTokensPaginator,
+        ListDevEnvironmentSessionsPaginator,
         ListDevEnvironmentsPaginator,
         ListEventLogsPaginator,
         ListProjectsPaginator,
         ListSourceRepositoriesPaginator,
         ListSourceRepositoryBranchesPaginator,
         ListSpacesPaginator,
     )
 
     session = Session()
     client: CodeCatalystClient = session.client("codecatalyst")
 
     list_access_tokens_paginator: ListAccessTokensPaginator = client.get_paginator("list_access_tokens")
+    list_dev_environment_sessions_paginator: ListDevEnvironmentSessionsPaginator = client.get_paginator("list_dev_environment_sessions")
     list_dev_environments_paginator: ListDevEnvironmentsPaginator = client.get_paginator("list_dev_environments")
     list_event_logs_paginator: ListEventLogsPaginator = client.get_paginator("list_event_logs")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_source_repositories_paginator: ListSourceRepositoriesPaginator = client.get_paginator("list_source_repositories")
     list_source_repository_branches_paginator: ListSourceRepositoryBranchesPaginator = client.get_paginator("list_source_repository_branches")
     list_spaces_paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
     ```
 """
 from .client import CodeCatalystClient
 from .paginator import (
     ListAccessTokensPaginator,
+    ListDevEnvironmentSessionsPaginator,
     ListDevEnvironmentsPaginator,
     ListEventLogsPaginator,
     ListProjectsPaginator,
     ListSourceRepositoriesPaginator,
     ListSourceRepositoryBranchesPaginator,
     ListSpacesPaginator,
 )
 
 Client = CodeCatalystClient
 
+
 __all__ = (
     "Client",
     "CodeCatalystClient",
     "ListAccessTokensPaginator",
+    "ListDevEnvironmentSessionsPaginator",
     "ListDevEnvironmentsPaginator",
     "ListEventLogsPaginator",
     "ListProjectsPaginator",
     "ListSourceRepositoriesPaginator",
     "ListSourceRepositoryBranchesPaginator",
     "ListSpacesPaginator",
 )
```

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/__main__.py` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeCatalyst 1.26.82\nVersion:         1.26.82\nBuilder"
-        " version: 7.12.5\nDocs:           "
+        "Type annotations for boto3.CodeCatalyst 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.82")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/client.py` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import InstanceTypeType
 from .paginator import (
     ListAccessTokensPaginator,
+    ListDevEnvironmentSessionsPaginator,
     ListDevEnvironmentsPaginator,
     ListEventLogsPaginator,
     ListProjectsPaginator,
     ListSourceRepositoriesPaginator,
     ListSourceRepositoryBranchesPaginator,
     ListSpacesPaginator,
 )
@@ -41,14 +42,15 @@
     GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSpaceResponseTypeDef,
     GetSubscriptionResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     IdeConfigurationTypeDef,
     ListAccessTokensResponseTypeDef,
+    ListDevEnvironmentSessionsResponseTypeDef,
     ListDevEnvironmentsResponseTypeDef,
     ListEventLogsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     PersistentStorageConfigurationTypeDef,
@@ -142,16 +144,16 @@
         repositories: Sequence[RepositoryInputTypeDef] = ...,
         clientToken: str = ...,
         alias: str = ...,
         ides: Sequence[IdeConfigurationTypeDef] = ...,
         inactivityTimeoutMinutes: int = ...
     ) -> CreateDevEnvironmentResponseTypeDef:
         """
-        Creates a Dev Environment in Amazon CodeCatalyst, a cloud-based development Dev
-        Environment that you can use to quickly work on the code stored in the source
+        Creates a Dev Environment in Amazon CodeCatalyst, a cloud-based development
+        environment that you can use to quickly work on the code stored in the source
         repositories of your project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_dev_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#create_dev_environment)
         """
 
     def create_project(
@@ -276,25 +278,41 @@
         Lists all personal access tokens (PATs) associated with the user who calls the
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_access_tokens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#list_access_tokens)
         """
 
+    def list_dev_environment_sessions(
+        self,
+        *,
+        spaceName: str,
+        projectName: str,
+        devEnvironmentId: str,
+        nextToken: str = ...,
+        maxResults: int = ...
+    ) -> ListDevEnvironmentSessionsResponseTypeDef:
+        """
+        Retrieves a list of active sessions for a Dev Environment in a project.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_dev_environment_sessions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#list_dev_environment_sessions)
+        """
+
     def list_dev_environments(
         self,
         *,
         spaceName: str,
         projectName: str,
         filters: Sequence[FilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListDevEnvironmentsResponseTypeDef:
         """
-        Retrives a list of Dev Environments in a project.
+        Retrieves a list of Dev Environments in a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_dev_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#list_dev_environments)
         """
 
     def list_event_logs(
         self,
@@ -450,14 +468,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_dev_environment_sessions"]
+    ) -> ListDevEnvironmentSessionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_dev_environments"]
     ) -> ListDevEnvironmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/client.pyi` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import InstanceTypeType
 from .paginator import (
     ListAccessTokensPaginator,
+    ListDevEnvironmentSessionsPaginator,
     ListDevEnvironmentsPaginator,
     ListEventLogsPaginator,
     ListProjectsPaginator,
     ListSourceRepositoriesPaginator,
     ListSourceRepositoryBranchesPaginator,
     ListSpacesPaginator,
 )
@@ -41,14 +42,15 @@
     GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSpaceResponseTypeDef,
     GetSubscriptionResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     IdeConfigurationTypeDef,
     ListAccessTokensResponseTypeDef,
+    ListDevEnvironmentSessionsResponseTypeDef,
     ListDevEnvironmentsResponseTypeDef,
     ListEventLogsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     PersistentStorageConfigurationTypeDef,
@@ -134,16 +136,16 @@
         repositories: Sequence[RepositoryInputTypeDef] = ...,
         clientToken: str = ...,
         alias: str = ...,
         ides: Sequence[IdeConfigurationTypeDef] = ...,
         inactivityTimeoutMinutes: int = ...
     ) -> CreateDevEnvironmentResponseTypeDef:
         """
-        Creates a Dev Environment in Amazon CodeCatalyst, a cloud-based development Dev
-        Environment that you can use to quickly work on the code stored in the source
+        Creates a Dev Environment in Amazon CodeCatalyst, a cloud-based development
+        environment that you can use to quickly work on the code stored in the source
         repositories of your project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_dev_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#create_dev_environment)
         """
     def create_project(
         self, *, spaceName: str, displayName: str, description: str = ...
@@ -255,25 +257,40 @@
         """
         Lists all personal access tokens (PATs) associated with the user who calls the
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_access_tokens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#list_access_tokens)
         """
+    def list_dev_environment_sessions(
+        self,
+        *,
+        spaceName: str,
+        projectName: str,
+        devEnvironmentId: str,
+        nextToken: str = ...,
+        maxResults: int = ...
+    ) -> ListDevEnvironmentSessionsResponseTypeDef:
+        """
+        Retrieves a list of active sessions for a Dev Environment in a project.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_dev_environment_sessions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#list_dev_environment_sessions)
+        """
     def list_dev_environments(
         self,
         *,
         spaceName: str,
         projectName: str,
         filters: Sequence[FilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListDevEnvironmentsResponseTypeDef:
         """
-        Retrives a list of Dev Environments in a project.
+        Retrieves a list of Dev Environments in a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.list_dev_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#list_dev_environments)
         """
     def list_event_logs(
         self,
         *,
@@ -416,14 +433,22 @@
     ) -> ListAccessTokensPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#get_paginator)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_dev_environment_sessions"]
+    ) -> ListDevEnvironmentSessionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_dev_environments"]
     ) -> ListDevEnvironmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#get_paginator)
         """
     @overload
```

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/literals.py` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 __all__ = (
     "ComparisonOperatorType",
     "DevEnvironmentSessionTypeType",
     "DevEnvironmentStatusType",
     "FilterKeyType",
     "InstanceTypeType",
     "ListAccessTokensPaginatorName",
+    "ListDevEnvironmentSessionsPaginatorName",
     "ListDevEnvironmentsPaginatorName",
     "ListEventLogsPaginatorName",
     "ListProjectsPaginatorName",
     "ListSourceRepositoriesPaginatorName",
     "ListSourceRepositoryBranchesPaginatorName",
     "ListSpacesPaginatorName",
     "OperationTypeType",
@@ -47,14 +48,15 @@
     "DELETED", "DELETING", "FAILED", "PENDING", "RUNNING", "STARTING", "STOPPED", "STOPPING"
 ]
 FilterKeyType = Literal["hasAccessTo"]
 InstanceTypeType = Literal[
     "dev.standard1.large", "dev.standard1.medium", "dev.standard1.small", "dev.standard1.xlarge"
 ]
 ListAccessTokensPaginatorName = Literal["list_access_tokens"]
+ListDevEnvironmentSessionsPaginatorName = Literal["list_dev_environment_sessions"]
 ListDevEnvironmentsPaginatorName = Literal["list_dev_environments"]
 ListEventLogsPaginatorName = Literal["list_event_logs"]
 ListProjectsPaginatorName = Literal["list_projects"]
 ListSourceRepositoriesPaginatorName = Literal["list_source_repositories"]
 ListSourceRepositoryBranchesPaginatorName = Literal["list_source_repository_branches"]
 ListSpacesPaginatorName = Literal["list_spaces"]
 OperationTypeType = Literal["MUTATION", "READONLY"]
@@ -71,14 +73,15 @@
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
@@ -118,14 +121,15 @@
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
@@ -223,14 +227,15 @@
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
@@ -266,14 +271,15 @@
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
@@ -292,16 +298,19 @@
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
@@ -385,15 +394,17 @@
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
@@ -413,14 +424,15 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_access_tokens",
+    "list_dev_environment_sessions",
     "list_dev_environments",
     "list_event_logs",
     "list_projects",
     "list_source_repositories",
     "list_source_repository_branches",
     "list_spaces",
 ]
```

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/literals.pyi` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 __all__ = (
     "ComparisonOperatorType",
     "DevEnvironmentSessionTypeType",
     "DevEnvironmentStatusType",
     "FilterKeyType",
     "InstanceTypeType",
     "ListAccessTokensPaginatorName",
+    "ListDevEnvironmentSessionsPaginatorName",
     "ListDevEnvironmentsPaginatorName",
     "ListEventLogsPaginatorName",
     "ListProjectsPaginatorName",
     "ListSourceRepositoriesPaginatorName",
     "ListSourceRepositoryBranchesPaginatorName",
     "ListSpacesPaginatorName",
     "OperationTypeType",
@@ -45,14 +46,15 @@
     "DELETED", "DELETING", "FAILED", "PENDING", "RUNNING", "STARTING", "STOPPED", "STOPPING"
 ]
 FilterKeyType = Literal["hasAccessTo"]
 InstanceTypeType = Literal[
     "dev.standard1.large", "dev.standard1.medium", "dev.standard1.small", "dev.standard1.xlarge"
 ]
 ListAccessTokensPaginatorName = Literal["list_access_tokens"]
+ListDevEnvironmentSessionsPaginatorName = Literal["list_dev_environment_sessions"]
 ListDevEnvironmentsPaginatorName = Literal["list_dev_environments"]
 ListEventLogsPaginatorName = Literal["list_event_logs"]
 ListProjectsPaginatorName = Literal["list_projects"]
 ListSourceRepositoriesPaginatorName = Literal["list_source_repositories"]
 ListSourceRepositoryBranchesPaginatorName = Literal["list_source_repository_branches"]
 ListSpacesPaginatorName = Literal["list_spaces"]
 OperationTypeType = Literal["MUTATION", "READONLY"]
@@ -69,14 +71,15 @@
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
@@ -116,14 +119,15 @@
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
@@ -221,14 +225,15 @@
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
@@ -264,14 +269,15 @@
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
@@ -290,16 +296,19 @@
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
@@ -383,15 +392,17 @@
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
@@ -411,14 +422,15 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_access_tokens",
+    "list_dev_environment_sessions",
     "list_dev_environments",
     "list_event_logs",
     "list_projects",
     "list_source_repositories",
     "list_source_repository_branches",
     "list_spaces",
 ]
```

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/paginator.py` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_codecatalyst.client import CodeCatalystClient
     from mypy_boto3_codecatalyst.paginator import (
         ListAccessTokensPaginator,
+        ListDevEnvironmentSessionsPaginator,
         ListDevEnvironmentsPaginator,
         ListEventLogsPaginator,
         ListProjectsPaginator,
         ListSourceRepositoriesPaginator,
         ListSourceRepositoryBranchesPaginator,
         ListSpacesPaginator,
     )
 
     session = Session()
     client: CodeCatalystClient = session.client("codecatalyst")
 
     list_access_tokens_paginator: ListAccessTokensPaginator = client.get_paginator("list_access_tokens")
+    list_dev_environment_sessions_paginator: ListDevEnvironmentSessionsPaginator = client.get_paginator("list_dev_environment_sessions")
     list_dev_environments_paginator: ListDevEnvironmentsPaginator = client.get_paginator("list_dev_environments")
     list_event_logs_paginator: ListEventLogsPaginator = client.get_paginator("list_event_logs")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_source_repositories_paginator: ListSourceRepositoriesPaginator = client.get_paginator("list_source_repositories")
     list_source_repository_branches_paginator: ListSourceRepositoryBranchesPaginator = client.get_paginator("list_source_repository_branches")
     list_spaces_paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
     ```
@@ -35,161 +37,173 @@
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     FilterTypeDef,
     ListAccessTokensResponseTypeDef,
+    ListDevEnvironmentSessionsResponseTypeDef,
     ListDevEnvironmentsResponseTypeDef,
     ListEventLogsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     PaginatorConfigTypeDef,
     ProjectListFilterTypeDef,
 )
 
 __all__ = (
     "ListAccessTokensPaginator",
+    "ListDevEnvironmentSessionsPaginator",
     "ListDevEnvironmentsPaginator",
     "ListEventLogsPaginator",
     "ListProjectsPaginator",
     "ListSourceRepositoriesPaginator",
     "ListSourceRepositoryBranchesPaginator",
     "ListSpacesPaginator",
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
 class ListAccessTokensPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listaccesstokenspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccessTokensResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listaccesstokenspaginator)
         """
 
+class ListDevEnvironmentSessionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentsessionspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        spaceName: str,
+        projectName: str,
+        devEnvironmentId: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListDevEnvironmentSessionsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentsessionspaginator)
+        """
 
 class ListDevEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentspaginator)
         """
 
-
 class ListEventLogsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listeventlogspaginator)
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         eventName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventLogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listeventlogspaginator)
         """
 
-
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listprojectspaginator)
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         filters: Sequence[ProjectListFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listprojectspaginator)
         """
 
-
 class ListSourceRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositoriespaginator)
     """
 
     def paginate(
-        self, *, spaceName: str, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, spaceName: str, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSourceRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositoriespaginator)
         """
 
-
 class ListSourceRepositoryBranchesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositorybranchespaginator)
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSourceRepositoryBranchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositorybranchespaginator)
         """
 
-
 class ListSpacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSpacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listspacespaginator)
         """
```

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/paginator.pyi` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_codecatalyst.client import CodeCatalystClient
     from mypy_boto3_codecatalyst.paginator import (
         ListAccessTokensPaginator,
+        ListDevEnvironmentSessionsPaginator,
         ListDevEnvironmentsPaginator,
         ListEventLogsPaginator,
         ListProjectsPaginator,
         ListSourceRepositoriesPaginator,
         ListSourceRepositoryBranchesPaginator,
         ListSpacesPaginator,
     )
 
     session = Session()
     client: CodeCatalystClient = session.client("codecatalyst")
 
     list_access_tokens_paginator: ListAccessTokensPaginator = client.get_paginator("list_access_tokens")
+    list_dev_environment_sessions_paginator: ListDevEnvironmentSessionsPaginator = client.get_paginator("list_dev_environment_sessions")
     list_dev_environments_paginator: ListDevEnvironmentsPaginator = client.get_paginator("list_dev_environments")
     list_event_logs_paginator: ListEventLogsPaginator = client.get_paginator("list_event_logs")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_source_repositories_paginator: ListSourceRepositoriesPaginator = client.get_paginator("list_source_repositories")
     list_source_repository_branches_paginator: ListSourceRepositoryBranchesPaginator = client.get_paginator("list_source_repository_branches")
     list_spaces_paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
     ```
@@ -35,152 +37,183 @@
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     FilterTypeDef,
     ListAccessTokensResponseTypeDef,
+    ListDevEnvironmentSessionsResponseTypeDef,
     ListDevEnvironmentsResponseTypeDef,
     ListEventLogsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     PaginatorConfigTypeDef,
     ProjectListFilterTypeDef,
 )
 
 __all__ = (
     "ListAccessTokensPaginator",
+    "ListDevEnvironmentSessionsPaginator",
     "ListDevEnvironmentsPaginator",
     "ListEventLogsPaginator",
     "ListProjectsPaginator",
     "ListSourceRepositoriesPaginator",
     "ListSourceRepositoryBranchesPaginator",
     "ListSpacesPaginator",
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
 class ListAccessTokensPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listaccesstokenspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccessTokensResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listaccesstokenspaginator)
         """
 
+
+class ListDevEnvironmentSessionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentsessionspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        spaceName: str,
+        projectName: str,
+        devEnvironmentId: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListDevEnvironmentSessionsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentsessionspaginator)
+        """
+
+
 class ListDevEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentspaginator)
         """
 
+
 class ListEventLogsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listeventlogspaginator)
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         eventName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventLogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listeventlogspaginator)
         """
 
+
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listprojectspaginator)
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         filters: Sequence[ProjectListFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listprojectspaginator)
         """
 
+
 class ListSourceRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositoriespaginator)
     """
 
     def paginate(
-        self, *, spaceName: str, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, spaceName: str, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSourceRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositoriespaginator)
         """
 
+
 class ListSourceRepositoryBranchesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositorybranchespaginator)
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSourceRepositoryBranchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositorybranchespaginator)
         """
 
+
 class ListSpacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSpacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listspacespaginator)
         """
```

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/type_defs.py` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -29,86 +29,89 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessTokenSummaryTypeDef",
     "CreateAccessTokenRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAccessTokenResponseTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
+    "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
+    "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchRequestRequestTypeDef",
+    "CreateSourceRepositoryBranchResponseTypeDef",
     "DeleteAccessTokenRequestRequestTypeDef",
     "DeleteDevEnvironmentRequestRequestTypeDef",
+    "DeleteDevEnvironmentResponseTypeDef",
     "DevEnvironmentAccessDetailsTypeDef",
     "DevEnvironmentRepositorySummaryTypeDef",
     "ExecuteCommandSessionConfigurationTypeDef",
+    "DevEnvironmentSessionSummaryTypeDef",
     "IdeTypeDef",
     "PersistentStorageTypeDef",
     "EmailAddressTypeDef",
     "EventPayloadTypeDef",
     "ProjectInformationTypeDef",
     "UserIdentityTypeDef",
     "FilterTypeDef",
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
+    "GetProjectResponseTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
     "GetSpaceRequestRequestTypeDef",
+    "GetSpaceResponseTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
+    "GetSubscriptionResponseTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
+    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    "ListDevEnvironmentSessionsRequestRequestTypeDef",
+    "ListEventLogsRequestListEventLogsPaginateTypeDef",
     "ListEventLogsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
     "ProjectSummaryTypeDef",
     "ListSourceRepositoriesItemTypeDef",
+    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
+    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
+    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
-    "StopDevEnvironmentRequestRequestTypeDef",
-    "StopDevEnvironmentSessionRequestRequestTypeDef",
-    "CreateAccessTokenResponseTypeDef",
-    "CreateDevEnvironmentResponseTypeDef",
-    "CreateProjectResponseTypeDef",
-    "CreateSourceRepositoryBranchResponseTypeDef",
-    "DeleteDevEnvironmentResponseTypeDef",
-    "GetProjectResponseTypeDef",
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
-    "GetSpaceResponseTypeDef",
-    "GetSubscriptionResponseTypeDef",
-    "ListAccessTokensResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentRequestRequestTypeDef",
     "StopDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
     "StopDevEnvironmentSessionResponseTypeDef",
     "VerifySessionResponseTypeDef",
+    "ListAccessTokensResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
+    "ListDevEnvironmentSessionsResponseTypeDef",
     "DevEnvironmentSummaryTypeDef",
     "GetDevEnvironmentResponseTypeDef",
     "GetUserDetailsResponseTypeDef",
     "EventLogEntryTypeDef",
-    "ListDevEnvironmentsRequestRequestTypeDef",
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
-    "ListEventLogsRequestListEventLogsPaginateTypeDef",
-    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    "ListSpacesRequestListSpacesPaginateTypeDef",
+    "ListDevEnvironmentsRequestRequestTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSourceRepositoriesResponseTypeDef",
     "ListSourceRepositoryBranchesResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "StartDevEnvironmentSessionRequestRequestTypeDef",
@@ -127,50 +130,46 @@
     "_OptionalAccessTokenSummaryTypeDef",
     {
         "expiresTime": datetime,
     },
     total=False,
 )
 
-
 class AccessTokenSummaryTypeDef(
     _RequiredAccessTokenSummaryTypeDef, _OptionalAccessTokenSummaryTypeDef
 ):
     pass
 
-
 _RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessTokenRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAccessTokenRequestRequestTypeDef",
     {
         "expiresTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class CreateAccessTokenRequestRequestTypeDef(
     _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
 ):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAccessTokenResponseTypeDef = TypedDict(
+    "CreateAccessTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "secret": str,
+        "name": str,
+        "expiresTime": datetime,
+        "accessTokenId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IdeConfigurationTypeDef = TypedDict(
     "IdeConfigurationTypeDef",
     {
         "runtime": str,
@@ -196,18 +195,26 @@
     "_OptionalRepositoryInputTypeDef",
     {
         "branchName": str,
     },
     total=False,
 )
 
-
 class RepositoryInputTypeDef(_RequiredRepositoryInputTypeDef, _OptionalRepositoryInputTypeDef):
     pass
 
+CreateDevEnvironmentResponseTypeDef = TypedDict(
+    "CreateDevEnvironmentResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "displayName": str,
     },
@@ -216,20 +223,29 @@
     "_OptionalCreateProjectRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSourceRepositoryBranchRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
@@ -240,21 +256,30 @@
     "_OptionalCreateSourceRepositoryBranchRequestRequestTypeDef",
     {
         "headCommitId": str,
     },
     total=False,
 )
 
-
 class CreateSourceRepositoryBranchRequestRequestTypeDef(
     _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef,
     _OptionalCreateSourceRepositoryBranchRequestRequestTypeDef,
 ):
     pass
 
+CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryBranchResponseTypeDef",
+    {
+        "ref": str,
+        "name": str,
+        "lastUpdatedTime": datetime,
+        "headCommitId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DeleteAccessTokenRequestRequestTypeDef = TypedDict(
     "DeleteAccessTokenRequestRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -264,14 +289,24 @@
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
 )
 
+DeleteDevEnvironmentResponseTypeDef = TypedDict(
+    "DeleteDevEnvironmentResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DevEnvironmentAccessDetailsTypeDef = TypedDict(
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
@@ -286,42 +321,49 @@
     "_OptionalDevEnvironmentRepositorySummaryTypeDef",
     {
         "branchName": str,
     },
     total=False,
 )
 
-
 class DevEnvironmentRepositorySummaryTypeDef(
     _RequiredDevEnvironmentRepositorySummaryTypeDef, _OptionalDevEnvironmentRepositorySummaryTypeDef
 ):
     pass
 
-
 _RequiredExecuteCommandSessionConfigurationTypeDef = TypedDict(
     "_RequiredExecuteCommandSessionConfigurationTypeDef",
     {
         "command": str,
     },
 )
 _OptionalExecuteCommandSessionConfigurationTypeDef = TypedDict(
     "_OptionalExecuteCommandSessionConfigurationTypeDef",
     {
         "arguments": Sequence[str],
     },
     total=False,
 )
 
-
 class ExecuteCommandSessionConfigurationTypeDef(
     _RequiredExecuteCommandSessionConfigurationTypeDef,
     _OptionalExecuteCommandSessionConfigurationTypeDef,
 ):
     pass
 
+DevEnvironmentSessionSummaryTypeDef = TypedDict(
+    "DevEnvironmentSessionSummaryTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "devEnvironmentId": str,
+        "startedTime": datetime,
+        "id": str,
+    },
+)
 
 IdeTypeDef = TypedDict(
     "IdeTypeDef",
     {
         "runtime": str,
         "name": str,
     },
@@ -374,19 +416,17 @@
     {
         "userName": str,
         "awsAccountId": str,
     },
     total=False,
 )
 
-
 class UserIdentityTypeDef(_RequiredUserIdentityTypeDef, _OptionalUserIdentityTypeDef):
     pass
 
-
 _RequiredFilterTypeDef = TypedDict(
     "_RequiredFilterTypeDef",
     {
         "key": str,
         "values": Sequence[str],
     },
 )
@@ -394,19 +434,17 @@
     "_OptionalFilterTypeDef",
     {
         "comparisonOperator": str,
     },
     total=False,
 )
 
-
 class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
     pass
 
-
 GetDevEnvironmentRequestRequestTypeDef = TypedDict(
     "GetDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
@@ -416,65 +454,170 @@
     "GetProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "name": str,
     },
 )
 
+GetProjectResponseTypeDef = TypedDict(
+    "GetProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSourceRepositoryCloneUrlsRequestRequestTypeDef = TypedDict(
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
 )
 
+GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    {
+        "https": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSpaceRequestRequestTypeDef = TypedDict(
     "GetSpaceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
+GetSpaceResponseTypeDef = TypedDict(
+    "GetSpaceResponseTypeDef",
+    {
+        "name": str,
+        "regionName": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSubscriptionRequestRequestTypeDef = TypedDict(
     "GetSubscriptionRequestRequestTypeDef",
     {
         "spaceName": str,
     },
 )
 
+GetSubscriptionResponseTypeDef = TypedDict(
+    "GetSubscriptionResponseTypeDef",
+    {
+        "subscriptionType": str,
+        "awsAccountName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetUserDetailsRequestRequestTypeDef = TypedDict(
     "GetUserDetailsRequestRequestTypeDef",
     {
         "id": str,
         "userName": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAccessTokensRequestRequestTypeDef = TypedDict(
     "ListAccessTokensRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "devEnvironmentId": str,
+    },
+)
+_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
+    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListDevEnvironmentSessionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentSessionsRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "devEnvironmentId": str,
+    },
+)
+_OptionalListDevEnvironmentSessionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentSessionsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListDevEnvironmentSessionsRequestRequestTypeDef(
+    _RequiredListDevEnvironmentSessionsRequestRequestTypeDef,
+    _OptionalListDevEnvironmentSessionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "eventName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEventLogsRequestListEventLogsPaginateTypeDef(
+    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
+    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
+):
+    pass
+
 _RequiredListEventLogsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventLogsRequestRequestTypeDef",
     {
         "spaceName": str,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
@@ -485,21 +628,19 @@
         "eventName": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListEventLogsRequestRequestTypeDef(
     _RequiredListEventLogsRequestRequestTypeDef, _OptionalListEventLogsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredProjectListFilterTypeDef = TypedDict(
     "_RequiredProjectListFilterTypeDef",
     {
         "key": Literal["hasAccessTo"],
         "values": Sequence[str],
     },
 )
@@ -507,21 +648,19 @@
     "_OptionalProjectListFilterTypeDef",
     {
         "comparisonOperator": ComparisonOperatorType,
     },
     total=False,
 )
 
-
 class ProjectListFilterTypeDef(
     _RequiredProjectListFilterTypeDef, _OptionalProjectListFilterTypeDef
 ):
     pass
 
-
 _RequiredProjectSummaryTypeDef = TypedDict(
     "_RequiredProjectSummaryTypeDef",
     {
         "name": str,
     },
 )
 _OptionalProjectSummaryTypeDef = TypedDict(
@@ -529,19 +668,17 @@
     {
         "displayName": str,
         "description": str,
     },
     total=False,
 )
 
-
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
-
 _RequiredListSourceRepositoriesItemTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesItemTypeDef",
     {
         "id": str,
         "name": str,
         "lastUpdatedTime": datetime,
         "createdTime": datetime,
@@ -551,20 +688,39 @@
     "_OptionalListSourceRepositoriesItemTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class ListSourceRepositoriesItemTypeDef(
     _RequiredListSourceRepositoriesItemTypeDef, _OptionalListSourceRepositoriesItemTypeDef
 ):
     pass
 
+_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+    },
+)
+_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
+    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+):
+    pass
 
 _RequiredListSourceRepositoriesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
@@ -574,33 +730,53 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListSourceRepositoriesRequestRequestTypeDef(
     _RequiredListSourceRepositoriesRequestRequestTypeDef,
     _OptionalListSourceRepositoriesRequestRequestTypeDef,
 ):
     pass
 
-
 ListSourceRepositoryBranchesItemTypeDef = TypedDict(
     "ListSourceRepositoryBranchesItemTypeDef",
     {
         "ref": str,
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
     },
     total=False,
 )
 
+_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "sourceRepositoryName": str,
+    },
+)
+_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
+    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+):
+    pass
+
 _RequiredListSourceRepositoryBranchesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoryBranchesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
@@ -610,21 +786,27 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListSourceRepositoryBranchesRequestRequestTypeDef(
     _RequiredListSourceRepositoryBranchesRequestRequestTypeDef,
     _OptionalListSourceRepositoryBranchesRequestRequestTypeDef,
 ):
     pass
 
+ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
+    "ListSpacesRequestListSpacesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListSpacesRequestRequestTypeDef = TypedDict(
     "ListSpacesRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
@@ -642,177 +824,104 @@
     {
         "displayName": str,
         "description": str,
     },
     total=False,
 )
 
-
 class SpaceSummaryTypeDef(_RequiredSpaceSummaryTypeDef, _OptionalSpaceSummaryTypeDef):
     pass
 
-
-StopDevEnvironmentRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentRequestRequestTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-    },
-)
-
-StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentSessionRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "sessionId": str,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-CreateAccessTokenResponseTypeDef = TypedDict(
-    "CreateAccessTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "secret": str,
-        "name": str,
-        "expiresTime": datetime,
-        "accessTokenId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-CreateDevEnvironmentResponseTypeDef = TypedDict(
-    "CreateDevEnvironmentResponseTypeDef",
+StartDevEnvironmentResponseTypeDef = TypedDict(
+    "StartDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
-    "CreateSourceRepositoryBranchResponseTypeDef",
-    {
-        "ref": str,
-        "name": str,
-        "lastUpdatedTime": datetime,
-        "headCommitId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "status": DevEnvironmentStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteDevEnvironmentResponseTypeDef = TypedDict(
-    "DeleteDevEnvironmentResponseTypeDef",
+StopDevEnvironmentRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProjectResponseTypeDef = TypedDict(
-    "GetProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
-    {
-        "https": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSpaceResponseTypeDef = TypedDict(
-    "GetSpaceResponseTypeDef",
-    {
-        "name": str,
-        "regionName": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetSubscriptionResponseTypeDef = TypedDict(
-    "GetSubscriptionResponseTypeDef",
-    {
-        "subscriptionType": str,
-        "awsAccountName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAccessTokensResponseTypeDef = TypedDict(
-    "ListAccessTokensResponseTypeDef",
-    {
-        "items": List[AccessTokenSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartDevEnvironmentResponseTypeDef = TypedDict(
-    "StartDevEnvironmentResponseTypeDef",
+StopDevEnvironmentResponseTypeDef = TypedDict(
+    "StopDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "status": DevEnvironmentStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopDevEnvironmentResponseTypeDef = TypedDict(
-    "StopDevEnvironmentResponseTypeDef",
+StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "status": DevEnvironmentStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "sessionId": str,
     },
 )
 
 StopDevEnvironmentSessionResponseTypeDef = TypedDict(
     "StopDevEnvironmentSessionResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "sessionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VerifySessionResponseTypeDef = TypedDict(
     "VerifySessionResponseTypeDef",
     {
         "identity": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAccessTokensResponseTypeDef = TypedDict(
+    "ListAccessTokensResponseTypeDef",
+    {
+        "items": List[AccessTokenSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -826,22 +935,20 @@
         "ides": Sequence[IdeConfigurationTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
     },
     total=False,
 )
 
-
 class StartDevEnvironmentRequestRequestTypeDef(
     _RequiredStartDevEnvironmentRequestRequestTypeDef,
     _OptionalStartDevEnvironmentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
@@ -854,34 +961,32 @@
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateDevEnvironmentRequestRequestTypeDef(
     _RequiredUpdateDevEnvironmentRequestRequestTypeDef,
     _OptionalUpdateDevEnvironmentRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateDevEnvironmentResponseTypeDef = TypedDict(
     "UpdateDevEnvironmentResponseTypeDef",
     {
         "id": str,
         "spaceName": str,
         "projectName": str,
         "alias": str,
         "ides": List[IdeConfigurationTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -898,31 +1003,29 @@
         "alias": str,
         "ides": Sequence[IdeConfigurationTypeDef],
         "inactivityTimeoutMinutes": int,
     },
     total=False,
 )
 
-
 class CreateDevEnvironmentRequestRequestTypeDef(
     _RequiredCreateDevEnvironmentRequestRequestTypeDef,
     _OptionalCreateDevEnvironmentRequestRequestTypeDef,
 ):
     pass
 
-
 StartDevEnvironmentSessionResponseTypeDef = TypedDict(
     "StartDevEnvironmentSessionResponseTypeDef",
     {
         "accessDetails": DevEnvironmentAccessDetailsTypeDef,
         "sessionId": str,
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDevEnvironmentSessionConfigurationTypeDef = TypedDict(
     "_RequiredDevEnvironmentSessionConfigurationTypeDef",
     {
         "sessionType": DevEnvironmentSessionTypeType,
@@ -932,21 +1035,28 @@
     "_OptionalDevEnvironmentSessionConfigurationTypeDef",
     {
         "executeCommandSessionConfiguration": ExecuteCommandSessionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DevEnvironmentSessionConfigurationTypeDef(
     _RequiredDevEnvironmentSessionConfigurationTypeDef,
     _OptionalDevEnvironmentSessionConfigurationTypeDef,
 ):
     pass
 
+ListDevEnvironmentSessionsResponseTypeDef = TypedDict(
+    "ListDevEnvironmentSessionsResponseTypeDef",
+    {
+        "items": List[DevEnvironmentSessionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredDevEnvironmentSummaryTypeDef = TypedDict(
     "_RequiredDevEnvironmentSummaryTypeDef",
     {
         "id": str,
         "lastUpdatedTime": datetime,
         "creatorId": str,
@@ -965,21 +1075,19 @@
         "statusReason": str,
         "alias": str,
         "ides": List[IdeTypeDef],
     },
     total=False,
 )
 
-
 class DevEnvironmentSummaryTypeDef(
     _RequiredDevEnvironmentSummaryTypeDef, _OptionalDevEnvironmentSummaryTypeDef
 ):
     pass
 
-
 GetDevEnvironmentResponseTypeDef = TypedDict(
     "GetDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "lastUpdatedTime": datetime,
@@ -988,27 +1096,27 @@
         "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
         "alias": str,
         "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserDetailsResponseTypeDef = TypedDict(
     "GetUserDetailsResponseTypeDef",
     {
         "userId": str,
         "userName": str,
         "displayName": str,
         "primaryEmail": EmailAddressTypeDef,
         "version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEventLogEntryTypeDef = TypedDict(
     "_RequiredEventLogEntryTypeDef",
     {
         "id": str,
@@ -1031,179 +1139,83 @@
         "errorCode": str,
         "sourceIpAddress": str,
         "userAgent": str,
     },
     total=False,
 )
 
-
 class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
     pass
 
-
-_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-    },
-)
-_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
-    {
-        "filters": Sequence[FilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class ListDevEnvironmentsRequestRequestTypeDef(
-    _RequiredListDevEnvironmentsRequestRequestTypeDef,
-    _OptionalListDevEnvironmentsRequestRequestTypeDef,
-):
-    pass
-
-
-ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
 _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef(
     _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
 ):
     pass
 
-
-_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "eventName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListEventLogsRequestListEventLogsPaginateTypeDef(
-    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
-    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-    },
-)
-_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
-    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
-        "sourceRepositoryName": str,
     },
 )
-_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "filters": Sequence[FilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-
-class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
-    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+class ListDevEnvironmentsRequestRequestTypeDef(
+    _RequiredListDevEnvironmentsRequestRequestTypeDef,
+    _OptionalListDevEnvironmentsRequestRequestTypeDef,
 ):
     pass
 
-
-ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
-    "ListSpacesRequestListSpacesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
     {
         "spaceName": str,
     },
 )
 _OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
     {
         "filters": Sequence[ProjectListFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListProjectsRequestListProjectsPaginateTypeDef(
     _RequiredListProjectsRequestListProjectsPaginateTypeDef,
     _OptionalListProjectsRequestListProjectsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListProjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectsRequestRequestTypeDef",
     {
         "spaceName": str,
     },
 )
 _OptionalListProjectsRequestRequestTypeDef = TypedDict(
@@ -1212,54 +1224,52 @@
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[ProjectListFilterTypeDef],
     },
     total=False,
 )
 
-
 class ListProjectsRequestRequestTypeDef(
     _RequiredListProjectsRequestRequestTypeDef, _OptionalListProjectsRequestRequestTypeDef
 ):
     pass
 
-
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSourceRepositoriesResponseTypeDef = TypedDict(
     "ListSourceRepositoriesResponseTypeDef",
     {
         "items": List[ListSourceRepositoriesItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSourceRepositoryBranchesResponseTypeDef = TypedDict(
     "ListSourceRepositoryBranchesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ListSourceRepositoryBranchesItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSpacesResponseTypeDef = TypedDict(
     "ListSpacesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[SpaceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1270,19 +1280,19 @@
 )
 
 ListDevEnvironmentsResponseTypeDef = TypedDict(
     "ListDevEnvironmentsResponseTypeDef",
     {
         "items": List[DevEnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventLogsResponseTypeDef = TypedDict(
     "ListEventLogsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[EventLogEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst/type_defs.pyi` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,85 +29,90 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccessTokenSummaryTypeDef",
     "CreateAccessTokenRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAccessTokenResponseTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
+    "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
+    "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchRequestRequestTypeDef",
+    "CreateSourceRepositoryBranchResponseTypeDef",
     "DeleteAccessTokenRequestRequestTypeDef",
     "DeleteDevEnvironmentRequestRequestTypeDef",
+    "DeleteDevEnvironmentResponseTypeDef",
     "DevEnvironmentAccessDetailsTypeDef",
     "DevEnvironmentRepositorySummaryTypeDef",
     "ExecuteCommandSessionConfigurationTypeDef",
+    "DevEnvironmentSessionSummaryTypeDef",
     "IdeTypeDef",
     "PersistentStorageTypeDef",
     "EmailAddressTypeDef",
     "EventPayloadTypeDef",
     "ProjectInformationTypeDef",
     "UserIdentityTypeDef",
     "FilterTypeDef",
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
+    "GetProjectResponseTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
     "GetSpaceRequestRequestTypeDef",
+    "GetSpaceResponseTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
+    "GetSubscriptionResponseTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
+    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    "ListDevEnvironmentSessionsRequestRequestTypeDef",
+    "ListEventLogsRequestListEventLogsPaginateTypeDef",
     "ListEventLogsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
     "ProjectSummaryTypeDef",
     "ListSourceRepositoriesItemTypeDef",
+    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
+    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
+    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
-    "StopDevEnvironmentRequestRequestTypeDef",
-    "StopDevEnvironmentSessionRequestRequestTypeDef",
-    "CreateAccessTokenResponseTypeDef",
-    "CreateDevEnvironmentResponseTypeDef",
-    "CreateProjectResponseTypeDef",
-    "CreateSourceRepositoryBranchResponseTypeDef",
-    "DeleteDevEnvironmentResponseTypeDef",
-    "GetProjectResponseTypeDef",
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
-    "GetSpaceResponseTypeDef",
-    "GetSubscriptionResponseTypeDef",
-    "ListAccessTokensResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentRequestRequestTypeDef",
     "StopDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
     "StopDevEnvironmentSessionResponseTypeDef",
     "VerifySessionResponseTypeDef",
+    "ListAccessTokensResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
+    "ListDevEnvironmentSessionsResponseTypeDef",
     "DevEnvironmentSummaryTypeDef",
     "GetDevEnvironmentResponseTypeDef",
     "GetUserDetailsResponseTypeDef",
     "EventLogEntryTypeDef",
-    "ListDevEnvironmentsRequestRequestTypeDef",
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
-    "ListEventLogsRequestListEventLogsPaginateTypeDef",
-    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    "ListSpacesRequestListSpacesPaginateTypeDef",
+    "ListDevEnvironmentsRequestRequestTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSourceRepositoriesResponseTypeDef",
     "ListSourceRepositoryBranchesResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "StartDevEnvironmentSessionRequestRequestTypeDef",
@@ -126,46 +131,50 @@
     "_OptionalAccessTokenSummaryTypeDef",
     {
         "expiresTime": datetime,
     },
     total=False,
 )
 
+
 class AccessTokenSummaryTypeDef(
     _RequiredAccessTokenSummaryTypeDef, _OptionalAccessTokenSummaryTypeDef
 ):
     pass
 
+
 _RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessTokenRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAccessTokenRequestRequestTypeDef",
     {
         "expiresTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class CreateAccessTokenRequestRequestTypeDef(
     _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+CreateAccessTokenResponseTypeDef = TypedDict(
+    "CreateAccessTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "secret": str,
+        "name": str,
+        "expiresTime": datetime,
+        "accessTokenId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IdeConfigurationTypeDef = TypedDict(
     "IdeConfigurationTypeDef",
     {
         "runtime": str,
@@ -191,17 +200,29 @@
     "_OptionalRepositoryInputTypeDef",
     {
         "branchName": str,
     },
     total=False,
 )
 
+
 class RepositoryInputTypeDef(_RequiredRepositoryInputTypeDef, _OptionalRepositoryInputTypeDef):
     pass
 
+
+CreateDevEnvironmentResponseTypeDef = TypedDict(
+    "CreateDevEnvironmentResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "displayName": str,
     },
 )
@@ -209,19 +230,32 @@
     "_OptionalCreateProjectRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSourceRepositoryBranchRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
         "name": str,
@@ -231,20 +265,33 @@
     "_OptionalCreateSourceRepositoryBranchRequestRequestTypeDef",
     {
         "headCommitId": str,
     },
     total=False,
 )
 
+
 class CreateSourceRepositoryBranchRequestRequestTypeDef(
     _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef,
     _OptionalCreateSourceRepositoryBranchRequestRequestTypeDef,
 ):
     pass
 
+
+CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryBranchResponseTypeDef",
+    {
+        "ref": str,
+        "name": str,
+        "lastUpdatedTime": datetime,
+        "headCommitId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteAccessTokenRequestRequestTypeDef = TypedDict(
     "DeleteAccessTokenRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -253,14 +300,24 @@
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
 )
 
+DeleteDevEnvironmentResponseTypeDef = TypedDict(
+    "DeleteDevEnvironmentResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DevEnvironmentAccessDetailsTypeDef = TypedDict(
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
@@ -275,39 +332,54 @@
     "_OptionalDevEnvironmentRepositorySummaryTypeDef",
     {
         "branchName": str,
     },
     total=False,
 )
 
+
 class DevEnvironmentRepositorySummaryTypeDef(
     _RequiredDevEnvironmentRepositorySummaryTypeDef, _OptionalDevEnvironmentRepositorySummaryTypeDef
 ):
     pass
 
+
 _RequiredExecuteCommandSessionConfigurationTypeDef = TypedDict(
     "_RequiredExecuteCommandSessionConfigurationTypeDef",
     {
         "command": str,
     },
 )
 _OptionalExecuteCommandSessionConfigurationTypeDef = TypedDict(
     "_OptionalExecuteCommandSessionConfigurationTypeDef",
     {
         "arguments": Sequence[str],
     },
     total=False,
 )
 
+
 class ExecuteCommandSessionConfigurationTypeDef(
     _RequiredExecuteCommandSessionConfigurationTypeDef,
     _OptionalExecuteCommandSessionConfigurationTypeDef,
 ):
     pass
 
+
+DevEnvironmentSessionSummaryTypeDef = TypedDict(
+    "DevEnvironmentSessionSummaryTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "devEnvironmentId": str,
+        "startedTime": datetime,
+        "id": str,
+    },
+)
+
 IdeTypeDef = TypedDict(
     "IdeTypeDef",
     {
         "runtime": str,
         "name": str,
     },
     total=False,
@@ -359,17 +431,19 @@
     {
         "userName": str,
         "awsAccountId": str,
     },
     total=False,
 )
 
+
 class UserIdentityTypeDef(_RequiredUserIdentityTypeDef, _OptionalUserIdentityTypeDef):
     pass
 
+
 _RequiredFilterTypeDef = TypedDict(
     "_RequiredFilterTypeDef",
     {
         "key": str,
         "values": Sequence[str],
     },
 )
@@ -377,17 +451,19 @@
     "_OptionalFilterTypeDef",
     {
         "comparisonOperator": str,
     },
     total=False,
 )
 
+
 class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
     pass
 
+
 GetDevEnvironmentRequestRequestTypeDef = TypedDict(
     "GetDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
@@ -397,65 +473,176 @@
     "GetProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "name": str,
     },
 )
 
+GetProjectResponseTypeDef = TypedDict(
+    "GetProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSourceRepositoryCloneUrlsRequestRequestTypeDef = TypedDict(
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
 )
 
+GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    {
+        "https": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSpaceRequestRequestTypeDef = TypedDict(
     "GetSpaceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
+GetSpaceResponseTypeDef = TypedDict(
+    "GetSpaceResponseTypeDef",
+    {
+        "name": str,
+        "regionName": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSubscriptionRequestRequestTypeDef = TypedDict(
     "GetSubscriptionRequestRequestTypeDef",
     {
         "spaceName": str,
     },
 )
 
+GetSubscriptionResponseTypeDef = TypedDict(
+    "GetSubscriptionResponseTypeDef",
+    {
+        "subscriptionType": str,
+        "awsAccountName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetUserDetailsRequestRequestTypeDef = TypedDict(
     "GetUserDetailsRequestRequestTypeDef",
     {
         "id": str,
         "userName": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAccessTokensRequestRequestTypeDef = TypedDict(
     "ListAccessTokensRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "devEnvironmentId": str,
+    },
+)
+_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
+    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDevEnvironmentSessionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentSessionsRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "devEnvironmentId": str,
+    },
+)
+_OptionalListDevEnvironmentSessionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentSessionsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListDevEnvironmentSessionsRequestRequestTypeDef(
+    _RequiredListDevEnvironmentSessionsRequestRequestTypeDef,
+    _OptionalListDevEnvironmentSessionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "eventName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEventLogsRequestListEventLogsPaginateTypeDef(
+    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
+    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEventLogsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventLogsRequestRequestTypeDef",
     {
         "spaceName": str,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
@@ -466,19 +653,21 @@
         "eventName": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListEventLogsRequestRequestTypeDef(
     _RequiredListEventLogsRequestRequestTypeDef, _OptionalListEventLogsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredProjectListFilterTypeDef = TypedDict(
     "_RequiredProjectListFilterTypeDef",
     {
         "key": Literal["hasAccessTo"],
         "values": Sequence[str],
     },
 )
@@ -486,19 +675,21 @@
     "_OptionalProjectListFilterTypeDef",
     {
         "comparisonOperator": ComparisonOperatorType,
     },
     total=False,
 )
 
+
 class ProjectListFilterTypeDef(
     _RequiredProjectListFilterTypeDef, _OptionalProjectListFilterTypeDef
 ):
     pass
 
+
 _RequiredProjectSummaryTypeDef = TypedDict(
     "_RequiredProjectSummaryTypeDef",
     {
         "name": str,
     },
 )
 _OptionalProjectSummaryTypeDef = TypedDict(
@@ -506,17 +697,19 @@
     {
         "displayName": str,
         "description": str,
     },
     total=False,
 )
 
+
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
+
 _RequiredListSourceRepositoriesItemTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesItemTypeDef",
     {
         "id": str,
         "name": str,
         "lastUpdatedTime": datetime,
         "createdTime": datetime,
@@ -526,19 +719,44 @@
     "_OptionalListSourceRepositoriesItemTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class ListSourceRepositoriesItemTypeDef(
     _RequiredListSourceRepositoriesItemTypeDef, _OptionalListSourceRepositoriesItemTypeDef
 ):
     pass
 
+
+_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+    },
+)
+_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
+    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSourceRepositoriesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
@@ -547,31 +765,57 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListSourceRepositoriesRequestRequestTypeDef(
     _RequiredListSourceRepositoriesRequestRequestTypeDef,
     _OptionalListSourceRepositoriesRequestRequestTypeDef,
 ):
     pass
 
+
 ListSourceRepositoryBranchesItemTypeDef = TypedDict(
     "ListSourceRepositoryBranchesItemTypeDef",
     {
         "ref": str,
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
     },
     total=False,
 )
 
+_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "sourceRepositoryName": str,
+    },
+)
+_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
+    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSourceRepositoryBranchesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoryBranchesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
@@ -581,20 +825,30 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListSourceRepositoryBranchesRequestRequestTypeDef(
     _RequiredListSourceRepositoryBranchesRequestRequestTypeDef,
     _OptionalListSourceRepositoryBranchesRequestRequestTypeDef,
 ):
     pass
 
+
+ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
+    "ListSpacesRequestListSpacesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSpacesRequestRequestTypeDef = TypedDict(
     "ListSpacesRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -611,175 +865,106 @@
     {
         "displayName": str,
         "description": str,
     },
     total=False,
 )
 
+
 class SpaceSummaryTypeDef(_RequiredSpaceSummaryTypeDef, _OptionalSpaceSummaryTypeDef):
     pass
 
-StopDevEnvironmentRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentRequestRequestTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-    },
-)
 
-StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentSessionRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "sessionId": str,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-CreateAccessTokenResponseTypeDef = TypedDict(
-    "CreateAccessTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "secret": str,
-        "name": str,
-        "expiresTime": datetime,
-        "accessTokenId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-CreateDevEnvironmentResponseTypeDef = TypedDict(
-    "CreateDevEnvironmentResponseTypeDef",
+StartDevEnvironmentResponseTypeDef = TypedDict(
+    "StartDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
-    "CreateSourceRepositoryBranchResponseTypeDef",
-    {
-        "ref": str,
-        "name": str,
-        "lastUpdatedTime": datetime,
-        "headCommitId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "status": DevEnvironmentStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteDevEnvironmentResponseTypeDef = TypedDict(
-    "DeleteDevEnvironmentResponseTypeDef",
+StopDevEnvironmentRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProjectResponseTypeDef = TypedDict(
-    "GetProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
-    {
-        "https": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSpaceResponseTypeDef = TypedDict(
-    "GetSpaceResponseTypeDef",
-    {
-        "name": str,
-        "regionName": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSubscriptionResponseTypeDef = TypedDict(
-    "GetSubscriptionResponseTypeDef",
-    {
-        "subscriptionType": str,
-        "awsAccountName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAccessTokensResponseTypeDef = TypedDict(
-    "ListAccessTokensResponseTypeDef",
-    {
-        "items": List[AccessTokenSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDevEnvironmentResponseTypeDef = TypedDict(
-    "StartDevEnvironmentResponseTypeDef",
+StopDevEnvironmentResponseTypeDef = TypedDict(
+    "StopDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "status": DevEnvironmentStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopDevEnvironmentResponseTypeDef = TypedDict(
-    "StopDevEnvironmentResponseTypeDef",
+StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "status": DevEnvironmentStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "sessionId": str,
     },
 )
 
 StopDevEnvironmentSessionResponseTypeDef = TypedDict(
     "StopDevEnvironmentSessionResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "sessionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VerifySessionResponseTypeDef = TypedDict(
     "VerifySessionResponseTypeDef",
     {
         "identity": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAccessTokensResponseTypeDef = TypedDict(
+    "ListAccessTokensResponseTypeDef",
+    {
+        "items": List[AccessTokenSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -793,20 +978,22 @@
         "ides": Sequence[IdeConfigurationTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
     },
     total=False,
 )
 
+
 class StartDevEnvironmentRequestRequestTypeDef(
     _RequiredStartDevEnvironmentRequestRequestTypeDef,
     _OptionalStartDevEnvironmentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
@@ -819,32 +1006,34 @@
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateDevEnvironmentRequestRequestTypeDef(
     _RequiredUpdateDevEnvironmentRequestRequestTypeDef,
     _OptionalUpdateDevEnvironmentRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateDevEnvironmentResponseTypeDef = TypedDict(
     "UpdateDevEnvironmentResponseTypeDef",
     {
         "id": str,
         "spaceName": str,
         "projectName": str,
         "alias": str,
         "ides": List[IdeConfigurationTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -861,29 +1050,31 @@
         "alias": str,
         "ides": Sequence[IdeConfigurationTypeDef],
         "inactivityTimeoutMinutes": int,
     },
     total=False,
 )
 
+
 class CreateDevEnvironmentRequestRequestTypeDef(
     _RequiredCreateDevEnvironmentRequestRequestTypeDef,
     _OptionalCreateDevEnvironmentRequestRequestTypeDef,
 ):
     pass
 
+
 StartDevEnvironmentSessionResponseTypeDef = TypedDict(
     "StartDevEnvironmentSessionResponseTypeDef",
     {
         "accessDetails": DevEnvironmentAccessDetailsTypeDef,
         "sessionId": str,
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDevEnvironmentSessionConfigurationTypeDef = TypedDict(
     "_RequiredDevEnvironmentSessionConfigurationTypeDef",
     {
         "sessionType": DevEnvironmentSessionTypeType,
@@ -893,20 +1084,31 @@
     "_OptionalDevEnvironmentSessionConfigurationTypeDef",
     {
         "executeCommandSessionConfiguration": ExecuteCommandSessionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DevEnvironmentSessionConfigurationTypeDef(
     _RequiredDevEnvironmentSessionConfigurationTypeDef,
     _OptionalDevEnvironmentSessionConfigurationTypeDef,
 ):
     pass
 
+
+ListDevEnvironmentSessionsResponseTypeDef = TypedDict(
+    "ListDevEnvironmentSessionsResponseTypeDef",
+    {
+        "items": List[DevEnvironmentSessionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDevEnvironmentSummaryTypeDef = TypedDict(
     "_RequiredDevEnvironmentSummaryTypeDef",
     {
         "id": str,
         "lastUpdatedTime": datetime,
         "creatorId": str,
         "status": DevEnvironmentStatusType,
@@ -924,19 +1126,21 @@
         "statusReason": str,
         "alias": str,
         "ides": List[IdeTypeDef],
     },
     total=False,
 )
 
+
 class DevEnvironmentSummaryTypeDef(
     _RequiredDevEnvironmentSummaryTypeDef, _OptionalDevEnvironmentSummaryTypeDef
 ):
     pass
 
+
 GetDevEnvironmentResponseTypeDef = TypedDict(
     "GetDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "lastUpdatedTime": datetime,
@@ -945,27 +1149,27 @@
         "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
         "alias": str,
         "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserDetailsResponseTypeDef = TypedDict(
     "GetUserDetailsResponseTypeDef",
     {
         "userId": str,
         "userName": str,
         "displayName": str,
         "primaryEmail": EmailAddressTypeDef,
         "version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEventLogEntryTypeDef = TypedDict(
     "_RequiredEventLogEntryTypeDef",
     {
         "id": str,
@@ -988,165 +1192,91 @@
         "errorCode": str,
         "sourceIpAddress": str,
         "userAgent": str,
     },
     total=False,
 )
 
-class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
-    pass
 
-_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-    },
-)
-_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
-    {
-        "filters": Sequence[FilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class ListDevEnvironmentsRequestRequestTypeDef(
-    _RequiredListDevEnvironmentsRequestRequestTypeDef,
-    _OptionalListDevEnvironmentsRequestRequestTypeDef,
-):
+class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
     pass
 
-ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
 _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef(
     _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
 ):
     pass
 
-_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "eventName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEventLogsRequestListEventLogsPaginateTypeDef(
-    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
-    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
-):
-    pass
 
-_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
+_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
-_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
+_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "filters": Sequence[FilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
-    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-):
-    pass
-
-_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "sourceRepositoryName": str,
-    },
-)
-_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
-class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
-    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+class ListDevEnvironmentsRequestRequestTypeDef(
+    _RequiredListDevEnvironmentsRequestRequestTypeDef,
+    _OptionalListDevEnvironmentsRequestRequestTypeDef,
 ):
     pass
 
-ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
-    "ListSpacesRequestListSpacesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 _RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
     {
         "spaceName": str,
     },
 )
 _OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
     {
         "filters": Sequence[ProjectListFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListProjectsRequestListProjectsPaginateTypeDef(
     _RequiredListProjectsRequestListProjectsPaginateTypeDef,
     _OptionalListProjectsRequestListProjectsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListProjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectsRequestRequestTypeDef",
     {
         "spaceName": str,
     },
 )
 _OptionalListProjectsRequestRequestTypeDef = TypedDict(
@@ -1155,52 +1285,54 @@
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[ProjectListFilterTypeDef],
     },
     total=False,
 )
 
+
 class ListProjectsRequestRequestTypeDef(
     _RequiredListProjectsRequestRequestTypeDef, _OptionalListProjectsRequestRequestTypeDef
 ):
     pass
 
+
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSourceRepositoriesResponseTypeDef = TypedDict(
     "ListSourceRepositoriesResponseTypeDef",
     {
         "items": List[ListSourceRepositoriesItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSourceRepositoryBranchesResponseTypeDef = TypedDict(
     "ListSourceRepositoryBranchesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ListSourceRepositoryBranchesItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSpacesResponseTypeDef = TypedDict(
     "ListSpacesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[SpaceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1211,19 +1343,19 @@
 )
 
 ListDevEnvironmentsResponseTypeDef = TypedDict(
     "ListDevEnvironmentsResponseTypeDef",
     {
         "items": List[DevEnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventLogsResponseTypeDef = TypedDict(
     "ListEventLogsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[EventLogEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/PKG-INFO` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecatalyst
-Version: 1.26.82
-Summary: Type annotations for boto3.CodeCatalyst 1.26.82 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeCatalyst 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-codecatalyst"></a>
 
 # mypy-boto3-codecatalyst
 
 [![PyPI - mypy-boto3-codecatalyst](https://img.shields.io/pypi/v/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.26.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,27 +281,31 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_codecatalyst import CodeCatalystClient
 from mypy_boto3_codecatalyst.paginator import (
     ListAccessTokensPaginator,
+    ListDevEnvironmentSessionsPaginator,
     ListDevEnvironmentsPaginator,
     ListEventLogsPaginator,
     ListProjectsPaginator,
     ListSourceRepositoriesPaginator,
     ListSourceRepositoryBranchesPaginator,
     ListSpacesPaginator,
 )
 
 client: CodeCatalystClient = Session().client("codecatalyst")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_access_tokens_paginator: ListAccessTokensPaginator = client.get_paginator("list_access_tokens")
+list_dev_environment_sessions_paginator: ListDevEnvironmentSessionsPaginator = client.get_paginator(
+    "list_dev_environment_sessions"
+)
 list_dev_environments_paginator: ListDevEnvironmentsPaginator = client.get_paginator(
     "list_dev_environments"
 )
 list_event_logs_paginator: ListEventLogsPaginator = client.get_paginator("list_event_logs")
 list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
 list_source_repositories_paginator: ListSourceRepositoriesPaginator = client.get_paginator(
     "list_source_repositories"
@@ -323,14 +327,15 @@
 from mypy_boto3_codecatalyst.literals import (
     ComparisonOperatorType,
     DevEnvironmentSessionTypeType,
     DevEnvironmentStatusType,
     FilterKeyType,
     InstanceTypeType,
     ListAccessTokensPaginatorName,
+    ListDevEnvironmentSessionsPaginatorName,
     ListDevEnvironmentsPaginatorName,
     ListEventLogsPaginatorName,
     ListProjectsPaginatorName,
     ListSourceRepositoriesPaginatorName,
     ListSourceRepositoryBranchesPaginatorName,
     ListSpacesPaginatorName,
     OperationTypeType,
@@ -353,82 +358,86 @@
 `mypy_boto3_codecatalyst.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
     CreateAccessTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAccessTokenResponseTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
+    CreateDevEnvironmentResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
+    CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
+    CreateSourceRepositoryBranchResponseTypeDef,
     DeleteAccessTokenRequestRequestTypeDef,
     DeleteDevEnvironmentRequestRequestTypeDef,
+    DeleteDevEnvironmentResponseTypeDef,
     DevEnvironmentAccessDetailsTypeDef,
     DevEnvironmentRepositorySummaryTypeDef,
     ExecuteCommandSessionConfigurationTypeDef,
+    DevEnvironmentSessionSummaryTypeDef,
     IdeTypeDef,
     PersistentStorageTypeDef,
     EmailAddressTypeDef,
     EventPayloadTypeDef,
     ProjectInformationTypeDef,
     UserIdentityTypeDef,
     FilterTypeDef,
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
+    GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
+    GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSpaceRequestRequestTypeDef,
+    GetSpaceResponseTypeDef,
     GetSubscriptionRequestRequestTypeDef,
+    GetSubscriptionResponseTypeDef,
     GetUserDetailsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
     ListAccessTokensRequestRequestTypeDef,
+    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    ListDevEnvironmentSessionsRequestRequestTypeDef,
+    ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
+    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
+    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
+    ListSpacesRequestListSpacesPaginateTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
-    StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentSessionRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
-    GetProjectResponseTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
-    GetSpaceResponseTypeDef,
-    GetSubscriptionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentRequestRequestTypeDef,
     StopDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentSessionRequestRequestTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     VerifySessionResponseTypeDef,
+    ListAccessTokensResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
+    ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestRequestTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
     ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
+    ListDevEnvironmentsRequestRequestTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
@@ -444,42 +453,42 @@
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

### Comparing `mypy-boto3-codecatalyst-1.26.82/mypy_boto3_codecatalyst.egg-info/SOURCES.txt` & `mypy-boto3-codecatalyst-1.27.0/mypy_boto3_codecatalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.26.82/setup.py` & `mypy-boto3-codecatalyst-1.27.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-codecatalyst.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codecatalyst",
-    version="1.26.82",
+    version="1.27.0",
     packages=["mypy_boto3_codecatalyst"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeCatalyst 1.26.82 service generated with mypy-boto3-builder"
-        " 7.12.5"
+        "Type annotations for boto3.CodeCatalyst 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/",
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


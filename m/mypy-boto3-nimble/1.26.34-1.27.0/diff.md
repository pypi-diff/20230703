# Comparing `tmp/mypy-boto3-nimble-1.26.34.tar.gz` & `tmp/mypy-boto3-nimble-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-nimble-1.26.34.tar", last modified: Tue Dec 20 20:26:41 2022, max compression
+gzip compressed data, was "mypy-boto3-nimble-1.27.0.tar", last modified: Mon Jul  3 19:51:10 2023, max compression
```

## Comparing `mypy-boto3-nimble-1.26.34.tar` & `mypy-boto3-nimble-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:41.030595 mypy-boto3-nimble-1.26.34/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-20 20:26:05.000000 mypy-boto3-nimble-1.26.34/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24516 2022-12-20 20:26:41.030595 mypy-boto3-nimble-1.26.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23027 2022-12-20 20:26:05.000000 mypy-boto3-nimble-1.26.34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:41.030595 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2022-12-20 20:26:05.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2022-12-20 20:26:05.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2022-12-20 20:26:05.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44528 2022-12-20 20:26:06.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    44450 2022-12-20 20:26:05.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17618 2022-12-20 20:26:06.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17616 2022-12-20 20:26:06.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2022-12-20 20:26:06.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2022-12-20 20:26:06.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:05.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    70000 2022-12-20 20:26:08.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69883 2022-12-20 20:26:07.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-20 20:26:05.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2022-12-20 20:26:06.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2022-12-20 20:26:06.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:41.030595 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24516 2022-12-20 20:26:40.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2022-12-20 20:26:40.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 20:26:40.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 20:26:40.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-20 20:26:40.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 20:26:40.000000 mypy-boto3-nimble-1.26.34/mypy_boto3_nimble.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 20:26:41.030595 mypy-boto3-nimble-1.26.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2022-12-20 20:26:05.000000 mypy-boto3-nimble-1.26.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.927730 mypy-boto3-nimble-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:49.000000 mypy-boto3-nimble-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24491 2023-07-03 19:51:10.927730 mypy-boto3-nimble-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-07-03 19:42:49.000000 mypy-boto3-nimble-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.923730 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-03 19:42:49.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-03 19:42:49.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:42:49.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44528 2023-07-03 19:42:50.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44450 2023-07-03 19:42:50.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-07-03 19:42:50.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-07-03 19:42:50.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-07-03 19:42:50.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-07-03 19:42:50.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:49.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70106 2023-07-03 19:42:53.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69989 2023-07-03 19:42:52.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:49.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-07-03 19:42:50.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-07-03 19:42:50.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.927730 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24491 2023-07-03 19:51:10.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:51:10.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:10.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:51:10.000000 mypy-boto3-nimble-1.27.0/mypy_boto3_nimble.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:10.927730 mypy-boto3-nimble-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-03 19:42:49.000000 mypy-boto3-nimble-1.27.0/setup.py
```

### Comparing `mypy-boto3-nimble-1.26.34/LICENSE` & `mypy-boto3-nimble-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-nimble-1.26.34/PKG-INFO` & `mypy-boto3-nimble-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-nimble
-Version: 1.26.34
-Summary: Type annotations for boto3.NimbleStudio 1.26.34 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.NimbleStudio 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-nimble"></a>
 
 # mypy-boto3-nimble
 
 [![PyPI - mypy-boto3-nimble](https://img.shields.io/pypi/v/mypy-boto3-nimble.svg?color=blue)](https://pypi.org/project/mypy-boto3-nimble)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-nimble.svg?color=blue)](https://pypi.org/project/mypy-boto3-nimble)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-nimble?color=blue)](https://pypistats.org/packages/mypy-boto3-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NimbleStudio 1.26.34](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[boto3.NimbleStudio 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
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
 [mypy-boto3-nimble docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/).
 
 See how it helps to find and fix potential bugs:
 
@@ -468,15 +468,14 @@
 `mypy_boto3_nimble.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_nimble.type_defs import (
     AcceptEulasRequestRequestTypeDef,
     EulaAcceptanceTypeDef,
-    ResponseMetadataTypeDef,
     ActiveDirectoryComputerAttributeTypeDef,
     ComputeFarmConfigurationTypeDef,
     CreateStreamingImageRequestRequestTypeDef,
     CreateStreamingSessionRequestRequestTypeDef,
     CreateStreamingSessionStreamRequestRequestTypeDef,
     StreamingSessionStreamTypeDef,
     ScriptParameterKeyValueTypeDef,
@@ -506,28 +505,40 @@
     GetStudioComponentRequestRequestTypeDef,
     GetStudioMemberRequestRequestTypeDef,
     StudioMembershipTypeDef,
     GetStudioRequestRequestTypeDef,
     LaunchProfileInitializationScriptTypeDef,
     ValidationResultTypeDef,
     LicenseServiceConfigurationTypeDef,
-    PaginatorConfigTypeDef,
+    ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
     ListEulaAcceptancesRequestRequestTypeDef,
+    ListEulasRequestListEulasPaginateTypeDef,
     ListEulasRequestRequestTypeDef,
+    ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
     ListLaunchProfileMembersRequestRequestTypeDef,
+    ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
     ListLaunchProfilesRequestRequestTypeDef,
+    ListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
     ListStreamingImagesRequestRequestTypeDef,
+    ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
     ListStreamingSessionBackupsRequestRequestTypeDef,
+    ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
     ListStreamingSessionsRequestRequestTypeDef,
+    ListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
     ListStudioComponentsRequestRequestTypeDef,
+    ListStudioMembersRequestListStudioMembersPaginateTypeDef,
     ListStudioMembersRequestRequestTypeDef,
+    ListStudiosRequestListStudiosPaginateTypeDef,
     ListStudiosRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SharedFileSystemConfigurationTypeDef,
     StartStreamingSessionRequestRequestTypeDef,
     StartStudioSSOConfigurationRepairRequestRequestTypeDef,
     StopStreamingSessionRequestRequestTypeDef,
     StreamConfigurationSessionBackupTypeDef,
     VolumeConfigurationTypeDef,
     StreamingSessionStorageRootTypeDef,
@@ -535,15 +546,14 @@
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLaunchProfileMemberRequestRequestTypeDef,
     UpdateStreamingImageRequestRequestTypeDef,
     UpdateStudioRequestRequestTypeDef,
     AcceptEulasResponseTypeDef,
     ListEulaAcceptancesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ActiveDirectoryConfigurationTypeDef,
     LaunchProfileInitializationActiveDirectoryTypeDef,
     CreateStreamingSessionStreamResponseTypeDef,
     GetStreamingSessionStreamResponseTypeDef,
     CreateStudioRequestRequestTypeDef,
     StudioTypeDef,
     GetEulaResponseTypeDef,
@@ -563,24 +573,14 @@
     GetStudioComponentRequestStudioComponentReadyWaitTypeDef,
     GetStudioRequestStudioDeletedWaitTypeDef,
     GetStudioRequestStudioReadyWaitTypeDef,
     GetStreamingSessionBackupResponseTypeDef,
     ListStreamingSessionBackupsResponseTypeDef,
     GetStudioMemberResponseTypeDef,
     ListStudioMembersResponseTypeDef,
-    ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
-    ListEulasRequestListEulasPaginateTypeDef,
-    ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
-    ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
-    ListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
-    ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
-    ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
-    ListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
-    ListStudioMembersRequestListStudioMembersPaginateTypeDef,
-    ListStudiosRequestListStudiosPaginateTypeDef,
     PutLaunchProfileMembersRequestRequestTypeDef,
     PutStudioMembersRequestRequestTypeDef,
     StreamingSessionTypeDef,
     StreamConfigurationSessionStorageTypeDef,
     StreamingImageTypeDef,
     StudioComponentConfigurationTypeDef,
     LaunchProfileInitializationTypeDef,
@@ -631,42 +631,42 @@
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

### Comparing `mypy-boto3-nimble-1.26.34/README.md` & `mypy-boto3-nimble-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-nimble"></a>
 
 # mypy-boto3-nimble
 
 [![PyPI - mypy-boto3-nimble](https://img.shields.io/pypi/v/mypy-boto3-nimble.svg?color=blue)](https://pypi.org/project/mypy-boto3-nimble)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-nimble.svg?color=blue)](https://pypi.org/project/mypy-boto3-nimble)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-nimble?color=blue)](https://pypistats.org/packages/mypy-boto3-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NimbleStudio 1.26.34](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[boto3.NimbleStudio 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
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
 [mypy-boto3-nimble docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/).
 
 See how it helps to find and fix potential bugs:
 
@@ -436,15 +436,14 @@
 `mypy_boto3_nimble.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_nimble.type_defs import (
     AcceptEulasRequestRequestTypeDef,
     EulaAcceptanceTypeDef,
-    ResponseMetadataTypeDef,
     ActiveDirectoryComputerAttributeTypeDef,
     ComputeFarmConfigurationTypeDef,
     CreateStreamingImageRequestRequestTypeDef,
     CreateStreamingSessionRequestRequestTypeDef,
     CreateStreamingSessionStreamRequestRequestTypeDef,
     StreamingSessionStreamTypeDef,
     ScriptParameterKeyValueTypeDef,
@@ -474,28 +473,40 @@
     GetStudioComponentRequestRequestTypeDef,
     GetStudioMemberRequestRequestTypeDef,
     StudioMembershipTypeDef,
     GetStudioRequestRequestTypeDef,
     LaunchProfileInitializationScriptTypeDef,
     ValidationResultTypeDef,
     LicenseServiceConfigurationTypeDef,
-    PaginatorConfigTypeDef,
+    ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
     ListEulaAcceptancesRequestRequestTypeDef,
+    ListEulasRequestListEulasPaginateTypeDef,
     ListEulasRequestRequestTypeDef,
+    ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
     ListLaunchProfileMembersRequestRequestTypeDef,
+    ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
     ListLaunchProfilesRequestRequestTypeDef,
+    ListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
     ListStreamingImagesRequestRequestTypeDef,
+    ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
     ListStreamingSessionBackupsRequestRequestTypeDef,
+    ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
     ListStreamingSessionsRequestRequestTypeDef,
+    ListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
     ListStudioComponentsRequestRequestTypeDef,
+    ListStudioMembersRequestListStudioMembersPaginateTypeDef,
     ListStudioMembersRequestRequestTypeDef,
+    ListStudiosRequestListStudiosPaginateTypeDef,
     ListStudiosRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SharedFileSystemConfigurationTypeDef,
     StartStreamingSessionRequestRequestTypeDef,
     StartStudioSSOConfigurationRepairRequestRequestTypeDef,
     StopStreamingSessionRequestRequestTypeDef,
     StreamConfigurationSessionBackupTypeDef,
     VolumeConfigurationTypeDef,
     StreamingSessionStorageRootTypeDef,
@@ -503,15 +514,14 @@
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLaunchProfileMemberRequestRequestTypeDef,
     UpdateStreamingImageRequestRequestTypeDef,
     UpdateStudioRequestRequestTypeDef,
     AcceptEulasResponseTypeDef,
     ListEulaAcceptancesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ActiveDirectoryConfigurationTypeDef,
     LaunchProfileInitializationActiveDirectoryTypeDef,
     CreateStreamingSessionStreamResponseTypeDef,
     GetStreamingSessionStreamResponseTypeDef,
     CreateStudioRequestRequestTypeDef,
     StudioTypeDef,
     GetEulaResponseTypeDef,
@@ -531,24 +541,14 @@
     GetStudioComponentRequestStudioComponentReadyWaitTypeDef,
     GetStudioRequestStudioDeletedWaitTypeDef,
     GetStudioRequestStudioReadyWaitTypeDef,
     GetStreamingSessionBackupResponseTypeDef,
     ListStreamingSessionBackupsResponseTypeDef,
     GetStudioMemberResponseTypeDef,
     ListStudioMembersResponseTypeDef,
-    ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
-    ListEulasRequestListEulasPaginateTypeDef,
-    ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
-    ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
-    ListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
-    ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
-    ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
-    ListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
-    ListStudioMembersRequestListStudioMembersPaginateTypeDef,
-    ListStudiosRequestListStudiosPaginateTypeDef,
     PutLaunchProfileMembersRequestRequestTypeDef,
     PutStudioMembersRequestRequestTypeDef,
     StreamingSessionTypeDef,
     StreamConfigurationSessionStorageTypeDef,
     StreamingImageTypeDef,
     StudioComponentConfigurationTypeDef,
     LaunchProfileInitializationTypeDef,
@@ -599,42 +599,42 @@
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

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/__init__.py` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/__init__.pyi` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/__main__.py` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.NimbleStudio 1.26.34\nVersion:         1.26.34\nBuilder"
-        " version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.NimbleStudio 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.34")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/client.py` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/client.pyi` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/literals.py` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,15 @@
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
@@ -343,31 +344,34 @@
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
@@ -446,14 +450,15 @@
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
@@ -464,18 +469,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -485,14 +492,15 @@
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
@@ -505,14 +513,15 @@
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
@@ -531,16 +540,19 @@
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
@@ -620,18 +632,21 @@
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
@@ -676,9 +691,19 @@
     "streaming_session_stream_ready",
     "studio_component_deleted",
     "studio_component_ready",
     "studio_deleted",
     "studio_ready",
 ]
 RegionName = Literal[
-    "ap-northeast-1", "ap-southeast-2", "ca-central-1", "eu-west-2", "us-east-1", "us-west-2"
+    "ap-northeast-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-north-1",
+    "eu-west-1",
+    "eu-west-2",
+    "us-east-1",
+    "us-east-2",
+    "us-west-2",
 ]
```

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/literals.pyi` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -313,14 +313,15 @@
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
@@ -341,31 +342,34 @@
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
@@ -444,14 +448,15 @@
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
@@ -462,18 +467,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -483,14 +490,15 @@
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
@@ -503,14 +511,15 @@
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
@@ -529,16 +538,19 @@
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
@@ -618,18 +630,21 @@
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
@@ -674,9 +689,19 @@
     "streaming_session_stream_ready",
     "studio_component_deleted",
     "studio_component_ready",
     "studio_deleted",
     "studio_ready",
 ]
 RegionName = Literal[
-    "ap-northeast-1", "ap-southeast-2", "ca-central-1", "eu-west-2", "us-east-1", "us-west-2"
+    "ap-northeast-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-north-1",
+    "eu-west-1",
+    "eu-west-2",
+    "us-east-1",
+    "us-east-2",
+    "us-west-2",
 ]
```

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/paginator.py` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,45 +87,49 @@
     """
 
     def paginate(
         self,
         *,
         studioId: str,
         eulaIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEulaAcceptancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulaAcceptances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#listeulaacceptancespaginator)
         """
 
 
 class ListEulasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#listeulaspaginator)
     """
 
     def paginate(
-        self, *, eulaIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, eulaIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEulasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#listeulaspaginator)
         """
 
 
 class ListLaunchProfileMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfileMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#listlaunchprofilememberspaginator)
     """
 
     def paginate(
-        self, *, launchProfileId: str, studioId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        launchProfileId: str,
+        studioId: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLaunchProfileMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfileMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#listlaunchprofilememberspaginator)
         """
 
 
@@ -137,45 +141,45 @@
 
     def paginate(
         self,
         *,
         studioId: str,
         principalId: str = ...,
         states: Sequence[LaunchProfileStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLaunchProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#listlaunchprofilespaginator)
         """
 
 
 class ListStreamingImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststreamingimagespaginator)
     """
 
     def paginate(
-        self, *, studioId: str, owner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, studioId: str, owner: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamingImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststreamingimagespaginator)
         """
 
 
 class ListStreamingSessionBackupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessionBackups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststreamingsessionbackupspaginator)
     """
 
     def paginate(
-        self, *, studioId: str, ownedBy: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, studioId: str, ownedBy: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamingSessionBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessionBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststreamingsessionbackupspaginator)
         """
 
 
@@ -188,15 +192,15 @@
     def paginate(
         self,
         *,
         studioId: str,
         createdBy: str = ...,
         ownedBy: str = ...,
         sessionIds: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamingSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststreamingsessionspaginator)
         """
 
 
@@ -208,43 +212,43 @@
 
     def paginate(
         self,
         *,
         studioId: str,
         states: Sequence[StudioComponentStateType] = ...,
         types: Sequence[StudioComponentTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStudioComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststudiocomponentspaginator)
         """
 
 
 class ListStudioMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststudiomemberspaginator)
     """
 
     def paginate(
-        self, *, studioId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, studioId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStudioMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststudiomemberspaginator)
         """
 
 
 class ListStudiosPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudios)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststudiospaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStudiosResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudios.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststudiospaginator)
         """
```

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/paginator.pyi` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -84,43 +84,47 @@
     """
 
     def paginate(
         self,
         *,
         studioId: str,
         eulaIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEulaAcceptancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulaAcceptances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#listeulaacceptancespaginator)
         """
 
 class ListEulasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#listeulaspaginator)
     """
 
     def paginate(
-        self, *, eulaIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, eulaIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEulasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#listeulaspaginator)
         """
 
 class ListLaunchProfileMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfileMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#listlaunchprofilememberspaginator)
     """
 
     def paginate(
-        self, *, launchProfileId: str, studioId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        launchProfileId: str,
+        studioId: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLaunchProfileMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfileMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#listlaunchprofilememberspaginator)
         """
 
 class ListLaunchProfilesPaginator(Paginator):
@@ -131,43 +135,43 @@
 
     def paginate(
         self,
         *,
         studioId: str,
         principalId: str = ...,
         states: Sequence[LaunchProfileStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLaunchProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#listlaunchprofilespaginator)
         """
 
 class ListStreamingImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststreamingimagespaginator)
     """
 
     def paginate(
-        self, *, studioId: str, owner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, studioId: str, owner: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamingImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststreamingimagespaginator)
         """
 
 class ListStreamingSessionBackupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessionBackups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststreamingsessionbackupspaginator)
     """
 
     def paginate(
-        self, *, studioId: str, ownedBy: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, studioId: str, ownedBy: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamingSessionBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessionBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststreamingsessionbackupspaginator)
         """
 
 class ListStreamingSessionsPaginator(Paginator):
@@ -179,15 +183,15 @@
     def paginate(
         self,
         *,
         studioId: str,
         createdBy: str = ...,
         ownedBy: str = ...,
         sessionIds: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamingSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststreamingsessionspaginator)
         """
 
 class ListStudioComponentsPaginator(Paginator):
@@ -198,41 +202,41 @@
 
     def paginate(
         self,
         *,
         studioId: str,
         states: Sequence[StudioComponentStateType] = ...,
         types: Sequence[StudioComponentTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStudioComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststudiocomponentspaginator)
         """
 
 class ListStudioMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststudiomemberspaginator)
     """
 
     def paginate(
-        self, *, studioId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, studioId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStudioMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststudiomemberspaginator)
         """
 
 class ListStudiosPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudios)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststudiospaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStudiosResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudios.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/paginators/#liststudiospaginator)
         """
```

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/type_defs.py` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,19 +49,17 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptEulasRequestRequestTypeDef",
     "EulaAcceptanceTypeDef",
-    "ResponseMetadataTypeDef",
     "ActiveDirectoryComputerAttributeTypeDef",
     "ComputeFarmConfigurationTypeDef",
     "CreateStreamingImageRequestRequestTypeDef",
     "CreateStreamingSessionRequestRequestTypeDef",
     "CreateStreamingSessionStreamRequestRequestTypeDef",
     "StreamingSessionStreamTypeDef",
     "ScriptParameterKeyValueTypeDef",
@@ -91,28 +89,40 @@
     "GetStudioComponentRequestRequestTypeDef",
     "GetStudioMemberRequestRequestTypeDef",
     "StudioMembershipTypeDef",
     "GetStudioRequestRequestTypeDef",
     "LaunchProfileInitializationScriptTypeDef",
     "ValidationResultTypeDef",
     "LicenseServiceConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
     "ListEulaAcceptancesRequestRequestTypeDef",
+    "ListEulasRequestListEulasPaginateTypeDef",
     "ListEulasRequestRequestTypeDef",
+    "ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
     "ListLaunchProfileMembersRequestRequestTypeDef",
+    "ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
     "ListLaunchProfilesRequestRequestTypeDef",
+    "ListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
     "ListStreamingImagesRequestRequestTypeDef",
+    "ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
     "ListStreamingSessionBackupsRequestRequestTypeDef",
+    "ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
     "ListStreamingSessionsRequestRequestTypeDef",
+    "ListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
     "ListStudioComponentsRequestRequestTypeDef",
+    "ListStudioMembersRequestListStudioMembersPaginateTypeDef",
     "ListStudioMembersRequestRequestTypeDef",
+    "ListStudiosRequestListStudiosPaginateTypeDef",
     "ListStudiosRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "NewLaunchProfileMemberTypeDef",
     "NewStudioMemberTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "SharedFileSystemConfigurationTypeDef",
     "StartStreamingSessionRequestRequestTypeDef",
     "StartStudioSSOConfigurationRepairRequestRequestTypeDef",
     "StopStreamingSessionRequestRequestTypeDef",
     "StreamConfigurationSessionBackupTypeDef",
     "VolumeConfigurationTypeDef",
     "StreamingSessionStorageRootTypeDef",
@@ -120,15 +130,14 @@
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLaunchProfileMemberRequestRequestTypeDef",
     "UpdateStreamingImageRequestRequestTypeDef",
     "UpdateStudioRequestRequestTypeDef",
     "AcceptEulasResponseTypeDef",
     "ListEulaAcceptancesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ActiveDirectoryConfigurationTypeDef",
     "LaunchProfileInitializationActiveDirectoryTypeDef",
     "CreateStreamingSessionStreamResponseTypeDef",
     "GetStreamingSessionStreamResponseTypeDef",
     "CreateStudioRequestRequestTypeDef",
     "StudioTypeDef",
     "GetEulaResponseTypeDef",
@@ -148,24 +157,14 @@
     "GetStudioComponentRequestStudioComponentReadyWaitTypeDef",
     "GetStudioRequestStudioDeletedWaitTypeDef",
     "GetStudioRequestStudioReadyWaitTypeDef",
     "GetStreamingSessionBackupResponseTypeDef",
     "ListStreamingSessionBackupsResponseTypeDef",
     "GetStudioMemberResponseTypeDef",
     "ListStudioMembersResponseTypeDef",
-    "ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
-    "ListEulasRequestListEulasPaginateTypeDef",
-    "ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
-    "ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
-    "ListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
-    "ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
-    "ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
-    "ListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
-    "ListStudioMembersRequestListStudioMembersPaginateTypeDef",
-    "ListStudiosRequestListStudiosPaginateTypeDef",
     "PutLaunchProfileMembersRequestRequestTypeDef",
     "PutStudioMembersRequestRequestTypeDef",
     "StreamingSessionTypeDef",
     "StreamConfigurationSessionStorageTypeDef",
     "StreamingImageTypeDef",
     "StudioComponentConfigurationTypeDef",
     "LaunchProfileInitializationTypeDef",
@@ -219,44 +218,31 @@
     {
         "clientToken": str,
         "eulaIds": Sequence[str],
     },
     total=False,
 )
 
-
 class AcceptEulasRequestRequestTypeDef(
     _RequiredAcceptEulasRequestRequestTypeDef, _OptionalAcceptEulasRequestRequestTypeDef
 ):
     pass
 
-
 EulaAcceptanceTypeDef = TypedDict(
     "EulaAcceptanceTypeDef",
     {
         "acceptedAt": datetime,
         "acceptedBy": str,
         "accepteeId": str,
         "eulaAcceptanceId": str,
         "eulaId": str,
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
 ActiveDirectoryComputerAttributeTypeDef = TypedDict(
     "ActiveDirectoryComputerAttributeTypeDef",
     {
         "name": str,
         "value": str,
     },
     total=False,
@@ -285,22 +271,20 @@
         "clientToken": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStreamingImageRequestRequestTypeDef(
     _RequiredCreateStreamingImageRequestRequestTypeDef,
     _OptionalCreateStreamingImageRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateStreamingSessionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamingSessionRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -312,22 +296,20 @@
         "ownedBy": str,
         "streamingImageId": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStreamingSessionRequestRequestTypeDef(
     _RequiredCreateStreamingSessionRequestRequestTypeDef,
     _OptionalCreateStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateStreamingSessionStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamingSessionStreamRequestRequestTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -336,22 +318,20 @@
     {
         "clientToken": str,
         "expirationInSeconds": int,
     },
     total=False,
 )
 
-
 class CreateStreamingSessionStreamRequestRequestTypeDef(
     _RequiredCreateStreamingSessionStreamRequestRequestTypeDef,
     _OptionalCreateStreamingSessionStreamRequestRequestTypeDef,
 ):
     pass
 
-
 StreamingSessionStreamTypeDef = TypedDict(
     "StreamingSessionStreamTypeDef",
     {
         "createdAt": datetime,
         "createdBy": str,
         "expiresAt": datetime,
         "ownedBy": str,
@@ -393,21 +373,19 @@
     "_OptionalStudioEncryptionConfigurationTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
 
-
 class StudioEncryptionConfigurationTypeDef(
     _RequiredStudioEncryptionConfigurationTypeDef, _OptionalStudioEncryptionConfigurationTypeDef
 ):
     pass
 
-
 _RequiredDeleteLaunchProfileMemberRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteLaunchProfileMemberRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "principalId": str,
         "studioId": str,
     },
@@ -416,22 +394,20 @@
     "_OptionalDeleteLaunchProfileMemberRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteLaunchProfileMemberRequestRequestTypeDef(
     _RequiredDeleteLaunchProfileMemberRequestRequestTypeDef,
     _OptionalDeleteLaunchProfileMemberRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteLaunchProfileRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -439,22 +415,20 @@
     "_OptionalDeleteLaunchProfileRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteLaunchProfileRequestRequestTypeDef(
     _RequiredDeleteLaunchProfileRequestRequestTypeDef,
     _OptionalDeleteLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStreamingImageRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamingImageRequestRequestTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -462,22 +436,20 @@
     "_OptionalDeleteStreamingImageRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteStreamingImageRequestRequestTypeDef(
     _RequiredDeleteStreamingImageRequestRequestTypeDef,
     _OptionalDeleteStreamingImageRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStreamingSessionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamingSessionRequestRequestTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -485,22 +457,20 @@
     "_OptionalDeleteStreamingSessionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteStreamingSessionRequestRequestTypeDef(
     _RequiredDeleteStreamingSessionRequestRequestTypeDef,
     _OptionalDeleteStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStudioComponentRequestRequestTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -508,22 +478,20 @@
     "_OptionalDeleteStudioComponentRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteStudioComponentRequestRequestTypeDef(
     _RequiredDeleteStudioComponentRequestRequestTypeDef,
     _OptionalDeleteStudioComponentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStudioMemberRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStudioMemberRequestRequestTypeDef",
     {
         "principalId": str,
         "studioId": str,
     },
 )
@@ -531,43 +499,39 @@
     "_OptionalDeleteStudioMemberRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteStudioMemberRequestRequestTypeDef(
     _RequiredDeleteStudioMemberRequestRequestTypeDef,
     _OptionalDeleteStudioMemberRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStudioRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStudioRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalDeleteStudioRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStudioRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteStudioRequestRequestTypeDef(
     _RequiredDeleteStudioRequestRequestTypeDef, _OptionalDeleteStudioRequestRequestTypeDef
 ):
     pass
 
-
 EulaTypeDef = TypedDict(
     "EulaTypeDef",
     {
         "content": str,
         "createdAt": datetime,
         "eulaId": str,
         "name": str,
@@ -765,24 +729,35 @@
     "LicenseServiceConfigurationTypeDef",
     {
         "endpoint": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
+    "_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "studioId": str,
+    },
+)
+_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
+    "_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
+    {
+        "eulaIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef(
+    _RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+    _OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+):
+    pass
+
 _RequiredListEulaAcceptancesRequestRequestTypeDef = TypedDict(
     "_RequiredListEulaAcceptancesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListEulaAcceptancesRequestRequestTypeDef = TypedDict(
@@ -790,31 +765,59 @@
     {
         "eulaIds": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListEulaAcceptancesRequestRequestTypeDef(
     _RequiredListEulaAcceptancesRequestRequestTypeDef,
     _OptionalListEulaAcceptancesRequestRequestTypeDef,
 ):
     pass
 
+ListEulasRequestListEulasPaginateTypeDef = TypedDict(
+    "ListEulasRequestListEulasPaginateTypeDef",
+    {
+        "eulaIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListEulasRequestRequestTypeDef = TypedDict(
     "ListEulasRequestRequestTypeDef",
     {
         "eulaIds": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
+    {
+        "launchProfileId": str,
+        "studioId": str,
+    },
+)
+_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef(
+    _RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
+    _OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
+):
+    pass
+
 _RequiredListLaunchProfileMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchProfileMembersRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -823,21 +826,41 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListLaunchProfileMembersRequestRequestTypeDef(
     _RequiredListLaunchProfileMembersRequestRequestTypeDef,
     _OptionalListLaunchProfileMembersRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
+    {
+        "principalId": str,
+        "states": Sequence[LaunchProfileStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef(
+    _RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
+    _OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
+):
+    pass
 
 _RequiredListLaunchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchProfilesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
@@ -848,21 +871,40 @@
         "nextToken": str,
         "principalId": str,
         "states": Sequence[LaunchProfileStateType],
     },
     total=False,
 )
 
-
 class ListLaunchProfilesRequestRequestTypeDef(
     _RequiredListLaunchProfilesRequestRequestTypeDef,
     _OptionalListLaunchProfilesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
+    "_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
+    "_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
+    {
+        "owner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStreamingImagesRequestListStreamingImagesPaginateTypeDef(
+    _RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
+    _OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
+):
+    pass
 
 _RequiredListStreamingImagesRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingImagesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
@@ -871,21 +913,40 @@
     {
         "nextToken": str,
         "owner": str,
     },
     total=False,
 )
 
-
 class ListStreamingImagesRequestRequestTypeDef(
     _RequiredListStreamingImagesRequestRequestTypeDef,
     _OptionalListStreamingImagesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
+    "_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
+    "_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
+    {
+        "ownedBy": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef(
+    _RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
+    _OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
+):
+    pass
 
 _RequiredListStreamingSessionBackupsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingSessionBackupsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
@@ -894,21 +955,42 @@
     {
         "nextToken": str,
         "ownedBy": str,
     },
     total=False,
 )
 
-
 class ListStreamingSessionBackupsRequestRequestTypeDef(
     _RequiredListStreamingSessionBackupsRequestRequestTypeDef,
     _OptionalListStreamingSessionBackupsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
+    {
+        "createdBy": str,
+        "ownedBy": str,
+        "sessionIds": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef(
+    _RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
+    _OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
+):
+    pass
 
 _RequiredListStreamingSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingSessionsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
@@ -919,21 +1001,41 @@
         "nextToken": str,
         "ownedBy": str,
         "sessionIds": str,
     },
     total=False,
 )
 
-
 class ListStreamingSessionsRequestRequestTypeDef(
     _RequiredListStreamingSessionsRequestRequestTypeDef,
     _OptionalListStreamingSessionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
+    "_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
+    "_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
+    {
+        "states": Sequence[StudioComponentStateType],
+        "types": Sequence[StudioComponentTypeType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStudioComponentsRequestListStudioComponentsPaginateTypeDef(
+    _RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
+    _OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
+):
+    pass
 
 _RequiredListStudioComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListStudioComponentsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
@@ -944,21 +1046,39 @@
         "nextToken": str,
         "states": Sequence[StudioComponentStateType],
         "types": Sequence[StudioComponentTypeType],
     },
     total=False,
 )
 
-
 class ListStudioComponentsRequestRequestTypeDef(
     _RequiredListStudioComponentsRequestRequestTypeDef,
     _OptionalListStudioComponentsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
+    "_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
+    "_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStudioMembersRequestListStudioMembersPaginateTypeDef(
+    _RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef,
+    _OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef,
+):
+    pass
 
 _RequiredListStudioMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListStudioMembersRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
@@ -967,20 +1087,26 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListStudioMembersRequestRequestTypeDef(
     _RequiredListStudioMembersRequestRequestTypeDef, _OptionalListStudioMembersRequestRequestTypeDef
 ):
     pass
 
+ListStudiosRequestListStudiosPaginateTypeDef = TypedDict(
+    "ListStudiosRequestListStudiosPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListStudiosRequestRequestTypeDef = TypedDict(
     "ListStudiosRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
@@ -989,14 +1115,22 @@
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
 NewLaunchProfileMemberTypeDef = TypedDict(
     "NewLaunchProfileMemberTypeDef",
     {
         "persona": Literal["USER"],
         "principalId": str,
     },
 )
@@ -1005,14 +1139,35 @@
     "NewStudioMemberTypeDef",
     {
         "persona": Literal["ADMINISTRATOR"],
         "principalId": str,
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
 SharedFileSystemConfigurationTypeDef = TypedDict(
     "SharedFileSystemConfigurationTypeDef",
     {
         "endpoint": str,
         "fileSystemId": str,
         "linuxMountPoint": str,
         "shareName": str,
@@ -1033,44 +1188,40 @@
     {
         "backupId": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class StartStreamingSessionRequestRequestTypeDef(
     _RequiredStartStreamingSessionRequestRequestTypeDef,
     _OptionalStartStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartStudioSSOConfigurationRepairRequestRequestTypeDef = TypedDict(
     "_RequiredStartStudioSSOConfigurationRepairRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalStartStudioSSOConfigurationRepairRequestRequestTypeDef = TypedDict(
     "_OptionalStartStudioSSOConfigurationRepairRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class StartStudioSSOConfigurationRepairRequestRequestTypeDef(
     _RequiredStartStudioSSOConfigurationRepairRequestRequestTypeDef,
     _OptionalStartStudioSSOConfigurationRepairRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStopStreamingSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStopStreamingSessionRequestRequestTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1079,22 +1230,20 @@
     {
         "clientToken": str,
         "volumeRetentionMode": VolumeRetentionModeType,
     },
     total=False,
 )
 
-
 class StopStreamingSessionRequestRequestTypeDef(
     _RequiredStopStreamingSessionRequestRequestTypeDef,
     _OptionalStopStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
-
 StreamConfigurationSessionBackupTypeDef = TypedDict(
     "StreamConfigurationSessionBackupTypeDef",
     {
         "maxBackupsToRetain": int,
         "mode": SessionBackupModeType,
     },
     total=False,
@@ -1129,43 +1278,39 @@
     "_OptionalStreamingImageEncryptionConfigurationTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
 
-
 class StreamingImageEncryptionConfigurationTypeDef(
     _RequiredStreamingImageEncryptionConfigurationTypeDef,
     _OptionalStreamingImageEncryptionConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1183,22 +1328,20 @@
     "_OptionalUpdateLaunchProfileMemberRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateLaunchProfileMemberRequestRequestTypeDef(
     _RequiredUpdateLaunchProfileMemberRequestRequestTypeDef,
     _OptionalUpdateLaunchProfileMemberRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateStreamingImageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingImageRequestRequestTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -1208,22 +1351,20 @@
         "clientToken": str,
         "description": str,
         "name": str,
     },
     total=False,
 )
 
-
 class UpdateStreamingImageRequestRequestTypeDef(
     _RequiredUpdateStreamingImageRequestRequestTypeDef,
     _OptionalUpdateStreamingImageRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateStudioRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStudioRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalUpdateStudioRequestRequestTypeDef = TypedDict(
@@ -1233,43 +1374,33 @@
         "clientToken": str,
         "displayName": str,
         "userRoleArn": str,
     },
     total=False,
 )
 
-
 class UpdateStudioRequestRequestTypeDef(
     _RequiredUpdateStudioRequestRequestTypeDef, _OptionalUpdateStudioRequestRequestTypeDef
 ):
     pass
 
-
 AcceptEulasResponseTypeDef = TypedDict(
     "AcceptEulasResponseTypeDef",
     {
         "eulaAcceptances": List[EulaAcceptanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEulaAcceptancesResponseTypeDef = TypedDict(
     "ListEulaAcceptancesResponseTypeDef",
     {
         "eulaAcceptances": List[EulaAcceptanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActiveDirectoryConfigurationTypeDef = TypedDict(
     "ActiveDirectoryConfigurationTypeDef",
     {
         "computerAttributes": Sequence[ActiveDirectoryComputerAttributeTypeDef],
@@ -1293,23 +1424,23 @@
     total=False,
 )
 
 CreateStreamingSessionStreamResponseTypeDef = TypedDict(
     "CreateStreamingSessionStreamResponseTypeDef",
     {
         "stream": StreamingSessionStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStreamingSessionStreamResponseTypeDef = TypedDict(
     "GetStreamingSessionStreamResponseTypeDef",
     {
         "stream": StreamingSessionStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateStudioRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStudioRequestRequestTypeDef",
     {
         "adminRoleArn": str,
@@ -1324,21 +1455,19 @@
         "clientToken": str,
         "studioEncryptionConfiguration": StudioEncryptionConfigurationTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStudioRequestRequestTypeDef(
     _RequiredCreateStudioRequestRequestTypeDef, _OptionalCreateStudioRequestRequestTypeDef
 ):
     pass
 
-
 StudioTypeDef = TypedDict(
     "StudioTypeDef",
     {
         "adminRoleArn": str,
         "arn": str,
         "createdAt": datetime,
         "displayName": str,
@@ -1358,49 +1487,49 @@
     total=False,
 )
 
 GetEulaResponseTypeDef = TypedDict(
     "GetEulaResponseTypeDef",
     {
         "eula": EulaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEulasResponseTypeDef = TypedDict(
     "ListEulasResponseTypeDef",
     {
         "eulas": List[EulaTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLaunchProfileMemberResponseTypeDef = TypedDict(
     "GetLaunchProfileMemberResponseTypeDef",
     {
         "member": LaunchProfileMembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLaunchProfileMembersResponseTypeDef = TypedDict(
     "ListLaunchProfileMembersResponseTypeDef",
     {
         "members": List[LaunchProfileMembershipTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLaunchProfileMemberResponseTypeDef = TypedDict(
     "UpdateLaunchProfileMemberResponseTypeDef",
     {
         "member": LaunchProfileMembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef = TypedDict(
     "_RequiredGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef",
     {
         "launchProfileId": str,
@@ -1411,22 +1540,20 @@
     "_OptionalGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef(
     _RequiredGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef,
     _OptionalGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef = TypedDict(
     "_RequiredGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -1434,22 +1561,20 @@
     "_OptionalGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetLaunchProfileRequestLaunchProfileReadyWaitTypeDef(
     _RequiredGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef,
     _OptionalGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingImageRequestStreamingImageDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingImageRequestStreamingImageDeletedWaitTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -1457,22 +1582,20 @@
     "_OptionalGetStreamingImageRequestStreamingImageDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingImageRequestStreamingImageDeletedWaitTypeDef(
     _RequiredGetStreamingImageRequestStreamingImageDeletedWaitTypeDef,
     _OptionalGetStreamingImageRequestStreamingImageDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingImageRequestStreamingImageReadyWaitTypeDef = TypedDict(
     "_RequiredGetStreamingImageRequestStreamingImageReadyWaitTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -1480,22 +1603,20 @@
     "_OptionalGetStreamingImageRequestStreamingImageReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingImageRequestStreamingImageReadyWaitTypeDef(
     _RequiredGetStreamingImageRequestStreamingImageReadyWaitTypeDef,
     _OptionalGetStreamingImageRequestStreamingImageReadyWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1503,22 +1624,20 @@
     "_OptionalGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef(
     _RequiredGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef,
     _OptionalGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1526,22 +1645,20 @@
     "_OptionalGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingSessionRequestStreamingSessionReadyWaitTypeDef(
     _RequiredGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef,
     _OptionalGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1549,22 +1666,20 @@
     "_OptionalGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef(
     _RequiredGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef,
     _OptionalGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef",
     {
         "sessionId": str,
         "streamId": str,
         "studioId": str,
     },
@@ -1573,22 +1688,20 @@
     "_OptionalGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef(
     _RequiredGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef,
     _OptionalGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStudioComponentRequestStudioComponentDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStudioComponentRequestStudioComponentDeletedWaitTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -1596,22 +1709,20 @@
     "_OptionalGetStudioComponentRequestStudioComponentDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStudioComponentRequestStudioComponentDeletedWaitTypeDef(
     _RequiredGetStudioComponentRequestStudioComponentDeletedWaitTypeDef,
     _OptionalGetStudioComponentRequestStudioComponentDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStudioComponentRequestStudioComponentReadyWaitTypeDef = TypedDict(
     "_RequiredGetStudioComponentRequestStudioComponentReadyWaitTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -1619,301 +1730,91 @@
     "_OptionalGetStudioComponentRequestStudioComponentReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStudioComponentRequestStudioComponentReadyWaitTypeDef(
     _RequiredGetStudioComponentRequestStudioComponentReadyWaitTypeDef,
     _OptionalGetStudioComponentRequestStudioComponentReadyWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStudioRequestStudioDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStudioRequestStudioDeletedWaitTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalGetStudioRequestStudioDeletedWaitTypeDef = TypedDict(
     "_OptionalGetStudioRequestStudioDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStudioRequestStudioDeletedWaitTypeDef(
     _RequiredGetStudioRequestStudioDeletedWaitTypeDef,
     _OptionalGetStudioRequestStudioDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStudioRequestStudioReadyWaitTypeDef = TypedDict(
     "_RequiredGetStudioRequestStudioReadyWaitTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalGetStudioRequestStudioReadyWaitTypeDef = TypedDict(
     "_OptionalGetStudioRequestStudioReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStudioRequestStudioReadyWaitTypeDef(
     _RequiredGetStudioRequestStudioReadyWaitTypeDef, _OptionalGetStudioRequestStudioReadyWaitTypeDef
 ):
     pass
 
-
 GetStreamingSessionBackupResponseTypeDef = TypedDict(
     "GetStreamingSessionBackupResponseTypeDef",
     {
         "streamingSessionBackup": StreamingSessionBackupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamingSessionBackupsResponseTypeDef = TypedDict(
     "ListStreamingSessionBackupsResponseTypeDef",
     {
         "nextToken": str,
         "streamingSessionBackups": List[StreamingSessionBackupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStudioMemberResponseTypeDef = TypedDict(
     "GetStudioMemberResponseTypeDef",
     {
         "member": StudioMembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStudioMembersResponseTypeDef = TypedDict(
     "ListStudioMembersResponseTypeDef",
     {
         "members": List[StudioMembershipTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
-    "_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
-    "_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
-    {
-        "eulaIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef(
-    _RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
-    _OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
-):
-    pass
-
-
-ListEulasRequestListEulasPaginateTypeDef = TypedDict(
-    "ListEulasRequestListEulasPaginateTypeDef",
-    {
-        "eulaIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
-    {
-        "launchProfileId": str,
-        "studioId": str,
-    },
-)
-_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef(
-    _RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
-    _OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
-    {
-        "principalId": str,
-        "states": Sequence[LaunchProfileStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef(
-    _RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
-    _OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
-    "_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
-    "_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
-    {
-        "owner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStreamingImagesRequestListStreamingImagesPaginateTypeDef(
-    _RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
-    _OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
-    "_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
-    "_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
-    {
-        "ownedBy": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef(
-    _RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
-    _OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
-    {
-        "createdBy": str,
-        "ownedBy": str,
-        "sessionIds": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef(
-    _RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
-    _OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
-    "_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
-    "_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
-    {
-        "states": Sequence[StudioComponentStateType],
-        "types": Sequence[StudioComponentTypeType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStudioComponentsRequestListStudioComponentsPaginateTypeDef(
-    _RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
-    _OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
-    "_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
-    "_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStudioMembersRequestListStudioMembersPaginateTypeDef(
-    _RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef,
-    _OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef,
-):
-    pass
-
-
-ListStudiosRequestListStudiosPaginateTypeDef = TypedDict(
-    "ListStudiosRequestListStudiosPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 _RequiredPutLaunchProfileMembersRequestRequestTypeDef = TypedDict(
     "_RequiredPutLaunchProfileMembersRequestRequestTypeDef",
     {
         "identityStoreId": str,
         "launchProfileId": str,
@@ -1925,22 +1826,20 @@
     "_OptionalPutLaunchProfileMembersRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class PutLaunchProfileMembersRequestRequestTypeDef(
     _RequiredPutLaunchProfileMembersRequestRequestTypeDef,
     _OptionalPutLaunchProfileMembersRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutStudioMembersRequestRequestTypeDef = TypedDict(
     "_RequiredPutStudioMembersRequestRequestTypeDef",
     {
         "identityStoreId": str,
         "members": Sequence[NewStudioMemberTypeDef],
         "studioId": str,
     },
@@ -1949,21 +1848,19 @@
     "_OptionalPutStudioMembersRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class PutStudioMembersRequestRequestTypeDef(
     _RequiredPutStudioMembersRequestRequestTypeDef, _OptionalPutStudioMembersRequestRequestTypeDef
 ):
     pass
 
-
 StreamingSessionTypeDef = TypedDict(
     "StreamingSessionTypeDef",
     {
         "arn": str,
         "automaticTerminationMode": AutomaticTerminationModeType,
         "backupMode": SessionBackupModeType,
         "createdAt": datetime,
@@ -2004,22 +1901,20 @@
     "_OptionalStreamConfigurationSessionStorageTypeDef",
     {
         "root": StreamingSessionStorageRootTypeDef,
     },
     total=False,
 )
 
-
 class StreamConfigurationSessionStorageTypeDef(
     _RequiredStreamConfigurationSessionStorageTypeDef,
     _OptionalStreamConfigurationSessionStorageTypeDef,
 ):
     pass
 
-
 StreamingImageTypeDef = TypedDict(
     "StreamingImageTypeDef",
     {
         "arn": str,
         "description": str,
         "ec2ImageId": str,
         "encryptionConfiguration": StreamingImageEncryptionConfigurationTypeDef,
@@ -2063,105 +1958,105 @@
     total=False,
 )
 
 CreateStudioResponseTypeDef = TypedDict(
     "CreateStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteStudioResponseTypeDef = TypedDict(
     "DeleteStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStudioResponseTypeDef = TypedDict(
     "GetStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStudiosResponseTypeDef = TypedDict(
     "ListStudiosResponseTypeDef",
     {
         "nextToken": str,
         "studios": List[StudioTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartStudioSSOConfigurationRepairResponseTypeDef = TypedDict(
     "StartStudioSSOConfigurationRepairResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStudioResponseTypeDef = TypedDict(
     "UpdateStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStreamingSessionResponseTypeDef = TypedDict(
     "CreateStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteStreamingSessionResponseTypeDef = TypedDict(
     "DeleteStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStreamingSessionResponseTypeDef = TypedDict(
     "GetStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamingSessionsResponseTypeDef = TypedDict(
     "ListStreamingSessionsResponseTypeDef",
     {
         "nextToken": str,
         "sessions": List[StreamingSessionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartStreamingSessionResponseTypeDef = TypedDict(
     "StartStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopStreamingSessionResponseTypeDef = TypedDict(
     "StopStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStreamConfigurationCreateTypeDef = TypedDict(
     "_RequiredStreamConfigurationCreateTypeDef",
     {
         "clipboardMode": StreamingClipboardModeType,
@@ -2179,21 +2074,19 @@
         "sessionPersistenceMode": SessionPersistenceModeType,
         "sessionStorage": StreamConfigurationSessionStorageTypeDef,
         "volumeConfiguration": VolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class StreamConfigurationCreateTypeDef(
     _RequiredStreamConfigurationCreateTypeDef, _OptionalStreamConfigurationCreateTypeDef
 ):
     pass
 
-
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "clipboardMode": StreamingClipboardModeType,
         "ec2InstanceTypes": List[StreamingInstanceTypeType],
         "streamingImageIds": List[str],
     },
@@ -2208,59 +2101,57 @@
         "sessionPersistenceMode": SessionPersistenceModeType,
         "sessionStorage": StreamConfigurationSessionStorageTypeDef,
         "volumeConfiguration": VolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
-
 CreateStreamingImageResponseTypeDef = TypedDict(
     "CreateStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteStreamingImageResponseTypeDef = TypedDict(
     "DeleteStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStreamingImageResponseTypeDef = TypedDict(
     "GetStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamingImagesResponseTypeDef = TypedDict(
     "ListStreamingImagesResponseTypeDef",
     {
         "nextToken": str,
         "streamingImages": List[StreamingImageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStreamingImageResponseTypeDef = TypedDict(
     "UpdateStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStudioComponentRequestRequestTypeDef",
     {
         "name": str,
@@ -2281,22 +2172,20 @@
         "secureInitializationRoleArn": str,
         "subtype": StudioComponentSubtypeType,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStudioComponentRequestRequestTypeDef(
     _RequiredCreateStudioComponentRequestRequestTypeDef,
     _OptionalCreateStudioComponentRequestRequestTypeDef,
 ):
     pass
 
-
 StudioComponentTypeDef = TypedDict(
     "StudioComponentTypeDef",
     {
         "arn": str,
         "configuration": StudioComponentConfigurationTypeDef,
         "createdAt": datetime,
         "createdBy": str,
@@ -2341,27 +2230,25 @@
         "secureInitializationRoleArn": str,
         "subtype": StudioComponentSubtypeType,
         "type": StudioComponentTypeType,
     },
     total=False,
 )
 
-
 class UpdateStudioComponentRequestRequestTypeDef(
     _RequiredUpdateStudioComponentRequestRequestTypeDef,
     _OptionalUpdateStudioComponentRequestRequestTypeDef,
 ):
     pass
 
-
 GetLaunchProfileInitializationResponseTypeDef = TypedDict(
     "GetLaunchProfileInitializationResponseTypeDef",
     {
         "launchProfileInitialization": LaunchProfileInitializationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchProfileRequestRequestTypeDef",
     {
         "ec2SubnetIds": Sequence[str],
@@ -2378,22 +2265,20 @@
         "clientToken": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateLaunchProfileRequestRequestTypeDef(
     _RequiredCreateLaunchProfileRequestRequestTypeDef,
     _OptionalCreateLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchProfileRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -2406,22 +2291,20 @@
         "name": str,
         "streamConfiguration": StreamConfigurationCreateTypeDef,
         "studioComponentIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateLaunchProfileRequestRequestTypeDef(
     _RequiredUpdateLaunchProfileRequestRequestTypeDef,
     _OptionalUpdateLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
-
 LaunchProfileTypeDef = TypedDict(
     "LaunchProfileTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "createdBy": str,
         "description": str,
@@ -2442,94 +2325,94 @@
     total=False,
 )
 
 CreateStudioComponentResponseTypeDef = TypedDict(
     "CreateStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteStudioComponentResponseTypeDef = TypedDict(
     "DeleteStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStudioComponentResponseTypeDef = TypedDict(
     "GetStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStudioComponentsResponseTypeDef = TypedDict(
     "ListStudioComponentsResponseTypeDef",
     {
         "nextToken": str,
         "studioComponents": List[StudioComponentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStudioComponentResponseTypeDef = TypedDict(
     "UpdateStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateLaunchProfileResponseTypeDef = TypedDict(
     "CreateLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteLaunchProfileResponseTypeDef = TypedDict(
     "DeleteLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLaunchProfileDetailsResponseTypeDef = TypedDict(
     "GetLaunchProfileDetailsResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
         "streamingImages": List[StreamingImageTypeDef],
         "studioComponentSummaries": List[StudioComponentSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLaunchProfileResponseTypeDef = TypedDict(
     "GetLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLaunchProfilesResponseTypeDef = TypedDict(
     "ListLaunchProfilesResponseTypeDef",
     {
         "launchProfiles": List[LaunchProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLaunchProfileResponseTypeDef = TypedDict(
     "UpdateLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/type_defs.pyi` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,18 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptEulasRequestRequestTypeDef",
     "EulaAcceptanceTypeDef",
-    "ResponseMetadataTypeDef",
     "ActiveDirectoryComputerAttributeTypeDef",
     "ComputeFarmConfigurationTypeDef",
     "CreateStreamingImageRequestRequestTypeDef",
     "CreateStreamingSessionRequestRequestTypeDef",
     "CreateStreamingSessionStreamRequestRequestTypeDef",
     "StreamingSessionStreamTypeDef",
     "ScriptParameterKeyValueTypeDef",
@@ -90,28 +90,40 @@
     "GetStudioComponentRequestRequestTypeDef",
     "GetStudioMemberRequestRequestTypeDef",
     "StudioMembershipTypeDef",
     "GetStudioRequestRequestTypeDef",
     "LaunchProfileInitializationScriptTypeDef",
     "ValidationResultTypeDef",
     "LicenseServiceConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
     "ListEulaAcceptancesRequestRequestTypeDef",
+    "ListEulasRequestListEulasPaginateTypeDef",
     "ListEulasRequestRequestTypeDef",
+    "ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
     "ListLaunchProfileMembersRequestRequestTypeDef",
+    "ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
     "ListLaunchProfilesRequestRequestTypeDef",
+    "ListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
     "ListStreamingImagesRequestRequestTypeDef",
+    "ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
     "ListStreamingSessionBackupsRequestRequestTypeDef",
+    "ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
     "ListStreamingSessionsRequestRequestTypeDef",
+    "ListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
     "ListStudioComponentsRequestRequestTypeDef",
+    "ListStudioMembersRequestListStudioMembersPaginateTypeDef",
     "ListStudioMembersRequestRequestTypeDef",
+    "ListStudiosRequestListStudiosPaginateTypeDef",
     "ListStudiosRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "NewLaunchProfileMemberTypeDef",
     "NewStudioMemberTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "SharedFileSystemConfigurationTypeDef",
     "StartStreamingSessionRequestRequestTypeDef",
     "StartStudioSSOConfigurationRepairRequestRequestTypeDef",
     "StopStreamingSessionRequestRequestTypeDef",
     "StreamConfigurationSessionBackupTypeDef",
     "VolumeConfigurationTypeDef",
     "StreamingSessionStorageRootTypeDef",
@@ -119,15 +131,14 @@
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLaunchProfileMemberRequestRequestTypeDef",
     "UpdateStreamingImageRequestRequestTypeDef",
     "UpdateStudioRequestRequestTypeDef",
     "AcceptEulasResponseTypeDef",
     "ListEulaAcceptancesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ActiveDirectoryConfigurationTypeDef",
     "LaunchProfileInitializationActiveDirectoryTypeDef",
     "CreateStreamingSessionStreamResponseTypeDef",
     "GetStreamingSessionStreamResponseTypeDef",
     "CreateStudioRequestRequestTypeDef",
     "StudioTypeDef",
     "GetEulaResponseTypeDef",
@@ -147,24 +158,14 @@
     "GetStudioComponentRequestStudioComponentReadyWaitTypeDef",
     "GetStudioRequestStudioDeletedWaitTypeDef",
     "GetStudioRequestStudioReadyWaitTypeDef",
     "GetStreamingSessionBackupResponseTypeDef",
     "ListStreamingSessionBackupsResponseTypeDef",
     "GetStudioMemberResponseTypeDef",
     "ListStudioMembersResponseTypeDef",
-    "ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
-    "ListEulasRequestListEulasPaginateTypeDef",
-    "ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
-    "ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
-    "ListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
-    "ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
-    "ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
-    "ListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
-    "ListStudioMembersRequestListStudioMembersPaginateTypeDef",
-    "ListStudiosRequestListStudiosPaginateTypeDef",
     "PutLaunchProfileMembersRequestRequestTypeDef",
     "PutStudioMembersRequestRequestTypeDef",
     "StreamingSessionTypeDef",
     "StreamConfigurationSessionStorageTypeDef",
     "StreamingImageTypeDef",
     "StudioComponentConfigurationTypeDef",
     "LaunchProfileInitializationTypeDef",
@@ -218,42 +219,33 @@
     {
         "clientToken": str,
         "eulaIds": Sequence[str],
     },
     total=False,
 )
 
+
 class AcceptEulasRequestRequestTypeDef(
     _RequiredAcceptEulasRequestRequestTypeDef, _OptionalAcceptEulasRequestRequestTypeDef
 ):
     pass
 
+
 EulaAcceptanceTypeDef = TypedDict(
     "EulaAcceptanceTypeDef",
     {
         "acceptedAt": datetime,
         "acceptedBy": str,
         "accepteeId": str,
         "eulaAcceptanceId": str,
         "eulaId": str,
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
 ActiveDirectoryComputerAttributeTypeDef = TypedDict(
     "ActiveDirectoryComputerAttributeTypeDef",
     {
         "name": str,
         "value": str,
     },
     total=False,
@@ -282,20 +274,22 @@
         "clientToken": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStreamingImageRequestRequestTypeDef(
     _RequiredCreateStreamingImageRequestRequestTypeDef,
     _OptionalCreateStreamingImageRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateStreamingSessionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamingSessionRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -307,20 +301,22 @@
         "ownedBy": str,
         "streamingImageId": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStreamingSessionRequestRequestTypeDef(
     _RequiredCreateStreamingSessionRequestRequestTypeDef,
     _OptionalCreateStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateStreamingSessionStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamingSessionStreamRequestRequestTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -329,20 +325,22 @@
     {
         "clientToken": str,
         "expirationInSeconds": int,
     },
     total=False,
 )
 
+
 class CreateStreamingSessionStreamRequestRequestTypeDef(
     _RequiredCreateStreamingSessionStreamRequestRequestTypeDef,
     _OptionalCreateStreamingSessionStreamRequestRequestTypeDef,
 ):
     pass
 
+
 StreamingSessionStreamTypeDef = TypedDict(
     "StreamingSessionStreamTypeDef",
     {
         "createdAt": datetime,
         "createdBy": str,
         "expiresAt": datetime,
         "ownedBy": str,
@@ -384,19 +382,21 @@
     "_OptionalStudioEncryptionConfigurationTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
 
+
 class StudioEncryptionConfigurationTypeDef(
     _RequiredStudioEncryptionConfigurationTypeDef, _OptionalStudioEncryptionConfigurationTypeDef
 ):
     pass
 
+
 _RequiredDeleteLaunchProfileMemberRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteLaunchProfileMemberRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "principalId": str,
         "studioId": str,
     },
@@ -405,20 +405,22 @@
     "_OptionalDeleteLaunchProfileMemberRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteLaunchProfileMemberRequestRequestTypeDef(
     _RequiredDeleteLaunchProfileMemberRequestRequestTypeDef,
     _OptionalDeleteLaunchProfileMemberRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteLaunchProfileRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -426,20 +428,22 @@
     "_OptionalDeleteLaunchProfileRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteLaunchProfileRequestRequestTypeDef(
     _RequiredDeleteLaunchProfileRequestRequestTypeDef,
     _OptionalDeleteLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStreamingImageRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamingImageRequestRequestTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -447,20 +451,22 @@
     "_OptionalDeleteStreamingImageRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteStreamingImageRequestRequestTypeDef(
     _RequiredDeleteStreamingImageRequestRequestTypeDef,
     _OptionalDeleteStreamingImageRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStreamingSessionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamingSessionRequestRequestTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -468,20 +474,22 @@
     "_OptionalDeleteStreamingSessionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteStreamingSessionRequestRequestTypeDef(
     _RequiredDeleteStreamingSessionRequestRequestTypeDef,
     _OptionalDeleteStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStudioComponentRequestRequestTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -489,20 +497,22 @@
     "_OptionalDeleteStudioComponentRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteStudioComponentRequestRequestTypeDef(
     _RequiredDeleteStudioComponentRequestRequestTypeDef,
     _OptionalDeleteStudioComponentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStudioMemberRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStudioMemberRequestRequestTypeDef",
     {
         "principalId": str,
         "studioId": str,
     },
 )
@@ -510,39 +520,43 @@
     "_OptionalDeleteStudioMemberRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteStudioMemberRequestRequestTypeDef(
     _RequiredDeleteStudioMemberRequestRequestTypeDef,
     _OptionalDeleteStudioMemberRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStudioRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStudioRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalDeleteStudioRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStudioRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteStudioRequestRequestTypeDef(
     _RequiredDeleteStudioRequestRequestTypeDef, _OptionalDeleteStudioRequestRequestTypeDef
 ):
     pass
 
+
 EulaTypeDef = TypedDict(
     "EulaTypeDef",
     {
         "content": str,
         "createdAt": datetime,
         "eulaId": str,
         "name": str,
@@ -740,24 +754,37 @@
     "LicenseServiceConfigurationTypeDef",
     {
         "endpoint": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
+    "_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "studioId": str,
+    },
+)
+_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
+    "_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
+    {
+        "eulaIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef(
+    _RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+    _OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEulaAcceptancesRequestRequestTypeDef = TypedDict(
     "_RequiredListEulaAcceptancesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListEulaAcceptancesRequestRequestTypeDef = TypedDict(
@@ -765,29 +792,63 @@
     {
         "eulaIds": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListEulaAcceptancesRequestRequestTypeDef(
     _RequiredListEulaAcceptancesRequestRequestTypeDef,
     _OptionalListEulaAcceptancesRequestRequestTypeDef,
 ):
     pass
 
+
+ListEulasRequestListEulasPaginateTypeDef = TypedDict(
+    "ListEulasRequestListEulasPaginateTypeDef",
+    {
+        "eulaIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEulasRequestRequestTypeDef = TypedDict(
     "ListEulasRequestRequestTypeDef",
     {
         "eulaIds": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
+    {
+        "launchProfileId": str,
+        "studioId": str,
+    },
+)
+_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef(
+    _RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
+    _OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListLaunchProfileMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchProfileMembersRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -796,20 +857,46 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListLaunchProfileMembersRequestRequestTypeDef(
     _RequiredListLaunchProfileMembersRequestRequestTypeDef,
     _OptionalListLaunchProfileMembersRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
+    {
+        "principalId": str,
+        "states": Sequence[LaunchProfileStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef(
+    _RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
+    _OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListLaunchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchProfilesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListLaunchProfilesRequestRequestTypeDef = TypedDict(
@@ -819,20 +906,45 @@
         "nextToken": str,
         "principalId": str,
         "states": Sequence[LaunchProfileStateType],
     },
     total=False,
 )
 
+
 class ListLaunchProfilesRequestRequestTypeDef(
     _RequiredListLaunchProfilesRequestRequestTypeDef,
     _OptionalListLaunchProfilesRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
+    "_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
+    "_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
+    {
+        "owner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStreamingImagesRequestListStreamingImagesPaginateTypeDef(
+    _RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
+    _OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListStreamingImagesRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingImagesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingImagesRequestRequestTypeDef = TypedDict(
@@ -840,20 +952,45 @@
     {
         "nextToken": str,
         "owner": str,
     },
     total=False,
 )
 
+
 class ListStreamingImagesRequestRequestTypeDef(
     _RequiredListStreamingImagesRequestRequestTypeDef,
     _OptionalListStreamingImagesRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
+    "_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
+    "_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
+    {
+        "ownedBy": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef(
+    _RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
+    _OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListStreamingSessionBackupsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingSessionBackupsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionBackupsRequestRequestTypeDef = TypedDict(
@@ -861,20 +998,47 @@
     {
         "nextToken": str,
         "ownedBy": str,
     },
     total=False,
 )
 
+
 class ListStreamingSessionBackupsRequestRequestTypeDef(
     _RequiredListStreamingSessionBackupsRequestRequestTypeDef,
     _OptionalListStreamingSessionBackupsRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
+    {
+        "createdBy": str,
+        "ownedBy": str,
+        "sessionIds": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef(
+    _RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
+    _OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListStreamingSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingSessionsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionsRequestRequestTypeDef = TypedDict(
@@ -884,20 +1048,46 @@
         "nextToken": str,
         "ownedBy": str,
         "sessionIds": str,
     },
     total=False,
 )
 
+
 class ListStreamingSessionsRequestRequestTypeDef(
     _RequiredListStreamingSessionsRequestRequestTypeDef,
     _OptionalListStreamingSessionsRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
+    "_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
+    "_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
+    {
+        "states": Sequence[StudioComponentStateType],
+        "types": Sequence[StudioComponentTypeType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStudioComponentsRequestListStudioComponentsPaginateTypeDef(
+    _RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
+    _OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListStudioComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListStudioComponentsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioComponentsRequestRequestTypeDef = TypedDict(
@@ -907,20 +1097,44 @@
         "nextToken": str,
         "states": Sequence[StudioComponentStateType],
         "types": Sequence[StudioComponentTypeType],
     },
     total=False,
 )
 
+
 class ListStudioComponentsRequestRequestTypeDef(
     _RequiredListStudioComponentsRequestRequestTypeDef,
     _OptionalListStudioComponentsRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
+    "_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef",
+    {
+        "studioId": str,
+    },
+)
+_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
+    "_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStudioMembersRequestListStudioMembersPaginateTypeDef(
+    _RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef,
+    _OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListStudioMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListStudioMembersRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioMembersRequestRequestTypeDef = TypedDict(
@@ -928,19 +1142,29 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListStudioMembersRequestRequestTypeDef(
     _RequiredListStudioMembersRequestRequestTypeDef, _OptionalListStudioMembersRequestRequestTypeDef
 ):
     pass
 
+
+ListStudiosRequestListStudiosPaginateTypeDef = TypedDict(
+    "ListStudiosRequestListStudiosPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStudiosRequestRequestTypeDef = TypedDict(
     "ListStudiosRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -948,14 +1172,22 @@
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
 NewLaunchProfileMemberTypeDef = TypedDict(
     "NewLaunchProfileMemberTypeDef",
     {
         "persona": Literal["USER"],
         "principalId": str,
     },
 )
@@ -964,14 +1196,35 @@
     "NewStudioMemberTypeDef",
     {
         "persona": Literal["ADMINISTRATOR"],
         "principalId": str,
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
 SharedFileSystemConfigurationTypeDef = TypedDict(
     "SharedFileSystemConfigurationTypeDef",
     {
         "endpoint": str,
         "fileSystemId": str,
         "linuxMountPoint": str,
         "shareName": str,
@@ -992,40 +1245,44 @@
     {
         "backupId": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class StartStreamingSessionRequestRequestTypeDef(
     _RequiredStartStreamingSessionRequestRequestTypeDef,
     _OptionalStartStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartStudioSSOConfigurationRepairRequestRequestTypeDef = TypedDict(
     "_RequiredStartStudioSSOConfigurationRepairRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalStartStudioSSOConfigurationRepairRequestRequestTypeDef = TypedDict(
     "_OptionalStartStudioSSOConfigurationRepairRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class StartStudioSSOConfigurationRepairRequestRequestTypeDef(
     _RequiredStartStudioSSOConfigurationRepairRequestRequestTypeDef,
     _OptionalStartStudioSSOConfigurationRepairRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStopStreamingSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStopStreamingSessionRequestRequestTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1034,20 +1291,22 @@
     {
         "clientToken": str,
         "volumeRetentionMode": VolumeRetentionModeType,
     },
     total=False,
 )
 
+
 class StopStreamingSessionRequestRequestTypeDef(
     _RequiredStopStreamingSessionRequestRequestTypeDef,
     _OptionalStopStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
+
 StreamConfigurationSessionBackupTypeDef = TypedDict(
     "StreamConfigurationSessionBackupTypeDef",
     {
         "maxBackupsToRetain": int,
         "mode": SessionBackupModeType,
     },
     total=False,
@@ -1082,39 +1341,43 @@
     "_OptionalStreamingImageEncryptionConfigurationTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
 
+
 class StreamingImageEncryptionConfigurationTypeDef(
     _RequiredStreamingImageEncryptionConfigurationTypeDef,
     _OptionalStreamingImageEncryptionConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1132,20 +1395,22 @@
     "_OptionalUpdateLaunchProfileMemberRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateLaunchProfileMemberRequestRequestTypeDef(
     _RequiredUpdateLaunchProfileMemberRequestRequestTypeDef,
     _OptionalUpdateLaunchProfileMemberRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateStreamingImageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingImageRequestRequestTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -1155,20 +1420,22 @@
         "clientToken": str,
         "description": str,
         "name": str,
     },
     total=False,
 )
 
+
 class UpdateStreamingImageRequestRequestTypeDef(
     _RequiredUpdateStreamingImageRequestRequestTypeDef,
     _OptionalUpdateStreamingImageRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateStudioRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStudioRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalUpdateStudioRequestRequestTypeDef = TypedDict(
@@ -1178,41 +1445,35 @@
         "clientToken": str,
         "displayName": str,
         "userRoleArn": str,
     },
     total=False,
 )
 
+
 class UpdateStudioRequestRequestTypeDef(
     _RequiredUpdateStudioRequestRequestTypeDef, _OptionalUpdateStudioRequestRequestTypeDef
 ):
     pass
 
+
 AcceptEulasResponseTypeDef = TypedDict(
     "AcceptEulasResponseTypeDef",
     {
         "eulaAcceptances": List[EulaAcceptanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEulaAcceptancesResponseTypeDef = TypedDict(
     "ListEulaAcceptancesResponseTypeDef",
     {
         "eulaAcceptances": List[EulaAcceptanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActiveDirectoryConfigurationTypeDef = TypedDict(
     "ActiveDirectoryConfigurationTypeDef",
     {
         "computerAttributes": Sequence[ActiveDirectoryComputerAttributeTypeDef],
@@ -1236,23 +1497,23 @@
     total=False,
 )
 
 CreateStreamingSessionStreamResponseTypeDef = TypedDict(
     "CreateStreamingSessionStreamResponseTypeDef",
     {
         "stream": StreamingSessionStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStreamingSessionStreamResponseTypeDef = TypedDict(
     "GetStreamingSessionStreamResponseTypeDef",
     {
         "stream": StreamingSessionStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateStudioRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStudioRequestRequestTypeDef",
     {
         "adminRoleArn": str,
@@ -1267,19 +1528,21 @@
         "clientToken": str,
         "studioEncryptionConfiguration": StudioEncryptionConfigurationTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStudioRequestRequestTypeDef(
     _RequiredCreateStudioRequestRequestTypeDef, _OptionalCreateStudioRequestRequestTypeDef
 ):
     pass
 
+
 StudioTypeDef = TypedDict(
     "StudioTypeDef",
     {
         "adminRoleArn": str,
         "arn": str,
         "createdAt": datetime,
         "displayName": str,
@@ -1299,49 +1562,49 @@
     total=False,
 )
 
 GetEulaResponseTypeDef = TypedDict(
     "GetEulaResponseTypeDef",
     {
         "eula": EulaTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEulasResponseTypeDef = TypedDict(
     "ListEulasResponseTypeDef",
     {
         "eulas": List[EulaTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLaunchProfileMemberResponseTypeDef = TypedDict(
     "GetLaunchProfileMemberResponseTypeDef",
     {
         "member": LaunchProfileMembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLaunchProfileMembersResponseTypeDef = TypedDict(
     "ListLaunchProfileMembersResponseTypeDef",
     {
         "members": List[LaunchProfileMembershipTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLaunchProfileMemberResponseTypeDef = TypedDict(
     "UpdateLaunchProfileMemberResponseTypeDef",
     {
         "member": LaunchProfileMembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef = TypedDict(
     "_RequiredGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef",
     {
         "launchProfileId": str,
@@ -1352,20 +1615,22 @@
     "_OptionalGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef(
     _RequiredGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef,
     _OptionalGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef = TypedDict(
     "_RequiredGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -1373,20 +1638,22 @@
     "_OptionalGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetLaunchProfileRequestLaunchProfileReadyWaitTypeDef(
     _RequiredGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef,
     _OptionalGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingImageRequestStreamingImageDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingImageRequestStreamingImageDeletedWaitTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -1394,20 +1661,22 @@
     "_OptionalGetStreamingImageRequestStreamingImageDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingImageRequestStreamingImageDeletedWaitTypeDef(
     _RequiredGetStreamingImageRequestStreamingImageDeletedWaitTypeDef,
     _OptionalGetStreamingImageRequestStreamingImageDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingImageRequestStreamingImageReadyWaitTypeDef = TypedDict(
     "_RequiredGetStreamingImageRequestStreamingImageReadyWaitTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -1415,20 +1684,22 @@
     "_OptionalGetStreamingImageRequestStreamingImageReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingImageRequestStreamingImageReadyWaitTypeDef(
     _RequiredGetStreamingImageRequestStreamingImageReadyWaitTypeDef,
     _OptionalGetStreamingImageRequestStreamingImageReadyWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1436,20 +1707,22 @@
     "_OptionalGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef(
     _RequiredGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef,
     _OptionalGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1457,20 +1730,22 @@
     "_OptionalGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingSessionRequestStreamingSessionReadyWaitTypeDef(
     _RequiredGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef,
     _OptionalGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1478,20 +1753,22 @@
     "_OptionalGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef(
     _RequiredGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef,
     _OptionalGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef",
     {
         "sessionId": str,
         "streamId": str,
         "studioId": str,
     },
@@ -1500,20 +1777,22 @@
     "_OptionalGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef(
     _RequiredGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef,
     _OptionalGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStudioComponentRequestStudioComponentDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStudioComponentRequestStudioComponentDeletedWaitTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -1521,20 +1800,22 @@
     "_OptionalGetStudioComponentRequestStudioComponentDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStudioComponentRequestStudioComponentDeletedWaitTypeDef(
     _RequiredGetStudioComponentRequestStudioComponentDeletedWaitTypeDef,
     _OptionalGetStudioComponentRequestStudioComponentDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStudioComponentRequestStudioComponentReadyWaitTypeDef = TypedDict(
     "_RequiredGetStudioComponentRequestStudioComponentReadyWaitTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -1542,279 +1823,97 @@
     "_OptionalGetStudioComponentRequestStudioComponentReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStudioComponentRequestStudioComponentReadyWaitTypeDef(
     _RequiredGetStudioComponentRequestStudioComponentReadyWaitTypeDef,
     _OptionalGetStudioComponentRequestStudioComponentReadyWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStudioRequestStudioDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStudioRequestStudioDeletedWaitTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalGetStudioRequestStudioDeletedWaitTypeDef = TypedDict(
     "_OptionalGetStudioRequestStudioDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStudioRequestStudioDeletedWaitTypeDef(
     _RequiredGetStudioRequestStudioDeletedWaitTypeDef,
     _OptionalGetStudioRequestStudioDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStudioRequestStudioReadyWaitTypeDef = TypedDict(
     "_RequiredGetStudioRequestStudioReadyWaitTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalGetStudioRequestStudioReadyWaitTypeDef = TypedDict(
     "_OptionalGetStudioRequestStudioReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStudioRequestStudioReadyWaitTypeDef(
     _RequiredGetStudioRequestStudioReadyWaitTypeDef, _OptionalGetStudioRequestStudioReadyWaitTypeDef
 ):
     pass
 
+
 GetStreamingSessionBackupResponseTypeDef = TypedDict(
     "GetStreamingSessionBackupResponseTypeDef",
     {
         "streamingSessionBackup": StreamingSessionBackupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamingSessionBackupsResponseTypeDef = TypedDict(
     "ListStreamingSessionBackupsResponseTypeDef",
     {
         "nextToken": str,
         "streamingSessionBackups": List[StreamingSessionBackupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStudioMemberResponseTypeDef = TypedDict(
     "GetStudioMemberResponseTypeDef",
     {
         "member": StudioMembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStudioMembersResponseTypeDef = TypedDict(
     "ListStudioMembersResponseTypeDef",
     {
         "members": List[StudioMembershipTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
-    "_RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = TypedDict(
-    "_OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef",
-    {
-        "eulaIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef(
-    _RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
-    _OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
-):
-    pass
-
-ListEulasRequestListEulasPaginateTypeDef = TypedDict(
-    "ListEulasRequestListEulasPaginateTypeDef",
-    {
-        "eulaIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
-    {
-        "launchProfileId": str,
-        "studioId": str,
-    },
-)
-_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef(
-    _RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
-    _OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
-):
-    pass
-
-_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
-    {
-        "principalId": str,
-        "states": Sequence[LaunchProfileStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef(
-    _RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
-    _OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
-):
-    pass
-
-_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
-    "_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
-    "_OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
-    {
-        "owner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListStreamingImagesRequestListStreamingImagesPaginateTypeDef(
-    _RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
-    _OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
-):
-    pass
-
-_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
-    "_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
-    "_OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
-    {
-        "ownedBy": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef(
-    _RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
-    _OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
-):
-    pass
-
-_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
-    {
-        "createdBy": str,
-        "ownedBy": str,
-        "sessionIds": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef(
-    _RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
-    _OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
-    "_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
-    "_OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
-    {
-        "states": Sequence[StudioComponentStateType],
-        "types": Sequence[StudioComponentTypeType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListStudioComponentsRequestListStudioComponentsPaginateTypeDef(
-    _RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
-    _OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
-):
-    pass
-
-_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
-    "_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef",
-    {
-        "studioId": str,
-    },
-)
-_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
-    "_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-class ListStudioMembersRequestListStudioMembersPaginateTypeDef(
-    _RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef,
-    _OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef,
-):
-    pass
-
-ListStudiosRequestListStudiosPaginateTypeDef = TypedDict(
-    "ListStudiosRequestListStudiosPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 _RequiredPutLaunchProfileMembersRequestRequestTypeDef = TypedDict(
     "_RequiredPutLaunchProfileMembersRequestRequestTypeDef",
     {
         "identityStoreId": str,
         "launchProfileId": str,
@@ -1826,20 +1925,22 @@
     "_OptionalPutLaunchProfileMembersRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class PutLaunchProfileMembersRequestRequestTypeDef(
     _RequiredPutLaunchProfileMembersRequestRequestTypeDef,
     _OptionalPutLaunchProfileMembersRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutStudioMembersRequestRequestTypeDef = TypedDict(
     "_RequiredPutStudioMembersRequestRequestTypeDef",
     {
         "identityStoreId": str,
         "members": Sequence[NewStudioMemberTypeDef],
         "studioId": str,
     },
@@ -1848,19 +1949,21 @@
     "_OptionalPutStudioMembersRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class PutStudioMembersRequestRequestTypeDef(
     _RequiredPutStudioMembersRequestRequestTypeDef, _OptionalPutStudioMembersRequestRequestTypeDef
 ):
     pass
 
+
 StreamingSessionTypeDef = TypedDict(
     "StreamingSessionTypeDef",
     {
         "arn": str,
         "automaticTerminationMode": AutomaticTerminationModeType,
         "backupMode": SessionBackupModeType,
         "createdAt": datetime,
@@ -1901,20 +2004,22 @@
     "_OptionalStreamConfigurationSessionStorageTypeDef",
     {
         "root": StreamingSessionStorageRootTypeDef,
     },
     total=False,
 )
 
+
 class StreamConfigurationSessionStorageTypeDef(
     _RequiredStreamConfigurationSessionStorageTypeDef,
     _OptionalStreamConfigurationSessionStorageTypeDef,
 ):
     pass
 
+
 StreamingImageTypeDef = TypedDict(
     "StreamingImageTypeDef",
     {
         "arn": str,
         "description": str,
         "ec2ImageId": str,
         "encryptionConfiguration": StreamingImageEncryptionConfigurationTypeDef,
@@ -1958,105 +2063,105 @@
     total=False,
 )
 
 CreateStudioResponseTypeDef = TypedDict(
     "CreateStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteStudioResponseTypeDef = TypedDict(
     "DeleteStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStudioResponseTypeDef = TypedDict(
     "GetStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStudiosResponseTypeDef = TypedDict(
     "ListStudiosResponseTypeDef",
     {
         "nextToken": str,
         "studios": List[StudioTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartStudioSSOConfigurationRepairResponseTypeDef = TypedDict(
     "StartStudioSSOConfigurationRepairResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStudioResponseTypeDef = TypedDict(
     "UpdateStudioResponseTypeDef",
     {
         "studio": StudioTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStreamingSessionResponseTypeDef = TypedDict(
     "CreateStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteStreamingSessionResponseTypeDef = TypedDict(
     "DeleteStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStreamingSessionResponseTypeDef = TypedDict(
     "GetStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamingSessionsResponseTypeDef = TypedDict(
     "ListStreamingSessionsResponseTypeDef",
     {
         "nextToken": str,
         "sessions": List[StreamingSessionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartStreamingSessionResponseTypeDef = TypedDict(
     "StartStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopStreamingSessionResponseTypeDef = TypedDict(
     "StopStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStreamConfigurationCreateTypeDef = TypedDict(
     "_RequiredStreamConfigurationCreateTypeDef",
     {
         "clipboardMode": StreamingClipboardModeType,
@@ -2074,19 +2179,21 @@
         "sessionPersistenceMode": SessionPersistenceModeType,
         "sessionStorage": StreamConfigurationSessionStorageTypeDef,
         "volumeConfiguration": VolumeConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class StreamConfigurationCreateTypeDef(
     _RequiredStreamConfigurationCreateTypeDef, _OptionalStreamConfigurationCreateTypeDef
 ):
     pass
 
+
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "clipboardMode": StreamingClipboardModeType,
         "ec2InstanceTypes": List[StreamingInstanceTypeType],
         "streamingImageIds": List[str],
     },
@@ -2101,57 +2208,59 @@
         "sessionPersistenceMode": SessionPersistenceModeType,
         "sessionStorage": StreamConfigurationSessionStorageTypeDef,
         "volumeConfiguration": VolumeConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
+
 CreateStreamingImageResponseTypeDef = TypedDict(
     "CreateStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteStreamingImageResponseTypeDef = TypedDict(
     "DeleteStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStreamingImageResponseTypeDef = TypedDict(
     "GetStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamingImagesResponseTypeDef = TypedDict(
     "ListStreamingImagesResponseTypeDef",
     {
         "nextToken": str,
         "streamingImages": List[StreamingImageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStreamingImageResponseTypeDef = TypedDict(
     "UpdateStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStudioComponentRequestRequestTypeDef",
     {
         "name": str,
@@ -2172,20 +2281,22 @@
         "secureInitializationRoleArn": str,
         "subtype": StudioComponentSubtypeType,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStudioComponentRequestRequestTypeDef(
     _RequiredCreateStudioComponentRequestRequestTypeDef,
     _OptionalCreateStudioComponentRequestRequestTypeDef,
 ):
     pass
 
+
 StudioComponentTypeDef = TypedDict(
     "StudioComponentTypeDef",
     {
         "arn": str,
         "configuration": StudioComponentConfigurationTypeDef,
         "createdAt": datetime,
         "createdBy": str,
@@ -2230,25 +2341,27 @@
         "secureInitializationRoleArn": str,
         "subtype": StudioComponentSubtypeType,
         "type": StudioComponentTypeType,
     },
     total=False,
 )
 
+
 class UpdateStudioComponentRequestRequestTypeDef(
     _RequiredUpdateStudioComponentRequestRequestTypeDef,
     _OptionalUpdateStudioComponentRequestRequestTypeDef,
 ):
     pass
 
+
 GetLaunchProfileInitializationResponseTypeDef = TypedDict(
     "GetLaunchProfileInitializationResponseTypeDef",
     {
         "launchProfileInitialization": LaunchProfileInitializationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchProfileRequestRequestTypeDef",
     {
         "ec2SubnetIds": Sequence[str],
@@ -2265,20 +2378,22 @@
         "clientToken": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateLaunchProfileRequestRequestTypeDef(
     _RequiredCreateLaunchProfileRequestRequestTypeDef,
     _OptionalCreateLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchProfileRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -2291,20 +2406,22 @@
         "name": str,
         "streamConfiguration": StreamConfigurationCreateTypeDef,
         "studioComponentIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateLaunchProfileRequestRequestTypeDef(
     _RequiredUpdateLaunchProfileRequestRequestTypeDef,
     _OptionalUpdateLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
+
 LaunchProfileTypeDef = TypedDict(
     "LaunchProfileTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "createdBy": str,
         "description": str,
@@ -2325,94 +2442,94 @@
     total=False,
 )
 
 CreateStudioComponentResponseTypeDef = TypedDict(
     "CreateStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteStudioComponentResponseTypeDef = TypedDict(
     "DeleteStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStudioComponentResponseTypeDef = TypedDict(
     "GetStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStudioComponentsResponseTypeDef = TypedDict(
     "ListStudioComponentsResponseTypeDef",
     {
         "nextToken": str,
         "studioComponents": List[StudioComponentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStudioComponentResponseTypeDef = TypedDict(
     "UpdateStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateLaunchProfileResponseTypeDef = TypedDict(
     "CreateLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteLaunchProfileResponseTypeDef = TypedDict(
     "DeleteLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLaunchProfileDetailsResponseTypeDef = TypedDict(
     "GetLaunchProfileDetailsResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
         "streamingImages": List[StreamingImageTypeDef],
         "studioComponentSummaries": List[StudioComponentSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLaunchProfileResponseTypeDef = TypedDict(
     "GetLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLaunchProfilesResponseTypeDef = TypedDict(
     "ListLaunchProfilesResponseTypeDef",
     {
         "launchProfiles": List[LaunchProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLaunchProfileResponseTypeDef = TypedDict(
     "UpdateLaunchProfileResponseTypeDef",
     {
         "launchProfile": LaunchProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/waiter.py` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble/waiter.pyi` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble.egg-info/PKG-INFO` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-nimble
-Version: 1.26.34
-Summary: Type annotations for boto3.NimbleStudio 1.26.34 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.NimbleStudio 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-nimble"></a>
 
 # mypy-boto3-nimble
 
 [![PyPI - mypy-boto3-nimble](https://img.shields.io/pypi/v/mypy-boto3-nimble.svg?color=blue)](https://pypi.org/project/mypy-boto3-nimble)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-nimble.svg?color=blue)](https://pypi.org/project/mypy-boto3-nimble)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-nimble?color=blue)](https://pypistats.org/packages/mypy-boto3-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NimbleStudio 1.26.34](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[boto3.NimbleStudio 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
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
 [mypy-boto3-nimble docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/).
 
 See how it helps to find and fix potential bugs:
 
@@ -468,15 +468,14 @@
 `mypy_boto3_nimble.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_nimble.type_defs import (
     AcceptEulasRequestRequestTypeDef,
     EulaAcceptanceTypeDef,
-    ResponseMetadataTypeDef,
     ActiveDirectoryComputerAttributeTypeDef,
     ComputeFarmConfigurationTypeDef,
     CreateStreamingImageRequestRequestTypeDef,
     CreateStreamingSessionRequestRequestTypeDef,
     CreateStreamingSessionStreamRequestRequestTypeDef,
     StreamingSessionStreamTypeDef,
     ScriptParameterKeyValueTypeDef,
@@ -506,28 +505,40 @@
     GetStudioComponentRequestRequestTypeDef,
     GetStudioMemberRequestRequestTypeDef,
     StudioMembershipTypeDef,
     GetStudioRequestRequestTypeDef,
     LaunchProfileInitializationScriptTypeDef,
     ValidationResultTypeDef,
     LicenseServiceConfigurationTypeDef,
-    PaginatorConfigTypeDef,
+    ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
     ListEulaAcceptancesRequestRequestTypeDef,
+    ListEulasRequestListEulasPaginateTypeDef,
     ListEulasRequestRequestTypeDef,
+    ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
     ListLaunchProfileMembersRequestRequestTypeDef,
+    ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
     ListLaunchProfilesRequestRequestTypeDef,
+    ListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
     ListStreamingImagesRequestRequestTypeDef,
+    ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
     ListStreamingSessionBackupsRequestRequestTypeDef,
+    ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
     ListStreamingSessionsRequestRequestTypeDef,
+    ListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
     ListStudioComponentsRequestRequestTypeDef,
+    ListStudioMembersRequestListStudioMembersPaginateTypeDef,
     ListStudioMembersRequestRequestTypeDef,
+    ListStudiosRequestListStudiosPaginateTypeDef,
     ListStudiosRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SharedFileSystemConfigurationTypeDef,
     StartStreamingSessionRequestRequestTypeDef,
     StartStudioSSOConfigurationRepairRequestRequestTypeDef,
     StopStreamingSessionRequestRequestTypeDef,
     StreamConfigurationSessionBackupTypeDef,
     VolumeConfigurationTypeDef,
     StreamingSessionStorageRootTypeDef,
@@ -535,15 +546,14 @@
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLaunchProfileMemberRequestRequestTypeDef,
     UpdateStreamingImageRequestRequestTypeDef,
     UpdateStudioRequestRequestTypeDef,
     AcceptEulasResponseTypeDef,
     ListEulaAcceptancesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ActiveDirectoryConfigurationTypeDef,
     LaunchProfileInitializationActiveDirectoryTypeDef,
     CreateStreamingSessionStreamResponseTypeDef,
     GetStreamingSessionStreamResponseTypeDef,
     CreateStudioRequestRequestTypeDef,
     StudioTypeDef,
     GetEulaResponseTypeDef,
@@ -563,24 +573,14 @@
     GetStudioComponentRequestStudioComponentReadyWaitTypeDef,
     GetStudioRequestStudioDeletedWaitTypeDef,
     GetStudioRequestStudioReadyWaitTypeDef,
     GetStreamingSessionBackupResponseTypeDef,
     ListStreamingSessionBackupsResponseTypeDef,
     GetStudioMemberResponseTypeDef,
     ListStudioMembersResponseTypeDef,
-    ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
-    ListEulasRequestListEulasPaginateTypeDef,
-    ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
-    ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
-    ListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
-    ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
-    ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
-    ListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
-    ListStudioMembersRequestListStudioMembersPaginateTypeDef,
-    ListStudiosRequestListStudiosPaginateTypeDef,
     PutLaunchProfileMembersRequestRequestTypeDef,
     PutStudioMembersRequestRequestTypeDef,
     StreamingSessionTypeDef,
     StreamConfigurationSessionStorageTypeDef,
     StreamingImageTypeDef,
     StudioComponentConfigurationTypeDef,
     LaunchProfileInitializationTypeDef,
@@ -631,42 +631,42 @@
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

### Comparing `mypy-boto3-nimble-1.26.34/mypy_boto3_nimble.egg-info/SOURCES.txt` & `mypy-boto3-nimble-1.27.0/mypy_boto3_nimble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.26.34/setup.py` & `mypy-boto3-nimble-1.27.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-nimble.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-nimble",
-    version="1.26.34",
+    version="1.27.0",
     packages=["mypy_boto3_nimble"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.NimbleStudio 1.26.34 service generated with mypy-boto3-builder"
-        " 7.12.0"
+        "Type annotations for boto3.NimbleStudio 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/",
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


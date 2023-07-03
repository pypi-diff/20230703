# Comparing `tmp/mypy-boto3-serverlessrepo-1.26.59.tar.gz` & `tmp/mypy-boto3-serverlessrepo-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-serverlessrepo-1.26.59.tar", last modified: Fri Jan 27 20:32:52 2023, max compression
+gzip compressed data, was "mypy-boto3-serverlessrepo-1.27.0.tar", last modified: Mon Jul  3 19:51:26 2023, max compression
```

## Comparing `mypy-boto3-serverlessrepo-1.26.59.tar` & `mypy-boto3-serverlessrepo-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:52.656097 mypy-boto3-serverlessrepo-1.26.59/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-01-27 20:32:52.656097 mypy-boto3-serverlessrepo-1.26.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:52.656097 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19275 2023-01-27 20:32:40.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19245 2023-01-27 20:32:40.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:52.656097 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-01-27 20:32:52.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-27 20:32:52.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:52.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:52.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 20:32:52.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-27 20:32:52.000000 mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 20:32:52.656097 mypy-boto3-serverlessrepo-1.26.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-01-27 20:32:39.000000 mypy-boto3-serverlessrepo-1.26.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.539982 mypy-boto3-serverlessrepo-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-07-03 19:51:26.539982 mypy-boto3-serverlessrepo-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.539982 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.539982 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-07-03 19:51:26.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:51:26.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:26.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:26.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:26.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:51:26.000000 mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:26.539982 mypy-boto3-serverlessrepo-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-03 19:47:53.000000 mypy-boto3-serverlessrepo-1.27.0/setup.py
```

### Comparing `mypy-boto3-serverlessrepo-1.26.59/LICENSE` & `mypy-boto3-serverlessrepo-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-serverlessrepo-1.26.59/PKG-INFO` & `mypy-boto3-serverlessrepo-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-serverlessrepo
-Version: 1.26.59
-Summary: Type annotations for boto3.ServerlessApplicationRepository 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ServerlessApplicationRepository 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-serverlessrepo"></a>
 
 # mypy-boto3-serverlessrepo
 
 [![PyPI - mypy-boto3-serverlessrepo](https://img.shields.io/pypi/v/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-serverlessrepo?color=blue)](https://pypistats.org/packages/mypy-boto3-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServerlessApplicationRepository 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[boto3.ServerlessApplicationRepository 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,46 +338,46 @@
 
 ```python
 from mypy_boto3_serverlessrepo.type_defs import (
     ApplicationDependencySummaryTypeDef,
     ApplicationPolicyStatementTypeDef,
     ApplicationSummaryTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateApplicationVersionRequestRequestTypeDef,
     ParameterDefinitionTypeDef,
     ParameterValueTypeDef,
     TagTypeDef,
+    CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateRequestRequestTypeDef,
+    CreateCloudFormationTemplateResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApplicationPolicyRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetCloudFormationTemplateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetCloudFormationTemplateResponseTypeDef,
+    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
     ListApplicationDependenciesRequestRequestTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     VersionSummaryTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RollbackTriggerTypeDef,
     UnshareApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    PutApplicationPolicyRequestRequestTypeDef,
-    CreateCloudFormationChangeSetResponseTypeDef,
-    CreateCloudFormationTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetApplicationPolicyResponseTypeDef,
-    GetCloudFormationTemplateResponseTypeDef,
     ListApplicationDependenciesResponseTypeDef,
-    ListApplicationsResponseTypeDef,
+    GetApplicationPolicyResponseTypeDef,
+    PutApplicationPolicyRequestRequestTypeDef,
     PutApplicationPolicyResponseTypeDef,
+    ListApplicationsResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     VersionTypeDef,
-    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationVersionsResponseTypeDef,
     RollbackConfigurationTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     CreateCloudFormationChangeSetRequestRequestTypeDef,
 )
@@ -390,42 +390,42 @@
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

### Comparing `mypy-boto3-serverlessrepo-1.26.59/README.md` & `mypy-boto3-serverlessrepo-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-serverlessrepo"></a>
 
 # mypy-boto3-serverlessrepo
 
 [![PyPI - mypy-boto3-serverlessrepo](https://img.shields.io/pypi/v/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-serverlessrepo?color=blue)](https://pypistats.org/packages/mypy-boto3-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServerlessApplicationRepository 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[boto3.ServerlessApplicationRepository 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,46 +306,46 @@
 
 ```python
 from mypy_boto3_serverlessrepo.type_defs import (
     ApplicationDependencySummaryTypeDef,
     ApplicationPolicyStatementTypeDef,
     ApplicationSummaryTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateApplicationVersionRequestRequestTypeDef,
     ParameterDefinitionTypeDef,
     ParameterValueTypeDef,
     TagTypeDef,
+    CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateRequestRequestTypeDef,
+    CreateCloudFormationTemplateResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApplicationPolicyRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetCloudFormationTemplateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetCloudFormationTemplateResponseTypeDef,
+    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
     ListApplicationDependenciesRequestRequestTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     VersionSummaryTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RollbackTriggerTypeDef,
     UnshareApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    PutApplicationPolicyRequestRequestTypeDef,
-    CreateCloudFormationChangeSetResponseTypeDef,
-    CreateCloudFormationTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetApplicationPolicyResponseTypeDef,
-    GetCloudFormationTemplateResponseTypeDef,
     ListApplicationDependenciesResponseTypeDef,
-    ListApplicationsResponseTypeDef,
+    GetApplicationPolicyResponseTypeDef,
+    PutApplicationPolicyRequestRequestTypeDef,
     PutApplicationPolicyResponseTypeDef,
+    ListApplicationsResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     VersionTypeDef,
-    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationVersionsResponseTypeDef,
     RollbackConfigurationTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     CreateCloudFormationChangeSetRequestRequestTypeDef,
 )
@@ -358,42 +358,42 @@
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

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/__init__.py` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/__init__.pyi` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/__main__.py` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServerlessApplicationRepository 1.26.59\nVersion:        "
-        " 1.26.59\nBuilder version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.ServerlessApplicationRepository 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.59")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/client.py` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/client.pyi` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/literals.py` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -91,21 +92,23 @@
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
@@ -184,14 +187,15 @@
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
@@ -202,14 +206,15 @@
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
@@ -245,14 +250,15 @@
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
@@ -271,16 +277,19 @@
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
@@ -360,18 +369,21 @@
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

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/literals.pyi` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
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
@@ -89,21 +90,23 @@
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
@@ -182,14 +185,15 @@
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
@@ -200,14 +204,15 @@
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
@@ -243,14 +248,15 @@
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
@@ -269,16 +275,19 @@
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
@@ -358,18 +367,21 @@
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

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/paginator.py` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,43 +58,43 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         SemanticVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationDependenciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationDependencies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationdependenciespaginator)
         """
 
 
 class ListApplicationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationversionspaginator)
     """
 
     def paginate(
-        self, *, ApplicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ApplicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationversionspaginator)
         """
 
 
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationspaginator)
         """
```

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/paginator.pyi` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,41 +55,41 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         SemanticVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationDependenciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationDependencies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationdependenciespaginator)
         """
 
 class ListApplicationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationversionspaginator)
     """
 
     def paginate(
-        self, *, ApplicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ApplicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationversionspaginator)
         """
 
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationspaginator)
         """
```

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/type_defs.py` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,46 +23,46 @@
 
 
 __all__ = (
     "ApplicationDependencySummaryTypeDef",
     "ApplicationPolicyStatementTypeDef",
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateApplicationVersionRequestRequestTypeDef",
     "ParameterDefinitionTypeDef",
     "ParameterValueTypeDef",
     "TagTypeDef",
+    "CreateCloudFormationChangeSetResponseTypeDef",
     "CreateCloudFormationTemplateRequestRequestTypeDef",
+    "CreateCloudFormationTemplateResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetApplicationPolicyRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetCloudFormationTemplateRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetCloudFormationTemplateResponseTypeDef",
+    "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
     "ListApplicationDependenciesRequestRequestTypeDef",
+    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "VersionSummaryTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RollbackTriggerTypeDef",
     "UnshareApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "PutApplicationPolicyRequestRequestTypeDef",
-    "CreateCloudFormationChangeSetResponseTypeDef",
-    "CreateCloudFormationTemplateResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetApplicationPolicyResponseTypeDef",
-    "GetCloudFormationTemplateResponseTypeDef",
     "ListApplicationDependenciesResponseTypeDef",
-    "ListApplicationsResponseTypeDef",
+    "GetApplicationPolicyResponseTypeDef",
+    "PutApplicationPolicyRequestRequestTypeDef",
     "PutApplicationPolicyResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
     "CreateApplicationVersionResponseTypeDef",
     "VersionTypeDef",
-    "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
-    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "RollbackConfigurationTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "CreateCloudFormationChangeSetRequestRequestTypeDef",
 )
@@ -155,25 +155,14 @@
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
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
 _RequiredCreateApplicationVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationVersionRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SemanticVersion": str,
     },
 )
@@ -240,14 +229,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
+    "CreateCloudFormationChangeSetResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "ChangeSetId": str,
+        "SemanticVersion": str,
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCloudFormationTemplateRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalCreateCloudFormationTemplateRequestRequestTypeDef = TypedDict(
@@ -262,21 +262,42 @@
 class CreateCloudFormationTemplateRequestRequestTypeDef(
     _RequiredCreateCloudFormationTemplateRequestRequestTypeDef,
     _OptionalCreateCloudFormationTemplateRequestRequestTypeDef,
 ):
     pass
 
 
+CreateCloudFormationTemplateResponseTypeDef = TypedDict(
+    "CreateCloudFormationTemplateResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "CreationTime": str,
+        "ExpirationTime": str,
+        "SemanticVersion": str,
+        "Status": StatusType,
+        "TemplateId": str,
+        "TemplateUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetApplicationPolicyRequestRequestTypeDef = TypedDict(
     "GetApplicationPolicyRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -305,24 +326,51 @@
     "GetCloudFormationTemplateRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "TemplateId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetCloudFormationTemplateResponseTypeDef = TypedDict(
+    "GetCloudFormationTemplateResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ApplicationId": str,
+        "CreationTime": str,
+        "ExpirationTime": str,
+        "SemanticVersion": str,
+        "Status": StatusType,
+        "TemplateId": str,
+        "TemplateUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    {
+        "SemanticVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(
+    _RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    _OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListApplicationDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationDependenciesRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalListApplicationDependenciesRequestRequestTypeDef = TypedDict(
@@ -339,14 +387,36 @@
 class ListApplicationDependenciesRequestRequestTypeDef(
     _RequiredListApplicationDependenciesRequestRequestTypeDef,
     _OptionalListApplicationDependenciesRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
+    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -383,23 +453,52 @@
 )
 
 
 class VersionSummaryTypeDef(_RequiredVersionSummaryTypeDef, _OptionalVersionSummaryTypeDef):
     pass
 
 
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxItems": int,
         "NextToken": str,
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
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
         "Type": str,
     },
 )
@@ -434,99 +533,53 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-PutApplicationPolicyRequestRequestTypeDef = TypedDict(
-    "PutApplicationPolicyRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
-    },
-)
-
-CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
-    "CreateCloudFormationChangeSetResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "ChangeSetId": str,
-        "SemanticVersion": str,
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCloudFormationTemplateResponseTypeDef = TypedDict(
-    "CreateCloudFormationTemplateResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "CreationTime": str,
-        "ExpirationTime": str,
-        "SemanticVersion": str,
-        "Status": StatusType,
-        "TemplateId": str,
-        "TemplateUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ListApplicationDependenciesResponseTypeDef = TypedDict(
+    "ListApplicationDependenciesResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Dependencies": List[ApplicationDependencySummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationPolicyResponseTypeDef = TypedDict(
     "GetApplicationPolicyResponseTypeDef",
     {
         "Statements": List[ApplicationPolicyStatementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetCloudFormationTemplateResponseTypeDef = TypedDict(
-    "GetCloudFormationTemplateResponseTypeDef",
+PutApplicationPolicyRequestRequestTypeDef = TypedDict(
+    "PutApplicationPolicyRequestRequestTypeDef",
     {
         "ApplicationId": str,
-        "CreationTime": str,
-        "ExpirationTime": str,
-        "SemanticVersion": str,
-        "Status": StatusType,
-        "TemplateId": str,
-        "TemplateUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
     },
 )
 
-ListApplicationDependenciesResponseTypeDef = TypedDict(
-    "ListApplicationDependenciesResponseTypeDef",
+PutApplicationPolicyResponseTypeDef = TypedDict(
+    "PutApplicationPolicyResponseTypeDef",
     {
-        "Dependencies": List[ApplicationDependencySummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Statements": List[ApplicationPolicyStatementTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "Applications": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutApplicationPolicyResponseTypeDef = TypedDict(
-    "PutApplicationPolicyResponseTypeDef",
-    {
-        "Statements": List[ApplicationPolicyStatementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateApplicationVersionResponseTypeDef = TypedDict(
     "CreateApplicationVersionResponseTypeDef",
     {
         "ApplicationId": str,
@@ -534,15 +587,15 @@
         "ParameterDefinitions": List[ParameterDefinitionTypeDef],
         "RequiredCapabilities": List[CapabilityType],
         "ResourcesSupported": bool,
         "SemanticVersion": str,
         "SourceCodeArchiveUrl": str,
         "SourceCodeUrl": str,
         "TemplateUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredVersionTypeDef = TypedDict(
     "_RequiredVersionTypeDef",
     {
         "ApplicationId": str,
@@ -564,73 +617,20 @@
 )
 
 
 class VersionTypeDef(_RequiredVersionTypeDef, _OptionalVersionTypeDef):
     pass
 
 
-_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
-    {
-        "SemanticVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(
-    _RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-    _OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
-    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListApplicationVersionsResponseTypeDef = TypedDict(
     "ListApplicationVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
         "MonitoringTimeInMinutes": int,
@@ -651,15 +651,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "ApplicationId": str,
@@ -671,15 +671,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "ApplicationId": str,
@@ -691,15 +691,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCloudFormationChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCloudFormationChangeSetRequestRequestTypeDef",
     {
         "ApplicationId": str,
```

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo/type_defs.pyi` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,46 +22,46 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApplicationDependencySummaryTypeDef",
     "ApplicationPolicyStatementTypeDef",
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateApplicationVersionRequestRequestTypeDef",
     "ParameterDefinitionTypeDef",
     "ParameterValueTypeDef",
     "TagTypeDef",
+    "CreateCloudFormationChangeSetResponseTypeDef",
     "CreateCloudFormationTemplateRequestRequestTypeDef",
+    "CreateCloudFormationTemplateResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetApplicationPolicyRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetCloudFormationTemplateRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetCloudFormationTemplateResponseTypeDef",
+    "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
     "ListApplicationDependenciesRequestRequestTypeDef",
+    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "VersionSummaryTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RollbackTriggerTypeDef",
     "UnshareApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "PutApplicationPolicyRequestRequestTypeDef",
-    "CreateCloudFormationChangeSetResponseTypeDef",
-    "CreateCloudFormationTemplateResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetApplicationPolicyResponseTypeDef",
-    "GetCloudFormationTemplateResponseTypeDef",
     "ListApplicationDependenciesResponseTypeDef",
-    "ListApplicationsResponseTypeDef",
+    "GetApplicationPolicyResponseTypeDef",
+    "PutApplicationPolicyRequestRequestTypeDef",
     "PutApplicationPolicyResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
     "CreateApplicationVersionResponseTypeDef",
     "VersionTypeDef",
-    "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
-    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "RollbackConfigurationTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "CreateCloudFormationChangeSetRequestRequestTypeDef",
 )
@@ -148,25 +148,14 @@
 )
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
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
 _RequiredCreateApplicationVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationVersionRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SemanticVersion": str,
     },
 )
@@ -229,14 +218,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
+    "CreateCloudFormationChangeSetResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "ChangeSetId": str,
+        "SemanticVersion": str,
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCloudFormationTemplateRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalCreateCloudFormationTemplateRequestRequestTypeDef = TypedDict(
@@ -249,21 +249,42 @@
 
 class CreateCloudFormationTemplateRequestRequestTypeDef(
     _RequiredCreateCloudFormationTemplateRequestRequestTypeDef,
     _OptionalCreateCloudFormationTemplateRequestRequestTypeDef,
 ):
     pass
 
+CreateCloudFormationTemplateResponseTypeDef = TypedDict(
+    "CreateCloudFormationTemplateResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "CreationTime": str,
+        "ExpirationTime": str,
+        "SemanticVersion": str,
+        "Status": StatusType,
+        "TemplateId": str,
+        "TemplateUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetApplicationPolicyRequestRequestTypeDef = TypedDict(
     "GetApplicationPolicyRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -290,24 +311,49 @@
     "GetCloudFormationTemplateRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "TemplateId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetCloudFormationTemplateResponseTypeDef = TypedDict(
+    "GetCloudFormationTemplateResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ApplicationId": str,
+        "CreationTime": str,
+        "ExpirationTime": str,
+        "SemanticVersion": str,
+        "Status": StatusType,
+        "TemplateId": str,
+        "TemplateUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    {
+        "SemanticVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(
+    _RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    _OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+):
+    pass
+
 _RequiredListApplicationDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationDependenciesRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalListApplicationDependenciesRequestRequestTypeDef = TypedDict(
@@ -322,14 +368,34 @@
 
 class ListApplicationDependenciesRequestRequestTypeDef(
     _RequiredListApplicationDependenciesRequestRequestTypeDef,
     _OptionalListApplicationDependenciesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
+    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -362,23 +428,52 @@
     },
     total=False,
 )
 
 class VersionSummaryTypeDef(_RequiredVersionSummaryTypeDef, _OptionalVersionSummaryTypeDef):
     pass
 
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxItems": int,
         "NextToken": str,
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
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
         "Type": str,
     },
 )
@@ -411,99 +506,53 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-PutApplicationPolicyRequestRequestTypeDef = TypedDict(
-    "PutApplicationPolicyRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
-    },
-)
-
-CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
-    "CreateCloudFormationChangeSetResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "ChangeSetId": str,
-        "SemanticVersion": str,
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCloudFormationTemplateResponseTypeDef = TypedDict(
-    "CreateCloudFormationTemplateResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "CreationTime": str,
-        "ExpirationTime": str,
-        "SemanticVersion": str,
-        "Status": StatusType,
-        "TemplateId": str,
-        "TemplateUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ListApplicationDependenciesResponseTypeDef = TypedDict(
+    "ListApplicationDependenciesResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Dependencies": List[ApplicationDependencySummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationPolicyResponseTypeDef = TypedDict(
     "GetApplicationPolicyResponseTypeDef",
     {
         "Statements": List[ApplicationPolicyStatementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetCloudFormationTemplateResponseTypeDef = TypedDict(
-    "GetCloudFormationTemplateResponseTypeDef",
+PutApplicationPolicyRequestRequestTypeDef = TypedDict(
+    "PutApplicationPolicyRequestRequestTypeDef",
     {
         "ApplicationId": str,
-        "CreationTime": str,
-        "ExpirationTime": str,
-        "SemanticVersion": str,
-        "Status": StatusType,
-        "TemplateId": str,
-        "TemplateUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
     },
 )
 
-ListApplicationDependenciesResponseTypeDef = TypedDict(
-    "ListApplicationDependenciesResponseTypeDef",
+PutApplicationPolicyResponseTypeDef = TypedDict(
+    "PutApplicationPolicyResponseTypeDef",
     {
-        "Dependencies": List[ApplicationDependencySummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Statements": List[ApplicationPolicyStatementTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "Applications": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutApplicationPolicyResponseTypeDef = TypedDict(
-    "PutApplicationPolicyResponseTypeDef",
-    {
-        "Statements": List[ApplicationPolicyStatementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateApplicationVersionResponseTypeDef = TypedDict(
     "CreateApplicationVersionResponseTypeDef",
     {
         "ApplicationId": str,
@@ -511,15 +560,15 @@
         "ParameterDefinitions": List[ParameterDefinitionTypeDef],
         "RequiredCapabilities": List[CapabilityType],
         "ResourcesSupported": bool,
         "SemanticVersion": str,
         "SourceCodeArchiveUrl": str,
         "SourceCodeUrl": str,
         "TemplateUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredVersionTypeDef = TypedDict(
     "_RequiredVersionTypeDef",
     {
         "ApplicationId": str,
@@ -539,69 +588,20 @@
     },
     total=False,
 )
 
 class VersionTypeDef(_RequiredVersionTypeDef, _OptionalVersionTypeDef):
     pass
 
-_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
-    {
-        "SemanticVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(
-    _RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-    _OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-):
-    pass
-
-_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
-    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-):
-    pass
-
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListApplicationVersionsResponseTypeDef = TypedDict(
     "ListApplicationVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
         "MonitoringTimeInMinutes": int,
@@ -622,15 +622,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "ApplicationId": str,
@@ -642,15 +642,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "ApplicationId": str,
@@ -662,15 +662,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCloudFormationChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCloudFormationChangeSetRequestRequestTypeDef",
     {
         "ApplicationId": str,
```

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo.egg-info/PKG-INFO` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-serverlessrepo
-Version: 1.26.59
-Summary: Type annotations for boto3.ServerlessApplicationRepository 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ServerlessApplicationRepository 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-serverlessrepo"></a>
 
 # mypy-boto3-serverlessrepo
 
 [![PyPI - mypy-boto3-serverlessrepo](https://img.shields.io/pypi/v/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-serverlessrepo?color=blue)](https://pypistats.org/packages/mypy-boto3-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServerlessApplicationRepository 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[boto3.ServerlessApplicationRepository 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,46 +338,46 @@
 
 ```python
 from mypy_boto3_serverlessrepo.type_defs import (
     ApplicationDependencySummaryTypeDef,
     ApplicationPolicyStatementTypeDef,
     ApplicationSummaryTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateApplicationVersionRequestRequestTypeDef,
     ParameterDefinitionTypeDef,
     ParameterValueTypeDef,
     TagTypeDef,
+    CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateRequestRequestTypeDef,
+    CreateCloudFormationTemplateResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApplicationPolicyRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetCloudFormationTemplateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetCloudFormationTemplateResponseTypeDef,
+    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
     ListApplicationDependenciesRequestRequestTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     VersionSummaryTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RollbackTriggerTypeDef,
     UnshareApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    PutApplicationPolicyRequestRequestTypeDef,
-    CreateCloudFormationChangeSetResponseTypeDef,
-    CreateCloudFormationTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetApplicationPolicyResponseTypeDef,
-    GetCloudFormationTemplateResponseTypeDef,
     ListApplicationDependenciesResponseTypeDef,
-    ListApplicationsResponseTypeDef,
+    GetApplicationPolicyResponseTypeDef,
+    PutApplicationPolicyRequestRequestTypeDef,
     PutApplicationPolicyResponseTypeDef,
+    ListApplicationsResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     VersionTypeDef,
-    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationVersionsResponseTypeDef,
     RollbackConfigurationTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     CreateCloudFormationChangeSetRequestRequestTypeDef,
 )
@@ -390,42 +390,42 @@
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

### Comparing `mypy-boto3-serverlessrepo-1.26.59/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt` & `mypy-boto3-serverlessrepo-1.27.0/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.26.59/setup.py` & `mypy-boto3-serverlessrepo-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-serverlessrepo.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-serverlessrepo",
-    version="1.26.59",
+    version="1.27.0",
     packages=["mypy_boto3_serverlessrepo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServerlessApplicationRepository 1.26.59 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.ServerlessApplicationRepository 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/",
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


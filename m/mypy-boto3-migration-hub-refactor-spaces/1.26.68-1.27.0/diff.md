# Comparing `tmp/mypy-boto3-migration-hub-refactor-spaces-1.26.68.tar.gz` & `tmp/mypy-boto3-migration-hub-refactor-spaces-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migration-hub-refactor-spaces-1.26.68.tar", last modified: Thu Feb  9 20:26:50 2023, max compression
+gzip compressed data, was "mypy-boto3-migration-hub-refactor-spaces-1.27.0.tar", last modified: Mon Jul  3 19:51:08 2023, max compression
```

## Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68.tar` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.998837 mypy-boto3-migration-hub-refactor-spaces-1.26.68/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-02-09 20:26:49.986837 mypy-boto3-migration-hub-refactor-spaces-1.26.68/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.982837 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28256 2023-02-09 20:26:34.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28227 2023-02-09 20:26:34.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.986837 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-02-09 20:26:49.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-09 20:26:49.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 20:26:49.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-09 20:26:49.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 20:26:49.998837 mypy-boto3-migration-hub-refactor-spaces-1.26.68/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.671689 mypy-boto3-migration-hub-refactor-spaces-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-07-03 19:51:08.671689 mypy-boto3-migration-hub-refactor-spaces-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.659689 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28408 2023-07-03 19:42:24.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-07-03 19:42:24.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.671689 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-07-03 19:51:08.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-03 19:51:08.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:08.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 19:51:08.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:08.671689 mypy-boto3-migration-hub-refactor-spaces-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-03 19:42:23.000000 mypy-boto3-migration-hub-refactor-spaces-1.27.0/setup.py
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/LICENSE` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/PKG-INFO` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migration-hub-refactor-spaces
-Version: 1.26.68
-Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.26.68 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-migration-hub-refactor-spaces"></a>
 
 # mypy-boto3-migration-hub-refactor-spaces
 
 [![PyPI - mypy-boto3-migration-hub-refactor-spaces](https://img.shields.io/pypi/v/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migration-hub-refactor-spaces?color=blue)](https://pypistats.org/packages/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,73 +352,73 @@
 
 ```python
 from mypy_boto3_migration_hub_refactor_spaces.type_defs import (
     ApiGatewayProxyConfigTypeDef,
     ApiGatewayProxyInputTypeDef,
     ApiGatewayProxySummaryTypeDef,
     ErrorResponseTypeDef,
-    ResponseMetadataTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
+    CreateEnvironmentResponseTypeDef,
     DefaultRouteInputTypeDef,
     UriPathRouteInputTypeDef,
     LambdaEndpointInputTypeDef,
     UrlEndpointInputTypeDef,
     DeleteApplicationRequestRequestTypeDef,
+    DeleteApplicationResponseTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
+    DeleteEnvironmentResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
+    DeleteRouteResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
+    DeleteServiceResponseTypeDef,
     EnvironmentVpcTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetRouteRequestRequestTypeDef,
     GetServiceRequestRequestTypeDef,
     LambdaEndpointConfigTypeDef,
     UrlEndpointConfigTypeDef,
     LambdaEndpointSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
     ListEnvironmentVpcsRequestRequestTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
+    ListRoutesRequestListRoutesPaginateTypeDef,
     ListRoutesRequestRequestTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UrlEndpointSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRouteRequestRequestTypeDef,
+    UpdateRouteResponseTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    CreateApplicationResponseTypeDef,
     ApplicationSummaryTypeDef,
     EnvironmentSummaryTypeDef,
-    RouteSummaryTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    DeleteApplicationResponseTypeDef,
-    DeleteEnvironmentResponseTypeDef,
-    DeleteRouteResponseTypeDef,
-    DeleteServiceResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetEnvironmentResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRouteResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateRouteResponseTypeDef,
+    RouteSummaryTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     GetServiceResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
-    ListRoutesRequestListRoutesPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ServiceSummaryTypeDef,
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
 )
 
@@ -430,42 +430,42 @@
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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/README.md` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-migration-hub-refactor-spaces"></a>
 
 # mypy-boto3-migration-hub-refactor-spaces
 
 [![PyPI - mypy-boto3-migration-hub-refactor-spaces](https://img.shields.io/pypi/v/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migration-hub-refactor-spaces?color=blue)](https://pypistats.org/packages/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,73 +320,73 @@
 
 ```python
 from mypy_boto3_migration_hub_refactor_spaces.type_defs import (
     ApiGatewayProxyConfigTypeDef,
     ApiGatewayProxyInputTypeDef,
     ApiGatewayProxySummaryTypeDef,
     ErrorResponseTypeDef,
-    ResponseMetadataTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
+    CreateEnvironmentResponseTypeDef,
     DefaultRouteInputTypeDef,
     UriPathRouteInputTypeDef,
     LambdaEndpointInputTypeDef,
     UrlEndpointInputTypeDef,
     DeleteApplicationRequestRequestTypeDef,
+    DeleteApplicationResponseTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
+    DeleteEnvironmentResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
+    DeleteRouteResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
+    DeleteServiceResponseTypeDef,
     EnvironmentVpcTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetRouteRequestRequestTypeDef,
     GetServiceRequestRequestTypeDef,
     LambdaEndpointConfigTypeDef,
     UrlEndpointConfigTypeDef,
     LambdaEndpointSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
     ListEnvironmentVpcsRequestRequestTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
+    ListRoutesRequestListRoutesPaginateTypeDef,
     ListRoutesRequestRequestTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UrlEndpointSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRouteRequestRequestTypeDef,
+    UpdateRouteResponseTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    CreateApplicationResponseTypeDef,
     ApplicationSummaryTypeDef,
     EnvironmentSummaryTypeDef,
-    RouteSummaryTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    DeleteApplicationResponseTypeDef,
-    DeleteEnvironmentResponseTypeDef,
-    DeleteRouteResponseTypeDef,
-    DeleteServiceResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetEnvironmentResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRouteResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateRouteResponseTypeDef,
+    RouteSummaryTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     GetServiceResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
-    ListRoutesRequestListRoutesPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ServiceSummaryTypeDef,
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
 )
 
@@ -398,42 +398,42 @@
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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/__init__.py` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/__main__.py` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubRefactorSpaces 1.26.68\nVersion:        "
-        " 1.26.68\nBuilder version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.MigrationHubRefactorSpaces 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces\nOther"
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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/client.py` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/client.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/literals.py` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApiGatewayEndpointTypeType",
     "ApplicationStateType",
     "EnvironmentStateType",
     "ErrorCodeType",
     "ErrorResourceTypeType",
     "HttpMethodType",
@@ -40,15 +39,14 @@
     "ServiceStateType",
     "MigrationHubRefactorSpacesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ApiGatewayEndpointTypeType = Literal["PRIVATE", "REGIONAL"]
 ApplicationStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 EnvironmentStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 ErrorCodeType = Literal[
     "INVALID_RESOURCE_STATE",
     "NOT_AUTHORIZED",
     "REQUEST_LIMIT_EXCEEDED",
@@ -108,14 +106,15 @@
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
@@ -155,14 +154,15 @@
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
@@ -241,14 +241,15 @@
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
@@ -259,14 +260,15 @@
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
@@ -302,14 +304,15 @@
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
@@ -328,16 +331,19 @@
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
@@ -417,18 +423,21 @@
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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/literals.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ApiGatewayEndpointTypeType",
     "ApplicationStateType",
     "EnvironmentStateType",
     "ErrorCodeType",
     "ErrorResourceTypeType",
     "HttpMethodType",
@@ -39,14 +40,15 @@
     "ServiceStateType",
     "MigrationHubRefactorSpacesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 ApiGatewayEndpointTypeType = Literal["PRIVATE", "REGIONAL"]
 ApplicationStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 EnvironmentStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 ErrorCodeType = Literal[
     "INVALID_RESOURCE_STATE",
     "NOT_AUTHORIZED",
     "REQUEST_LIMIT_EXCEEDED",
@@ -106,14 +108,15 @@
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
@@ -153,14 +156,15 @@
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
@@ -239,14 +243,15 @@
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
@@ -257,14 +262,15 @@
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
@@ -300,14 +306,15 @@
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
@@ -326,16 +333,19 @@
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
@@ -415,18 +425,21 @@
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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/paginator.py` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,45 +62,45 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, EnvironmentIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, EnvironmentIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listapplicationspaginator)
         """
 
 
 class ListEnvironmentVpcsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironmentVpcs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentvpcspaginator)
     """
 
     def paginate(
-        self, *, EnvironmentIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, EnvironmentIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentVpcsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironmentVpcs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentvpcspaginator)
         """
 
 
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentspaginator)
         """
 
 
@@ -111,15 +111,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRoutesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listroutespaginator)
         """
 
 
@@ -130,13 +130,13 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listservicespaginator)
         """
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -59,43 +59,43 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, EnvironmentIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, EnvironmentIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listapplicationspaginator)
         """
 
 class ListEnvironmentVpcsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironmentVpcs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentvpcspaginator)
     """
 
     def paginate(
-        self, *, EnvironmentIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, EnvironmentIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentVpcsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironmentVpcs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentvpcspaginator)
         """
 
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentspaginator)
         """
 
 class ListRoutesPaginator(Paginator):
@@ -105,15 +105,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRoutesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listroutespaginator)
         """
 
 class ListServicesPaginator(Paginator):
@@ -123,13 +123,13 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listservicespaginator)
         """
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/type_defs.py` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,73 +41,73 @@
 
 
 __all__ = (
     "ApiGatewayProxyConfigTypeDef",
     "ApiGatewayProxyInputTypeDef",
     "ApiGatewayProxySummaryTypeDef",
     "ErrorResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
+    "CreateEnvironmentResponseTypeDef",
     "DefaultRouteInputTypeDef",
     "UriPathRouteInputTypeDef",
     "LambdaEndpointInputTypeDef",
     "UrlEndpointInputTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
+    "DeleteApplicationResponseTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
+    "DeleteEnvironmentResponseTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
+    "DeleteRouteResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
+    "DeleteServiceResponseTypeDef",
     "EnvironmentVpcTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "GetRouteRequestRequestTypeDef",
     "GetServiceRequestRequestTypeDef",
     "LambdaEndpointConfigTypeDef",
     "UrlEndpointConfigTypeDef",
     "LambdaEndpointSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
     "ListEnvironmentVpcsRequestRequestTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
+    "ListRoutesRequestListRoutesPaginateTypeDef",
     "ListRoutesRequestRequestTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UrlEndpointSummaryTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRouteRequestRequestTypeDef",
+    "UpdateRouteResponseTypeDef",
     "CreateApplicationRequestRequestTypeDef",
+    "CreateApplicationResponseTypeDef",
     "ApplicationSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
-    "RouteSummaryTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "CreateEnvironmentResponseTypeDef",
-    "DeleteApplicationResponseTypeDef",
-    "DeleteEnvironmentResponseTypeDef",
-    "DeleteRouteResponseTypeDef",
-    "DeleteServiceResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "GetEnvironmentResponseTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetRouteResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateRouteResponseTypeDef",
+    "RouteSummaryTypeDef",
     "CreateRouteRequestRequestTypeDef",
     "CreateRouteResponseTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "ListEnvironmentVpcsResponseTypeDef",
     "GetServiceResponseTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    "ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    "ListRoutesRequestListRoutesPaginateTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ServiceSummaryTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "ListRoutesResponseTypeDef",
     "ListServicesResponseTypeDef",
 )
 
@@ -157,25 +157,14 @@
         "Message": str,
         "ResourceIdentifier": str,
         "ResourceType": ErrorResourceTypeType,
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
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "Name": str,
         "NetworkFabricType": NetworkFabricTypeType,
     },
 )
@@ -192,14 +181,31 @@
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
 
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedTime": datetime,
+        "Description": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "NetworkFabricType": NetworkFabricTypeType,
+        "OwnerAccountId": str,
+        "State": EnvironmentStateType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DefaultRouteInputTypeDef = TypedDict(
     "DefaultRouteInputTypeDef",
     {
         "ActivationState": RouteActivationStateType,
     },
     total=False,
 )
@@ -210,14 +216,15 @@
         "ActivationState": RouteActivationStateType,
         "SourcePath": str,
     },
 )
 _OptionalUriPathRouteInputTypeDef = TypedDict(
     "_OptionalUriPathRouteInputTypeDef",
     {
+        "AppendSourcePath": bool,
         "IncludeChildPaths": bool,
         "Methods": Sequence[HttpMethodType],
     },
     total=False,
 )
 
 
@@ -257,21 +264,46 @@
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
 
+DeleteApplicationResponseTypeDef = TypedDict(
+    "DeleteApplicationResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "State": ApplicationStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
     },
 )
 
+DeleteEnvironmentResponseTypeDef = TypedDict(
+    "DeleteEnvironmentResponseTypeDef",
+    {
+        "Arn": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "State": EnvironmentStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -280,23 +312,50 @@
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "RouteIdentifier": str,
     },
 )
 
+DeleteRouteResponseTypeDef = TypedDict(
+    "DeleteRouteResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "LastUpdatedTime": datetime,
+        "RouteId": str,
+        "ServiceId": str,
+        "State": RouteStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "ServiceIdentifier": str,
     },
 )
 
+DeleteServiceResponseTypeDef = TypedDict(
+    "DeleteServiceResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "ServiceId": str,
+        "State": ServiceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnvironmentVpcTypeDef = TypedDict(
     "EnvironmentVpcTypeDef",
     {
         "AccountId": str,
         "CidrBlocks": List[str],
         "CreatedTime": datetime,
         "EnvironmentId": str,
@@ -325,14 +384,22 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRouteRequestRequestTypeDef = TypedDict(
     "GetRouteRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "RouteIdentifier": str,
     },
@@ -368,24 +435,36 @@
     "LambdaEndpointSummaryTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationsRequestListApplicationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListApplicationsRequestListApplicationsPaginateTypeDef(
+    _RequiredListApplicationsRequestListApplicationsPaginateTypeDef,
+    _OptionalListApplicationsRequestListApplicationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListApplicationsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationsRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
     },
 )
 _OptionalListApplicationsRequestRequestTypeDef = TypedDict(
@@ -400,14 +479,36 @@
 
 class ListApplicationsRequestRequestTypeDef(
     _RequiredListApplicationsRequestRequestTypeDef, _OptionalListApplicationsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
+    "_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
+    {
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
+    "_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef(
+    _RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
+    _OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEnvironmentVpcsRequestRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentVpcsRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
     },
 )
 _OptionalListEnvironmentVpcsRequestRequestTypeDef = TypedDict(
@@ -423,23 +524,54 @@
 class ListEnvironmentVpcsRequestRequestTypeDef(
     _RequiredListEnvironmentVpcsRequestRequestTypeDef,
     _OptionalListEnvironmentVpcsRequestRequestTypeDef,
 ):
     pass
 
 
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListRoutesRequestListRoutesPaginateTypeDef",
+    {
+        "ApplicationIdentifier": str,
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListRoutesRequestListRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRoutesRequestListRoutesPaginateTypeDef(
+    _RequiredListRoutesRequestListRoutesPaginateTypeDef,
+    _OptionalListRoutesRequestListRoutesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutesRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
@@ -455,14 +587,37 @@
 
 class ListRoutesRequestRequestTypeDef(
     _RequiredListRoutesRequestRequestTypeDef, _OptionalListRoutesRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "_RequiredListServicesRequestListServicesPaginateTypeDef",
+    {
+        "ApplicationIdentifier": str,
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "_OptionalListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListServicesRequestListServicesPaginateTypeDef(
+    _RequiredListServicesRequestListServicesPaginateTypeDef,
+    _OptionalListServicesRequestListServicesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListServicesRequestRequestTypeDef = TypedDict(
     "_RequiredListServicesRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
@@ -485,22 +640,51 @@
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "Policy": str,
         "ResourceArn": str,
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
 UrlEndpointSummaryTypeDef = TypedDict(
     "UrlEndpointSummaryTypeDef",
     {
         "HealthUrl": str,
         "Url": str,
     },
     total=False,
@@ -528,14 +712,27 @@
         "ActivationState": RouteActivationStateType,
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "RouteIdentifier": str,
     },
 )
 
+UpdateRouteResponseTypeDef = TypedDict(
+    "UpdateRouteResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "LastUpdatedTime": datetime,
+        "RouteId": str,
+        "ServiceId": str,
+        "State": RouteStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
         "Name": str,
         "ProxyType": Literal["API_GATEWAY"],
         "VpcId": str,
@@ -554,165 +751,72 @@
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-ApplicationSummaryTypeDef = TypedDict(
-    "ApplicationSummaryTypeDef",
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
     {
-        "ApiGatewayProxy": ApiGatewayProxySummaryTypeDef,
+        "ApiGatewayProxy": ApiGatewayProxyInputTypeDef,
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
         "EnvironmentId": str,
-        "Error": ErrorResponseTypeDef,
         "LastUpdatedTime": datetime,
         "Name": str,
         "OwnerAccountId": str,
         "ProxyType": Literal["API_GATEWAY"],
         "State": ApplicationStateType,
         "Tags": Dict[str, str],
         "VpcId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-EnvironmentSummaryTypeDef = TypedDict(
-    "EnvironmentSummaryTypeDef",
-    {
-        "Arn": str,
-        "CreatedTime": datetime,
-        "Description": str,
-        "EnvironmentId": str,
-        "Error": ErrorResponseTypeDef,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "NetworkFabricType": NetworkFabricTypeType,
-        "OwnerAccountId": str,
-        "State": EnvironmentStateType,
-        "Tags": Dict[str, str],
-        "TransitGatewayId": str,
-    },
-    total=False,
-)
-
-RouteSummaryTypeDef = TypedDict(
-    "RouteSummaryTypeDef",
+ApplicationSummaryTypeDef = TypedDict(
+    "ApplicationSummaryTypeDef",
     {
+        "ApiGatewayProxy": ApiGatewayProxySummaryTypeDef,
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
         "EnvironmentId": str,
         "Error": ErrorResponseTypeDef,
-        "IncludeChildPaths": bool,
-        "LastUpdatedTime": datetime,
-        "Methods": List[HttpMethodType],
-        "OwnerAccountId": str,
-        "PathResourceToId": Dict[str, str],
-        "RouteId": str,
-        "RouteType": RouteTypeType,
-        "ServiceId": str,
-        "SourcePath": str,
-        "State": RouteStateType,
-        "Tags": Dict[str, str],
-    },
-    total=False,
-)
-
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "ApiGatewayProxy": ApiGatewayProxyInputTypeDef,
-        "ApplicationId": str,
-        "Arn": str,
-        "CreatedByAccountId": str,
-        "CreatedTime": datetime,
-        "EnvironmentId": str,
         "LastUpdatedTime": datetime,
         "Name": str,
         "OwnerAccountId": str,
         "ProxyType": Literal["API_GATEWAY"],
         "State": ApplicationStateType,
         "Tags": Dict[str, str],
         "VpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
+EnvironmentSummaryTypeDef = TypedDict(
+    "EnvironmentSummaryTypeDef",
     {
         "Arn": str,
         "CreatedTime": datetime,
         "Description": str,
         "EnvironmentId": str,
+        "Error": ErrorResponseTypeDef,
         "LastUpdatedTime": datetime,
         "Name": str,
         "NetworkFabricType": NetworkFabricTypeType,
         "OwnerAccountId": str,
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteApplicationResponseTypeDef = TypedDict(
-    "DeleteApplicationResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "State": ApplicationStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteEnvironmentResponseTypeDef = TypedDict(
-    "DeleteEnvironmentResponseTypeDef",
-    {
-        "Arn": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "State": EnvironmentStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRouteResponseTypeDef = TypedDict(
-    "DeleteRouteResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "LastUpdatedTime": datetime,
-        "RouteId": str,
-        "ServiceId": str,
-        "State": RouteStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteServiceResponseTypeDef = TypedDict(
-    "DeleteServiceResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "ServiceId": str,
-        "State": ServiceStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TransitGatewayId": str,
     },
+    total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "ApiGatewayProxy": ApiGatewayProxyConfigTypeDef,
         "ApplicationId": str,
@@ -724,15 +828,15 @@
         "LastUpdatedTime": datetime,
         "Name": str,
         "OwnerAccountId": str,
         "ProxyType": Literal["API_GATEWAY"],
         "State": ApplicationStateType,
         "Tags": Dict[str, str],
         "VpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "Arn": str,
@@ -743,29 +847,22 @@
         "LastUpdatedTime": datetime,
         "Name": str,
         "NetworkFabricType": NetworkFabricTypeType,
         "OwnerAccountId": str,
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
         "TransitGatewayId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRouteResponseTypeDef = TypedDict(
     "GetRouteResponseTypeDef",
     {
+        "AppendSourcePath": bool,
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
         "EnvironmentId": str,
         "Error": ErrorResponseTypeDef,
         "IncludeChildPaths": bool,
@@ -775,37 +872,41 @@
         "PathResourceToId": Dict[str, str],
         "RouteId": str,
         "RouteType": RouteTypeType,
         "ServiceId": str,
         "SourcePath": str,
         "State": RouteStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRouteResponseTypeDef = TypedDict(
-    "UpdateRouteResponseTypeDef",
+RouteSummaryTypeDef = TypedDict(
+    "RouteSummaryTypeDef",
     {
+        "AppendSourcePath": bool,
         "ApplicationId": str,
         "Arn": str,
+        "CreatedByAccountId": str,
+        "CreatedTime": datetime,
+        "EnvironmentId": str,
+        "Error": ErrorResponseTypeDef,
+        "IncludeChildPaths": bool,
         "LastUpdatedTime": datetime,
+        "Methods": List[HttpMethodType],
+        "OwnerAccountId": str,
+        "PathResourceToId": Dict[str, str],
         "RouteId": str,
+        "RouteType": RouteTypeType,
         "ServiceId": str,
+        "SourcePath": str,
         "State": RouteStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": Dict[str, str],
     },
+    total=False,
 )
 
 _RequiredCreateRouteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
@@ -842,15 +943,15 @@
         "OwnerAccountId": str,
         "RouteId": str,
         "RouteType": RouteTypeType,
         "ServiceId": str,
         "State": RouteStateType,
         "Tags": Dict[str, str],
         "UriPathRoute": UriPathRouteInputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
@@ -894,24 +995,24 @@
         "Name": str,
         "OwnerAccountId": str,
         "ServiceId": str,
         "State": ServiceStateType,
         "Tags": Dict[str, str],
         "UrlEndpoint": UrlEndpointInputTypeDef,
         "VpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentVpcsResponseTypeDef = TypedDict(
     "ListEnvironmentVpcsResponseTypeDef",
     {
         "EnvironmentVpcList": List[EnvironmentVpcTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "ApplicationId": str,
@@ -927,116 +1028,18 @@
         "Name": str,
         "OwnerAccountId": str,
         "ServiceId": str,
         "State": ServiceStateType,
         "Tags": Dict[str, str],
         "UrlEndpoint": UrlEndpointConfigTypeDef,
         "VpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListApplicationsRequestListApplicationsPaginateTypeDef(
-    _RequiredListApplicationsRequestListApplicationsPaginateTypeDef,
-    _OptionalListApplicationsRequestListApplicationsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
-    "_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
-    {
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
-    "_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef(
-    _RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-    _OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-):
-    pass
-
-
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListRoutesRequestListRoutesPaginateTypeDef",
-    {
-        "ApplicationIdentifier": str,
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListRoutesRequestListRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRoutesRequestListRoutesPaginateTypeDef(
-    _RequiredListRoutesRequestListRoutesPaginateTypeDef,
-    _OptionalListRoutesRequestListRoutesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "_RequiredListServicesRequestListServicesPaginateTypeDef",
-    {
-        "ApplicationIdentifier": str,
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "_OptionalListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListServicesRequestListServicesPaginateTypeDef(
-    _RequiredListServicesRequestListServicesPaginateTypeDef,
-    _OptionalListServicesRequestListServicesPaginateTypeDef,
-):
-    pass
-
-
 ServiceSummaryTypeDef = TypedDict(
     "ServiceSummaryTypeDef",
     {
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
@@ -1058,37 +1061,37 @@
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationSummaryList": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "EnvironmentSummaryList": List[EnvironmentSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRoutesResponseTypeDef = TypedDict(
     "ListRoutesResponseTypeDef",
     {
         "NextToken": str,
         "RouteSummaryList": List[RouteSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "NextToken": str,
         "ServiceSummaryList": List[ServiceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -40,73 +40,73 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApiGatewayProxyConfigTypeDef",
     "ApiGatewayProxyInputTypeDef",
     "ApiGatewayProxySummaryTypeDef",
     "ErrorResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
+    "CreateEnvironmentResponseTypeDef",
     "DefaultRouteInputTypeDef",
     "UriPathRouteInputTypeDef",
     "LambdaEndpointInputTypeDef",
     "UrlEndpointInputTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
+    "DeleteApplicationResponseTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
+    "DeleteEnvironmentResponseTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
+    "DeleteRouteResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
+    "DeleteServiceResponseTypeDef",
     "EnvironmentVpcTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "GetRouteRequestRequestTypeDef",
     "GetServiceRequestRequestTypeDef",
     "LambdaEndpointConfigTypeDef",
     "UrlEndpointConfigTypeDef",
     "LambdaEndpointSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
     "ListEnvironmentVpcsRequestRequestTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
+    "ListRoutesRequestListRoutesPaginateTypeDef",
     "ListRoutesRequestRequestTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UrlEndpointSummaryTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRouteRequestRequestTypeDef",
+    "UpdateRouteResponseTypeDef",
     "CreateApplicationRequestRequestTypeDef",
+    "CreateApplicationResponseTypeDef",
     "ApplicationSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
-    "RouteSummaryTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "CreateEnvironmentResponseTypeDef",
-    "DeleteApplicationResponseTypeDef",
-    "DeleteEnvironmentResponseTypeDef",
-    "DeleteRouteResponseTypeDef",
-    "DeleteServiceResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "GetEnvironmentResponseTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetRouteResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateRouteResponseTypeDef",
+    "RouteSummaryTypeDef",
     "CreateRouteRequestRequestTypeDef",
     "CreateRouteResponseTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "ListEnvironmentVpcsResponseTypeDef",
     "GetServiceResponseTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    "ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    "ListRoutesRequestListRoutesPaginateTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ServiceSummaryTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "ListRoutesResponseTypeDef",
     "ListServicesResponseTypeDef",
 )
 
@@ -156,25 +156,14 @@
         "Message": str,
         "ResourceIdentifier": str,
         "ResourceType": ErrorResourceTypeType,
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
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "Name": str,
         "NetworkFabricType": NetworkFabricTypeType,
     },
 )
@@ -189,14 +178,31 @@
 )
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedTime": datetime,
+        "Description": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "NetworkFabricType": NetworkFabricTypeType,
+        "OwnerAccountId": str,
+        "State": EnvironmentStateType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DefaultRouteInputTypeDef = TypedDict(
     "DefaultRouteInputTypeDef",
     {
         "ActivationState": RouteActivationStateType,
     },
     total=False,
 )
@@ -207,14 +213,15 @@
         "ActivationState": RouteActivationStateType,
         "SourcePath": str,
     },
 )
 _OptionalUriPathRouteInputTypeDef = TypedDict(
     "_OptionalUriPathRouteInputTypeDef",
     {
+        "AppendSourcePath": bool,
         "IncludeChildPaths": bool,
         "Methods": Sequence[HttpMethodType],
     },
     total=False,
 )
 
 class UriPathRouteInputTypeDef(
@@ -250,21 +257,46 @@
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
 
+DeleteApplicationResponseTypeDef = TypedDict(
+    "DeleteApplicationResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "State": ApplicationStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
     },
 )
 
+DeleteEnvironmentResponseTypeDef = TypedDict(
+    "DeleteEnvironmentResponseTypeDef",
+    {
+        "Arn": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "State": EnvironmentStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -273,23 +305,50 @@
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "RouteIdentifier": str,
     },
 )
 
+DeleteRouteResponseTypeDef = TypedDict(
+    "DeleteRouteResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "LastUpdatedTime": datetime,
+        "RouteId": str,
+        "ServiceId": str,
+        "State": RouteStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "ServiceIdentifier": str,
     },
 )
 
+DeleteServiceResponseTypeDef = TypedDict(
+    "DeleteServiceResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "ServiceId": str,
+        "State": ServiceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnvironmentVpcTypeDef = TypedDict(
     "EnvironmentVpcTypeDef",
     {
         "AccountId": str,
         "CidrBlocks": List[str],
         "CreatedTime": datetime,
         "EnvironmentId": str,
@@ -318,14 +377,22 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRouteRequestRequestTypeDef = TypedDict(
     "GetRouteRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "RouteIdentifier": str,
     },
@@ -361,24 +428,34 @@
     "LambdaEndpointSummaryTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationsRequestListApplicationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListApplicationsRequestListApplicationsPaginateTypeDef(
+    _RequiredListApplicationsRequestListApplicationsPaginateTypeDef,
+    _OptionalListApplicationsRequestListApplicationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListApplicationsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationsRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
     },
 )
 _OptionalListApplicationsRequestRequestTypeDef = TypedDict(
@@ -391,14 +468,34 @@
 )
 
 class ListApplicationsRequestRequestTypeDef(
     _RequiredListApplicationsRequestRequestTypeDef, _OptionalListApplicationsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
+    "_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
+    {
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
+    "_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef(
+    _RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
+    _OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
+):
+    pass
+
 _RequiredListEnvironmentVpcsRequestRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentVpcsRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
     },
 )
 _OptionalListEnvironmentVpcsRequestRequestTypeDef = TypedDict(
@@ -412,23 +509,52 @@
 
 class ListEnvironmentVpcsRequestRequestTypeDef(
     _RequiredListEnvironmentVpcsRequestRequestTypeDef,
     _OptionalListEnvironmentVpcsRequestRequestTypeDef,
 ):
     pass
 
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListRoutesRequestListRoutesPaginateTypeDef",
+    {
+        "ApplicationIdentifier": str,
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListRoutesRequestListRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRoutesRequestListRoutesPaginateTypeDef(
+    _RequiredListRoutesRequestListRoutesPaginateTypeDef,
+    _OptionalListRoutesRequestListRoutesPaginateTypeDef,
+):
+    pass
+
 _RequiredListRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutesRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
@@ -442,14 +568,35 @@
 )
 
 class ListRoutesRequestRequestTypeDef(
     _RequiredListRoutesRequestRequestTypeDef, _OptionalListRoutesRequestRequestTypeDef
 ):
     pass
 
+_RequiredListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "_RequiredListServicesRequestListServicesPaginateTypeDef",
+    {
+        "ApplicationIdentifier": str,
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "_OptionalListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListServicesRequestListServicesPaginateTypeDef(
+    _RequiredListServicesRequestListServicesPaginateTypeDef,
+    _OptionalListServicesRequestListServicesPaginateTypeDef,
+):
+    pass
+
 _RequiredListServicesRequestRequestTypeDef = TypedDict(
     "_RequiredListServicesRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
@@ -470,22 +617,51 @@
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "Policy": str,
         "ResourceArn": str,
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
 UrlEndpointSummaryTypeDef = TypedDict(
     "UrlEndpointSummaryTypeDef",
     {
         "HealthUrl": str,
         "Url": str,
     },
     total=False,
@@ -513,14 +689,27 @@
         "ActivationState": RouteActivationStateType,
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "RouteIdentifier": str,
     },
 )
 
+UpdateRouteResponseTypeDef = TypedDict(
+    "UpdateRouteResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "LastUpdatedTime": datetime,
+        "RouteId": str,
+        "ServiceId": str,
+        "State": RouteStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
         "Name": str,
         "ProxyType": Literal["API_GATEWAY"],
         "VpcId": str,
@@ -537,165 +726,72 @@
 )
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-ApplicationSummaryTypeDef = TypedDict(
-    "ApplicationSummaryTypeDef",
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
     {
-        "ApiGatewayProxy": ApiGatewayProxySummaryTypeDef,
+        "ApiGatewayProxy": ApiGatewayProxyInputTypeDef,
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
         "EnvironmentId": str,
-        "Error": ErrorResponseTypeDef,
         "LastUpdatedTime": datetime,
         "Name": str,
         "OwnerAccountId": str,
         "ProxyType": Literal["API_GATEWAY"],
         "State": ApplicationStateType,
         "Tags": Dict[str, str],
         "VpcId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-EnvironmentSummaryTypeDef = TypedDict(
-    "EnvironmentSummaryTypeDef",
-    {
-        "Arn": str,
-        "CreatedTime": datetime,
-        "Description": str,
-        "EnvironmentId": str,
-        "Error": ErrorResponseTypeDef,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "NetworkFabricType": NetworkFabricTypeType,
-        "OwnerAccountId": str,
-        "State": EnvironmentStateType,
-        "Tags": Dict[str, str],
-        "TransitGatewayId": str,
-    },
-    total=False,
-)
-
-RouteSummaryTypeDef = TypedDict(
-    "RouteSummaryTypeDef",
+ApplicationSummaryTypeDef = TypedDict(
+    "ApplicationSummaryTypeDef",
     {
+        "ApiGatewayProxy": ApiGatewayProxySummaryTypeDef,
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
         "EnvironmentId": str,
         "Error": ErrorResponseTypeDef,
-        "IncludeChildPaths": bool,
-        "LastUpdatedTime": datetime,
-        "Methods": List[HttpMethodType],
-        "OwnerAccountId": str,
-        "PathResourceToId": Dict[str, str],
-        "RouteId": str,
-        "RouteType": RouteTypeType,
-        "ServiceId": str,
-        "SourcePath": str,
-        "State": RouteStateType,
-        "Tags": Dict[str, str],
-    },
-    total=False,
-)
-
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "ApiGatewayProxy": ApiGatewayProxyInputTypeDef,
-        "ApplicationId": str,
-        "Arn": str,
-        "CreatedByAccountId": str,
-        "CreatedTime": datetime,
-        "EnvironmentId": str,
         "LastUpdatedTime": datetime,
         "Name": str,
         "OwnerAccountId": str,
         "ProxyType": Literal["API_GATEWAY"],
         "State": ApplicationStateType,
         "Tags": Dict[str, str],
         "VpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
+EnvironmentSummaryTypeDef = TypedDict(
+    "EnvironmentSummaryTypeDef",
     {
         "Arn": str,
         "CreatedTime": datetime,
         "Description": str,
         "EnvironmentId": str,
+        "Error": ErrorResponseTypeDef,
         "LastUpdatedTime": datetime,
         "Name": str,
         "NetworkFabricType": NetworkFabricTypeType,
         "OwnerAccountId": str,
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteApplicationResponseTypeDef = TypedDict(
-    "DeleteApplicationResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "State": ApplicationStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteEnvironmentResponseTypeDef = TypedDict(
-    "DeleteEnvironmentResponseTypeDef",
-    {
-        "Arn": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "State": EnvironmentStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRouteResponseTypeDef = TypedDict(
-    "DeleteRouteResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "LastUpdatedTime": datetime,
-        "RouteId": str,
-        "ServiceId": str,
-        "State": RouteStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteServiceResponseTypeDef = TypedDict(
-    "DeleteServiceResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "ServiceId": str,
-        "State": ServiceStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TransitGatewayId": str,
     },
+    total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "ApiGatewayProxy": ApiGatewayProxyConfigTypeDef,
         "ApplicationId": str,
@@ -707,15 +803,15 @@
         "LastUpdatedTime": datetime,
         "Name": str,
         "OwnerAccountId": str,
         "ProxyType": Literal["API_GATEWAY"],
         "State": ApplicationStateType,
         "Tags": Dict[str, str],
         "VpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "Arn": str,
@@ -726,29 +822,22 @@
         "LastUpdatedTime": datetime,
         "Name": str,
         "NetworkFabricType": NetworkFabricTypeType,
         "OwnerAccountId": str,
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
         "TransitGatewayId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRouteResponseTypeDef = TypedDict(
     "GetRouteResponseTypeDef",
     {
+        "AppendSourcePath": bool,
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
         "EnvironmentId": str,
         "Error": ErrorResponseTypeDef,
         "IncludeChildPaths": bool,
@@ -758,37 +847,41 @@
         "PathResourceToId": Dict[str, str],
         "RouteId": str,
         "RouteType": RouteTypeType,
         "ServiceId": str,
         "SourcePath": str,
         "State": RouteStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRouteResponseTypeDef = TypedDict(
-    "UpdateRouteResponseTypeDef",
+RouteSummaryTypeDef = TypedDict(
+    "RouteSummaryTypeDef",
     {
+        "AppendSourcePath": bool,
         "ApplicationId": str,
         "Arn": str,
+        "CreatedByAccountId": str,
+        "CreatedTime": datetime,
+        "EnvironmentId": str,
+        "Error": ErrorResponseTypeDef,
+        "IncludeChildPaths": bool,
         "LastUpdatedTime": datetime,
+        "Methods": List[HttpMethodType],
+        "OwnerAccountId": str,
+        "PathResourceToId": Dict[str, str],
         "RouteId": str,
+        "RouteType": RouteTypeType,
         "ServiceId": str,
+        "SourcePath": str,
         "State": RouteStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": Dict[str, str],
     },
+    total=False,
 )
 
 _RequiredCreateRouteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
@@ -823,15 +916,15 @@
         "OwnerAccountId": str,
         "RouteId": str,
         "RouteType": RouteTypeType,
         "ServiceId": str,
         "State": RouteStateType,
         "Tags": Dict[str, str],
         "UriPathRoute": UriPathRouteInputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
@@ -873,24 +966,24 @@
         "Name": str,
         "OwnerAccountId": str,
         "ServiceId": str,
         "State": ServiceStateType,
         "Tags": Dict[str, str],
         "UrlEndpoint": UrlEndpointInputTypeDef,
         "VpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentVpcsResponseTypeDef = TypedDict(
     "ListEnvironmentVpcsResponseTypeDef",
     {
         "EnvironmentVpcList": List[EnvironmentVpcTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "ApplicationId": str,
@@ -906,108 +999,18 @@
         "Name": str,
         "OwnerAccountId": str,
         "ServiceId": str,
         "State": ServiceStateType,
         "Tags": Dict[str, str],
         "UrlEndpoint": UrlEndpointConfigTypeDef,
         "VpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListApplicationsRequestListApplicationsPaginateTypeDef(
-    _RequiredListApplicationsRequestListApplicationsPaginateTypeDef,
-    _OptionalListApplicationsRequestListApplicationsPaginateTypeDef,
-):
-    pass
-
-_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
-    "_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
-    {
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
-    "_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef(
-    _RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-    _OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-):
-    pass
-
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListRoutesRequestListRoutesPaginateTypeDef",
-    {
-        "ApplicationIdentifier": str,
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListRoutesRequestListRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRoutesRequestListRoutesPaginateTypeDef(
-    _RequiredListRoutesRequestListRoutesPaginateTypeDef,
-    _OptionalListRoutesRequestListRoutesPaginateTypeDef,
-):
-    pass
-
-_RequiredListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "_RequiredListServicesRequestListServicesPaginateTypeDef",
-    {
-        "ApplicationIdentifier": str,
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "_OptionalListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListServicesRequestListServicesPaginateTypeDef(
-    _RequiredListServicesRequestListServicesPaginateTypeDef,
-    _OptionalListServicesRequestListServicesPaginateTypeDef,
-):
-    pass
-
 ServiceSummaryTypeDef = TypedDict(
     "ServiceSummaryTypeDef",
     {
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
@@ -1029,37 +1032,37 @@
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationSummaryList": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "EnvironmentSummaryList": List[EnvironmentSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRoutesResponseTypeDef = TypedDict(
     "ListRoutesResponseTypeDef",
     {
         "NextToken": str,
         "RouteSummaryList": List[RouteSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "NextToken": str,
         "ServiceSummaryList": List[ServiceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migration-hub-refactor-spaces
-Version: 1.26.68
-Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.26.68 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-migration-hub-refactor-spaces"></a>
 
 # mypy-boto3-migration-hub-refactor-spaces
 
 [![PyPI - mypy-boto3-migration-hub-refactor-spaces](https://img.shields.io/pypi/v/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migration-hub-refactor-spaces?color=blue)](https://pypistats.org/packages/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,73 +352,73 @@
 
 ```python
 from mypy_boto3_migration_hub_refactor_spaces.type_defs import (
     ApiGatewayProxyConfigTypeDef,
     ApiGatewayProxyInputTypeDef,
     ApiGatewayProxySummaryTypeDef,
     ErrorResponseTypeDef,
-    ResponseMetadataTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
+    CreateEnvironmentResponseTypeDef,
     DefaultRouteInputTypeDef,
     UriPathRouteInputTypeDef,
     LambdaEndpointInputTypeDef,
     UrlEndpointInputTypeDef,
     DeleteApplicationRequestRequestTypeDef,
+    DeleteApplicationResponseTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
+    DeleteEnvironmentResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
+    DeleteRouteResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
+    DeleteServiceResponseTypeDef,
     EnvironmentVpcTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetRouteRequestRequestTypeDef,
     GetServiceRequestRequestTypeDef,
     LambdaEndpointConfigTypeDef,
     UrlEndpointConfigTypeDef,
     LambdaEndpointSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
     ListEnvironmentVpcsRequestRequestTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
+    ListRoutesRequestListRoutesPaginateTypeDef,
     ListRoutesRequestRequestTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UrlEndpointSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRouteRequestRequestTypeDef,
+    UpdateRouteResponseTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    CreateApplicationResponseTypeDef,
     ApplicationSummaryTypeDef,
     EnvironmentSummaryTypeDef,
-    RouteSummaryTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    DeleteApplicationResponseTypeDef,
-    DeleteEnvironmentResponseTypeDef,
-    DeleteRouteResponseTypeDef,
-    DeleteServiceResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetEnvironmentResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRouteResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateRouteResponseTypeDef,
+    RouteSummaryTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     GetServiceResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
-    ListRoutesRequestListRoutesPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ServiceSummaryTypeDef,
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
 )
 
@@ -430,42 +430,42 @@
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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.68/setup.py` & `mypy-boto3-migration-hub-refactor-spaces-1.27.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-migration-hub-refactor-spaces.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migration-hub-refactor-spaces",
-    version="1.26.68",
+    version="1.27.0",
     packages=["mypy_boto3_migration_hub_refactor_spaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubRefactorSpaces 1.26.68 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.MigrationHubRefactorSpaces 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -50,11 +50,11 @@
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/"
         ),
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


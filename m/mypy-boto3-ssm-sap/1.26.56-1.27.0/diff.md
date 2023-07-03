# Comparing `tmp/mypy-boto3-ssm-sap-1.26.56.tar.gz` & `tmp/mypy-boto3-ssm-sap-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-sap-1.26.56.tar", last modified: Tue Jan 24 20:25:10 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-sap-1.27.0.tar", last modified: Mon Jul  3 19:51:30 2023, max compression
```

## Comparing `mypy-boto3-ssm-sap-1.26.56.tar` & `mypy-boto3-ssm-sap-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:25:10.916532 mypy-boto3-ssm-sap-1.26.56/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14963 2023-01-24 20:25:10.916532 mypy-boto3-ssm-sap-1.26.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:25:10.916532 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:25:10.916532 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14963 2023-01-24 20:25:10.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-24 20:25:10.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 20:25:10.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 20:25:10.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-24 20:25:10.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-24 20:25:10.000000 mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 20:25:10.916532 mypy-boto3-ssm-sap-1.26.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-01-24 20:25:01.000000 mypy-boto3-ssm-sap-1.26.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:30.936056 mypy-boto3-ssm-sap-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-07-03 19:51:30.932056 mypy-boto3-ssm-sap-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:30.932056 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-07-03 19:48:43.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15295 2023-07-03 19:48:43.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:30.932056 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-07-03 19:51:30.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 19:51:30.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:30.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:30.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:30.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:51:30.000000 mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:30.936056 mypy-boto3-ssm-sap-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-03 19:48:42.000000 mypy-boto3-ssm-sap-1.27.0/setup.py
```

### Comparing `mypy-boto3-ssm-sap-1.26.56/LICENSE` & `mypy-boto3-ssm-sap-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-ssm-sap-1.26.56/PKG-INFO` & `mypy-boto3-ssm-sap-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-sap
-Version: 1.26.56
-Summary: Type annotations for boto3.SsmSap 1.26.56 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.SsmSap 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ssm-sap"></a>
 
 # mypy-boto3-ssm-sap
 
 [![PyPI - mypy-boto3-ssm-sap](https://img.shields.io/pypi/v/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-sap?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SsmSap 1.26.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[boto3.SsmSap 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
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
 [mypy-boto3-ssm-sap docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -347,52 +347,52 @@
     ApplicationCredentialTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     ComponentSummaryTypeDef,
     HostTypeDef,
     DatabaseSummaryTypeDef,
     DeleteResourcePermissionInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteResourcePermissionOutputTypeDef,
     DeregisterApplicationInputRequestTypeDef,
     FilterTypeDef,
     GetApplicationInputRequestTypeDef,
     GetComponentInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetOperationInputRequestTypeDef,
     OperationTypeDef,
     GetResourcePermissionInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetResourcePermissionOutputTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
+    ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePermissionInputRequestTypeDef,
+    PutResourcePermissionOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateApplicationSettingsOutputTypeDef,
     DatabaseTypeDef,
     RegisterApplicationInputRequestTypeDef,
     UpdateApplicationSettingsInputRequestTypeDef,
-    ComponentTypeDef,
-    DeleteResourcePermissionOutputTypeDef,
-    GetApplicationOutputTypeDef,
-    GetResourcePermissionOutputTypeDef,
     ListApplicationsOutputTypeDef,
+    GetApplicationOutputTypeDef,
+    RegisterApplicationOutputTypeDef,
     ListComponentsOutputTypeDef,
+    ComponentTypeDef,
     ListDatabasesOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutResourcePermissionOutputTypeDef,
-    RegisterApplicationOutputTypeDef,
-    UpdateApplicationSettingsOutputTypeDef,
+    ListOperationsInputListOperationsPaginateTypeDef,
     ListOperationsInputRequestTypeDef,
     GetOperationOutputTypeDef,
     ListOperationsOutputTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
-    ListComponentsInputListComponentsPaginateTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
-    ListOperationsInputListOperationsPaginateTypeDef,
     GetDatabaseOutputTypeDef,
     GetComponentOutputTypeDef,
 )
 
 
 def get_structure() -> ApplicationCredentialTypeDef:
     return {...}
@@ -401,42 +401,42 @@
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

### Comparing `mypy-boto3-ssm-sap-1.26.56/README.md` & `mypy-boto3-ssm-sap-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ssm-sap"></a>
 
 # mypy-boto3-ssm-sap
 
 [![PyPI - mypy-boto3-ssm-sap](https://img.shields.io/pypi/v/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-sap?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SsmSap 1.26.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[boto3.SsmSap 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
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
 [mypy-boto3-ssm-sap docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -315,52 +315,52 @@
     ApplicationCredentialTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     ComponentSummaryTypeDef,
     HostTypeDef,
     DatabaseSummaryTypeDef,
     DeleteResourcePermissionInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteResourcePermissionOutputTypeDef,
     DeregisterApplicationInputRequestTypeDef,
     FilterTypeDef,
     GetApplicationInputRequestTypeDef,
     GetComponentInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetOperationInputRequestTypeDef,
     OperationTypeDef,
     GetResourcePermissionInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetResourcePermissionOutputTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
+    ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePermissionInputRequestTypeDef,
+    PutResourcePermissionOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateApplicationSettingsOutputTypeDef,
     DatabaseTypeDef,
     RegisterApplicationInputRequestTypeDef,
     UpdateApplicationSettingsInputRequestTypeDef,
-    ComponentTypeDef,
-    DeleteResourcePermissionOutputTypeDef,
-    GetApplicationOutputTypeDef,
-    GetResourcePermissionOutputTypeDef,
     ListApplicationsOutputTypeDef,
+    GetApplicationOutputTypeDef,
+    RegisterApplicationOutputTypeDef,
     ListComponentsOutputTypeDef,
+    ComponentTypeDef,
     ListDatabasesOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutResourcePermissionOutputTypeDef,
-    RegisterApplicationOutputTypeDef,
-    UpdateApplicationSettingsOutputTypeDef,
+    ListOperationsInputListOperationsPaginateTypeDef,
     ListOperationsInputRequestTypeDef,
     GetOperationOutputTypeDef,
     ListOperationsOutputTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
-    ListComponentsInputListComponentsPaginateTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
-    ListOperationsInputListOperationsPaginateTypeDef,
     GetDatabaseOutputTypeDef,
     GetComponentOutputTypeDef,
 )
 
 
 def get_structure() -> ApplicationCredentialTypeDef:
     return {...}
@@ -369,42 +369,42 @@
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

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/__init__.py` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/__init__.pyi` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/__main__.py` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SsmSap 1.26.56\nVersion:         1.26.56\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.SsmSap 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.56")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/client.py` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/client.pyi` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/literals.py` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,15 @@
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
@@ -111,21 +112,23 @@
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
@@ -204,14 +207,15 @@
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
@@ -222,14 +226,15 @@
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
@@ -265,14 +270,15 @@
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
@@ -291,16 +297,19 @@
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
@@ -380,18 +389,21 @@
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

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/literals.pyi` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -70,14 +70,15 @@
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
@@ -109,21 +110,23 @@
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
@@ -202,14 +205,15 @@
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
@@ -220,14 +224,15 @@
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
@@ -263,14 +268,15 @@
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
@@ -289,16 +295,19 @@
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
@@ -378,18 +387,21 @@
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

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/paginator.py` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,30 +59,30 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listapplicationspaginator)
         """
 
 
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listcomponentspaginator)
     """
 
     def paginate(
-        self, *, ApplicationId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ApplicationId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listcomponentspaginator)
         """
 
 
@@ -93,15 +93,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listdatabasespaginator)
         """
 
 
@@ -112,13 +112,13 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listoperationspaginator)
         """
```

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/paginator.pyi` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -56,29 +56,29 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listapplicationspaginator)
         """
 
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listcomponentspaginator)
     """
 
     def paginate(
-        self, *, ApplicationId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ApplicationId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listcomponentspaginator)
         """
 
 class ListDatabasesPaginator(Paginator):
@@ -88,15 +88,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listdatabasespaginator)
         """
 
 class ListOperationsPaginator(Paginator):
@@ -106,13 +106,13 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listoperationspaginator)
         """
```

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/type_defs.py` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,52 +38,52 @@
     "ApplicationCredentialTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "ComponentSummaryTypeDef",
     "HostTypeDef",
     "DatabaseSummaryTypeDef",
     "DeleteResourcePermissionInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DeleteResourcePermissionOutputTypeDef",
     "DeregisterApplicationInputRequestTypeDef",
     "FilterTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetComponentInputRequestTypeDef",
     "GetDatabaseInputRequestTypeDef",
     "GetOperationInputRequestTypeDef",
     "OperationTypeDef",
     "GetResourcePermissionInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetResourcePermissionOutputTypeDef",
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListApplicationsInputRequestTypeDef",
+    "ListComponentsInputListComponentsPaginateTypeDef",
     "ListComponentsInputRequestTypeDef",
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutResourcePermissionInputRequestTypeDef",
+    "PutResourcePermissionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateApplicationSettingsOutputTypeDef",
     "DatabaseTypeDef",
     "RegisterApplicationInputRequestTypeDef",
     "UpdateApplicationSettingsInputRequestTypeDef",
-    "ComponentTypeDef",
-    "DeleteResourcePermissionOutputTypeDef",
-    "GetApplicationOutputTypeDef",
-    "GetResourcePermissionOutputTypeDef",
     "ListApplicationsOutputTypeDef",
+    "GetApplicationOutputTypeDef",
+    "RegisterApplicationOutputTypeDef",
     "ListComponentsOutputTypeDef",
+    "ComponentTypeDef",
     "ListDatabasesOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutResourcePermissionOutputTypeDef",
-    "RegisterApplicationOutputTypeDef",
-    "UpdateApplicationSettingsOutputTypeDef",
+    "ListOperationsInputListOperationsPaginateTypeDef",
     "ListOperationsInputRequestTypeDef",
     "GetOperationOutputTypeDef",
     "ListOperationsOutputTypeDef",
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
-    "ListComponentsInputListComponentsPaginateTypeDef",
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
-    "ListOperationsInputListOperationsPaginateTypeDef",
     "GetDatabaseOutputTypeDef",
     "GetComponentOutputTypeDef",
 )
 
 ApplicationCredentialTypeDef = TypedDict(
     "ApplicationCredentialTypeDef",
     {
@@ -173,22 +173,19 @@
 class DeleteResourcePermissionInputRequestTypeDef(
     _RequiredDeleteResourcePermissionInputRequestTypeDef,
     _OptionalDeleteResourcePermissionInputRequestTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DeleteResourcePermissionOutputTypeDef = TypedDict(
+    "DeleteResourcePermissionOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeregisterApplicationInputRequestTypeDef = TypedDict(
     "DeregisterApplicationInputRequestTypeDef",
     {
         "ApplicationId": str,
@@ -276,43 +273,68 @@
 class GetResourcePermissionInputRequestTypeDef(
     _RequiredGetResourcePermissionInputRequestTypeDef,
     _OptionalGetResourcePermissionInputRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetResourcePermissionOutputTypeDef = TypedDict(
+    "GetResourcePermissionOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationsInputRequestTypeDef = TypedDict(
     "ListApplicationsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
+    "ListComponentsInputListComponentsPaginateTypeDef",
+    {
+        "ApplicationId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListComponentsInputRequestTypeDef = TypedDict(
     "ListComponentsInputRequestTypeDef",
     {
         "ApplicationId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "ApplicationId": str,
+        "ComponentId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatabasesInputRequestTypeDef = TypedDict(
     "ListDatabasesInputRequestTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
         "NextToken": str,
         "MaxResults": int,
@@ -323,23 +345,60 @@
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
 PutResourcePermissionInputRequestTypeDef = TypedDict(
     "PutResourcePermissionInputRequestTypeDef",
     {
         "ActionType": Literal["RESTORE"],
         "SourceResourceArn": str,
         "ResourceArn": str,
     },
 )
 
+PutResourcePermissionOutputTypeDef = TypedDict(
+    "PutResourcePermissionOutputTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
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
@@ -348,14 +407,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateApplicationSettingsOutputTypeDef = TypedDict(
+    "UpdateApplicationSettingsOutputTypeDef",
+    {
+        "Message": str,
+        "OperationIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DatabaseTypeDef = TypedDict(
     "DatabaseTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
         "Credentials": List[ApplicationCredentialTypeDef],
         "DatabaseId": str,
@@ -415,114 +483,96 @@
 class UpdateApplicationSettingsInputRequestTypeDef(
     _RequiredUpdateApplicationSettingsInputRequestTypeDef,
     _OptionalUpdateApplicationSettingsInputRequestTypeDef,
 ):
     pass
 
 
-ComponentTypeDef = TypedDict(
-    "ComponentTypeDef",
-    {
-        "ComponentId": str,
-        "ApplicationId": str,
-        "ComponentType": Literal["HANA"],
-        "Status": Literal["ACTIVATED"],
-        "Databases": List[str],
-        "Hosts": List[HostTypeDef],
-        "PrimaryHost": str,
-        "LastUpdated": datetime,
-    },
-    total=False,
-)
-
-DeleteResourcePermissionOutputTypeDef = TypedDict(
-    "DeleteResourcePermissionOutputTypeDef",
+ListApplicationsOutputTypeDef = TypedDict(
+    "ListApplicationsOutputTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Applications": List[ApplicationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationOutputTypeDef = TypedDict(
     "GetApplicationOutputTypeDef",
     {
         "Application": ApplicationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetResourcePermissionOutputTypeDef = TypedDict(
-    "GetResourcePermissionOutputTypeDef",
+RegisterApplicationOutputTypeDef = TypedDict(
+    "RegisterApplicationOutputTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Application": ApplicationTypeDef,
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListApplicationsOutputTypeDef = TypedDict(
-    "ListApplicationsOutputTypeDef",
+ListComponentsOutputTypeDef = TypedDict(
+    "ListComponentsOutputTypeDef",
     {
-        "Applications": List[ApplicationSummaryTypeDef],
+        "Components": List[ComponentSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListComponentsOutputTypeDef = TypedDict(
-    "ListComponentsOutputTypeDef",
+ComponentTypeDef = TypedDict(
+    "ComponentTypeDef",
     {
-        "Components": List[ComponentSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ComponentId": str,
+        "ApplicationId": str,
+        "ComponentType": Literal["HANA"],
+        "Status": Literal["ACTIVATED"],
+        "Databases": List[str],
+        "Hosts": List[HostTypeDef],
+        "PrimaryHost": str,
+        "LastUpdated": datetime,
     },
+    total=False,
 )
 
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "Databases": List[DatabaseSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListOperationsInputListOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListOperationsInputListOperationsPaginateTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
     },
 )
-
-PutResourcePermissionOutputTypeDef = TypedDict(
-    "PutResourcePermissionOutputTypeDef",
+_OptionalListOperationsInputListOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListOperationsInputListOperationsPaginateTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
-RegisterApplicationOutputTypeDef = TypedDict(
-    "RegisterApplicationOutputTypeDef",
-    {
-        "Application": ApplicationTypeDef,
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateApplicationSettingsOutputTypeDef = TypedDict(
-    "UpdateApplicationSettingsOutputTypeDef",
-    {
-        "Message": str,
-        "OperationIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class ListOperationsInputListOperationsPaginateTypeDef(
+    _RequiredListOperationsInputListOperationsPaginateTypeDef,
+    _OptionalListOperationsInputListOperationsPaginateTypeDef,
+):
+    pass
+
 
 _RequiredListOperationsInputRequestTypeDef = TypedDict(
     "_RequiredListOperationsInputRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
@@ -543,86 +593,36 @@
     pass
 
 
 GetOperationOutputTypeDef = TypedDict(
     "GetOperationOutputTypeDef",
     {
         "Operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOperationsOutputTypeDef = TypedDict(
     "ListOperationsOutputTypeDef",
     {
         "Operations": List[OperationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
-    "ListComponentsInputListComponentsPaginateTypeDef",
-    {
-        "ApplicationId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "ApplicationId": str,
-        "ComponentId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListOperationsInputListOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListOperationsInputListOperationsPaginateTypeDef",
-    {
-        "ApplicationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListOperationsInputListOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListOperationsInputListOperationsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListOperationsInputListOperationsPaginateTypeDef(
-    _RequiredListOperationsInputListOperationsPaginateTypeDef,
-    _OptionalListOperationsInputListOperationsPaginateTypeDef,
-):
-    pass
-
 
 GetDatabaseOutputTypeDef = TypedDict(
     "GetDatabaseOutputTypeDef",
     {
         "Database": DatabaseTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetComponentOutputTypeDef = TypedDict(
     "GetComponentOutputTypeDef",
     {
         "Component": ComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap/type_defs.pyi` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,52 +37,52 @@
     "ApplicationCredentialTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "ComponentSummaryTypeDef",
     "HostTypeDef",
     "DatabaseSummaryTypeDef",
     "DeleteResourcePermissionInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DeleteResourcePermissionOutputTypeDef",
     "DeregisterApplicationInputRequestTypeDef",
     "FilterTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetComponentInputRequestTypeDef",
     "GetDatabaseInputRequestTypeDef",
     "GetOperationInputRequestTypeDef",
     "OperationTypeDef",
     "GetResourcePermissionInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetResourcePermissionOutputTypeDef",
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListApplicationsInputRequestTypeDef",
+    "ListComponentsInputListComponentsPaginateTypeDef",
     "ListComponentsInputRequestTypeDef",
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutResourcePermissionInputRequestTypeDef",
+    "PutResourcePermissionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateApplicationSettingsOutputTypeDef",
     "DatabaseTypeDef",
     "RegisterApplicationInputRequestTypeDef",
     "UpdateApplicationSettingsInputRequestTypeDef",
-    "ComponentTypeDef",
-    "DeleteResourcePermissionOutputTypeDef",
-    "GetApplicationOutputTypeDef",
-    "GetResourcePermissionOutputTypeDef",
     "ListApplicationsOutputTypeDef",
+    "GetApplicationOutputTypeDef",
+    "RegisterApplicationOutputTypeDef",
     "ListComponentsOutputTypeDef",
+    "ComponentTypeDef",
     "ListDatabasesOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutResourcePermissionOutputTypeDef",
-    "RegisterApplicationOutputTypeDef",
-    "UpdateApplicationSettingsOutputTypeDef",
+    "ListOperationsInputListOperationsPaginateTypeDef",
     "ListOperationsInputRequestTypeDef",
     "GetOperationOutputTypeDef",
     "ListOperationsOutputTypeDef",
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
-    "ListComponentsInputListComponentsPaginateTypeDef",
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
-    "ListOperationsInputListOperationsPaginateTypeDef",
     "GetDatabaseOutputTypeDef",
     "GetComponentOutputTypeDef",
 )
 
 ApplicationCredentialTypeDef = TypedDict(
     "ApplicationCredentialTypeDef",
     {
@@ -170,22 +170,19 @@
 
 class DeleteResourcePermissionInputRequestTypeDef(
     _RequiredDeleteResourcePermissionInputRequestTypeDef,
     _OptionalDeleteResourcePermissionInputRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DeleteResourcePermissionOutputTypeDef = TypedDict(
+    "DeleteResourcePermissionOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeregisterApplicationInputRequestTypeDef = TypedDict(
     "DeregisterApplicationInputRequestTypeDef",
     {
         "ApplicationId": str,
@@ -271,43 +268,68 @@
 
 class GetResourcePermissionInputRequestTypeDef(
     _RequiredGetResourcePermissionInputRequestTypeDef,
     _OptionalGetResourcePermissionInputRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetResourcePermissionOutputTypeDef = TypedDict(
+    "GetResourcePermissionOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationsInputRequestTypeDef = TypedDict(
     "ListApplicationsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
+    "ListComponentsInputListComponentsPaginateTypeDef",
+    {
+        "ApplicationId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListComponentsInputRequestTypeDef = TypedDict(
     "ListComponentsInputRequestTypeDef",
     {
         "ApplicationId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "ApplicationId": str,
+        "ComponentId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDatabasesInputRequestTypeDef = TypedDict(
     "ListDatabasesInputRequestTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
         "NextToken": str,
         "MaxResults": int,
@@ -318,23 +340,60 @@
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
 PutResourcePermissionInputRequestTypeDef = TypedDict(
     "PutResourcePermissionInputRequestTypeDef",
     {
         "ActionType": Literal["RESTORE"],
         "SourceResourceArn": str,
         "ResourceArn": str,
     },
 )
 
+PutResourcePermissionOutputTypeDef = TypedDict(
+    "PutResourcePermissionOutputTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
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
@@ -343,14 +402,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateApplicationSettingsOutputTypeDef = TypedDict(
+    "UpdateApplicationSettingsOutputTypeDef",
+    {
+        "Message": str,
+        "OperationIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DatabaseTypeDef = TypedDict(
     "DatabaseTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
         "Credentials": List[ApplicationCredentialTypeDef],
         "DatabaseId": str,
@@ -406,114 +474,94 @@
 
 class UpdateApplicationSettingsInputRequestTypeDef(
     _RequiredUpdateApplicationSettingsInputRequestTypeDef,
     _OptionalUpdateApplicationSettingsInputRequestTypeDef,
 ):
     pass
 
-ComponentTypeDef = TypedDict(
-    "ComponentTypeDef",
-    {
-        "ComponentId": str,
-        "ApplicationId": str,
-        "ComponentType": Literal["HANA"],
-        "Status": Literal["ACTIVATED"],
-        "Databases": List[str],
-        "Hosts": List[HostTypeDef],
-        "PrimaryHost": str,
-        "LastUpdated": datetime,
-    },
-    total=False,
-)
-
-DeleteResourcePermissionOutputTypeDef = TypedDict(
-    "DeleteResourcePermissionOutputTypeDef",
+ListApplicationsOutputTypeDef = TypedDict(
+    "ListApplicationsOutputTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Applications": List[ApplicationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationOutputTypeDef = TypedDict(
     "GetApplicationOutputTypeDef",
     {
         "Application": ApplicationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetResourcePermissionOutputTypeDef = TypedDict(
-    "GetResourcePermissionOutputTypeDef",
+RegisterApplicationOutputTypeDef = TypedDict(
+    "RegisterApplicationOutputTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Application": ApplicationTypeDef,
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListApplicationsOutputTypeDef = TypedDict(
-    "ListApplicationsOutputTypeDef",
+ListComponentsOutputTypeDef = TypedDict(
+    "ListComponentsOutputTypeDef",
     {
-        "Applications": List[ApplicationSummaryTypeDef],
+        "Components": List[ComponentSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListComponentsOutputTypeDef = TypedDict(
-    "ListComponentsOutputTypeDef",
+ComponentTypeDef = TypedDict(
+    "ComponentTypeDef",
     {
-        "Components": List[ComponentSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ComponentId": str,
+        "ApplicationId": str,
+        "ComponentType": Literal["HANA"],
+        "Status": Literal["ACTIVATED"],
+        "Databases": List[str],
+        "Hosts": List[HostTypeDef],
+        "PrimaryHost": str,
+        "LastUpdated": datetime,
     },
+    total=False,
 )
 
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "Databases": List[DatabaseSummaryTypeDef],
         "NextToken": str,
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
 
-PutResourcePermissionOutputTypeDef = TypedDict(
-    "PutResourcePermissionOutputTypeDef",
+_RequiredListOperationsInputListOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListOperationsInputListOperationsPaginateTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
     },
 )
-
-RegisterApplicationOutputTypeDef = TypedDict(
-    "RegisterApplicationOutputTypeDef",
+_OptionalListOperationsInputListOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListOperationsInputListOperationsPaginateTypeDef",
     {
-        "Application": ApplicationTypeDef,
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
-UpdateApplicationSettingsOutputTypeDef = TypedDict(
-    "UpdateApplicationSettingsOutputTypeDef",
-    {
-        "Message": str,
-        "OperationIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class ListOperationsInputListOperationsPaginateTypeDef(
+    _RequiredListOperationsInputListOperationsPaginateTypeDef,
+    _OptionalListOperationsInputListOperationsPaginateTypeDef,
+):
+    pass
 
 _RequiredListOperationsInputRequestTypeDef = TypedDict(
     "_RequiredListOperationsInputRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
@@ -532,84 +580,36 @@
 ):
     pass
 
 GetOperationOutputTypeDef = TypedDict(
     "GetOperationOutputTypeDef",
     {
         "Operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOperationsOutputTypeDef = TypedDict(
     "ListOperationsOutputTypeDef",
     {
         "Operations": List[OperationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
-    "ListComponentsInputListComponentsPaginateTypeDef",
-    {
-        "ApplicationId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "ApplicationId": str,
-        "ComponentId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListOperationsInputListOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListOperationsInputListOperationsPaginateTypeDef",
-    {
-        "ApplicationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListOperationsInputListOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListOperationsInputListOperationsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListOperationsInputListOperationsPaginateTypeDef(
-    _RequiredListOperationsInputListOperationsPaginateTypeDef,
-    _OptionalListOperationsInputListOperationsPaginateTypeDef,
-):
-    pass
 
 GetDatabaseOutputTypeDef = TypedDict(
     "GetDatabaseOutputTypeDef",
     {
         "Database": DatabaseTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetComponentOutputTypeDef = TypedDict(
     "GetComponentOutputTypeDef",
     {
         "Component": ComponentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap.egg-info/PKG-INFO` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-sap
-Version: 1.26.56
-Summary: Type annotations for boto3.SsmSap 1.26.56 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.SsmSap 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ssm-sap"></a>
 
 # mypy-boto3-ssm-sap
 
 [![PyPI - mypy-boto3-ssm-sap](https://img.shields.io/pypi/v/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-sap?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SsmSap 1.26.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[boto3.SsmSap 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
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
 [mypy-boto3-ssm-sap docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -347,52 +347,52 @@
     ApplicationCredentialTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     ComponentSummaryTypeDef,
     HostTypeDef,
     DatabaseSummaryTypeDef,
     DeleteResourcePermissionInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteResourcePermissionOutputTypeDef,
     DeregisterApplicationInputRequestTypeDef,
     FilterTypeDef,
     GetApplicationInputRequestTypeDef,
     GetComponentInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetOperationInputRequestTypeDef,
     OperationTypeDef,
     GetResourcePermissionInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetResourcePermissionOutputTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
+    ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePermissionInputRequestTypeDef,
+    PutResourcePermissionOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateApplicationSettingsOutputTypeDef,
     DatabaseTypeDef,
     RegisterApplicationInputRequestTypeDef,
     UpdateApplicationSettingsInputRequestTypeDef,
-    ComponentTypeDef,
-    DeleteResourcePermissionOutputTypeDef,
-    GetApplicationOutputTypeDef,
-    GetResourcePermissionOutputTypeDef,
     ListApplicationsOutputTypeDef,
+    GetApplicationOutputTypeDef,
+    RegisterApplicationOutputTypeDef,
     ListComponentsOutputTypeDef,
+    ComponentTypeDef,
     ListDatabasesOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutResourcePermissionOutputTypeDef,
-    RegisterApplicationOutputTypeDef,
-    UpdateApplicationSettingsOutputTypeDef,
+    ListOperationsInputListOperationsPaginateTypeDef,
     ListOperationsInputRequestTypeDef,
     GetOperationOutputTypeDef,
     ListOperationsOutputTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
-    ListComponentsInputListComponentsPaginateTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
-    ListOperationsInputListOperationsPaginateTypeDef,
     GetDatabaseOutputTypeDef,
     GetComponentOutputTypeDef,
 )
 
 
 def get_structure() -> ApplicationCredentialTypeDef:
     return {...}
@@ -401,42 +401,42 @@
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

### Comparing `mypy-boto3-ssm-sap-1.26.56/mypy_boto3_ssm_sap.egg-info/SOURCES.txt` & `mypy-boto3-ssm-sap-1.27.0/mypy_boto3_ssm_sap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.26.56/setup.py` & `mypy-boto3-ssm-sap-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-ssm-sap.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-sap",
-    version="1.26.56",
+    version="1.27.0",
     packages=["mypy_boto3_ssm_sap"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SsmSap 1.26.56 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.SsmSap 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/",
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


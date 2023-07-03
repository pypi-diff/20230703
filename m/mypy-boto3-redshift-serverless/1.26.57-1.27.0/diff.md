# Comparing `tmp/mypy-boto3-redshift-serverless-1.26.57.tar.gz` & `tmp/mypy-boto3-redshift-serverless-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-serverless-1.26.57.tar", last modified: Wed Jan 25 20:48:07 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-serverless-1.27.0.tar", last modified: Mon Jul  3 19:51:19 2023, max compression
```

## Comparing `mypy-boto3-redshift-serverless-1.26.57.tar` & `mypy-boto3-redshift-serverless-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:48:07.700256 mypy-boto3-redshift-serverless-1.26.57/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18364 2023-01-25 20:48:07.696256 mypy-boto3-redshift-serverless-1.26.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:48:07.692256 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32938 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-01-25 20:47:33.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33722 2023-01-25 20:47:33.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33691 2023-01-25 20:47:33.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:48:07.696256 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18364 2023-01-25 20:48:07.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-01-25 20:48:07.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:48:07.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:48:07.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-25 20:48:07.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-25 20:48:07.000000 mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 20:48:07.700256 mypy-boto3-redshift-serverless-1.26.57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-01-25 20:47:32.000000 mypy-boto3-redshift-serverless-1.26.57/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.411873 mypy-boto3-redshift-serverless-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18352 2023-07-03 19:51:19.411873 mypy-boto3-redshift-serverless-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.411873 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32938 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33810 2023-07-03 19:46:08.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33779 2023-07-03 19:46:08.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.411873 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18352 2023-07-03 19:51:19.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:51:19.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:19.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 19:51:19.000000 mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:19.411873 mypy-boto3-redshift-serverless-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-03 19:46:07.000000 mypy-boto3-redshift-serverless-1.27.0/setup.py
```

### Comparing `mypy-boto3-redshift-serverless-1.26.57/LICENSE` & `mypy-boto3-redshift-serverless-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-redshift-serverless-1.26.57/PKG-INFO` & `mypy-boto3-redshift-serverless-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-serverless
-Version: 1.26.57
-Summary: Type annotations for boto3.RedshiftServerless 1.26.57 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.RedshiftServerless 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-redshift-serverless"></a>
 
 # mypy-boto3-redshift-serverless
 
 [![PyPI - mypy-boto3-redshift-serverless](https://img.shields.io/pypi/v/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.26.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,66 +355,73 @@
 `mypy_boto3_redshift_serverless.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_serverless.type_defs import (
     ConfigParameterTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     SnapshotTypeDef,
     CreateEndpointAccessRequestRequestTypeDef,
     NamespaceTypeDef,
     CreateUsageLimitRequestRequestTypeDef,
     UsageLimitTypeDef,
     DeleteEndpointAccessRequestRequestTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteUsageLimitRequestRequestTypeDef,
     DeleteWorkgroupRequestRequestTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     GetCredentialsRequestRequestTypeDef,
+    GetCredentialsResponseTypeDef,
     GetEndpointAccessRequestRequestTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetRecoveryPointRequestRequestTypeDef,
     RecoveryPointTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     ResourcePolicyTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetTableRestoreStatusRequestRequestTypeDef,
     TableRestoreStatusTypeDef,
     GetUsageLimitRequestRequestTypeDef,
     GetWorkgroupRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
+    ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
+    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
     ListRecoveryPointsRequestRequestTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
+    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
+    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     RestoreTableFromSnapshotRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEndpointAccessRequestRequestTypeDef,
     UpdateNamespaceRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateUsageLimitRequestRequestTypeDef,
     UpdateWorkgroupRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateWorkgroupRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    GetCredentialsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     GetSnapshotResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateNamespaceResponseTypeDef,
@@ -432,21 +439,14 @@
     GetRecoveryPointResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     GetTableRestoreStatusResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
-    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
-    ListNamespacesRequestListNamespacesPaginateTypeDef,
-    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
-    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
-    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -467,42 +467,42 @@
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

### Comparing `mypy-boto3-redshift-serverless-1.26.57/README.md` & `mypy-boto3-redshift-serverless-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-redshift-serverless"></a>
 
 # mypy-boto3-redshift-serverless
 
 [![PyPI - mypy-boto3-redshift-serverless](https://img.shields.io/pypi/v/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.26.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,66 +323,73 @@
 `mypy_boto3_redshift_serverless.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_serverless.type_defs import (
     ConfigParameterTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     SnapshotTypeDef,
     CreateEndpointAccessRequestRequestTypeDef,
     NamespaceTypeDef,
     CreateUsageLimitRequestRequestTypeDef,
     UsageLimitTypeDef,
     DeleteEndpointAccessRequestRequestTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteUsageLimitRequestRequestTypeDef,
     DeleteWorkgroupRequestRequestTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     GetCredentialsRequestRequestTypeDef,
+    GetCredentialsResponseTypeDef,
     GetEndpointAccessRequestRequestTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetRecoveryPointRequestRequestTypeDef,
     RecoveryPointTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     ResourcePolicyTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetTableRestoreStatusRequestRequestTypeDef,
     TableRestoreStatusTypeDef,
     GetUsageLimitRequestRequestTypeDef,
     GetWorkgroupRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
+    ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
+    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
     ListRecoveryPointsRequestRequestTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
+    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
+    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     RestoreTableFromSnapshotRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEndpointAccessRequestRequestTypeDef,
     UpdateNamespaceRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateUsageLimitRequestRequestTypeDef,
     UpdateWorkgroupRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateWorkgroupRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    GetCredentialsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     GetSnapshotResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateNamespaceResponseTypeDef,
@@ -400,21 +407,14 @@
     GetRecoveryPointResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     GetTableRestoreStatusResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
-    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
-    ListNamespacesRequestListNamespacesPaginateTypeDef,
-    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
-    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
-    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -435,42 +435,42 @@
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

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/__init__.py` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/__init__.pyi` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/__main__.py` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RedshiftServerless 1.26.57\nVersion:         1.26.57\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.RedshiftServerless 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.57")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/client.py` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/client.pyi` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/literals.py` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,15 @@
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
@@ -107,21 +108,23 @@
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
@@ -200,14 +203,15 @@
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
@@ -218,14 +222,15 @@
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
@@ -261,14 +266,15 @@
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
@@ -287,16 +293,19 @@
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
@@ -376,18 +385,21 @@
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
@@ -417,17 +429,21 @@
     "list_table_restore_status",
     "list_usage_limits",
     "list_workgroups",
 ]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
+    "eu-west-3",
     "us-east-1",
     "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/literals.pyi` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,15 @@
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
@@ -105,21 +106,23 @@
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
@@ -198,14 +201,15 @@
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
@@ -216,14 +220,15 @@
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
@@ -259,14 +264,15 @@
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
@@ -285,16 +291,19 @@
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
@@ -374,18 +383,21 @@
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
@@ -415,17 +427,21 @@
     "list_table_restore_status",
     "list_usage_limits",
     "list_workgroups",
 ]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
+    "eu-west-3",
     "us-east-1",
     "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/paginator.py` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -54,146 +54,137 @@
     "ListRecoveryPointsPaginator",
     "ListSnapshotsPaginator",
     "ListTableRestoreStatusPaginator",
     "ListUsageLimitsPaginator",
     "ListWorkgroupsPaginator",
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
 class ListEndpointAccessPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListEndpointAccess)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listendpointaccesspaginator)
     """
 
     def paginate(
         self,
         *,
         vpcId: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEndpointAccessResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListEndpointAccess.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listendpointaccesspaginator)
         """
 
-
 class ListNamespacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listnamespacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listnamespacespaginator)
         """
 
-
 class ListRecoveryPointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listrecoverypointspaginator)
     """
 
     def paginate(
         self,
         *,
         endTime: Union[datetime, str] = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         startTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecoveryPointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listrecoverypointspaginator)
         """
 
-
 class ListSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listsnapshotspaginator)
     """
 
     def paginate(
         self,
         *,
         endTime: Union[datetime, str] = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         ownerAccount: str = ...,
         startTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listsnapshotspaginator)
         """
 
-
 class ListTableRestoreStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListTableRestoreStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listtablerestorestatuspaginator)
     """
 
     def paginate(
         self,
         *,
         namespaceName: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTableRestoreStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListTableRestoreStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listtablerestorestatuspaginator)
         """
 
-
 class ListUsageLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListUsageLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listusagelimitspaginator)
     """
 
     def paginate(
         self,
         *,
         resourceArn: str = ...,
         usageType: UsageLimitUsageTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsageLimitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListUsageLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listusagelimitspaginator)
         """
 
-
 class ListWorkgroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listworkgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkgroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listworkgroupspaginator)
         """
```

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/paginator.pyi` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/paginator.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,137 +54,146 @@
     "ListRecoveryPointsPaginator",
     "ListSnapshotsPaginator",
     "ListTableRestoreStatusPaginator",
     "ListUsageLimitsPaginator",
     "ListWorkgroupsPaginator",
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
 class ListEndpointAccessPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListEndpointAccess)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listendpointaccesspaginator)
     """
 
     def paginate(
         self,
         *,
         vpcId: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEndpointAccessResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListEndpointAccess.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listendpointaccesspaginator)
         """
 
+
 class ListNamespacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listnamespacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listnamespacespaginator)
         """
 
+
 class ListRecoveryPointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listrecoverypointspaginator)
     """
 
     def paginate(
         self,
         *,
         endTime: Union[datetime, str] = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         startTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecoveryPointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listrecoverypointspaginator)
         """
 
+
 class ListSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listsnapshotspaginator)
     """
 
     def paginate(
         self,
         *,
         endTime: Union[datetime, str] = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         ownerAccount: str = ...,
         startTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listsnapshotspaginator)
         """
 
+
 class ListTableRestoreStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListTableRestoreStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listtablerestorestatuspaginator)
     """
 
     def paginate(
         self,
         *,
         namespaceName: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTableRestoreStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListTableRestoreStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listtablerestorestatuspaginator)
         """
 
+
 class ListUsageLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListUsageLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listusagelimitspaginator)
     """
 
     def paginate(
         self,
         *,
         resourceArn: str = ...,
         usageType: UsageLimitUsageTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsageLimitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListUsageLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listusagelimitspaginator)
         """
 
+
 class ListWorkgroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listworkgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkgroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listworkgroupspaginator)
         """
```

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/type_defs.py` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/type_defs.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -26,70 +26,76 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ConfigParameterTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "SnapshotTypeDef",
     "CreateEndpointAccessRequestRequestTypeDef",
     "NamespaceTypeDef",
     "CreateUsageLimitRequestRequestTypeDef",
     "UsageLimitTypeDef",
     "DeleteEndpointAccessRequestRequestTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
     "DeleteUsageLimitRequestRequestTypeDef",
     "DeleteWorkgroupRequestRequestTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "GetCredentialsRequestRequestTypeDef",
+    "GetCredentialsResponseTypeDef",
     "GetEndpointAccessRequestRequestTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetRecoveryPointRequestRequestTypeDef",
     "RecoveryPointTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetTableRestoreStatusRequestRequestTypeDef",
     "TableRestoreStatusTypeDef",
     "GetUsageLimitRequestRequestTypeDef",
     "GetWorkgroupRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
     "ListEndpointAccessRequestRequestTypeDef",
+    "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
     "ListRecoveryPointsRequestRequestTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
     "ListTableRestoreStatusRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
     "ListUsageLimitsRequestRequestTypeDef",
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
     "ListWorkgroupsRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
+    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "RestoreTableFromSnapshotRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEndpointAccessRequestRequestTypeDef",
     "UpdateNamespaceRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateUsageLimitRequestRequestTypeDef",
     "UpdateWorkgroupRequestRequestTypeDef",
     "ConvertRecoveryPointToSnapshotRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateWorkgroupRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "GetCredentialsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DeleteSnapshotResponseTypeDef",
     "GetSnapshotResponseTypeDef",
     "ListSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
     "CreateNamespaceResponseTypeDef",
@@ -107,21 +113,14 @@
     "GetRecoveryPointResponseTypeDef",
     "ListRecoveryPointsResponseTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
     "GetTableRestoreStatusResponseTypeDef",
     "ListTableRestoreStatusResponseTypeDef",
     "RestoreTableFromSnapshotResponseTypeDef",
-    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
-    "ListNamespacesRequestListNamespacesPaginateTypeDef",
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
     "VpcEndpointTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "CreateEndpointAccessResponseTypeDef",
     "DeleteEndpointAccessResponseTypeDef",
     "GetEndpointAccessResponseTypeDef",
     "ListEndpointAccessResponseTypeDef",
@@ -147,25 +146,14 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
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
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "accountsWithProvisionedRestoreAccess": List[str],
         "accountsWithRestoreAccess": List[str],
         "actualIncrementalBackupSizeInMegaBytes": float,
         "adminUsername": str,
@@ -201,22 +189,20 @@
     "_OptionalCreateEndpointAccessRequestRequestTypeDef",
     {
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateEndpointAccessRequestRequestTypeDef(
     _RequiredCreateEndpointAccessRequestRequestTypeDef,
     _OptionalCreateEndpointAccessRequestRequestTypeDef,
 ):
     pass
 
-
 NamespaceTypeDef = TypedDict(
     "NamespaceTypeDef",
     {
         "adminUsername": str,
         "creationDate": datetime,
         "dbName": str,
         "defaultIamRoleArn": str,
@@ -244,21 +230,19 @@
     {
         "breachAction": UsageLimitBreachActionType,
         "period": UsageLimitPeriodType,
     },
     total=False,
 )
 
-
 class CreateUsageLimitRequestRequestTypeDef(
     _RequiredCreateUsageLimitRequestRequestTypeDef, _OptionalCreateUsageLimitRequestRequestTypeDef
 ):
     pass
 
-
 UsageLimitTypeDef = TypedDict(
     "UsageLimitTypeDef",
     {
         "amount": int,
         "breachAction": UsageLimitBreachActionType,
         "period": UsageLimitPeriodType,
         "resourceArn": str,
@@ -287,21 +271,19 @@
     {
         "finalSnapshotName": str,
         "finalSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
-
 class DeleteNamespaceRequestRequestTypeDef(
     _RequiredDeleteNamespaceRequestRequestTypeDef, _OptionalDeleteNamespaceRequestRequestTypeDef
 ):
     pass
 
-
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -346,20 +328,29 @@
     {
         "dbName": str,
         "durationSeconds": int,
     },
     total=False,
 )
 
-
 class GetCredentialsRequestRequestTypeDef(
     _RequiredGetCredentialsRequestRequestTypeDef, _OptionalGetCredentialsRequestRequestTypeDef
 ):
     pass
 
+GetCredentialsResponseTypeDef = TypedDict(
+    "GetCredentialsResponseTypeDef",
+    {
+        "dbPassword": str,
+        "dbUser": str,
+        "expiration": datetime,
+        "nextRefreshTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 GetEndpointAccessRequestRequestTypeDef = TypedDict(
     "GetEndpointAccessRequestRequestTypeDef",
     {
         "endpointName": str,
     },
 )
@@ -456,20 +447,20 @@
 GetWorkgroupRequestRequestTypeDef = TypedDict(
     "GetWorkgroupRequestRequestTypeDef",
     {
         "workgroupName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = TypedDict(
+    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "vpcId": str,
+        "workgroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListEndpointAccessRequestRequestTypeDef = TypedDict(
     "ListEndpointAccessRequestRequestTypeDef",
     {
@@ -477,50 +468,93 @@
         "nextToken": str,
         "vpcId": str,
         "workgroupName": str,
     },
     total=False,
 )
 
+ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
+    "ListNamespacesRequestListNamespacesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListNamespacesRequestRequestTypeDef = TypedDict(
     "ListNamespacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "namespaceArn": str,
+        "namespaceName": str,
+        "startTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRecoveryPointsRequestRequestTypeDef = TypedDict(
     "ListRecoveryPointsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "maxResults": int,
         "namespaceArn": str,
         "namespaceName": str,
         "nextToken": str,
         "startTime": Union[datetime, str],
     },
     total=False,
 )
 
+ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ownerAccount": str,
+        "startTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSnapshotsRequestRequestTypeDef = TypedDict(
     "ListSnapshotsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "maxResults": int,
         "namespaceArn": str,
         "namespaceName": str,
         "nextToken": str,
         "ownerAccount": str,
         "startTime": Union[datetime, str],
     },
     total=False,
 )
 
+ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+    {
+        "namespaceName": str,
+        "workgroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTableRestoreStatusRequestRequestTypeDef = TypedDict(
     "ListTableRestoreStatusRequestRequestTypeDef",
     {
         "maxResults": int,
         "namespaceName": str,
         "nextToken": str,
         "workgroupName": str,
@@ -531,25 +565,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "usageType": UsageLimitUsageTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListUsageLimitsRequestRequestTypeDef = TypedDict(
     "ListUsageLimitsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "resourceArn": str,
         "usageType": UsageLimitUsageTypeType,
     },
     total=False,
 )
 
+ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListWorkgroupsRequestRequestTypeDef = TypedDict(
     "ListWorkgroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -562,22 +614,43 @@
         "networkInterfaceId": str,
         "privateIpAddress": str,
         "subnetId": str,
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
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
 RestoreFromRecoveryPointRequestRequestTypeDef = TypedDict(
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     {
         "namespaceName": str,
         "recoveryPointId": str,
         "workgroupName": str,
     },
@@ -596,22 +669,20 @@
         "ownerAccount": str,
         "snapshotArn": str,
         "snapshotName": str,
     },
     total=False,
 )
 
-
 class RestoreFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreTableFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreTableFromSnapshotRequestRequestTypeDef",
     {
         "namespaceName": str,
         "newTableName": str,
         "snapshotName": str,
         "sourceDatabaseName": str,
@@ -626,22 +697,20 @@
         "sourceSchemaName": str,
         "targetDatabaseName": str,
         "targetSchemaName": str,
     },
     total=False,
 )
 
-
 class RestoreTableFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreTableFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreTableFromSnapshotRequestRequestTypeDef,
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
@@ -656,22 +725,20 @@
     "_OptionalUpdateEndpointAccessRequestRequestTypeDef",
     {
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateEndpointAccessRequestRequestTypeDef(
     _RequiredUpdateEndpointAccessRequestRequestTypeDef,
     _OptionalUpdateEndpointAccessRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNamespaceRequestRequestTypeDef",
     {
         "namespaceName": str,
     },
 )
 _OptionalUpdateNamespaceRequestRequestTypeDef = TypedDict(
@@ -683,42 +750,38 @@
         "iamRoles": Sequence[str],
         "kmsKeyId": str,
         "logExports": Sequence[LogExportType],
     },
     total=False,
 )
 
-
 class UpdateNamespaceRequestRequestTypeDef(
     _RequiredUpdateNamespaceRequestRequestTypeDef, _OptionalUpdateNamespaceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
         "snapshotName": str,
     },
 )
 _OptionalUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "retentionPeriod": int,
     },
     total=False,
 )
 
-
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateUsageLimitRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUsageLimitRequestRequestTypeDef",
     {
         "usageLimitId": str,
     },
 )
 _OptionalUpdateUsageLimitRequestRequestTypeDef = TypedDict(
@@ -726,21 +789,19 @@
     {
         "amount": int,
         "breachAction": UsageLimitBreachActionType,
     },
     total=False,
 )
 
-
 class UpdateUsageLimitRequestRequestTypeDef(
     _RequiredUpdateUsageLimitRequestRequestTypeDef, _OptionalUpdateUsageLimitRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateWorkgroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkgroupRequestRequestTypeDef",
     {
         "workgroupName": str,
     },
 )
 _OptionalUpdateWorkgroupRequestRequestTypeDef = TypedDict(
@@ -753,21 +814,19 @@
         "publiclyAccessible": bool,
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateWorkgroupRequestRequestTypeDef(
     _RequiredUpdateWorkgroupRequestRequestTypeDef, _OptionalUpdateWorkgroupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredConvertRecoveryPointToSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredConvertRecoveryPointToSnapshotRequestRequestTypeDef",
     {
         "recoveryPointId": str,
         "snapshotName": str,
     },
 )
@@ -776,22 +835,20 @@
     {
         "retentionPeriod": int,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ConvertRecoveryPointToSnapshotRequestRequestTypeDef(
     _RequiredConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     _OptionalConvertRecoveryPointToSnapshotRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNamespaceRequestRequestTypeDef",
     {
         "namespaceName": str,
     },
 )
 _OptionalCreateNamespaceRequestRequestTypeDef = TypedDict(
@@ -805,21 +862,19 @@
         "kmsKeyId": str,
         "logExports": Sequence[LogExportType],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateNamespaceRequestRequestTypeDef(
     _RequiredCreateNamespaceRequestRequestTypeDef, _OptionalCreateNamespaceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "namespaceName": str,
         "snapshotName": str,
     },
 )
@@ -828,21 +883,19 @@
     {
         "retentionPeriod": int,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateWorkgroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkgroupRequestRequestTypeDef",
     {
         "namespaceName": str,
         "workgroupName": str,
     },
 )
@@ -857,327 +910,243 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateWorkgroupRequestRequestTypeDef(
     _RequiredCreateWorkgroupRequestRequestTypeDef, _OptionalCreateWorkgroupRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
-GetCredentialsResponseTypeDef = TypedDict(
-    "GetCredentialsResponseTypeDef",
-    {
-        "dbPassword": str,
-        "dbUser": str,
-        "expiration": datetime,
-        "nextRefreshTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ConvertRecoveryPointToSnapshotResponseTypeDef = TypedDict(
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSnapshotResponseTypeDef = TypedDict(
     "CreateSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSnapshotResponseTypeDef = TypedDict(
     "DeleteSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSnapshotResponseTypeDef = TypedDict(
     "GetSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSnapshotsResponseTypeDef = TypedDict(
     "ListSnapshotsResponseTypeDef",
     {
         "nextToken": str,
         "snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSnapshotResponseTypeDef = TypedDict(
     "UpdateSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateNamespaceResponseTypeDef = TypedDict(
     "CreateNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteNamespaceResponseTypeDef = TypedDict(
     "DeleteNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNamespaceResponseTypeDef = TypedDict(
     "GetNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "namespaces": List[NamespaceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreFromRecoveryPointResponseTypeDef = TypedDict(
     "RestoreFromRecoveryPointResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
         "recoveryPointId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreFromSnapshotResponseTypeDef = TypedDict(
     "RestoreFromSnapshotResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
         "ownerAccount": str,
         "snapshotName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNamespaceResponseTypeDef = TypedDict(
     "UpdateNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateUsageLimitResponseTypeDef = TypedDict(
     "CreateUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteUsageLimitResponseTypeDef = TypedDict(
     "DeleteUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUsageLimitResponseTypeDef = TypedDict(
     "GetUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUsageLimitsResponseTypeDef = TypedDict(
     "ListUsageLimitsResponseTypeDef",
     {
         "nextToken": str,
         "usageLimits": List[UsageLimitTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUsageLimitResponseTypeDef = TypedDict(
     "UpdateUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecoveryPointResponseTypeDef = TypedDict(
     "GetRecoveryPointResponseTypeDef",
     {
         "recoveryPoint": RecoveryPointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecoveryPointsResponseTypeDef = TypedDict(
     "ListRecoveryPointsResponseTypeDef",
     {
         "nextToken": str,
         "recoveryPoints": List[RecoveryPointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourcePolicyResponseTypeDef = TypedDict(
     "GetResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutResourcePolicyResponseTypeDef = TypedDict(
     "PutResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTableRestoreStatusResponseTypeDef = TypedDict(
     "GetTableRestoreStatusResponseTypeDef",
     {
         "tableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTableRestoreStatusResponseTypeDef = TypedDict(
     "ListTableRestoreStatusResponseTypeDef",
     {
         "nextToken": str,
         "tableRestoreStatuses": List[TableRestoreStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreTableFromSnapshotResponseTypeDef = TypedDict(
     "RestoreTableFromSnapshotResponseTypeDef",
     {
         "tableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = TypedDict(
-    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
-    {
-        "vpcId": str,
-        "workgroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
-    "ListNamespacesRequestListNamespacesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
-        "namespaceName": str,
-        "startTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
-        "namespaceName": str,
-        "ownerAccount": str,
-        "startTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
-    {
-        "namespaceName": str,
-        "workgroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
-    {
-        "resourceArn": str,
-        "usageType": UsageLimitUsageTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "vpcEndpointId": str,
         "vpcId": str,
     },
@@ -1211,48 +1180,48 @@
     total=False,
 )
 
 CreateEndpointAccessResponseTypeDef = TypedDict(
     "CreateEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEndpointAccessResponseTypeDef = TypedDict(
     "DeleteEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEndpointAccessResponseTypeDef = TypedDict(
     "GetEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEndpointAccessResponseTypeDef = TypedDict(
     "ListEndpointAccessResponseTypeDef",
     {
         "endpoints": List[EndpointAccessTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointAccessResponseTypeDef = TypedDict(
     "UpdateEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkgroupTypeDef = TypedDict(
     "WorkgroupTypeDef",
     {
         "baseCapacity": int,
@@ -1273,43 +1242,43 @@
     total=False,
 )
 
 CreateWorkgroupResponseTypeDef = TypedDict(
     "CreateWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteWorkgroupResponseTypeDef = TypedDict(
     "DeleteWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkgroupResponseTypeDef = TypedDict(
     "GetWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkgroupsResponseTypeDef = TypedDict(
     "ListWorkgroupsResponseTypeDef",
     {
         "nextToken": str,
         "workgroups": List[WorkgroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateWorkgroupResponseTypeDef = TypedDict(
     "UpdateWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless/type_defs.pyi` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,69 +26,77 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ConfigParameterTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "SnapshotTypeDef",
     "CreateEndpointAccessRequestRequestTypeDef",
     "NamespaceTypeDef",
     "CreateUsageLimitRequestRequestTypeDef",
     "UsageLimitTypeDef",
     "DeleteEndpointAccessRequestRequestTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
     "DeleteUsageLimitRequestRequestTypeDef",
     "DeleteWorkgroupRequestRequestTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "GetCredentialsRequestRequestTypeDef",
+    "GetCredentialsResponseTypeDef",
     "GetEndpointAccessRequestRequestTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetRecoveryPointRequestRequestTypeDef",
     "RecoveryPointTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetTableRestoreStatusRequestRequestTypeDef",
     "TableRestoreStatusTypeDef",
     "GetUsageLimitRequestRequestTypeDef",
     "GetWorkgroupRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
     "ListEndpointAccessRequestRequestTypeDef",
+    "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
     "ListRecoveryPointsRequestRequestTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
     "ListTableRestoreStatusRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
     "ListUsageLimitsRequestRequestTypeDef",
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
     "ListWorkgroupsRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
+    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "RestoreTableFromSnapshotRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEndpointAccessRequestRequestTypeDef",
     "UpdateNamespaceRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateUsageLimitRequestRequestTypeDef",
     "UpdateWorkgroupRequestRequestTypeDef",
     "ConvertRecoveryPointToSnapshotRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateWorkgroupRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "GetCredentialsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DeleteSnapshotResponseTypeDef",
     "GetSnapshotResponseTypeDef",
     "ListSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
     "CreateNamespaceResponseTypeDef",
@@ -106,21 +114,14 @@
     "GetRecoveryPointResponseTypeDef",
     "ListRecoveryPointsResponseTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
     "GetTableRestoreStatusResponseTypeDef",
     "ListTableRestoreStatusResponseTypeDef",
     "RestoreTableFromSnapshotResponseTypeDef",
-    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
-    "ListNamespacesRequestListNamespacesPaginateTypeDef",
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
     "VpcEndpointTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "CreateEndpointAccessResponseTypeDef",
     "DeleteEndpointAccessResponseTypeDef",
     "GetEndpointAccessResponseTypeDef",
     "ListEndpointAccessResponseTypeDef",
@@ -146,25 +147,14 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
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
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "accountsWithProvisionedRestoreAccess": List[str],
         "accountsWithRestoreAccess": List[str],
         "actualIncrementalBackupSizeInMegaBytes": float,
         "adminUsername": str,
@@ -200,20 +190,22 @@
     "_OptionalCreateEndpointAccessRequestRequestTypeDef",
     {
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateEndpointAccessRequestRequestTypeDef(
     _RequiredCreateEndpointAccessRequestRequestTypeDef,
     _OptionalCreateEndpointAccessRequestRequestTypeDef,
 ):
     pass
 
+
 NamespaceTypeDef = TypedDict(
     "NamespaceTypeDef",
     {
         "adminUsername": str,
         "creationDate": datetime,
         "dbName": str,
         "defaultIamRoleArn": str,
@@ -241,19 +233,21 @@
     {
         "breachAction": UsageLimitBreachActionType,
         "period": UsageLimitPeriodType,
     },
     total=False,
 )
 
+
 class CreateUsageLimitRequestRequestTypeDef(
     _RequiredCreateUsageLimitRequestRequestTypeDef, _OptionalCreateUsageLimitRequestRequestTypeDef
 ):
     pass
 
+
 UsageLimitTypeDef = TypedDict(
     "UsageLimitTypeDef",
     {
         "amount": int,
         "breachAction": UsageLimitBreachActionType,
         "period": UsageLimitPeriodType,
         "resourceArn": str,
@@ -282,19 +276,21 @@
     {
         "finalSnapshotName": str,
         "finalSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
+
 class DeleteNamespaceRequestRequestTypeDef(
     _RequiredDeleteNamespaceRequestRequestTypeDef, _OptionalDeleteNamespaceRequestRequestTypeDef
 ):
     pass
 
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -339,19 +335,32 @@
     {
         "dbName": str,
         "durationSeconds": int,
     },
     total=False,
 )
 
+
 class GetCredentialsRequestRequestTypeDef(
     _RequiredGetCredentialsRequestRequestTypeDef, _OptionalGetCredentialsRequestRequestTypeDef
 ):
     pass
 
+
+GetCredentialsResponseTypeDef = TypedDict(
+    "GetCredentialsResponseTypeDef",
+    {
+        "dbPassword": str,
+        "dbUser": str,
+        "expiration": datetime,
+        "nextRefreshTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetEndpointAccessRequestRequestTypeDef = TypedDict(
     "GetEndpointAccessRequestRequestTypeDef",
     {
         "endpointName": str,
     },
 )
 
@@ -447,20 +456,20 @@
 GetWorkgroupRequestRequestTypeDef = TypedDict(
     "GetWorkgroupRequestRequestTypeDef",
     {
         "workgroupName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = TypedDict(
+    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "vpcId": str,
+        "workgroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListEndpointAccessRequestRequestTypeDef = TypedDict(
     "ListEndpointAccessRequestRequestTypeDef",
     {
@@ -468,50 +477,93 @@
         "nextToken": str,
         "vpcId": str,
         "workgroupName": str,
     },
     total=False,
 )
 
+ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
+    "ListNamespacesRequestListNamespacesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListNamespacesRequestRequestTypeDef = TypedDict(
     "ListNamespacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "namespaceArn": str,
+        "namespaceName": str,
+        "startTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRecoveryPointsRequestRequestTypeDef = TypedDict(
     "ListRecoveryPointsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "maxResults": int,
         "namespaceArn": str,
         "namespaceName": str,
         "nextToken": str,
         "startTime": Union[datetime, str],
     },
     total=False,
 )
 
+ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ownerAccount": str,
+        "startTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSnapshotsRequestRequestTypeDef = TypedDict(
     "ListSnapshotsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "maxResults": int,
         "namespaceArn": str,
         "namespaceName": str,
         "nextToken": str,
         "ownerAccount": str,
         "startTime": Union[datetime, str],
     },
     total=False,
 )
 
+ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+    {
+        "namespaceName": str,
+        "workgroupName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTableRestoreStatusRequestRequestTypeDef = TypedDict(
     "ListTableRestoreStatusRequestRequestTypeDef",
     {
         "maxResults": int,
         "namespaceName": str,
         "nextToken": str,
         "workgroupName": str,
@@ -522,25 +574,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "usageType": UsageLimitUsageTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListUsageLimitsRequestRequestTypeDef = TypedDict(
     "ListUsageLimitsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "resourceArn": str,
         "usageType": UsageLimitUsageTypeType,
     },
     total=False,
 )
 
+ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListWorkgroupsRequestRequestTypeDef = TypedDict(
     "ListWorkgroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -553,22 +623,43 @@
         "networkInterfaceId": str,
         "privateIpAddress": str,
         "subnetId": str,
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
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
 RestoreFromRecoveryPointRequestRequestTypeDef = TypedDict(
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     {
         "namespaceName": str,
         "recoveryPointId": str,
         "workgroupName": str,
     },
@@ -587,20 +678,22 @@
         "ownerAccount": str,
         "snapshotArn": str,
         "snapshotName": str,
     },
     total=False,
 )
 
+
 class RestoreFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreTableFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreTableFromSnapshotRequestRequestTypeDef",
     {
         "namespaceName": str,
         "newTableName": str,
         "snapshotName": str,
         "sourceDatabaseName": str,
@@ -615,20 +708,22 @@
         "sourceSchemaName": str,
         "targetDatabaseName": str,
         "targetSchemaName": str,
     },
     total=False,
 )
 
+
 class RestoreTableFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreTableFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreTableFromSnapshotRequestRequestTypeDef,
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
@@ -643,20 +738,22 @@
     "_OptionalUpdateEndpointAccessRequestRequestTypeDef",
     {
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateEndpointAccessRequestRequestTypeDef(
     _RequiredUpdateEndpointAccessRequestRequestTypeDef,
     _OptionalUpdateEndpointAccessRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNamespaceRequestRequestTypeDef",
     {
         "namespaceName": str,
     },
 )
 _OptionalUpdateNamespaceRequestRequestTypeDef = TypedDict(
@@ -668,38 +765,42 @@
         "iamRoles": Sequence[str],
         "kmsKeyId": str,
         "logExports": Sequence[LogExportType],
     },
     total=False,
 )
 
+
 class UpdateNamespaceRequestRequestTypeDef(
     _RequiredUpdateNamespaceRequestRequestTypeDef, _OptionalUpdateNamespaceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
         "snapshotName": str,
     },
 )
 _OptionalUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "retentionPeriod": int,
     },
     total=False,
 )
 
+
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateUsageLimitRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUsageLimitRequestRequestTypeDef",
     {
         "usageLimitId": str,
     },
 )
 _OptionalUpdateUsageLimitRequestRequestTypeDef = TypedDict(
@@ -707,19 +808,21 @@
     {
         "amount": int,
         "breachAction": UsageLimitBreachActionType,
     },
     total=False,
 )
 
+
 class UpdateUsageLimitRequestRequestTypeDef(
     _RequiredUpdateUsageLimitRequestRequestTypeDef, _OptionalUpdateUsageLimitRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateWorkgroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkgroupRequestRequestTypeDef",
     {
         "workgroupName": str,
     },
 )
 _OptionalUpdateWorkgroupRequestRequestTypeDef = TypedDict(
@@ -732,19 +835,21 @@
         "publiclyAccessible": bool,
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateWorkgroupRequestRequestTypeDef(
     _RequiredUpdateWorkgroupRequestRequestTypeDef, _OptionalUpdateWorkgroupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredConvertRecoveryPointToSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredConvertRecoveryPointToSnapshotRequestRequestTypeDef",
     {
         "recoveryPointId": str,
         "snapshotName": str,
     },
 )
@@ -753,20 +858,22 @@
     {
         "retentionPeriod": int,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ConvertRecoveryPointToSnapshotRequestRequestTypeDef(
     _RequiredConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     _OptionalConvertRecoveryPointToSnapshotRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNamespaceRequestRequestTypeDef",
     {
         "namespaceName": str,
     },
 )
 _OptionalCreateNamespaceRequestRequestTypeDef = TypedDict(
@@ -780,19 +887,21 @@
         "kmsKeyId": str,
         "logExports": Sequence[LogExportType],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateNamespaceRequestRequestTypeDef(
     _RequiredCreateNamespaceRequestRequestTypeDef, _OptionalCreateNamespaceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "namespaceName": str,
         "snapshotName": str,
     },
 )
@@ -801,19 +910,21 @@
     {
         "retentionPeriod": int,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateWorkgroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkgroupRequestRequestTypeDef",
     {
         "namespaceName": str,
         "workgroupName": str,
     },
 )
@@ -828,323 +939,243 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateWorkgroupRequestRequestTypeDef(
     _RequiredCreateWorkgroupRequestRequestTypeDef, _OptionalCreateWorkgroupRequestRequestTypeDef
 ):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
 
-GetCredentialsResponseTypeDef = TypedDict(
-    "GetCredentialsResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "dbPassword": str,
-        "dbUser": str,
-        "expiration": datetime,
-        "nextRefreshTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
 ConvertRecoveryPointToSnapshotResponseTypeDef = TypedDict(
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSnapshotResponseTypeDef = TypedDict(
     "CreateSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSnapshotResponseTypeDef = TypedDict(
     "DeleteSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSnapshotResponseTypeDef = TypedDict(
     "GetSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSnapshotsResponseTypeDef = TypedDict(
     "ListSnapshotsResponseTypeDef",
     {
         "nextToken": str,
         "snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSnapshotResponseTypeDef = TypedDict(
     "UpdateSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateNamespaceResponseTypeDef = TypedDict(
     "CreateNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteNamespaceResponseTypeDef = TypedDict(
     "DeleteNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNamespaceResponseTypeDef = TypedDict(
     "GetNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "namespaces": List[NamespaceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreFromRecoveryPointResponseTypeDef = TypedDict(
     "RestoreFromRecoveryPointResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
         "recoveryPointId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreFromSnapshotResponseTypeDef = TypedDict(
     "RestoreFromSnapshotResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
         "ownerAccount": str,
         "snapshotName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNamespaceResponseTypeDef = TypedDict(
     "UpdateNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateUsageLimitResponseTypeDef = TypedDict(
     "CreateUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteUsageLimitResponseTypeDef = TypedDict(
     "DeleteUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUsageLimitResponseTypeDef = TypedDict(
     "GetUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUsageLimitsResponseTypeDef = TypedDict(
     "ListUsageLimitsResponseTypeDef",
     {
         "nextToken": str,
         "usageLimits": List[UsageLimitTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUsageLimitResponseTypeDef = TypedDict(
     "UpdateUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecoveryPointResponseTypeDef = TypedDict(
     "GetRecoveryPointResponseTypeDef",
     {
         "recoveryPoint": RecoveryPointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecoveryPointsResponseTypeDef = TypedDict(
     "ListRecoveryPointsResponseTypeDef",
     {
         "nextToken": str,
         "recoveryPoints": List[RecoveryPointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourcePolicyResponseTypeDef = TypedDict(
     "GetResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutResourcePolicyResponseTypeDef = TypedDict(
     "PutResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTableRestoreStatusResponseTypeDef = TypedDict(
     "GetTableRestoreStatusResponseTypeDef",
     {
         "tableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTableRestoreStatusResponseTypeDef = TypedDict(
     "ListTableRestoreStatusResponseTypeDef",
     {
         "nextToken": str,
         "tableRestoreStatuses": List[TableRestoreStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreTableFromSnapshotResponseTypeDef = TypedDict(
     "RestoreTableFromSnapshotResponseTypeDef",
     {
         "tableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = TypedDict(
-    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
-    {
-        "vpcId": str,
-        "workgroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
-    "ListNamespacesRequestListNamespacesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
-        "namespaceName": str,
-        "startTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
-        "namespaceName": str,
-        "ownerAccount": str,
-        "startTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
-    {
-        "namespaceName": str,
-        "workgroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
-    {
-        "resourceArn": str,
-        "usageType": UsageLimitUsageTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "vpcEndpointId": str,
@@ -1180,48 +1211,48 @@
     total=False,
 )
 
 CreateEndpointAccessResponseTypeDef = TypedDict(
     "CreateEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEndpointAccessResponseTypeDef = TypedDict(
     "DeleteEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEndpointAccessResponseTypeDef = TypedDict(
     "GetEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEndpointAccessResponseTypeDef = TypedDict(
     "ListEndpointAccessResponseTypeDef",
     {
         "endpoints": List[EndpointAccessTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointAccessResponseTypeDef = TypedDict(
     "UpdateEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkgroupTypeDef = TypedDict(
     "WorkgroupTypeDef",
     {
         "baseCapacity": int,
@@ -1242,43 +1273,43 @@
     total=False,
 )
 
 CreateWorkgroupResponseTypeDef = TypedDict(
     "CreateWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteWorkgroupResponseTypeDef = TypedDict(
     "DeleteWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkgroupResponseTypeDef = TypedDict(
     "GetWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkgroupsResponseTypeDef = TypedDict(
     "ListWorkgroupsResponseTypeDef",
     {
         "nextToken": str,
         "workgroups": List[WorkgroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateWorkgroupResponseTypeDef = TypedDict(
     "UpdateWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless.egg-info/PKG-INFO` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-serverless
-Version: 1.26.57
-Summary: Type annotations for boto3.RedshiftServerless 1.26.57 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.RedshiftServerless 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-redshift-serverless"></a>
 
 # mypy-boto3-redshift-serverless
 
 [![PyPI - mypy-boto3-redshift-serverless](https://img.shields.io/pypi/v/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.26.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,66 +355,73 @@
 `mypy_boto3_redshift_serverless.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_serverless.type_defs import (
     ConfigParameterTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     SnapshotTypeDef,
     CreateEndpointAccessRequestRequestTypeDef,
     NamespaceTypeDef,
     CreateUsageLimitRequestRequestTypeDef,
     UsageLimitTypeDef,
     DeleteEndpointAccessRequestRequestTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteUsageLimitRequestRequestTypeDef,
     DeleteWorkgroupRequestRequestTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     GetCredentialsRequestRequestTypeDef,
+    GetCredentialsResponseTypeDef,
     GetEndpointAccessRequestRequestTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetRecoveryPointRequestRequestTypeDef,
     RecoveryPointTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     ResourcePolicyTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetTableRestoreStatusRequestRequestTypeDef,
     TableRestoreStatusTypeDef,
     GetUsageLimitRequestRequestTypeDef,
     GetWorkgroupRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
+    ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
+    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
     ListRecoveryPointsRequestRequestTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
+    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
+    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     RestoreTableFromSnapshotRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEndpointAccessRequestRequestTypeDef,
     UpdateNamespaceRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateUsageLimitRequestRequestTypeDef,
     UpdateWorkgroupRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateWorkgroupRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    GetCredentialsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     GetSnapshotResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateNamespaceResponseTypeDef,
@@ -432,21 +439,14 @@
     GetRecoveryPointResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     GetTableRestoreStatusResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
-    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
-    ListNamespacesRequestListNamespacesPaginateTypeDef,
-    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
-    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
-    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -467,42 +467,42 @@
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

### Comparing `mypy-boto3-redshift-serverless-1.26.57/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt` & `mypy-boto3-redshift-serverless-1.27.0/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.26.57/setup.py` & `mypy-boto3-redshift-serverless-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-redshift-serverless.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift-serverless",
-    version="1.26.57",
+    version="1.27.0",
     packages=["mypy_boto3_redshift_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RedshiftServerless 1.26.57 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.RedshiftServerless 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -47,11 +47,11 @@
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/"
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


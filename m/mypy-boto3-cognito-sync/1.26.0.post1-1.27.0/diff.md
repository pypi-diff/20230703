# Comparing `tmp/mypy-boto3-cognito-sync-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-cognito-sync-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-sync-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:16 2022, max compression
+gzip compressed data, was "mypy-boto3-cognito-sync-1.27.0.tar", last modified: Mon Jul  3 19:50:34 2023, max compression
```

## Comparing `mypy-boto3-cognito-sync-1.26.0.post1.tar` & `mypy-boto3-cognito-sync-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:16.144819 mypy-boto3-cognito-sync-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13652 2022-11-01 21:43:16.140819 mypy-boto3-cognito-sync-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12192 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:16.136819 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14125 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    14102 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7437 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7435 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    12740 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    12730 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:32:08.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:16.136819 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13652 2022-11-01 21:43:15.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-11-01 21:43:15.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:15.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:15.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:15.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-01 21:43:15.000000 mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:16.144819 mypy-boto3-cognito-sync-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-11-01 21:32:07.000000 mypy-boto3-cognito-sync-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.195028 mypy-boto3-cognito-sync-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-03 19:50:34.195028 mypy-boto3-cognito-sync-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.191028 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.195028 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-03 19:50:34.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 19:50:34.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:34.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:34.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:34.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:34.000000 mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:34.195028 mypy-boto3-cognito-sync-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-03 19:34:38.000000 mypy-boto3-cognito-sync-1.27.0/setup.py
```

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/LICENSE` & `mypy-boto3-cognito-sync-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/PKG-INFO` & `mypy-boto3-cognito-sync-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-sync
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CognitoSync 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CognitoSync 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/
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
 
 <a id="mypy-boto3-cognito-sync"></a>
 
 # mypy-boto3-cognito-sync
 
 [![PyPI - mypy-boto3-cognito-sync](https://img.shields.io/pypi/v/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-sync?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoSync 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[boto3.CognitoSync 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
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
 [mypy-boto3-cognito-sync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,41 +301,41 @@
 
 `mypy_boto3_cognito_sync.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_sync.type_defs import (
     BulkPublishRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    BulkPublishResponseTypeDef,
     CognitoStreamsTypeDef,
     DatasetTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeIdentityPoolUsageRequestRequestTypeDef,
     IdentityPoolUsageTypeDef,
     DescribeIdentityUsageRequestRequestTypeDef,
     IdentityUsageTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsRequestRequestTypeDef,
+    GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsRequestRequestTypeDef,
+    GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationRequestRequestTypeDef,
     PushSyncTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListIdentityPoolUsageRequestRequestTypeDef,
     ListRecordsRequestRequestTypeDef,
     RecordTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceRequestRequestTypeDef,
+    RegisterDeviceResponseTypeDef,
+    ResponseMetadataTypeDef,
     SetCognitoEventsRequestRequestTypeDef,
     SubscribeToDatasetRequestRequestTypeDef,
     UnsubscribeFromDatasetRequestRequestTypeDef,
-    BulkPublishResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetBulkPublishDetailsResponseTypeDef,
-    GetCognitoEventsResponseTypeDef,
-    RegisterDeviceResponseTypeDef,
     DeleteDatasetResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeIdentityPoolUsageResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     DescribeIdentityUsageResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
@@ -353,42 +354,42 @@
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

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/README.md` & `mypy-boto3-cognito-sync-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cognito-sync"></a>
 
 # mypy-boto3-cognito-sync
 
 [![PyPI - mypy-boto3-cognito-sync](https://img.shields.io/pypi/v/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-sync?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoSync 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[boto3.CognitoSync 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
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
 [mypy-boto3-cognito-sync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,41 +269,41 @@
 
 `mypy_boto3_cognito_sync.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_sync.type_defs import (
     BulkPublishRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    BulkPublishResponseTypeDef,
     CognitoStreamsTypeDef,
     DatasetTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeIdentityPoolUsageRequestRequestTypeDef,
     IdentityPoolUsageTypeDef,
     DescribeIdentityUsageRequestRequestTypeDef,
     IdentityUsageTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsRequestRequestTypeDef,
+    GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsRequestRequestTypeDef,
+    GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationRequestRequestTypeDef,
     PushSyncTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListIdentityPoolUsageRequestRequestTypeDef,
     ListRecordsRequestRequestTypeDef,
     RecordTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceRequestRequestTypeDef,
+    RegisterDeviceResponseTypeDef,
+    ResponseMetadataTypeDef,
     SetCognitoEventsRequestRequestTypeDef,
     SubscribeToDatasetRequestRequestTypeDef,
     UnsubscribeFromDatasetRequestRequestTypeDef,
-    BulkPublishResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetBulkPublishDetailsResponseTypeDef,
-    GetCognitoEventsResponseTypeDef,
-    RegisterDeviceResponseTypeDef,
     DeleteDatasetResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeIdentityPoolUsageResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     DescribeIdentityUsageResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
@@ -322,42 +322,42 @@
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

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/__main__.py` & `mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoSync 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CognitoSync 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/client.py` & `mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/client.pyi` & `mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/literals.py` & `mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BulkPublishStatusType",
     "OperationType",
     "PlatformType",
     "StreamingStatusType",
     "CognitoSyncServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 BulkPublishStatusType = Literal["FAILED", "IN_PROGRESS", "NOT_STARTED", "SUCCEEDED"]
 OperationType = Literal["remove", "replace"]
 PlatformType = Literal["ADM", "APNS", "APNS_SANDBOX", "GCM"]
 StreamingStatusType = Literal["DISABLED", "ENABLED"]
 CognitoSyncServiceName = Literal["cognito-sync"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -47,23 +45,25 @@
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
@@ -73,30 +73,35 @@
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
@@ -122,14 +127,15 @@
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
@@ -174,51 +180,57 @@
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
@@ -231,14 +243,15 @@
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
@@ -250,28 +263,35 @@
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
@@ -280,14 +300,15 @@
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
@@ -298,55 +319,64 @@
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

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/literals.pyi` & `mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "BulkPublishStatusType",
     "OperationType",
     "PlatformType",
     "StreamingStatusType",
     "CognitoSyncServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 BulkPublishStatusType = Literal["FAILED", "IN_PROGRESS", "NOT_STARTED", "SUCCEEDED"]
 OperationType = Literal["remove", "replace"]
 PlatformType = Literal["ADM", "APNS", "APNS_SANDBOX", "GCM"]
 StreamingStatusType = Literal["DISABLED", "ENABLED"]
 CognitoSyncServiceName = Literal["cognito-sync"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -45,23 +47,25 @@
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
@@ -71,30 +75,35 @@
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
@@ -120,14 +129,15 @@
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
@@ -172,51 +182,57 @@
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
@@ -229,14 +245,15 @@
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
@@ -248,28 +265,35 @@
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
@@ -278,14 +302,15 @@
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
@@ -296,55 +321,64 @@
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

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/type_defs.py` & `mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,41 +21,41 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BulkPublishRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "BulkPublishResponseTypeDef",
     "CognitoStreamsTypeDef",
     "DatasetTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeIdentityPoolUsageRequestRequestTypeDef",
     "IdentityPoolUsageTypeDef",
     "DescribeIdentityUsageRequestRequestTypeDef",
     "IdentityUsageTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetBulkPublishDetailsRequestRequestTypeDef",
+    "GetBulkPublishDetailsResponseTypeDef",
     "GetCognitoEventsRequestRequestTypeDef",
+    "GetCognitoEventsResponseTypeDef",
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     "PushSyncTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListIdentityPoolUsageRequestRequestTypeDef",
     "ListRecordsRequestRequestTypeDef",
     "RecordTypeDef",
     "RecordPatchTypeDef",
     "RegisterDeviceRequestRequestTypeDef",
+    "RegisterDeviceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SetCognitoEventsRequestRequestTypeDef",
     "SubscribeToDatasetRequestRequestTypeDef",
     "UnsubscribeFromDatasetRequestRequestTypeDef",
-    "BulkPublishResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetBulkPublishDetailsResponseTypeDef",
-    "GetCognitoEventsResponseTypeDef",
-    "RegisterDeviceResponseTypeDef",
     "DeleteDatasetResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeIdentityPoolUsageResponseTypeDef",
     "ListIdentityPoolUsageResponseTypeDef",
     "DescribeIdentityUsageResponseTypeDef",
     "GetIdentityPoolConfigurationResponseTypeDef",
@@ -69,22 +69,19 @@
 BulkPublishRequestRequestTypeDef = TypedDict(
     "BulkPublishRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+BulkPublishResponseTypeDef = TypedDict(
+    "BulkPublishResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "IdentityPoolId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CognitoStreamsTypeDef = TypedDict(
     "CognitoStreamsTypeDef",
     {
         "StreamName": str,
@@ -160,28 +157,55 @@
         "LastModifiedDate": datetime,
         "DatasetCount": int,
         "DataStorage": int,
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
 GetBulkPublishDetailsRequestRequestTypeDef = TypedDict(
     "GetBulkPublishDetailsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
+GetBulkPublishDetailsResponseTypeDef = TypedDict(
+    "GetBulkPublishDetailsResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "BulkPublishStartTime": datetime,
+        "BulkPublishCompleteTime": datetime,
+        "BulkPublishStatus": BulkPublishStatusType,
+        "FailureMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetCognitoEventsRequestRequestTypeDef = TypedDict(
     "GetCognitoEventsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
+GetCognitoEventsResponseTypeDef = TypedDict(
+    "GetCognitoEventsResponseTypeDef",
+    {
+        "Events": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
@@ -293,14 +317,33 @@
         "IdentityPoolId": str,
         "IdentityId": str,
         "Platform": PlatformType,
         "Token": str,
     },
 )
 
+RegisterDeviceResponseTypeDef = TypedDict(
+    "RegisterDeviceResponseTypeDef",
+    {
+        "DeviceId": str,
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
 SetCognitoEventsRequestRequestTypeDef = TypedDict(
     "SetCognitoEventsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "Events": Mapping[str, str],
     },
 )
@@ -321,117 +364,74 @@
         "IdentityPoolId": str,
         "IdentityId": str,
         "DatasetName": str,
         "DeviceId": str,
     },
 )
 
-BulkPublishResponseTypeDef = TypedDict(
-    "BulkPublishResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBulkPublishDetailsResponseTypeDef = TypedDict(
-    "GetBulkPublishDetailsResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "BulkPublishStartTime": datetime,
-        "BulkPublishCompleteTime": datetime,
-        "BulkPublishStatus": BulkPublishStatusType,
-        "FailureMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCognitoEventsResponseTypeDef = TypedDict(
-    "GetCognitoEventsResponseTypeDef",
-    {
-        "Events": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterDeviceResponseTypeDef = TypedDict(
-    "RegisterDeviceResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeleteDatasetResponseTypeDef = TypedDict(
     "DeleteDatasetResponseTypeDef",
     {
         "Dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "Dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetTypeDef],
         "Count": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeIdentityPoolUsageResponseTypeDef = TypedDict(
     "DescribeIdentityPoolUsageResponseTypeDef",
     {
         "IdentityPoolUsage": IdentityPoolUsageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentityPoolUsageResponseTypeDef = TypedDict(
     "ListIdentityPoolUsageResponseTypeDef",
     {
         "IdentityPoolUsages": List[IdentityPoolUsageTypeDef],
         "MaxResults": int,
         "Count": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeIdentityUsageResponseTypeDef = TypedDict(
     "DescribeIdentityUsageResponseTypeDef",
     {
         "IdentityUsage": IdentityUsageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "GetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
         "PushSync": PushSyncTypeDef,
         "CognitoStreams": CognitoStreamsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
@@ -456,15 +456,15 @@
 
 SetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "SetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
         "PushSync": PushSyncTypeDef,
         "CognitoStreams": CognitoStreamsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecordsResponseTypeDef = TypedDict(
     "ListRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
@@ -472,23 +472,23 @@
         "Count": int,
         "DatasetSyncCount": int,
         "LastModifiedBy": str,
         "MergedDatasetNames": List[str],
         "DatasetExists": bool,
         "DatasetDeletedAfterRequestedSyncCount": bool,
         "SyncSessionToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRecordsResponseTypeDef = TypedDict(
     "UpdateRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRecordsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
```

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync/type_defs.pyi` & `mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -20,41 +20,41 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BulkPublishRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "BulkPublishResponseTypeDef",
     "CognitoStreamsTypeDef",
     "DatasetTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeIdentityPoolUsageRequestRequestTypeDef",
     "IdentityPoolUsageTypeDef",
     "DescribeIdentityUsageRequestRequestTypeDef",
     "IdentityUsageTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetBulkPublishDetailsRequestRequestTypeDef",
+    "GetBulkPublishDetailsResponseTypeDef",
     "GetCognitoEventsRequestRequestTypeDef",
+    "GetCognitoEventsResponseTypeDef",
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     "PushSyncTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListIdentityPoolUsageRequestRequestTypeDef",
     "ListRecordsRequestRequestTypeDef",
     "RecordTypeDef",
     "RecordPatchTypeDef",
     "RegisterDeviceRequestRequestTypeDef",
+    "RegisterDeviceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SetCognitoEventsRequestRequestTypeDef",
     "SubscribeToDatasetRequestRequestTypeDef",
     "UnsubscribeFromDatasetRequestRequestTypeDef",
-    "BulkPublishResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetBulkPublishDetailsResponseTypeDef",
-    "GetCognitoEventsResponseTypeDef",
-    "RegisterDeviceResponseTypeDef",
     "DeleteDatasetResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeIdentityPoolUsageResponseTypeDef",
     "ListIdentityPoolUsageResponseTypeDef",
     "DescribeIdentityUsageResponseTypeDef",
     "GetIdentityPoolConfigurationResponseTypeDef",
@@ -68,22 +68,19 @@
 BulkPublishRequestRequestTypeDef = TypedDict(
     "BulkPublishRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+BulkPublishResponseTypeDef = TypedDict(
+    "BulkPublishResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "IdentityPoolId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CognitoStreamsTypeDef = TypedDict(
     "CognitoStreamsTypeDef",
     {
         "StreamName": str,
@@ -159,28 +156,55 @@
         "LastModifiedDate": datetime,
         "DatasetCount": int,
         "DataStorage": int,
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
 GetBulkPublishDetailsRequestRequestTypeDef = TypedDict(
     "GetBulkPublishDetailsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
+GetBulkPublishDetailsResponseTypeDef = TypedDict(
+    "GetBulkPublishDetailsResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "BulkPublishStartTime": datetime,
+        "BulkPublishCompleteTime": datetime,
+        "BulkPublishStatus": BulkPublishStatusType,
+        "FailureMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetCognitoEventsRequestRequestTypeDef = TypedDict(
     "GetCognitoEventsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
+GetCognitoEventsResponseTypeDef = TypedDict(
+    "GetCognitoEventsResponseTypeDef",
+    {
+        "Events": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
@@ -286,14 +310,33 @@
         "IdentityPoolId": str,
         "IdentityId": str,
         "Platform": PlatformType,
         "Token": str,
     },
 )
 
+RegisterDeviceResponseTypeDef = TypedDict(
+    "RegisterDeviceResponseTypeDef",
+    {
+        "DeviceId": str,
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
 SetCognitoEventsRequestRequestTypeDef = TypedDict(
     "SetCognitoEventsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "Events": Mapping[str, str],
     },
 )
@@ -314,117 +357,74 @@
         "IdentityPoolId": str,
         "IdentityId": str,
         "DatasetName": str,
         "DeviceId": str,
     },
 )
 
-BulkPublishResponseTypeDef = TypedDict(
-    "BulkPublishResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBulkPublishDetailsResponseTypeDef = TypedDict(
-    "GetBulkPublishDetailsResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "BulkPublishStartTime": datetime,
-        "BulkPublishCompleteTime": datetime,
-        "BulkPublishStatus": BulkPublishStatusType,
-        "FailureMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCognitoEventsResponseTypeDef = TypedDict(
-    "GetCognitoEventsResponseTypeDef",
-    {
-        "Events": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterDeviceResponseTypeDef = TypedDict(
-    "RegisterDeviceResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeleteDatasetResponseTypeDef = TypedDict(
     "DeleteDatasetResponseTypeDef",
     {
         "Dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "Dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetTypeDef],
         "Count": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeIdentityPoolUsageResponseTypeDef = TypedDict(
     "DescribeIdentityPoolUsageResponseTypeDef",
     {
         "IdentityPoolUsage": IdentityPoolUsageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentityPoolUsageResponseTypeDef = TypedDict(
     "ListIdentityPoolUsageResponseTypeDef",
     {
         "IdentityPoolUsages": List[IdentityPoolUsageTypeDef],
         "MaxResults": int,
         "Count": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeIdentityUsageResponseTypeDef = TypedDict(
     "DescribeIdentityUsageResponseTypeDef",
     {
         "IdentityUsage": IdentityUsageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "GetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
         "PushSync": PushSyncTypeDef,
         "CognitoStreams": CognitoStreamsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
@@ -447,15 +447,15 @@
 
 SetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "SetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
         "PushSync": PushSyncTypeDef,
         "CognitoStreams": CognitoStreamsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecordsResponseTypeDef = TypedDict(
     "ListRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
@@ -463,23 +463,23 @@
         "Count": int,
         "DatasetSyncCount": int,
         "LastModifiedBy": str,
         "MergedDatasetNames": List[str],
         "DatasetExists": bool,
         "DatasetDeletedAfterRequestedSyncCount": bool,
         "SyncSessionToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRecordsResponseTypeDef = TypedDict(
     "UpdateRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRecordsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
```

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync.egg-info/PKG-INFO` & `mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-sync
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CognitoSync 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CognitoSync 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/
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
 
 <a id="mypy-boto3-cognito-sync"></a>
 
 # mypy-boto3-cognito-sync
 
 [![PyPI - mypy-boto3-cognito-sync](https://img.shields.io/pypi/v/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-sync?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoSync 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[boto3.CognitoSync 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
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
 [mypy-boto3-cognito-sync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,41 +301,41 @@
 
 `mypy_boto3_cognito_sync.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_sync.type_defs import (
     BulkPublishRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    BulkPublishResponseTypeDef,
     CognitoStreamsTypeDef,
     DatasetTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeIdentityPoolUsageRequestRequestTypeDef,
     IdentityPoolUsageTypeDef,
     DescribeIdentityUsageRequestRequestTypeDef,
     IdentityUsageTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsRequestRequestTypeDef,
+    GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsRequestRequestTypeDef,
+    GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationRequestRequestTypeDef,
     PushSyncTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListIdentityPoolUsageRequestRequestTypeDef,
     ListRecordsRequestRequestTypeDef,
     RecordTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceRequestRequestTypeDef,
+    RegisterDeviceResponseTypeDef,
+    ResponseMetadataTypeDef,
     SetCognitoEventsRequestRequestTypeDef,
     SubscribeToDatasetRequestRequestTypeDef,
     UnsubscribeFromDatasetRequestRequestTypeDef,
-    BulkPublishResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetBulkPublishDetailsResponseTypeDef,
-    GetCognitoEventsResponseTypeDef,
-    RegisterDeviceResponseTypeDef,
     DeleteDatasetResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeIdentityPoolUsageResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     DescribeIdentityUsageResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
@@ -353,42 +354,42 @@
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

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/mypy_boto3_cognito_sync.egg-info/SOURCES.txt` & `mypy-boto3-cognito-sync-1.27.0/mypy_boto3_cognito_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.26.0.post1/setup.py` & `mypy-boto3-cognito-sync-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-cognito-sync.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-sync",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_cognito_sync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CognitoSync 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.CognitoSync 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 cognito-sync type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_cognito_sync": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_cognito_sync": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/",
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


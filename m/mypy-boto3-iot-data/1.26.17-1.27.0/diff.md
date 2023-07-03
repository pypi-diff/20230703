# Comparing `tmp/mypy-boto3-iot-data-1.26.17.tar.gz` & `tmp/mypy-boto3-iot-data-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-data-1.26.17.tar", last modified: Mon Nov 28 04:09:25 2022, max compression
+gzip compressed data, was "mypy-boto3-iot-data-1.27.0.tar", last modified: Mon Jul  3 19:50:53 2023, max compression
```

## Comparing `mypy-boto3-iot-data-1.26.17.tar` & `mypy-boto3-iot-data-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:25.564745 mypy-boto3-iot-data-1.26.17/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    13371 2022-11-28 04:09:25.552745 mypy-boto3-iot-data-1.26.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11926 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:25.552745 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/
--rw-r--r--   0 runner    (1001) docker     (122)      644 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      920 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8451 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     8436 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     7668 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)     7666 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1917 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1914 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     6857 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6846 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:25.552745 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13371 2022-11-28 04:09:25.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      699 2022-11-28 04:09:25.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:09:25.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:09:25.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-28 04:09:25.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2022-11-28 04:09:25.000000 mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 04:09:25.564745 mypy-boto3-iot-data-1.26.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1975 2022-11-28 04:08:42.000000 mypy-boto3-iot-data-1.26.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.991405 mypy-boto3-iot-data-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-07-03 19:50:52.991405 mypy-boto3-iot-data-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.991405 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.991405 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-07-03 19:50:52.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:50:52.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:52.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:52.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:52.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:50:52.000000 mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:52.991405 mypy-boto3-iot-data-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-03 19:39:28.000000 mypy-boto3-iot-data-1.27.0/setup.py
```

### Comparing `mypy-boto3-iot-data-1.26.17/LICENSE` & `mypy-boto3-iot-data-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-iot-data-1.26.17/PKG-INFO` & `mypy-boto3-iot-data-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-data
-Version: 1.26.17
-Summary: Type annotations for boto3.IoTDataPlane 1.26.17 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTDataPlane 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/
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
 
 <a id="mypy-boto3-iot-data"></a>
 
 # mypy-boto3-iot-data
 
 [![PyPI - mypy-boto3-iot-data](https://img.shields.io/pypi/v/mypy-boto3-iot-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-data)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot-data?color=blue)](https://pypistats.org/packages/mypy-boto3-iot-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDataPlane 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
+[boto3.IoTDataPlane 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iot-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,30 +322,30 @@
 
 `mypy_boto3_iot_data.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_data.type_defs import (
     DeleteThingShadowRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteThingShadowResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetRetainedMessageRequestRequestTypeDef,
+    GetRetainedMessageResponseTypeDef,
     GetThingShadowRequestRequestTypeDef,
+    GetThingShadowResponseTypeDef,
     ListNamedShadowsForThingRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListNamedShadowsForThingResponseTypeDef,
+    ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef,
     ListRetainedMessagesRequestRequestTypeDef,
     RetainedMessageSummaryTypeDef,
+    PaginatorConfigTypeDef,
     PublishRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UpdateThingShadowRequestRequestTypeDef,
-    DeleteThingShadowResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetRetainedMessageResponseTypeDef,
-    GetThingShadowResponseTypeDef,
-    ListNamedShadowsForThingResponseTypeDef,
     UpdateThingShadowResponseTypeDef,
-    ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef,
     ListRetainedMessagesResponseTypeDef,
 )
 
 
 def get_structure() -> DeleteThingShadowRequestRequestTypeDef:
     return {...}
 ```
@@ -352,42 +353,42 @@
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

### Comparing `mypy-boto3-iot-data-1.26.17/README.md` & `mypy-boto3-iot-data-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iot-data"></a>
 
 # mypy-boto3-iot-data
 
 [![PyPI - mypy-boto3-iot-data](https://img.shields.io/pypi/v/mypy-boto3-iot-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-data)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot-data?color=blue)](https://pypistats.org/packages/mypy-boto3-iot-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDataPlane 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
+[boto3.IoTDataPlane 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iot-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,30 +290,30 @@
 
 `mypy_boto3_iot_data.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_data.type_defs import (
     DeleteThingShadowRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteThingShadowResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetRetainedMessageRequestRequestTypeDef,
+    GetRetainedMessageResponseTypeDef,
     GetThingShadowRequestRequestTypeDef,
+    GetThingShadowResponseTypeDef,
     ListNamedShadowsForThingRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListNamedShadowsForThingResponseTypeDef,
+    ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef,
     ListRetainedMessagesRequestRequestTypeDef,
     RetainedMessageSummaryTypeDef,
+    PaginatorConfigTypeDef,
     PublishRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UpdateThingShadowRequestRequestTypeDef,
-    DeleteThingShadowResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetRetainedMessageResponseTypeDef,
-    GetThingShadowResponseTypeDef,
-    ListNamedShadowsForThingResponseTypeDef,
     UpdateThingShadowResponseTypeDef,
-    ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef,
     ListRetainedMessagesResponseTypeDef,
 )
 
 
 def get_structure() -> DeleteThingShadowRequestRequestTypeDef:
     return {...}
 ```
@@ -321,42 +321,42 @@
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

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/__init__.py` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/__init__.pyi` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/__main__.py` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTDataPlane 1.26.17\nVersion:         1.26.17\nBuilder"
-        " version: 7.11.11\nDocs:           "
+        "Type annotations for boto3.IoTDataPlane 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.17")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/client.py` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/client.pyi` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/literals.py` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,23 +44,25 @@
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
@@ -71,30 +73,34 @@
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
@@ -120,14 +126,15 @@
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
@@ -172,14 +179,15 @@
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
@@ -190,34 +198,38 @@
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
@@ -230,14 +242,15 @@
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
@@ -250,28 +263,34 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -299,30 +318,34 @@
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
     "scheduler",
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
@@ -338,18 +361,21 @@
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

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/literals.pyi` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -42,23 +42,25 @@
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
@@ -69,30 +71,34 @@
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
@@ -118,14 +124,15 @@
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
@@ -170,14 +177,15 @@
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
@@ -188,34 +196,38 @@
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
@@ -228,14 +240,15 @@
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
@@ -248,28 +261,34 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -297,30 +316,34 @@
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
     "scheduler",
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
@@ -336,18 +359,21 @@
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

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/paginator.py` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListRetainedMessagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Paginator.ListRetainedMessages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/paginators/#listretainedmessagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRetainedMessagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Paginator.ListRetainedMessages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/paginators/#listretainedmessagespaginator)
         """
```

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/paginator.pyi` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListRetainedMessagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Paginator.ListRetainedMessages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/paginators/#listretainedmessagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRetainedMessagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Paginator.ListRetainedMessages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/paginators/#listretainedmessagespaginator)
         """
```

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/type_defs.py` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -19,33 +19,32 @@
 from .literals import PayloadFormatIndicatorType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "DeleteThingShadowRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DeleteThingShadowResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetRetainedMessageRequestRequestTypeDef",
+    "GetRetainedMessageResponseTypeDef",
     "GetThingShadowRequestRequestTypeDef",
+    "GetThingShadowResponseTypeDef",
     "ListNamedShadowsForThingRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListNamedShadowsForThingResponseTypeDef",
+    "ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef",
     "ListRetainedMessagesRequestRequestTypeDef",
     "RetainedMessageSummaryTypeDef",
+    "PaginatorConfigTypeDef",
     "PublishRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateThingShadowRequestRequestTypeDef",
-    "DeleteThingShadowResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetRetainedMessageResponseTypeDef",
-    "GetThingShadowResponseTypeDef",
-    "ListNamedShadowsForThingResponseTypeDef",
     "UpdateThingShadowResponseTypeDef",
-    "ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef",
     "ListRetainedMessagesResponseTypeDef",
 )
 
 _RequiredDeleteThingShadowRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteThingShadowRequestRequestTypeDef",
     {
         "thingName": str,
@@ -55,59 +54,79 @@
     "_OptionalDeleteThingShadowRequestRequestTypeDef",
     {
         "shadowName": str,
     },
     total=False,
 )
 
-
 class DeleteThingShadowRequestRequestTypeDef(
     _RequiredDeleteThingShadowRequestRequestTypeDef, _OptionalDeleteThingShadowRequestRequestTypeDef
 ):
     pass
 
+DeleteThingShadowResponseTypeDef = TypedDict(
+    "DeleteThingShadowResponseTypeDef",
+    {
+        "payload": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRetainedMessageRequestRequestTypeDef = TypedDict(
     "GetRetainedMessageRequestRequestTypeDef",
     {
         "topic": str,
     },
 )
 
+GetRetainedMessageResponseTypeDef = TypedDict(
+    "GetRetainedMessageResponseTypeDef",
+    {
+        "topic": str,
+        "payload": bytes,
+        "qos": int,
+        "lastModifiedTime": int,
+        "userProperties": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetThingShadowRequestRequestTypeDef = TypedDict(
     "_RequiredGetThingShadowRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalGetThingShadowRequestRequestTypeDef = TypedDict(
     "_OptionalGetThingShadowRequestRequestTypeDef",
     {
         "shadowName": str,
     },
     total=False,
 )
 
-
 class GetThingShadowRequestRequestTypeDef(
     _RequiredGetThingShadowRequestRequestTypeDef, _OptionalGetThingShadowRequestRequestTypeDef
 ):
     pass
 
+GetThingShadowResponseTypeDef = TypedDict(
+    "GetThingShadowResponseTypeDef",
+    {
+        "payload": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredListNamedShadowsForThingRequestRequestTypeDef = TypedDict(
     "_RequiredListNamedShadowsForThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
@@ -116,28 +135,34 @@
     {
         "nextToken": str,
         "pageSize": int,
     },
     total=False,
 )
 
-
 class ListNamedShadowsForThingRequestRequestTypeDef(
     _RequiredListNamedShadowsForThingRequestRequestTypeDef,
     _OptionalListNamedShadowsForThingRequestRequestTypeDef,
 ):
     pass
 
+ListNamedShadowsForThingResponseTypeDef = TypedDict(
+    "ListNamedShadowsForThingResponseTypeDef",
+    {
+        "results": List[str],
+        "nextToken": str,
+        "timestamp": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef = TypedDict(
+    "ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListRetainedMessagesRequestRequestTypeDef = TypedDict(
     "ListRetainedMessagesRequestRequestTypeDef",
     {
@@ -154,14 +179,24 @@
         "payloadSize": int,
         "qos": int,
         "lastModifiedTime": int,
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
 _RequiredPublishRequestRequestTypeDef = TypedDict(
     "_RequiredPublishRequestRequestTypeDef",
     {
         "topic": str,
     },
 )
 _OptionalPublishRequestRequestTypeDef = TypedDict(
@@ -176,20 +211,29 @@
         "responseTopic": str,
         "correlationData": str,
         "messageExpiry": int,
     },
     total=False,
 )
 
-
 class PublishRequestRequestTypeDef(
     _RequiredPublishRequestRequestTypeDef, _OptionalPublishRequestRequestTypeDef
 ):
     pass
 
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
 
 _RequiredUpdateThingShadowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThingShadowRequestRequestTypeDef",
     {
         "thingName": str,
         "payload": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -198,82 +242,28 @@
     "_OptionalUpdateThingShadowRequestRequestTypeDef",
     {
         "shadowName": str,
     },
     total=False,
 )
 
-
 class UpdateThingShadowRequestRequestTypeDef(
     _RequiredUpdateThingShadowRequestRequestTypeDef, _OptionalUpdateThingShadowRequestRequestTypeDef
 ):
     pass
 
-
-DeleteThingShadowResponseTypeDef = TypedDict(
-    "DeleteThingShadowResponseTypeDef",
-    {
-        "payload": StreamingBody,
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
-GetRetainedMessageResponseTypeDef = TypedDict(
-    "GetRetainedMessageResponseTypeDef",
-    {
-        "topic": str,
-        "payload": bytes,
-        "qos": int,
-        "lastModifiedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetThingShadowResponseTypeDef = TypedDict(
-    "GetThingShadowResponseTypeDef",
-    {
-        "payload": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListNamedShadowsForThingResponseTypeDef = TypedDict(
-    "ListNamedShadowsForThingResponseTypeDef",
-    {
-        "results": List[str],
-        "nextToken": str,
-        "timestamp": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateThingShadowResponseTypeDef = TypedDict(
     "UpdateThingShadowResponseTypeDef",
     {
         "payload": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef = TypedDict(
-    "ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListRetainedMessagesResponseTypeDef = TypedDict(
     "ListRetainedMessagesResponseTypeDef",
     {
         "retainedTopics": List[RetainedMessageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data/type_defs.pyi` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,32 +19,33 @@
 from .literals import PayloadFormatIndicatorType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "DeleteThingShadowRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DeleteThingShadowResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetRetainedMessageRequestRequestTypeDef",
+    "GetRetainedMessageResponseTypeDef",
     "GetThingShadowRequestRequestTypeDef",
+    "GetThingShadowResponseTypeDef",
     "ListNamedShadowsForThingRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListNamedShadowsForThingResponseTypeDef",
+    "ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef",
     "ListRetainedMessagesRequestRequestTypeDef",
     "RetainedMessageSummaryTypeDef",
+    "PaginatorConfigTypeDef",
     "PublishRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateThingShadowRequestRequestTypeDef",
-    "DeleteThingShadowResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetRetainedMessageResponseTypeDef",
-    "GetThingShadowResponseTypeDef",
-    "ListNamedShadowsForThingResponseTypeDef",
     "UpdateThingShadowResponseTypeDef",
-    "ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef",
     "ListRetainedMessagesResponseTypeDef",
 )
 
 _RequiredDeleteThingShadowRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteThingShadowRequestRequestTypeDef",
     {
         "thingName": str,
@@ -54,56 +55,84 @@
     "_OptionalDeleteThingShadowRequestRequestTypeDef",
     {
         "shadowName": str,
     },
     total=False,
 )
 
+
 class DeleteThingShadowRequestRequestTypeDef(
     _RequiredDeleteThingShadowRequestRequestTypeDef, _OptionalDeleteThingShadowRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+DeleteThingShadowResponseTypeDef = TypedDict(
+    "DeleteThingShadowResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "payload": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRetainedMessageRequestRequestTypeDef = TypedDict(
     "GetRetainedMessageRequestRequestTypeDef",
     {
         "topic": str,
     },
 )
 
+GetRetainedMessageResponseTypeDef = TypedDict(
+    "GetRetainedMessageResponseTypeDef",
+    {
+        "topic": str,
+        "payload": bytes,
+        "qos": int,
+        "lastModifiedTime": int,
+        "userProperties": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetThingShadowRequestRequestTypeDef = TypedDict(
     "_RequiredGetThingShadowRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalGetThingShadowRequestRequestTypeDef = TypedDict(
     "_OptionalGetThingShadowRequestRequestTypeDef",
     {
         "shadowName": str,
     },
     total=False,
 )
 
+
 class GetThingShadowRequestRequestTypeDef(
     _RequiredGetThingShadowRequestRequestTypeDef, _OptionalGetThingShadowRequestRequestTypeDef
 ):
     pass
 
+
+GetThingShadowResponseTypeDef = TypedDict(
+    "GetThingShadowResponseTypeDef",
+    {
+        "payload": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListNamedShadowsForThingRequestRequestTypeDef = TypedDict(
     "_RequiredListNamedShadowsForThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListNamedShadowsForThingRequestRequestTypeDef = TypedDict(
@@ -111,26 +140,36 @@
     {
         "nextToken": str,
         "pageSize": int,
     },
     total=False,
 )
 
+
 class ListNamedShadowsForThingRequestRequestTypeDef(
     _RequiredListNamedShadowsForThingRequestRequestTypeDef,
     _OptionalListNamedShadowsForThingRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+ListNamedShadowsForThingResponseTypeDef = TypedDict(
+    "ListNamedShadowsForThingResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "results": List[str],
+        "nextToken": str,
+        "timestamp": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef = TypedDict(
+    "ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListRetainedMessagesRequestRequestTypeDef = TypedDict(
     "ListRetainedMessagesRequestRequestTypeDef",
     {
@@ -147,14 +186,24 @@
         "payloadSize": int,
         "qos": int,
         "lastModifiedTime": int,
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
 _RequiredPublishRequestRequestTypeDef = TypedDict(
     "_RequiredPublishRequestRequestTypeDef",
     {
         "topic": str,
     },
 )
 _OptionalPublishRequestRequestTypeDef = TypedDict(
@@ -169,19 +218,32 @@
         "responseTopic": str,
         "correlationData": str,
         "messageExpiry": int,
     },
     total=False,
 )
 
+
 class PublishRequestRequestTypeDef(
     _RequiredPublishRequestRequestTypeDef, _OptionalPublishRequestRequestTypeDef
 ):
     pass
 
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
 _RequiredUpdateThingShadowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThingShadowRequestRequestTypeDef",
     {
         "thingName": str,
         "payload": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
@@ -189,80 +251,30 @@
     "_OptionalUpdateThingShadowRequestRequestTypeDef",
     {
         "shadowName": str,
     },
     total=False,
 )
 
+
 class UpdateThingShadowRequestRequestTypeDef(
     _RequiredUpdateThingShadowRequestRequestTypeDef, _OptionalUpdateThingShadowRequestRequestTypeDef
 ):
     pass
 
-DeleteThingShadowResponseTypeDef = TypedDict(
-    "DeleteThingShadowResponseTypeDef",
-    {
-        "payload": StreamingBody,
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
-GetRetainedMessageResponseTypeDef = TypedDict(
-    "GetRetainedMessageResponseTypeDef",
-    {
-        "topic": str,
-        "payload": bytes,
-        "qos": int,
-        "lastModifiedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetThingShadowResponseTypeDef = TypedDict(
-    "GetThingShadowResponseTypeDef",
-    {
-        "payload": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListNamedShadowsForThingResponseTypeDef = TypedDict(
-    "ListNamedShadowsForThingResponseTypeDef",
-    {
-        "results": List[str],
-        "nextToken": str,
-        "timestamp": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 UpdateThingShadowResponseTypeDef = TypedDict(
     "UpdateThingShadowResponseTypeDef",
     {
         "payload": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef = TypedDict(
-    "ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListRetainedMessagesResponseTypeDef = TypedDict(
     "ListRetainedMessagesResponseTypeDef",
     {
         "retainedTopics": List[RetainedMessageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data.egg-info/PKG-INFO` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-data
-Version: 1.26.17
-Summary: Type annotations for boto3.IoTDataPlane 1.26.17 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTDataPlane 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/
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
 
 <a id="mypy-boto3-iot-data"></a>
 
 # mypy-boto3-iot-data
 
 [![PyPI - mypy-boto3-iot-data](https://img.shields.io/pypi/v/mypy-boto3-iot-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-data)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot-data?color=blue)](https://pypistats.org/packages/mypy-boto3-iot-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDataPlane 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
+[boto3.IoTDataPlane 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iot-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,30 +322,30 @@
 
 `mypy_boto3_iot_data.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_data.type_defs import (
     DeleteThingShadowRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteThingShadowResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetRetainedMessageRequestRequestTypeDef,
+    GetRetainedMessageResponseTypeDef,
     GetThingShadowRequestRequestTypeDef,
+    GetThingShadowResponseTypeDef,
     ListNamedShadowsForThingRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListNamedShadowsForThingResponseTypeDef,
+    ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef,
     ListRetainedMessagesRequestRequestTypeDef,
     RetainedMessageSummaryTypeDef,
+    PaginatorConfigTypeDef,
     PublishRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UpdateThingShadowRequestRequestTypeDef,
-    DeleteThingShadowResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetRetainedMessageResponseTypeDef,
-    GetThingShadowResponseTypeDef,
-    ListNamedShadowsForThingResponseTypeDef,
     UpdateThingShadowResponseTypeDef,
-    ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef,
     ListRetainedMessagesResponseTypeDef,
 )
 
 
 def get_structure() -> DeleteThingShadowRequestRequestTypeDef:
     return {...}
 ```
@@ -352,42 +353,42 @@
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

### Comparing `mypy-boto3-iot-data-1.26.17/mypy_boto3_iot_data.egg-info/SOURCES.txt` & `mypy-boto3-iot-data-1.27.0/mypy_boto3_iot_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-data-1.26.17/setup.py` & `mypy-boto3-iot-data-1.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-iot-data.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot-data",
-    version="1.26.17",
+    version="1.27.0",
     packages=["mypy_boto3_iot_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTDataPlane 1.26.17 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.IoTDataPlane 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 iot-data type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_iot_data": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_iot_data": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/",
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


# Comparing `tmp/mypy-boto3-sagemaker-runtime-1.26.93.tar.gz` & `tmp/mypy-boto3-sagemaker-runtime-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-runtime-1.26.93.tar", last modified: Thu Mar 16 19:19:49 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-runtime-1.27.0.tar", last modified: Mon Jul  3 19:51:24 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-runtime-1.26.93.tar` & `mypy-boto3-sagemaker-runtime-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:19:49.219278 mypy-boto3-sagemaker-runtime-1.26.93/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-16 19:19:39.000000 mypy-boto3-sagemaker-runtime-1.26.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-03-16 19:19:49.219278 mypy-boto3-sagemaker-runtime-1.26.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-03-16 19:19:39.000000 mypy-boto3-sagemaker-runtime-1.26.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:19:49.219278 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-16 19:19:39.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-16 19:19:39.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-16 19:19:39.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-03-16 19:19:40.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-03-16 19:19:39.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-03-16 19:19:40.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-03-16 19:19:40.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 19:19:39.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-03-16 19:19:40.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-16 19:19:40.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-16 19:19:39.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:19:49.219278 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-03-16 19:19:49.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-16 19:19:49.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 19:19:49.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 19:19:49.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-16 19:19:49.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-16 19:19:49.000000 mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 19:19:49.219278 mypy-boto3-sagemaker-runtime-1.26.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-16 19:19:39.000000 mypy-boto3-sagemaker-runtime-1.26.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.607948 mypy-boto3-sagemaker-runtime-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-07-03 19:51:24.599948 mypy-boto3-sagemaker-runtime-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.599948 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.599948 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:24.607948 mypy-boto3-sagemaker-runtime-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-03 19:47:28.000000 mypy-boto3-sagemaker-runtime-1.27.0/setup.py
```

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/LICENSE` & `mypy-boto3-sagemaker-runtime-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/PKG-INFO` & `mypy-boto3-sagemaker-runtime-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-runtime
-Version: 1.26.93
-Summary: Type annotations for boto3.SageMakerRuntime 1.26.93 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.SageMakerRuntime 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sagemaker-runtime"></a>
 
 # mypy-boto3-sagemaker-runtime
 
 [![PyPI - mypy-boto3-sagemaker-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerRuntime 1.26.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
+[boto3.SageMakerRuntime 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
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
 [mypy-boto3-sagemaker-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,60 +298,60 @@
 
 `mypy_boto3_sagemaker_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_runtime.type_defs import (
     InvokeEndpointAsyncInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    InvokeEndpointInputRequestTypeDef,
     InvokeEndpointAsyncOutputTypeDef,
+    InvokeEndpointInputRequestTypeDef,
     InvokeEndpointOutputTypeDef,
+    ResponseMetadataTypeDef,
 )
 
 
 def get_structure() -> InvokeEndpointAsyncInputRequestTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/README.md` & `mypy-boto3-sagemaker-runtime-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sagemaker-runtime"></a>
 
 # mypy-boto3-sagemaker-runtime
 
 [![PyPI - mypy-boto3-sagemaker-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerRuntime 1.26.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
+[boto3.SageMakerRuntime 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
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
 [mypy-boto3-sagemaker-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,60 +266,60 @@
 
 `mypy_boto3_sagemaker_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_runtime.type_defs import (
     InvokeEndpointAsyncInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    InvokeEndpointInputRequestTypeDef,
     InvokeEndpointAsyncOutputTypeDef,
+    InvokeEndpointInputRequestTypeDef,
     InvokeEndpointOutputTypeDef,
+    ResponseMetadataTypeDef,
 )
 
 
 def get_structure() -> InvokeEndpointAsyncInputRequestTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/__main__.py` & `mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakerRuntime 1.26.93\nVersion:         1.26.93\nBuilder"
-        " version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.SageMakerRuntime 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.93")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/client.py` & `mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/client.pyi` & `mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/literals.py` & `mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SageMakerRuntimeServiceName", "ServiceName", "ResourceServiceName", "RegionName")
 
-
 SageMakerRuntimeServiceName = Literal["sagemaker-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -34,14 +32,15 @@
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
@@ -81,14 +80,15 @@
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
@@ -186,14 +186,15 @@
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
@@ -229,14 +230,15 @@
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
@@ -255,16 +257,19 @@
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
@@ -348,15 +353,17 @@
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
@@ -381,21 +388,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/literals.pyi` & `mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("SageMakerRuntimeServiceName", "ServiceName", "ResourceServiceName", "RegionName")
 
+
 SageMakerRuntimeServiceName = Literal["sagemaker-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -32,14 +34,15 @@
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
@@ -79,14 +82,15 @@
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
@@ -184,14 +188,15 @@
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
@@ -227,14 +232,15 @@
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
@@ -253,16 +259,19 @@
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
@@ -346,15 +355,17 @@
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
@@ -379,21 +390,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/type_defs.py` & `mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,18 +20,18 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "InvokeEndpointAsyncInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "InvokeEndpointInputRequestTypeDef",
     "InvokeEndpointAsyncOutputTypeDef",
+    "InvokeEndpointInputRequestTypeDef",
     "InvokeEndpointOutputTypeDef",
+    "ResponseMetadataTypeDef",
 )
 
 _RequiredInvokeEndpointAsyncInputRequestTypeDef = TypedDict(
     "_RequiredInvokeEndpointAsyncInputRequestTypeDef",
     {
         "EndpointName": str,
         "InputLocation": str,
@@ -53,22 +53,21 @@
 
 class InvokeEndpointAsyncInputRequestTypeDef(
     _RequiredInvokeEndpointAsyncInputRequestTypeDef, _OptionalInvokeEndpointAsyncInputRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+InvokeEndpointAsyncOutputTypeDef = TypedDict(
+    "InvokeEndpointAsyncOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "InferenceId": str,
+        "OutputLocation": str,
+        "FailureLocation": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredInvokeEndpointInputRequestTypeDef = TypedDict(
     "_RequiredInvokeEndpointInputRequestTypeDef",
     {
         "EndpointName": str,
@@ -93,26 +92,28 @@
 
 class InvokeEndpointInputRequestTypeDef(
     _RequiredInvokeEndpointInputRequestTypeDef, _OptionalInvokeEndpointInputRequestTypeDef
 ):
     pass
 
 
-InvokeEndpointAsyncOutputTypeDef = TypedDict(
-    "InvokeEndpointAsyncOutputTypeDef",
-    {
-        "InferenceId": str,
-        "OutputLocation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 InvokeEndpointOutputTypeDef = TypedDict(
     "InvokeEndpointOutputTypeDef",
     {
         "Body": StreamingBody,
         "ContentType": str,
         "InvokedProductionVariant": str,
         "CustomAttributes": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
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
     },
 )
```

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime/type_defs.pyi` & `mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "InvokeEndpointAsyncInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "InvokeEndpointInputRequestTypeDef",
     "InvokeEndpointAsyncOutputTypeDef",
+    "InvokeEndpointInputRequestTypeDef",
     "InvokeEndpointOutputTypeDef",
+    "ResponseMetadataTypeDef",
 )
 
 _RequiredInvokeEndpointAsyncInputRequestTypeDef = TypedDict(
     "_RequiredInvokeEndpointAsyncInputRequestTypeDef",
     {
         "EndpointName": str,
         "InputLocation": str,
@@ -50,22 +50,21 @@
 )
 
 class InvokeEndpointAsyncInputRequestTypeDef(
     _RequiredInvokeEndpointAsyncInputRequestTypeDef, _OptionalInvokeEndpointAsyncInputRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+InvokeEndpointAsyncOutputTypeDef = TypedDict(
+    "InvokeEndpointAsyncOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "InferenceId": str,
+        "OutputLocation": str,
+        "FailureLocation": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredInvokeEndpointInputRequestTypeDef = TypedDict(
     "_RequiredInvokeEndpointInputRequestTypeDef",
     {
         "EndpointName": str,
@@ -88,26 +87,28 @@
 )
 
 class InvokeEndpointInputRequestTypeDef(
     _RequiredInvokeEndpointInputRequestTypeDef, _OptionalInvokeEndpointInputRequestTypeDef
 ):
     pass
 
-InvokeEndpointAsyncOutputTypeDef = TypedDict(
-    "InvokeEndpointAsyncOutputTypeDef",
-    {
-        "InferenceId": str,
-        "OutputLocation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 InvokeEndpointOutputTypeDef = TypedDict(
     "InvokeEndpointOutputTypeDef",
     {
         "Body": StreamingBody,
         "ContentType": str,
         "InvokedProductionVariant": str,
         "CustomAttributes": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
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
     },
 )
```

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-runtime
-Version: 1.26.93
-Summary: Type annotations for boto3.SageMakerRuntime 1.26.93 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.SageMakerRuntime 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sagemaker-runtime"></a>
 
 # mypy-boto3-sagemaker-runtime
 
 [![PyPI - mypy-boto3-sagemaker-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerRuntime 1.26.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
+[boto3.SageMakerRuntime 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
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
 [mypy-boto3-sagemaker-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,60 +298,60 @@
 
 `mypy_boto3_sagemaker_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_runtime.type_defs import (
     InvokeEndpointAsyncInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    InvokeEndpointInputRequestTypeDef,
     InvokeEndpointAsyncOutputTypeDef,
+    InvokeEndpointInputRequestTypeDef,
     InvokeEndpointOutputTypeDef,
+    ResponseMetadataTypeDef,
 )
 
 
 def get_structure() -> InvokeEndpointAsyncInputRequestTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/mypy_boto3_sagemaker_runtime.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-runtime-1.27.0/mypy_boto3_sagemaker_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-runtime-1.26.93/setup.py` & `mypy-boto3-sagemaker-runtime-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-sagemaker-runtime.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-runtime",
-    version="1.26.93",
+    version="1.27.0",
     packages=["mypy_boto3_sagemaker_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakerRuntime 1.26.93 service generated with"
-        " mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.SageMakerRuntime 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/",
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


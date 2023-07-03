# Comparing `tmp/mypy-boto3-sso-oidc-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-sso-oidc-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sso-oidc-1.26.0.post1.tar", last modified: Tue Nov  1 21:44:03 2022, max compression
+gzip compressed data, was "mypy-boto3-sso-oidc-1.27.0.tar", last modified: Mon Jul  3 19:51:31 2023, max compression
```

## Comparing `mypy-boto3-sso-oidc-1.26.0.post1.tar` & `mypy-boto3-sso-oidc-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:03.396852 mypy-boto3-sso-oidc-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12092 2022-11-01 21:44:03.396852 mypy-boto3-sso-oidc-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10648 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:03.396852 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5468 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5459 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7196 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7194 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3307 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:03.396852 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12092 2022-11-01 21:44:03.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-01 21:44:03.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:03.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:03.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:44:03.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-01 21:44:03.000000 mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:44:03.396852 mypy-boto3-sso-oidc-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-11-01 21:41:53.000000 mypy-boto3-sso-oidc-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:31.192060 mypy-boto3-sso-oidc-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-07-03 19:51:31.188060 mypy-boto3-sso-oidc-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:31.184060 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:31.188060 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-07-03 19:51:31.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-03 19:51:31.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:31.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:31.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:31.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:31.000000 mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:31.192060 mypy-boto3-sso-oidc-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-03 19:48:46.000000 mypy-boto3-sso-oidc-1.27.0/setup.py
```

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/LICENSE` & `mypy-boto3-sso-oidc-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/PKG-INFO` & `mypy-boto3-sso-oidc-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-oidc
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SSOOIDC 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SSOOIDC 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/
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
 
 <a id="mypy-boto3-sso-oidc"></a>
 
 # mypy-boto3-sso-oidc
 
 [![PyPI - mypy-boto3-sso-oidc](https://img.shields.io/pypi/v/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso-oidc?color=blue)](https://pypistats.org/packages/mypy-boto3-sso-oidc)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOOIDC 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
+[boto3.SSOOIDC 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
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
 [mypy-boto3-sso-oidc docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,19 +296,19 @@
 
 `mypy_boto3_sso_oidc.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso_oidc.type_defs import (
     CreateTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RegisterClientRequestRequestTypeDef,
-    StartDeviceAuthorizationRequestRequestTypeDef,
     CreateTokenResponseTypeDef,
+    RegisterClientRequestRequestTypeDef,
     RegisterClientResponseTypeDef,
+    ResponseMetadataTypeDef,
+    StartDeviceAuthorizationRequestRequestTypeDef,
     StartDeviceAuthorizationResponseTypeDef,
 )
 
 
 def get_structure() -> CreateTokenRequestRequestTypeDef:
     return {...}
 ```
@@ -315,42 +316,42 @@
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

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/README.md` & `mypy-boto3-sso-oidc-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sso-oidc"></a>
 
 # mypy-boto3-sso-oidc
 
 [![PyPI - mypy-boto3-sso-oidc](https://img.shields.io/pypi/v/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso-oidc?color=blue)](https://pypistats.org/packages/mypy-boto3-sso-oidc)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOOIDC 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
+[boto3.SSOOIDC 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
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
 [mypy-boto3-sso-oidc docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,19 +264,19 @@
 
 `mypy_boto3_sso_oidc.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso_oidc.type_defs import (
     CreateTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RegisterClientRequestRequestTypeDef,
-    StartDeviceAuthorizationRequestRequestTypeDef,
     CreateTokenResponseTypeDef,
+    RegisterClientRequestRequestTypeDef,
     RegisterClientResponseTypeDef,
+    ResponseMetadataTypeDef,
+    StartDeviceAuthorizationRequestRequestTypeDef,
     StartDeviceAuthorizationResponseTypeDef,
 )
 
 
 def get_structure() -> CreateTokenRequestRequestTypeDef:
     return {...}
 ```
@@ -284,42 +284,42 @@
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

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/__main__.py` & `mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSOOIDC 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.SSOOIDC 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC\nOther"
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

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/client.py` & `mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/client.pyi` & `mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/literals.py` & `mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SSOOIDCServiceName", "ServiceName", "ResourceServiceName", "RegionName")
 
-
 SSOOIDCServiceName = Literal["sso-oidc"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -34,23 +32,25 @@
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
@@ -60,30 +60,35 @@
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
@@ -109,14 +114,15 @@
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
@@ -161,51 +167,57 @@
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
@@ -218,14 +230,15 @@
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
@@ -237,28 +250,35 @@
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
@@ -267,14 +287,15 @@
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
@@ -285,55 +306,64 @@
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
@@ -352,27 +382,30 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/literals.pyi` & `mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("SSOOIDCServiceName", "ServiceName", "ResourceServiceName", "RegionName")
 
+
 SSOOIDCServiceName = Literal["sso-oidc"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -32,23 +34,25 @@
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
@@ -58,30 +62,35 @@
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
@@ -107,14 +116,15 @@
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
@@ -159,51 +169,57 @@
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
@@ -216,14 +232,15 @@
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
@@ -235,28 +252,35 @@
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
@@ -265,14 +289,15 @@
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
@@ -283,55 +308,64 @@
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
@@ -350,27 +384,30 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/type_defs.py` & `mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CreateTokenRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "RegisterClientRequestRequestTypeDef",
-    "StartDeviceAuthorizationRequestRequestTypeDef",
     "CreateTokenResponseTypeDef",
+    "RegisterClientRequestRequestTypeDef",
     "RegisterClientResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartDeviceAuthorizationRequestRequestTypeDef",
     "StartDeviceAuthorizationResponseTypeDef",
 )
 
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "clientId": str,
@@ -53,22 +53,23 @@
 
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateTokenResponseTypeDef = TypedDict(
+    "CreateTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "accessToken": str,
+        "tokenType": str,
+        "expiresIn": int,
+        "refreshToken": str,
+        "idToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterClientRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterClientRequestRequestTypeDef",
     {
         "clientName": str,
@@ -86,53 +87,52 @@
 
 class RegisterClientRequestRequestTypeDef(
     _RequiredRegisterClientRequestRequestTypeDef, _OptionalRegisterClientRequestRequestTypeDef
 ):
     pass
 
 
-StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
-    "StartDeviceAuthorizationRequestRequestTypeDef",
+RegisterClientResponseTypeDef = TypedDict(
+    "RegisterClientResponseTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
-        "startUrl": str,
+        "clientIdIssuedAt": int,
+        "clientSecretExpiresAt": int,
+        "authorizationEndpoint": str,
+        "tokenEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateTokenResponseTypeDef = TypedDict(
-    "CreateTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "accessToken": str,
-        "tokenType": str,
-        "expiresIn": int,
-        "refreshToken": str,
-        "idToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-RegisterClientResponseTypeDef = TypedDict(
-    "RegisterClientResponseTypeDef",
+StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
+    "StartDeviceAuthorizationRequestRequestTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
-        "clientIdIssuedAt": int,
-        "clientSecretExpiresAt": int,
-        "authorizationEndpoint": str,
-        "tokenEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "startUrl": str,
     },
 )
 
 StartDeviceAuthorizationResponseTypeDef = TypedDict(
     "StartDeviceAuthorizationResponseTypeDef",
     {
         "deviceCode": str,
         "userCode": str,
         "verificationUri": str,
         "verificationUriComplete": str,
         "expiresIn": int,
         "interval": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc/type_defs.pyi` & `mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CreateTokenRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "RegisterClientRequestRequestTypeDef",
-    "StartDeviceAuthorizationRequestRequestTypeDef",
     "CreateTokenResponseTypeDef",
+    "RegisterClientRequestRequestTypeDef",
     "RegisterClientResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartDeviceAuthorizationRequestRequestTypeDef",
     "StartDeviceAuthorizationResponseTypeDef",
 )
 
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "clientId": str,
@@ -50,22 +50,23 @@
 )
 
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateTokenResponseTypeDef = TypedDict(
+    "CreateTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "accessToken": str,
+        "tokenType": str,
+        "expiresIn": int,
+        "refreshToken": str,
+        "idToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterClientRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterClientRequestRequestTypeDef",
     {
         "clientName": str,
@@ -81,53 +82,52 @@
 )
 
 class RegisterClientRequestRequestTypeDef(
     _RequiredRegisterClientRequestRequestTypeDef, _OptionalRegisterClientRequestRequestTypeDef
 ):
     pass
 
-StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
-    "StartDeviceAuthorizationRequestRequestTypeDef",
+RegisterClientResponseTypeDef = TypedDict(
+    "RegisterClientResponseTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
-        "startUrl": str,
+        "clientIdIssuedAt": int,
+        "clientSecretExpiresAt": int,
+        "authorizationEndpoint": str,
+        "tokenEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateTokenResponseTypeDef = TypedDict(
-    "CreateTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "accessToken": str,
-        "tokenType": str,
-        "expiresIn": int,
-        "refreshToken": str,
-        "idToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-RegisterClientResponseTypeDef = TypedDict(
-    "RegisterClientResponseTypeDef",
+StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
+    "StartDeviceAuthorizationRequestRequestTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
-        "clientIdIssuedAt": int,
-        "clientSecretExpiresAt": int,
-        "authorizationEndpoint": str,
-        "tokenEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "startUrl": str,
     },
 )
 
 StartDeviceAuthorizationResponseTypeDef = TypedDict(
     "StartDeviceAuthorizationResponseTypeDef",
     {
         "deviceCode": str,
         "userCode": str,
         "verificationUri": str,
         "verificationUriComplete": str,
         "expiresIn": int,
         "interval": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc.egg-info/PKG-INFO` & `mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-oidc
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SSOOIDC 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SSOOIDC 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/
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
 
 <a id="mypy-boto3-sso-oidc"></a>
 
 # mypy-boto3-sso-oidc
 
 [![PyPI - mypy-boto3-sso-oidc](https://img.shields.io/pypi/v/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso-oidc?color=blue)](https://pypistats.org/packages/mypy-boto3-sso-oidc)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOOIDC 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
+[boto3.SSOOIDC 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
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
 [mypy-boto3-sso-oidc docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,19 +296,19 @@
 
 `mypy_boto3_sso_oidc.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso_oidc.type_defs import (
     CreateTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RegisterClientRequestRequestTypeDef,
-    StartDeviceAuthorizationRequestRequestTypeDef,
     CreateTokenResponseTypeDef,
+    RegisterClientRequestRequestTypeDef,
     RegisterClientResponseTypeDef,
+    ResponseMetadataTypeDef,
+    StartDeviceAuthorizationRequestRequestTypeDef,
     StartDeviceAuthorizationResponseTypeDef,
 )
 
 
 def get_structure() -> CreateTokenRequestRequestTypeDef:
     return {...}
 ```
@@ -315,42 +316,42 @@
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

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/mypy_boto3_sso_oidc.egg-info/SOURCES.txt` & `mypy-boto3-sso-oidc-1.27.0/mypy_boto3_sso_oidc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-oidc-1.26.0.post1/setup.py` & `mypy-boto3-sso-oidc-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 """
 Setup script for mypy-boto3-sso-oidc.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sso-oidc",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_sso_oidc"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSOOIDC 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.SSOOIDC 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 sso-oidc type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_sso_oidc": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_sso_oidc": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/",
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


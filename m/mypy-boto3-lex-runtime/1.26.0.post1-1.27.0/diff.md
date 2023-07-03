# Comparing `tmp/mypy-boto3-lex-runtime-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-lex-runtime-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lex-runtime-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:38 2022, max compression
+gzip compressed data, was "mypy-boto3-lex-runtime-1.27.0.tar", last modified: Mon Jul  3 19:51:01 2023, max compression
```

## Comparing `mypy-boto3-lex-runtime-1.26.0.post1.tar` & `mypy-boto3-lex-runtime-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:38.932832 mypy-boto3-lex-runtime-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12832 2022-11-01 21:43:38.932832 mypy-boto3-lex-runtime-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11369 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:38.932832 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7229 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7218 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7729 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7727 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     9663 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9650 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:38.932832 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12832 2022-11-01 21:43:38.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-11-01 21:43:38.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:38.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:38.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:38.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-01 21:43:38.000000 mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:38.932832 mypy-boto3-lex-runtime-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-11-01 21:37:00.000000 mypy-boto3-lex-runtime-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.467557 mypy-boto3-lex-runtime-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:43.000000 mypy-boto3-lex-runtime-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-07-03 19:51:01.467557 mypy-boto3-lex-runtime-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-03 19:40:43.000000 mypy-boto3-lex-runtime-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.459557 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-03 19:40:43.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-03 19:40:43.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:40:43.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-03 19:40:43.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-03 19:40:43.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-07-03 19:40:43.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-03 19:40:43.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:43.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-03 19:40:44.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-03 19:40:44.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:43.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.467557 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-07-03 19:51:01.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-03 19:51:01.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:01.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 19:51:01.000000 mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:01.467557 mypy-boto3-lex-runtime-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-03 19:40:43.000000 mypy-boto3-lex-runtime-1.27.0/setup.py
```

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/LICENSE` & `mypy-boto3-lex-runtime-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/PKG-INFO` & `mypy-boto3-lex-runtime-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-runtime
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.LexRuntimeService 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.LexRuntimeService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/
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
 
 <a id="mypy-boto3-lex-runtime"></a>
 
 # mypy-boto3-lex-runtime
 
 [![PyPI - mypy-boto3-lex-runtime](https://img.shields.io/pypi/v/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lex-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[boto3.LexRuntimeService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [mypy-boto3-lex-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,26 +305,26 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lex_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteSessionResponseTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentSummaryTypeDef,
     IntentConfidenceTypeDef,
     PostContentRequestRequestTypeDef,
+    PostContentResponseTypeDef,
     SentimentResponseTypeDef,
+    PutSessionResponseTypeDef,
+    ResponseMetadataTypeDef,
     ActiveContextTypeDef,
     GenericAttachmentTypeDef,
-    DeleteSessionResponseTypeDef,
-    PostContentResponseTypeDef,
-    PutSessionResponseTypeDef,
     PredictedIntentTypeDef,
     GetSessionResponseTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
     ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
@@ -336,42 +337,42 @@
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

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/README.md` & `mypy-boto3-lex-runtime-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lex-runtime"></a>
 
 # mypy-boto3-lex-runtime
 
 [![PyPI - mypy-boto3-lex-runtime](https://img.shields.io/pypi/v/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lex-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[boto3.LexRuntimeService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [mypy-boto3-lex-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -273,26 +273,26 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lex_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteSessionResponseTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentSummaryTypeDef,
     IntentConfidenceTypeDef,
     PostContentRequestRequestTypeDef,
+    PostContentResponseTypeDef,
     SentimentResponseTypeDef,
+    PutSessionResponseTypeDef,
+    ResponseMetadataTypeDef,
     ActiveContextTypeDef,
     GenericAttachmentTypeDef,
-    DeleteSessionResponseTypeDef,
-    PostContentResponseTypeDef,
-    PutSessionResponseTypeDef,
     PredictedIntentTypeDef,
     GetSessionResponseTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
     ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
@@ -305,42 +305,42 @@
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

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/__main__.py` & `mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexRuntimeService 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.LexRuntimeService 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService\nOther"
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

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/client.py` & `mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/client.pyi` & `mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/literals.py` & `mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ConfirmationStatusType",
     "ContentTypeType",
     "DialogActionTypeType",
     "DialogStateType",
     "FulfillmentStateType",
     "MessageFormatTypeType",
     "LexRuntimeServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ConfirmationStatusType = Literal["Confirmed", "Denied", "None"]
 ContentTypeType = Literal["application/vnd.amazonaws.card.generic"]
 DialogActionTypeType = Literal["Close", "ConfirmIntent", "Delegate", "ElicitIntent", "ElicitSlot"]
 DialogStateType = Literal[
     "ConfirmIntent", "ElicitIntent", "ElicitSlot", "Failed", "Fulfilled", "ReadyForFulfillment"
 ]
 FulfillmentStateType = Literal["Failed", "Fulfilled", "ReadyForFulfillment"]
@@ -53,23 +51,25 @@
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
@@ -79,30 +79,35 @@
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
@@ -128,14 +133,15 @@
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
@@ -180,51 +186,57 @@
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
@@ -237,14 +249,15 @@
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
@@ -256,28 +269,35 @@
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
@@ -286,14 +306,15 @@
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
@@ -304,55 +325,64 @@
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

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/literals.pyi` & `mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ConfirmationStatusType",
     "ContentTypeType",
     "DialogActionTypeType",
     "DialogStateType",
     "FulfillmentStateType",
     "MessageFormatTypeType",
     "LexRuntimeServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 ConfirmationStatusType = Literal["Confirmed", "Denied", "None"]
 ContentTypeType = Literal["application/vnd.amazonaws.card.generic"]
 DialogActionTypeType = Literal["Close", "ConfirmIntent", "Delegate", "ElicitIntent", "ElicitSlot"]
 DialogStateType = Literal[
     "ConfirmIntent", "ElicitIntent", "ElicitSlot", "Failed", "Fulfilled", "ReadyForFulfillment"
 ]
 FulfillmentStateType = Literal["Failed", "Fulfilled", "ReadyForFulfillment"]
@@ -51,23 +53,25 @@
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
@@ -77,30 +81,35 @@
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
@@ -126,14 +135,15 @@
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
@@ -178,51 +188,57 @@
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
@@ -235,14 +251,15 @@
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
@@ -254,28 +271,35 @@
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
@@ -284,14 +308,15 @@
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
@@ -302,55 +327,64 @@
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

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/type_defs.py` & `mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,31 +29,30 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DeleteSessionResponseTypeDef",
     "DialogActionTypeDef",
     "GetSessionRequestRequestTypeDef",
     "IntentSummaryTypeDef",
     "IntentConfidenceTypeDef",
     "PostContentRequestRequestTypeDef",
+    "PostContentResponseTypeDef",
     "SentimentResponseTypeDef",
+    "PutSessionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ActiveContextTypeDef",
     "GenericAttachmentTypeDef",
-    "DeleteSessionResponseTypeDef",
-    "PostContentResponseTypeDef",
-    "PutSessionResponseTypeDef",
     "PredictedIntentTypeDef",
     "GetSessionResponseTypeDef",
     "PostTextRequestRequestTypeDef",
     "PutSessionRequestRequestTypeDef",
     "ResponseCardTypeDef",
     "PostTextResponseTypeDef",
 )
@@ -80,22 +79,22 @@
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DeleteSessionResponseTypeDef = TypedDict(
+    "DeleteSessionResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "botName": str,
+        "botAlias": str,
+        "userId": str,
+        "sessionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
@@ -110,19 +109,17 @@
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
 
-
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
-
 _RequiredGetSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
@@ -131,21 +128,19 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "checkpointLabelFilter": str,
     },
     total=False,
 )
 
-
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredIntentSummaryTypeDef = TypedDict(
     "_RequiredIntentSummaryTypeDef",
     {
         "dialogActionType": DialogActionTypeType,
     },
 )
 _OptionalIntentSummaryTypeDef = TypedDict(
@@ -157,19 +152,17 @@
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
-
 class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
     pass
 
-
 IntentConfidenceTypeDef = TypedDict(
     "IntentConfidenceTypeDef",
     {
         "score": float,
     },
     total=False,
 )
@@ -191,62 +184,19 @@
         "requestAttributes": str,
         "accept": str,
         "activeContexts": str,
     },
     total=False,
 )
 
-
 class PostContentRequestRequestTypeDef(
     _RequiredPostContentRequestRequestTypeDef, _OptionalPostContentRequestRequestTypeDef
 ):
     pass
 
-
-SentimentResponseTypeDef = TypedDict(
-    "SentimentResponseTypeDef",
-    {
-        "sentimentLabel": str,
-        "sentimentScore": str,
-    },
-    total=False,
-)
-
-ActiveContextTypeDef = TypedDict(
-    "ActiveContextTypeDef",
-    {
-        "name": str,
-        "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "parameters": Dict[str, str],
-    },
-)
-
-GenericAttachmentTypeDef = TypedDict(
-    "GenericAttachmentTypeDef",
-    {
-        "title": str,
-        "subTitle": str,
-        "attachmentLinkUrl": str,
-        "imageUrl": str,
-        "buttons": List[ButtonTypeDef],
-    },
-    total=False,
-)
-
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
-    {
-        "botName": str,
-        "botAlias": str,
-        "userId": str,
-        "sessionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PostContentResponseTypeDef = TypedDict(
     "PostContentResponseTypeDef",
     {
         "contentType": str,
         "intentName": str,
         "nluIntentConfidence": str,
         "alternativeIntents": str,
@@ -260,18 +210,27 @@
         "slotToElicit": str,
         "inputTranscript": str,
         "encodedInputTranscript": str,
         "audioStream": StreamingBody,
         "botVersion": str,
         "sessionId": str,
         "activeContexts": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SentimentResponseTypeDef = TypedDict(
+    "SentimentResponseTypeDef",
+    {
+        "sentimentLabel": str,
+        "sentimentScore": str,
+    },
+    total=False,
+)
+
 PutSessionResponseTypeDef = TypedDict(
     "PutSessionResponseTypeDef",
     {
         "contentType": str,
         "intentName": str,
         "slots": str,
         "sessionAttributes": str,
@@ -279,18 +238,50 @@
         "encodedMessage": str,
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "audioStream": StreamingBody,
         "sessionId": str,
         "activeContexts": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
+ActiveContextTypeDef = TypedDict(
+    "ActiveContextTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "parameters": Dict[str, str],
+    },
+)
+
+GenericAttachmentTypeDef = TypedDict(
+    "GenericAttachmentTypeDef",
+    {
+        "title": str,
+        "subTitle": str,
+        "attachmentLinkUrl": str,
+        "imageUrl": str,
+        "buttons": List[ButtonTypeDef],
+    },
+    total=False,
+)
+
 PredictedIntentTypeDef = TypedDict(
     "PredictedIntentTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "slots": Dict[str, str],
     },
@@ -301,15 +292,15 @@
     "GetSessionResponseTypeDef",
     {
         "recentIntentSummaryView": List[IntentSummaryTypeDef],
         "sessionAttributes": Dict[str, str],
         "sessionId": str,
         "dialogAction": DialogActionTypeDef,
         "activeContexts": List[ActiveContextTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPostTextRequestRequestTypeDef = TypedDict(
     "_RequiredPostTextRequestRequestTypeDef",
     {
         "botName": str,
@@ -324,21 +315,19 @@
         "sessionAttributes": Mapping[str, str],
         "requestAttributes": Mapping[str, str],
         "activeContexts": Sequence[ActiveContextTypeDef],
     },
     total=False,
 )
 
-
 class PostTextRequestRequestTypeDef(
     _RequiredPostTextRequestRequestTypeDef, _OptionalPostTextRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
@@ -351,21 +340,19 @@
         "recentIntentSummaryView": Sequence[IntentSummaryTypeDef],
         "accept": str,
         "activeContexts": Sequence[ActiveContextTypeDef],
     },
     total=False,
 )
 
-
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
 
-
 ResponseCardTypeDef = TypedDict(
     "ResponseCardTypeDef",
     {
         "version": str,
         "contentType": Literal["application/vnd.amazonaws.card.generic"],
         "genericAttachments": List[GenericAttachmentTypeDef],
     },
@@ -385,10 +372,10 @@
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "responseCard": ResponseCardTypeDef,
         "sessionId": str,
         "botVersion": str,
         "activeContexts": List[ActiveContextTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime/type_defs.pyi` & `mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,30 +29,31 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DeleteSessionResponseTypeDef",
     "DialogActionTypeDef",
     "GetSessionRequestRequestTypeDef",
     "IntentSummaryTypeDef",
     "IntentConfidenceTypeDef",
     "PostContentRequestRequestTypeDef",
+    "PostContentResponseTypeDef",
     "SentimentResponseTypeDef",
+    "PutSessionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ActiveContextTypeDef",
     "GenericAttachmentTypeDef",
-    "DeleteSessionResponseTypeDef",
-    "PostContentResponseTypeDef",
-    "PutSessionResponseTypeDef",
     "PredictedIntentTypeDef",
     "GetSessionResponseTypeDef",
     "PostTextRequestRequestTypeDef",
     "PutSessionRequestRequestTypeDef",
     "ResponseCardTypeDef",
     "PostTextResponseTypeDef",
 )
@@ -79,22 +80,22 @@
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DeleteSessionResponseTypeDef = TypedDict(
+    "DeleteSessionResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "botName": str,
+        "botAlias": str,
+        "userId": str,
+        "sessionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
@@ -109,17 +110,19 @@
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
 
+
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
+
 _RequiredGetSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
@@ -128,19 +131,21 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "checkpointLabelFilter": str,
     },
     total=False,
 )
 
+
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredIntentSummaryTypeDef = TypedDict(
     "_RequiredIntentSummaryTypeDef",
     {
         "dialogActionType": DialogActionTypeType,
     },
 )
 _OptionalIntentSummaryTypeDef = TypedDict(
@@ -152,17 +157,19 @@
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
+
 class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
     pass
 
+
 IntentConfidenceTypeDef = TypedDict(
     "IntentConfidenceTypeDef",
     {
         "score": float,
     },
     total=False,
 )
@@ -184,59 +191,20 @@
         "requestAttributes": str,
         "accept": str,
         "activeContexts": str,
     },
     total=False,
 )
 
+
 class PostContentRequestRequestTypeDef(
     _RequiredPostContentRequestRequestTypeDef, _OptionalPostContentRequestRequestTypeDef
 ):
     pass
 
-SentimentResponseTypeDef = TypedDict(
-    "SentimentResponseTypeDef",
-    {
-        "sentimentLabel": str,
-        "sentimentScore": str,
-    },
-    total=False,
-)
-
-ActiveContextTypeDef = TypedDict(
-    "ActiveContextTypeDef",
-    {
-        "name": str,
-        "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "parameters": Dict[str, str],
-    },
-)
-
-GenericAttachmentTypeDef = TypedDict(
-    "GenericAttachmentTypeDef",
-    {
-        "title": str,
-        "subTitle": str,
-        "attachmentLinkUrl": str,
-        "imageUrl": str,
-        "buttons": List[ButtonTypeDef],
-    },
-    total=False,
-)
-
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
-    {
-        "botName": str,
-        "botAlias": str,
-        "userId": str,
-        "sessionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 PostContentResponseTypeDef = TypedDict(
     "PostContentResponseTypeDef",
     {
         "contentType": str,
         "intentName": str,
         "nluIntentConfidence": str,
@@ -251,16 +219,25 @@
         "slotToElicit": str,
         "inputTranscript": str,
         "encodedInputTranscript": str,
         "audioStream": StreamingBody,
         "botVersion": str,
         "sessionId": str,
         "activeContexts": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SentimentResponseTypeDef = TypedDict(
+    "SentimentResponseTypeDef",
+    {
+        "sentimentLabel": str,
+        "sentimentScore": str,
     },
+    total=False,
 )
 
 PutSessionResponseTypeDef = TypedDict(
     "PutSessionResponseTypeDef",
     {
         "contentType": str,
         "intentName": str,
@@ -270,16 +247,48 @@
         "encodedMessage": str,
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "audioStream": StreamingBody,
         "sessionId": str,
         "activeContexts": str,
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
+    },
+)
+
+ActiveContextTypeDef = TypedDict(
+    "ActiveContextTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "parameters": Dict[str, str],
+    },
+)
+
+GenericAttachmentTypeDef = TypedDict(
+    "GenericAttachmentTypeDef",
+    {
+        "title": str,
+        "subTitle": str,
+        "attachmentLinkUrl": str,
+        "imageUrl": str,
+        "buttons": List[ButtonTypeDef],
     },
+    total=False,
 )
 
 PredictedIntentTypeDef = TypedDict(
     "PredictedIntentTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
@@ -292,15 +301,15 @@
     "GetSessionResponseTypeDef",
     {
         "recentIntentSummaryView": List[IntentSummaryTypeDef],
         "sessionAttributes": Dict[str, str],
         "sessionId": str,
         "dialogAction": DialogActionTypeDef,
         "activeContexts": List[ActiveContextTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPostTextRequestRequestTypeDef = TypedDict(
     "_RequiredPostTextRequestRequestTypeDef",
     {
         "botName": str,
@@ -315,19 +324,21 @@
         "sessionAttributes": Mapping[str, str],
         "requestAttributes": Mapping[str, str],
         "activeContexts": Sequence[ActiveContextTypeDef],
     },
     total=False,
 )
 
+
 class PostTextRequestRequestTypeDef(
     _RequiredPostTextRequestRequestTypeDef, _OptionalPostTextRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
@@ -340,19 +351,21 @@
         "recentIntentSummaryView": Sequence[IntentSummaryTypeDef],
         "accept": str,
         "activeContexts": Sequence[ActiveContextTypeDef],
     },
     total=False,
 )
 
+
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
 
+
 ResponseCardTypeDef = TypedDict(
     "ResponseCardTypeDef",
     {
         "version": str,
         "contentType": Literal["application/vnd.amazonaws.card.generic"],
         "genericAttachments": List[GenericAttachmentTypeDef],
     },
@@ -372,10 +385,10 @@
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "responseCard": ResponseCardTypeDef,
         "sessionId": str,
         "botVersion": str,
         "activeContexts": List[ActiveContextTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime.egg-info/PKG-INFO` & `mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-runtime
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.LexRuntimeService 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.LexRuntimeService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/
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
 
 <a id="mypy-boto3-lex-runtime"></a>
 
 # mypy-boto3-lex-runtime
 
 [![PyPI - mypy-boto3-lex-runtime](https://img.shields.io/pypi/v/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lex-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[boto3.LexRuntimeService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [mypy-boto3-lex-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,26 +305,26 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lex_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteSessionResponseTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentSummaryTypeDef,
     IntentConfidenceTypeDef,
     PostContentRequestRequestTypeDef,
+    PostContentResponseTypeDef,
     SentimentResponseTypeDef,
+    PutSessionResponseTypeDef,
+    ResponseMetadataTypeDef,
     ActiveContextTypeDef,
     GenericAttachmentTypeDef,
-    DeleteSessionResponseTypeDef,
-    PostContentResponseTypeDef,
-    PutSessionResponseTypeDef,
     PredictedIntentTypeDef,
     GetSessionResponseTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
     ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
@@ -336,42 +337,42 @@
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

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/mypy_boto3_lex_runtime.egg-info/SOURCES.txt` & `mypy-boto3-lex-runtime-1.27.0/mypy_boto3_lex_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.26.0.post1/setup.py` & `mypy-boto3-lex-runtime-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-lex-runtime.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lex-runtime",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_lex_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexRuntimeService 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.LexRuntimeService 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
     keywords="boto3 lex-runtime type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_lex_runtime": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_lex_runtime": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/",
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


# Comparing `tmp/mypy-boto3-lexv2-runtime-1.26.68.tar.gz` & `tmp/mypy-boto3-lexv2-runtime-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lexv2-runtime-1.26.68.tar", last modified: Thu Feb  9 20:26:49 2023, max compression
+gzip compressed data, was "mypy-boto3-lexv2-runtime-1.27.0.tar", last modified: Mon Jul  3 19:51:01 2023, max compression
```

## Comparing `mypy-boto3-lexv2-runtime-1.26.68.tar` & `mypy-boto3-lexv2-runtime-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.978837 mypy-boto3-lexv2-runtime-1.26.68/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-runtime-1.26.68/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-02-09 20:26:49.978837 mypy-boto3-lexv2-runtime-1.26.68/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11656 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-runtime-1.26.68/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.978837 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-02-09 20:26:26.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-02-09 20:26:26.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.978837 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-02-09 20:26:49.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-09 20:26:49.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 20:26:49.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 20:26:49.000000 mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 20:26:49.978837 mypy-boto3-lexv2-runtime-1.26.68/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-runtime-1.26.68/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.527558 mypy-boto3-lexv2-runtime-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13148 2023-07-03 19:51:01.527558 mypy-boto3-lexv2-runtime-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.519558 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.527558 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13148 2023-07-03 19:51:01.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-03 19:51:01.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:01.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:51:01.000000 mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:01.527558 mypy-boto3-lexv2-runtime-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-03 19:40:59.000000 mypy-boto3-lexv2-runtime-1.27.0/setup.py
```

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/LICENSE` & `mypy-boto3-lexv2-runtime-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/PKG-INFO` & `mypy-boto3-lexv2-runtime-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-runtime
-Version: 1.26.68
-Summary: Type annotations for boto3.LexRuntimeV2 1.26.68 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.LexRuntimeV2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-lexv2-runtime"></a>
 
 # mypy-boto3-lexv2-runtime
 
 [![PyPI - mypy-boto3-lexv2-runtime](https://img.shields.io/pypi/v/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeV2 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
+[boto3.LexRuntimeV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [mypy-boto3-lexv2-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,30 +307,30 @@
 
 ```python
 from mypy_boto3_lexv2_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteSessionResponseTypeDef,
     DialogActionTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentTypeDef,
+    PutSessionResponseTypeDef,
     RecognizedBotMemberTypeDef,
     RecognizeUtteranceRequestRequestTypeDef,
+    RecognizeUtteranceResponseTypeDef,
+    ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
     RuntimeHintsTypeDef,
     SentimentScoreTypeDef,
     ValueTypeDef,
     ActiveContextTypeDef,
     ImageResponseCardTypeDef,
-    DeleteSessionResponseTypeDef,
-    PutSessionResponseTypeDef,
-    RecognizeUtteranceResponseTypeDef,
     RuntimeHintDetailsTypeDef,
     SentimentResponseTypeDef,
     SlotTypeDef,
     SessionStateTypeDef,
     MessageTypeDef,
     InterpretationTypeDef,
     RecognizeTextRequestRequestTypeDef,
@@ -347,42 +347,42 @@
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

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/README.md` & `mypy-boto3-lexv2-runtime-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lexv2-runtime"></a>
 
 # mypy-boto3-lexv2-runtime
 
 [![PyPI - mypy-boto3-lexv2-runtime](https://img.shields.io/pypi/v/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeV2 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
+[boto3.LexRuntimeV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [mypy-boto3-lexv2-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -275,30 +275,30 @@
 
 ```python
 from mypy_boto3_lexv2_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteSessionResponseTypeDef,
     DialogActionTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentTypeDef,
+    PutSessionResponseTypeDef,
     RecognizedBotMemberTypeDef,
     RecognizeUtteranceRequestRequestTypeDef,
+    RecognizeUtteranceResponseTypeDef,
+    ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
     RuntimeHintsTypeDef,
     SentimentScoreTypeDef,
     ValueTypeDef,
     ActiveContextTypeDef,
     ImageResponseCardTypeDef,
-    DeleteSessionResponseTypeDef,
-    PutSessionResponseTypeDef,
-    RecognizeUtteranceResponseTypeDef,
     RuntimeHintDetailsTypeDef,
     SentimentResponseTypeDef,
     SlotTypeDef,
     SessionStateTypeDef,
     MessageTypeDef,
     InterpretationTypeDef,
     RecognizeTextRequestRequestTypeDef,
@@ -315,42 +315,42 @@
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

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/__main__.py` & `mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexRuntimeV2 1.26.68\nVersion:         1.26.68\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.LexRuntimeV2 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2\nOther"
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

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/client.py` & `mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/client.pyi` & `mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/literals.py` & `mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
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
@@ -104,14 +105,15 @@
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
@@ -190,14 +192,15 @@
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
@@ -208,14 +211,15 @@
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
@@ -251,14 +255,15 @@
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
@@ -277,16 +282,19 @@
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
@@ -366,18 +374,21 @@
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

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/literals.pyi` & `mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
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
@@ -102,14 +103,15 @@
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
@@ -188,14 +190,15 @@
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
@@ -206,14 +209,15 @@
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
@@ -249,14 +253,15 @@
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
@@ -275,16 +280,19 @@
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
@@ -364,18 +372,21 @@
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

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/type_defs.py` & `mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,30 +33,30 @@
 
 
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
     "ButtonTypeDef",
     "ConfidenceScoreTypeDef",
     "DeleteSessionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DeleteSessionResponseTypeDef",
     "DialogActionTypeDef",
     "ElicitSubSlotTypeDef",
     "GetSessionRequestRequestTypeDef",
     "IntentTypeDef",
+    "PutSessionResponseTypeDef",
     "RecognizedBotMemberTypeDef",
     "RecognizeUtteranceRequestRequestTypeDef",
+    "RecognizeUtteranceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RuntimeHintValueTypeDef",
     "RuntimeHintsTypeDef",
     "SentimentScoreTypeDef",
     "ValueTypeDef",
     "ActiveContextTypeDef",
     "ImageResponseCardTypeDef",
-    "DeleteSessionResponseTypeDef",
-    "PutSessionResponseTypeDef",
-    "RecognizeUtteranceResponseTypeDef",
     "RuntimeHintDetailsTypeDef",
     "SentimentResponseTypeDef",
     "SlotTypeDef",
     "SessionStateTypeDef",
     "MessageTypeDef",
     "InterpretationTypeDef",
     "RecognizeTextRequestRequestTypeDef",
@@ -95,22 +95,22 @@
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
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
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
@@ -177,14 +177,27 @@
 )
 
 
 class IntentTypeDef(_RequiredIntentTypeDef, _OptionalIntentTypeDef):
     pass
 
 
+PutSessionResponseTypeDef = TypedDict(
+    "PutSessionResponseTypeDef",
+    {
+        "contentType": str,
+        "messages": str,
+        "sessionState": str,
+        "requestAttributes": str,
+        "sessionId": str,
+        "audioStream": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRecognizedBotMemberTypeDef = TypedDict(
     "_RequiredRecognizedBotMemberTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalRecognizedBotMemberTypeDef = TypedDict(
@@ -227,14 +240,42 @@
 class RecognizeUtteranceRequestRequestTypeDef(
     _RequiredRecognizeUtteranceRequestRequestTypeDef,
     _OptionalRecognizeUtteranceRequestRequestTypeDef,
 ):
     pass
 
 
+RecognizeUtteranceResponseTypeDef = TypedDict(
+    "RecognizeUtteranceResponseTypeDef",
+    {
+        "inputMode": str,
+        "contentType": str,
+        "messages": str,
+        "interpretations": str,
+        "sessionState": str,
+        "requestAttributes": str,
+        "sessionId": str,
+        "inputTranscript": str,
+        "audioStream": StreamingBody,
+        "recognizedBotMember": str,
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
 RuntimeHintValueTypeDef = TypedDict(
     "RuntimeHintValueTypeDef",
     {
         "phrase": str,
     },
 )
 
@@ -305,55 +346,14 @@
 
 class ImageResponseCardTypeDef(
     _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
 ):
     pass
 
 
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutSessionResponseTypeDef = TypedDict(
-    "PutSessionResponseTypeDef",
-    {
-        "contentType": str,
-        "messages": str,
-        "sessionState": str,
-        "requestAttributes": str,
-        "sessionId": str,
-        "audioStream": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RecognizeUtteranceResponseTypeDef = TypedDict(
-    "RecognizeUtteranceResponseTypeDef",
-    {
-        "inputMode": str,
-        "contentType": str,
-        "messages": str,
-        "interpretations": str,
-        "sessionState": str,
-        "requestAttributes": str,
-        "sessionId": str,
-        "inputTranscript": str,
-        "audioStream": StreamingBody,
-        "recognizedBotMember": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RuntimeHintDetailsTypeDef = TypedDict(
     "RuntimeHintDetailsTypeDef",
     {
         "runtimeHintValues": List[RuntimeHintValueTypeDef],
         "subSlotHints": Dict[str, Dict[str, Any]],
     },
     total=False,
@@ -478,23 +478,23 @@
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "sessionId": str,
         "messages": List[MessageTypeDef],
         "interpretations": List[InterpretationTypeDef],
         "sessionState": SessionStateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecognizeTextResponseTypeDef = TypedDict(
     "RecognizeTextResponseTypeDef",
     {
         "messages": List[MessageTypeDef],
         "sessionState": SessionStateTypeDef,
         "interpretations": List[InterpretationTypeDef],
         "requestAttributes": Dict[str, str],
         "sessionId": str,
         "recognizedBotMember": RecognizedBotMemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime/type_defs.pyi` & `mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -32,30 +32,30 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
     "ButtonTypeDef",
     "ConfidenceScoreTypeDef",
     "DeleteSessionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DeleteSessionResponseTypeDef",
     "DialogActionTypeDef",
     "ElicitSubSlotTypeDef",
     "GetSessionRequestRequestTypeDef",
     "IntentTypeDef",
+    "PutSessionResponseTypeDef",
     "RecognizedBotMemberTypeDef",
     "RecognizeUtteranceRequestRequestTypeDef",
+    "RecognizeUtteranceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RuntimeHintValueTypeDef",
     "RuntimeHintsTypeDef",
     "SentimentScoreTypeDef",
     "ValueTypeDef",
     "ActiveContextTypeDef",
     "ImageResponseCardTypeDef",
-    "DeleteSessionResponseTypeDef",
-    "PutSessionResponseTypeDef",
-    "RecognizeUtteranceResponseTypeDef",
     "RuntimeHintDetailsTypeDef",
     "SentimentResponseTypeDef",
     "SlotTypeDef",
     "SessionStateTypeDef",
     "MessageTypeDef",
     "InterpretationTypeDef",
     "RecognizeTextRequestRequestTypeDef",
@@ -94,22 +94,22 @@
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
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
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
@@ -170,14 +170,27 @@
     },
     total=False,
 )
 
 class IntentTypeDef(_RequiredIntentTypeDef, _OptionalIntentTypeDef):
     pass
 
+PutSessionResponseTypeDef = TypedDict(
+    "PutSessionResponseTypeDef",
+    {
+        "contentType": str,
+        "messages": str,
+        "sessionState": str,
+        "requestAttributes": str,
+        "sessionId": str,
+        "audioStream": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRecognizedBotMemberTypeDef = TypedDict(
     "_RequiredRecognizedBotMemberTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalRecognizedBotMemberTypeDef = TypedDict(
@@ -216,14 +229,42 @@
 
 class RecognizeUtteranceRequestRequestTypeDef(
     _RequiredRecognizeUtteranceRequestRequestTypeDef,
     _OptionalRecognizeUtteranceRequestRequestTypeDef,
 ):
     pass
 
+RecognizeUtteranceResponseTypeDef = TypedDict(
+    "RecognizeUtteranceResponseTypeDef",
+    {
+        "inputMode": str,
+        "contentType": str,
+        "messages": str,
+        "interpretations": str,
+        "sessionState": str,
+        "requestAttributes": str,
+        "sessionId": str,
+        "inputTranscript": str,
+        "audioStream": StreamingBody,
+        "recognizedBotMember": str,
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
 RuntimeHintValueTypeDef = TypedDict(
     "RuntimeHintValueTypeDef",
     {
         "phrase": str,
     },
 )
 
@@ -290,55 +331,14 @@
 )
 
 class ImageResponseCardTypeDef(
     _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
 ):
     pass
 
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutSessionResponseTypeDef = TypedDict(
-    "PutSessionResponseTypeDef",
-    {
-        "contentType": str,
-        "messages": str,
-        "sessionState": str,
-        "requestAttributes": str,
-        "sessionId": str,
-        "audioStream": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RecognizeUtteranceResponseTypeDef = TypedDict(
-    "RecognizeUtteranceResponseTypeDef",
-    {
-        "inputMode": str,
-        "contentType": str,
-        "messages": str,
-        "interpretations": str,
-        "sessionState": str,
-        "requestAttributes": str,
-        "sessionId": str,
-        "inputTranscript": str,
-        "audioStream": StreamingBody,
-        "recognizedBotMember": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RuntimeHintDetailsTypeDef = TypedDict(
     "RuntimeHintDetailsTypeDef",
     {
         "runtimeHintValues": List[RuntimeHintValueTypeDef],
         "subSlotHints": Dict[str, Dict[str, Any]],
     },
     total=False,
@@ -457,23 +457,23 @@
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "sessionId": str,
         "messages": List[MessageTypeDef],
         "interpretations": List[InterpretationTypeDef],
         "sessionState": SessionStateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecognizeTextResponseTypeDef = TypedDict(
     "RecognizeTextResponseTypeDef",
     {
         "messages": List[MessageTypeDef],
         "sessionState": SessionStateTypeDef,
         "interpretations": List[InterpretationTypeDef],
         "requestAttributes": Dict[str, str],
         "sessionId": str,
         "recognizedBotMember": RecognizedBotMemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO` & `mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-runtime
-Version: 1.26.68
-Summary: Type annotations for boto3.LexRuntimeV2 1.26.68 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.LexRuntimeV2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-lexv2-runtime"></a>
 
 # mypy-boto3-lexv2-runtime
 
 [![PyPI - mypy-boto3-lexv2-runtime](https://img.shields.io/pypi/v/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeV2 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
+[boto3.LexRuntimeV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [mypy-boto3-lexv2-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,30 +307,30 @@
 
 ```python
 from mypy_boto3_lexv2_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteSessionResponseTypeDef,
     DialogActionTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentTypeDef,
+    PutSessionResponseTypeDef,
     RecognizedBotMemberTypeDef,
     RecognizeUtteranceRequestRequestTypeDef,
+    RecognizeUtteranceResponseTypeDef,
+    ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
     RuntimeHintsTypeDef,
     SentimentScoreTypeDef,
     ValueTypeDef,
     ActiveContextTypeDef,
     ImageResponseCardTypeDef,
-    DeleteSessionResponseTypeDef,
-    PutSessionResponseTypeDef,
-    RecognizeUtteranceResponseTypeDef,
     RuntimeHintDetailsTypeDef,
     SentimentResponseTypeDef,
     SlotTypeDef,
     SessionStateTypeDef,
     MessageTypeDef,
     InterpretationTypeDef,
     RecognizeTextRequestRequestTypeDef,
@@ -347,42 +347,42 @@
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

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt` & `mypy-boto3-lexv2-runtime-1.27.0/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.26.68/setup.py` & `mypy-boto3-lexv2-runtime-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-lexv2-runtime.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lexv2-runtime",
-    version="1.26.68",
+    version="1.27.0",
     packages=["mypy_boto3_lexv2_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexRuntimeV2 1.26.68 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.LexRuntimeV2 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/",
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


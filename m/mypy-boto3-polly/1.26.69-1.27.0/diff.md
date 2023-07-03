# Comparing `tmp/mypy-boto3-polly-1.26.69.tar.gz` & `tmp/mypy-boto3-polly-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-polly-1.26.69.tar", last modified: Fri Feb 10 20:27:29 2023, max compression
+gzip compressed data, was "mypy-boto3-polly-1.27.0.tar", last modified: Mon Jul  3 19:51:16 2023, max compression
```

## Comparing `mypy-boto3-polly-1.26.69.tar` & `mypy-boto3-polly-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:27:29.498390 mypy-boto3-polly-1.26.69/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-02-10 20:27:29.490389 mypy-boto3-polly-1.26.69/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:27:29.490389 mypy-boto3-polly-1.26.69/mypy_boto3_polly/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-02-10 20:26:54.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-02-10 20:26:54.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-02-10 20:26:54.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:27:29.490389 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-02-10 20:27:29.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-10 20:27:29.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 20:27:29.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 20:27:29.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-10 20:27:29.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-10 20:27:29.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 20:27:29.498390 mypy-boto3-polly-1.26.69/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:16.603826 mypy-boto3-polly-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13873 2023-07-03 19:51:16.603826 mypy-boto3-polly-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:16.603826 mypy-boto3-polly-1.27.0/mypy_boto3_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10606 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:16.603826 mypy-boto3-polly-1.27.0/mypy_boto3_polly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13873 2023-07-03 19:51:16.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 19:51:16.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:16.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:16.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:16.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 19:51:16.000000 mypy-boto3-polly-1.27.0/mypy_boto3_polly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:16.603826 mypy-boto3-polly-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 19:43:45.000000 mypy-boto3-polly-1.27.0/setup.py
```

### Comparing `mypy-boto3-polly-1.26.69/LICENSE` & `mypy-boto3-polly-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-polly-1.26.69/PKG-INFO` & `mypy-boto3-polly-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-polly
-Version: 1.26.69
-Summary: Type annotations for boto3.Polly 1.26.69 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Polly 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-polly"></a>
 
 # mypy-boto3-polly
 
 [![PyPI - mypy-boto3-polly](https://img.shields.io/pypi/v/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-polly?color=blue)](https://pypistats.org/packages/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.26.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,31 +337,31 @@
 
 `mypy_boto3_polly.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_polly.type_defs import (
     DeleteLexiconInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
     DescribeVoicesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     VoiceTypeDef,
     GetLexiconInputRequestTypeDef,
     LexiconAttributesTypeDef,
     LexiconTypeDef,
     GetSpeechSynthesisTaskInputRequestTypeDef,
     SynthesisTaskTypeDef,
+    ListLexiconsInputListLexiconsPaginateTypeDef,
     ListLexiconsInputRequestTypeDef,
+    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     ListSpeechSynthesisTasksInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutLexiconInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartSpeechSynthesisTaskInputRequestTypeDef,
     SynthesizeSpeechInputRequestTypeDef,
-    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
-    ListLexiconsInputListLexiconsPaginateTypeDef,
-    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     SynthesizeSpeechOutputTypeDef,
     DescribeVoicesOutputTypeDef,
     LexiconDescriptionTypeDef,
     GetLexiconOutputTypeDef,
     GetSpeechSynthesisTaskOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     StartSpeechSynthesisTaskOutputTypeDef,
@@ -376,42 +376,42 @@
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

### Comparing `mypy-boto3-polly-1.26.69/README.md` & `mypy-boto3-polly-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-polly"></a>
 
 # mypy-boto3-polly
 
 [![PyPI - mypy-boto3-polly](https://img.shields.io/pypi/v/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-polly?color=blue)](https://pypistats.org/packages/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.26.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,31 +305,31 @@
 
 `mypy_boto3_polly.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_polly.type_defs import (
     DeleteLexiconInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
     DescribeVoicesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     VoiceTypeDef,
     GetLexiconInputRequestTypeDef,
     LexiconAttributesTypeDef,
     LexiconTypeDef,
     GetSpeechSynthesisTaskInputRequestTypeDef,
     SynthesisTaskTypeDef,
+    ListLexiconsInputListLexiconsPaginateTypeDef,
     ListLexiconsInputRequestTypeDef,
+    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     ListSpeechSynthesisTasksInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutLexiconInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartSpeechSynthesisTaskInputRequestTypeDef,
     SynthesizeSpeechInputRequestTypeDef,
-    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
-    ListLexiconsInputListLexiconsPaginateTypeDef,
-    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     SynthesizeSpeechOutputTypeDef,
     DescribeVoicesOutputTypeDef,
     LexiconDescriptionTypeDef,
     GetLexiconOutputTypeDef,
     GetSpeechSynthesisTaskOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     StartSpeechSynthesisTaskOutputTypeDef,
@@ -344,42 +344,42 @@
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

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly/__init__.py` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly/__init__.pyi` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly/__main__.py` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Polly 1.26.69\nVersion:         1.26.69\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Polly 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.69")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly/client.py` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly/client.pyi` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly/literals.py` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeVoicesPaginatorName",
     "EngineType",
     "GenderType",
     "LanguageCodeType",
     "ListLexiconsPaginatorName",
     "ListSpeechSynthesisTasksPaginatorName",
@@ -34,15 +33,14 @@
     "PollyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeVoicesPaginatorName = Literal["describe_voices"]
 EngineType = Literal["neural", "standard"]
 GenderType = Literal["Female", "Male"]
 LanguageCodeType = Literal[
     "ar-AE",
     "arb",
     "ca-ES",
@@ -50,14 +48,15 @@
     "cy-GB",
     "da-DK",
     "de-AT",
     "de-DE",
     "en-AU",
     "en-GB",
     "en-GB-WLS",
+    "en-IE",
     "en-IN",
     "en-NZ",
     "en-US",
     "en-ZA",
     "es-ES",
     "es-MX",
     "es-US",
@@ -147,28 +146,30 @@
     "Mathieu",
     "Matthew",
     "Maxim",
     "Mia",
     "Miguel",
     "Mizuki",
     "Naja",
+    "Niamh",
     "Nicole",
     "Ola",
     "Olivia",
     "Pedro",
     "Penelope",
     "Raveena",
     "Remi",
     "Ricardo",
     "Ruben",
     "Russell",
     "Ruth",
     "Salli",
     "Seoyeon",
     "Sergio",
+    "Sofie",
     "Stephen",
     "Suvi",
     "Takumi",
     "Tatyana",
     "Thiago",
     "Tomoko",
     "Vicki",
@@ -188,14 +189,15 @@
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
@@ -235,14 +237,15 @@
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
@@ -321,14 +324,15 @@
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
@@ -339,14 +343,15 @@
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
@@ -382,14 +387,15 @@
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
@@ -408,16 +414,19 @@
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
@@ -497,18 +506,21 @@
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
@@ -532,14 +544,15 @@
 ]
 PaginatorName = Literal["describe_voices", "list_lexicons", "list_speech_synthesis_tasks"]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
```

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly/literals.pyi` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DescribeVoicesPaginatorName",
     "EngineType",
     "GenderType",
     "LanguageCodeType",
     "ListLexiconsPaginatorName",
     "ListSpeechSynthesisTasksPaginatorName",
@@ -33,14 +34,15 @@
     "PollyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DescribeVoicesPaginatorName = Literal["describe_voices"]
 EngineType = Literal["neural", "standard"]
 GenderType = Literal["Female", "Male"]
 LanguageCodeType = Literal[
     "ar-AE",
     "arb",
     "ca-ES",
@@ -48,14 +50,15 @@
     "cy-GB",
     "da-DK",
     "de-AT",
     "de-DE",
     "en-AU",
     "en-GB",
     "en-GB-WLS",
+    "en-IE",
     "en-IN",
     "en-NZ",
     "en-US",
     "en-ZA",
     "es-ES",
     "es-MX",
     "es-US",
@@ -145,28 +148,30 @@
     "Mathieu",
     "Matthew",
     "Maxim",
     "Mia",
     "Miguel",
     "Mizuki",
     "Naja",
+    "Niamh",
     "Nicole",
     "Ola",
     "Olivia",
     "Pedro",
     "Penelope",
     "Raveena",
     "Remi",
     "Ricardo",
     "Ruben",
     "Russell",
     "Ruth",
     "Salli",
     "Seoyeon",
     "Sergio",
+    "Sofie",
     "Stephen",
     "Suvi",
     "Takumi",
     "Tatyana",
     "Thiago",
     "Tomoko",
     "Vicki",
@@ -186,14 +191,15 @@
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
@@ -233,14 +239,15 @@
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
@@ -319,14 +326,15 @@
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
@@ -337,14 +345,15 @@
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
@@ -380,14 +389,15 @@
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
@@ -406,16 +416,19 @@
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
@@ -495,18 +508,21 @@
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
@@ -530,14 +546,15 @@
 ]
 PaginatorName = Literal["describe_voices", "list_lexicons", "list_speech_synthesis_tasks"]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
```

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly/paginator.py` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,43 +56,43 @@
 
     def paginate(
         self,
         *,
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         IncludeAdditionalLanguageCodes: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeVoicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.DescribeVoices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#describevoicespaginator)
         """
 
 
 class ListLexiconsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listlexiconspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLexiconsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listlexiconspaginator)
         """
 
 
 class ListSpeechSynthesisTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listspeechsynthesistaskspaginator)
     """
 
     def paginate(
-        self, *, Status: TaskStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Status: TaskStatusType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSpeechSynthesisTasksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listspeechsynthesistaskspaginator)
         """
```

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly/paginator.pyi` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,41 +53,41 @@
 
     def paginate(
         self,
         *,
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         IncludeAdditionalLanguageCodes: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeVoicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.DescribeVoices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#describevoicespaginator)
         """
 
 class ListLexiconsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listlexiconspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLexiconsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listlexiconspaginator)
         """
 
 class ListSpeechSynthesisTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listspeechsynthesistaskspaginator)
     """
 
     def paginate(
-        self, *, Status: TaskStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Status: TaskStatusType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSpeechSynthesisTasksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listspeechsynthesistaskspaginator)
         """
```

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly/type_defs.py` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,34 +29,33 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "DeleteLexiconInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
     "DescribeVoicesInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "VoiceTypeDef",
     "GetLexiconInputRequestTypeDef",
     "LexiconAttributesTypeDef",
     "LexiconTypeDef",
     "GetSpeechSynthesisTaskInputRequestTypeDef",
     "SynthesisTaskTypeDef",
+    "ListLexiconsInputListLexiconsPaginateTypeDef",
     "ListLexiconsInputRequestTypeDef",
+    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
     "ListSpeechSynthesisTasksInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutLexiconInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "StartSpeechSynthesisTaskInputRequestTypeDef",
     "SynthesizeSpeechInputRequestTypeDef",
-    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
-    "ListLexiconsInputListLexiconsPaginateTypeDef",
-    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
     "SynthesizeSpeechOutputTypeDef",
     "DescribeVoicesOutputTypeDef",
     "LexiconDescriptionTypeDef",
     "GetLexiconOutputTypeDef",
     "GetSpeechSynthesisTaskOutputTypeDef",
     "ListSpeechSynthesisTasksOutputTypeDef",
     "StartSpeechSynthesisTaskOutputTypeDef",
@@ -66,20 +65,21 @@
 DeleteLexiconInputRequestTypeDef = TypedDict(
     "DeleteLexiconInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeVoicesInputDescribeVoicesPaginateTypeDef = TypedDict(
+    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Engine": EngineType,
+        "LanguageCode": LanguageCodeType,
+        "IncludeAdditionalLanguageCodes": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeVoicesInputRequestTypeDef = TypedDict(
     "DescribeVoicesInputRequestTypeDef",
     {
@@ -87,25 +87,14 @@
         "LanguageCode": LanguageCodeType,
         "IncludeAdditionalLanguageCodes": bool,
         "NextToken": str,
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
 VoiceTypeDef = TypedDict(
     "VoiceTypeDef",
     {
         "Gender": GenderType,
         "Id": VoiceIdType,
         "LanguageCode": LanguageCodeType,
         "LanguageName": str,
@@ -170,40 +159,78 @@
         "TextType": TextTypeType,
         "VoiceId": VoiceIdType,
         "LanguageCode": LanguageCodeType,
     },
     total=False,
 )
 
+ListLexiconsInputListLexiconsPaginateTypeDef = TypedDict(
+    "ListLexiconsInputListLexiconsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLexiconsInputRequestTypeDef = TypedDict(
     "ListLexiconsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef = TypedDict(
+    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
+    {
+        "Status": TaskStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSpeechSynthesisTasksInputRequestTypeDef = TypedDict(
     "ListSpeechSynthesisTasksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Status": TaskStatusType,
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
 PutLexiconInputRequestTypeDef = TypedDict(
     "PutLexiconInputRequestTypeDef",
     {
         "Name": str,
         "Content": str,
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
 _RequiredStartSpeechSynthesisTaskInputRequestTypeDef = TypedDict(
     "_RequiredStartSpeechSynthesisTaskInputRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
         "OutputS3BucketName": str,
         "Text": str,
         "VoiceId": VoiceIdType,
@@ -220,22 +247,20 @@
         "SnsTopicArn": str,
         "SpeechMarkTypes": Sequence[SpeechMarkTypeType],
         "TextType": TextTypeType,
     },
     total=False,
 )
 
-
 class StartSpeechSynthesisTaskInputRequestTypeDef(
     _RequiredStartSpeechSynthesisTaskInputRequestTypeDef,
     _OptionalStartSpeechSynthesisTaskInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredSynthesizeSpeechInputRequestTypeDef = TypedDict(
     "_RequiredSynthesizeSpeechInputRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
         "Text": str,
         "VoiceId": VoiceIdType,
     },
@@ -249,65 +274,35 @@
         "SampleRate": str,
         "SpeechMarkTypes": Sequence[SpeechMarkTypeType],
         "TextType": TextTypeType,
     },
     total=False,
 )
 
-
 class SynthesizeSpeechInputRequestTypeDef(
     _RequiredSynthesizeSpeechInputRequestTypeDef, _OptionalSynthesizeSpeechInputRequestTypeDef
 ):
     pass
 
-
-DescribeVoicesInputDescribeVoicesPaginateTypeDef = TypedDict(
-    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
-    {
-        "Engine": EngineType,
-        "LanguageCode": LanguageCodeType,
-        "IncludeAdditionalLanguageCodes": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListLexiconsInputListLexiconsPaginateTypeDef = TypedDict(
-    "ListLexiconsInputListLexiconsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef = TypedDict(
-    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
-    {
-        "Status": TaskStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 SynthesizeSpeechOutputTypeDef = TypedDict(
     "SynthesizeSpeechOutputTypeDef",
     {
         "AudioStream": StreamingBody,
         "ContentType": str,
         "RequestCharacters": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVoicesOutputTypeDef = TypedDict(
     "DescribeVoicesOutputTypeDef",
     {
         "Voices": List[VoiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LexiconDescriptionTypeDef = TypedDict(
     "LexiconDescriptionTypeDef",
     {
         "Name": str,
@@ -317,44 +312,44 @@
 )
 
 GetLexiconOutputTypeDef = TypedDict(
     "GetLexiconOutputTypeDef",
     {
         "Lexicon": LexiconTypeDef,
         "LexiconAttributes": LexiconAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "GetSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSpeechSynthesisTasksOutputTypeDef = TypedDict(
     "ListSpeechSynthesisTasksOutputTypeDef",
     {
         "NextToken": str,
         "SynthesisTasks": List[SynthesisTaskTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "StartSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLexiconsOutputTypeDef = TypedDict(
     "ListLexiconsOutputTypeDef",
     {
         "Lexicons": List[LexiconDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly/type_defs.pyi` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,33 +29,34 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "DeleteLexiconInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
     "DescribeVoicesInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "VoiceTypeDef",
     "GetLexiconInputRequestTypeDef",
     "LexiconAttributesTypeDef",
     "LexiconTypeDef",
     "GetSpeechSynthesisTaskInputRequestTypeDef",
     "SynthesisTaskTypeDef",
+    "ListLexiconsInputListLexiconsPaginateTypeDef",
     "ListLexiconsInputRequestTypeDef",
+    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
     "ListSpeechSynthesisTasksInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutLexiconInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "StartSpeechSynthesisTaskInputRequestTypeDef",
     "SynthesizeSpeechInputRequestTypeDef",
-    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
-    "ListLexiconsInputListLexiconsPaginateTypeDef",
-    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
     "SynthesizeSpeechOutputTypeDef",
     "DescribeVoicesOutputTypeDef",
     "LexiconDescriptionTypeDef",
     "GetLexiconOutputTypeDef",
     "GetSpeechSynthesisTaskOutputTypeDef",
     "ListSpeechSynthesisTasksOutputTypeDef",
     "StartSpeechSynthesisTaskOutputTypeDef",
@@ -65,20 +66,21 @@
 DeleteLexiconInputRequestTypeDef = TypedDict(
     "DeleteLexiconInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeVoicesInputDescribeVoicesPaginateTypeDef = TypedDict(
+    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Engine": EngineType,
+        "LanguageCode": LanguageCodeType,
+        "IncludeAdditionalLanguageCodes": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeVoicesInputRequestTypeDef = TypedDict(
     "DescribeVoicesInputRequestTypeDef",
     {
@@ -86,25 +88,14 @@
         "LanguageCode": LanguageCodeType,
         "IncludeAdditionalLanguageCodes": bool,
         "NextToken": str,
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
 VoiceTypeDef = TypedDict(
     "VoiceTypeDef",
     {
         "Gender": GenderType,
         "Id": VoiceIdType,
         "LanguageCode": LanguageCodeType,
         "LanguageName": str,
@@ -169,40 +160,78 @@
         "TextType": TextTypeType,
         "VoiceId": VoiceIdType,
         "LanguageCode": LanguageCodeType,
     },
     total=False,
 )
 
+ListLexiconsInputListLexiconsPaginateTypeDef = TypedDict(
+    "ListLexiconsInputListLexiconsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLexiconsInputRequestTypeDef = TypedDict(
     "ListLexiconsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef = TypedDict(
+    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
+    {
+        "Status": TaskStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSpeechSynthesisTasksInputRequestTypeDef = TypedDict(
     "ListSpeechSynthesisTasksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Status": TaskStatusType,
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
 PutLexiconInputRequestTypeDef = TypedDict(
     "PutLexiconInputRequestTypeDef",
     {
         "Name": str,
         "Content": str,
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
 _RequiredStartSpeechSynthesisTaskInputRequestTypeDef = TypedDict(
     "_RequiredStartSpeechSynthesisTaskInputRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
         "OutputS3BucketName": str,
         "Text": str,
         "VoiceId": VoiceIdType,
@@ -219,20 +248,22 @@
         "SnsTopicArn": str,
         "SpeechMarkTypes": Sequence[SpeechMarkTypeType],
         "TextType": TextTypeType,
     },
     total=False,
 )
 
+
 class StartSpeechSynthesisTaskInputRequestTypeDef(
     _RequiredStartSpeechSynthesisTaskInputRequestTypeDef,
     _OptionalStartSpeechSynthesisTaskInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredSynthesizeSpeechInputRequestTypeDef = TypedDict(
     "_RequiredSynthesizeSpeechInputRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
         "Text": str,
         "VoiceId": VoiceIdType,
     },
@@ -246,63 +277,37 @@
         "SampleRate": str,
         "SpeechMarkTypes": Sequence[SpeechMarkTypeType],
         "TextType": TextTypeType,
     },
     total=False,
 )
 
+
 class SynthesizeSpeechInputRequestTypeDef(
     _RequiredSynthesizeSpeechInputRequestTypeDef, _OptionalSynthesizeSpeechInputRequestTypeDef
 ):
     pass
 
-DescribeVoicesInputDescribeVoicesPaginateTypeDef = TypedDict(
-    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
-    {
-        "Engine": EngineType,
-        "LanguageCode": LanguageCodeType,
-        "IncludeAdditionalLanguageCodes": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListLexiconsInputListLexiconsPaginateTypeDef = TypedDict(
-    "ListLexiconsInputListLexiconsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef = TypedDict(
-    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
-    {
-        "Status": TaskStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 SynthesizeSpeechOutputTypeDef = TypedDict(
     "SynthesizeSpeechOutputTypeDef",
     {
         "AudioStream": StreamingBody,
         "ContentType": str,
         "RequestCharacters": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVoicesOutputTypeDef = TypedDict(
     "DescribeVoicesOutputTypeDef",
     {
         "Voices": List[VoiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LexiconDescriptionTypeDef = TypedDict(
     "LexiconDescriptionTypeDef",
     {
         "Name": str,
@@ -312,44 +317,44 @@
 )
 
 GetLexiconOutputTypeDef = TypedDict(
     "GetLexiconOutputTypeDef",
     {
         "Lexicon": LexiconTypeDef,
         "LexiconAttributes": LexiconAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "GetSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSpeechSynthesisTasksOutputTypeDef = TypedDict(
     "ListSpeechSynthesisTasksOutputTypeDef",
     {
         "NextToken": str,
         "SynthesisTasks": List[SynthesisTaskTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "StartSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLexiconsOutputTypeDef = TypedDict(
     "ListLexiconsOutputTypeDef",
     {
         "Lexicons": List[LexiconDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/PKG-INFO` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-polly
-Version: 1.26.69
-Summary: Type annotations for boto3.Polly 1.26.69 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Polly 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-polly"></a>
 
 # mypy-boto3-polly
 
 [![PyPI - mypy-boto3-polly](https://img.shields.io/pypi/v/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-polly?color=blue)](https://pypistats.org/packages/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.26.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,31 +337,31 @@
 
 `mypy_boto3_polly.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_polly.type_defs import (
     DeleteLexiconInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
     DescribeVoicesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     VoiceTypeDef,
     GetLexiconInputRequestTypeDef,
     LexiconAttributesTypeDef,
     LexiconTypeDef,
     GetSpeechSynthesisTaskInputRequestTypeDef,
     SynthesisTaskTypeDef,
+    ListLexiconsInputListLexiconsPaginateTypeDef,
     ListLexiconsInputRequestTypeDef,
+    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     ListSpeechSynthesisTasksInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutLexiconInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartSpeechSynthesisTaskInputRequestTypeDef,
     SynthesizeSpeechInputRequestTypeDef,
-    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
-    ListLexiconsInputListLexiconsPaginateTypeDef,
-    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     SynthesizeSpeechOutputTypeDef,
     DescribeVoicesOutputTypeDef,
     LexiconDescriptionTypeDef,
     GetLexiconOutputTypeDef,
     GetSpeechSynthesisTaskOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     StartSpeechSynthesisTaskOutputTypeDef,
@@ -376,42 +376,42 @@
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

### Comparing `mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/SOURCES.txt` & `mypy-boto3-polly-1.27.0/mypy_boto3_polly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.69/setup.py` & `mypy-boto3-polly-1.27.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-polly.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-polly",
-    version="1.26.69",
+    version="1.27.0",
     packages=["mypy_boto3_polly"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Polly 1.26.69 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.Polly 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/",
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


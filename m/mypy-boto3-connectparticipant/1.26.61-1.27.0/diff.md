# Comparing `tmp/mypy-boto3-connectparticipant-1.26.61.tar.gz` & `tmp/mypy-boto3-connectparticipant-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectparticipant-1.26.61.tar", last modified: Tue Jan 31 20:49:53 2023, max compression
+gzip compressed data, was "mypy-boto3-connectparticipant-1.27.0.tar", last modified: Mon Jul  3 19:50:36 2023, max compression
```

## Comparing `mypy-boto3-connectparticipant-1.26.61.tar` & `mypy-boto3-connectparticipant-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.610128 mypy-boto3-connectparticipant-1.26.61/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-01-31 20:49:53.610128 mypy-boto3-connectparticipant-1.26.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.610128 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.610128 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-01-31 20:49:53.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-01-31 20:49:53.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:53.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:53.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:53.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-31 20:49:53.000000 mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:49:53.610128 mypy-boto3-connectparticipant-1.26.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-01-31 20:47:30.000000 mypy-boto3-connectparticipant-1.26.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.403068 mypy-boto3-connectparticipant-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-03 19:50:36.403068 mypy-boto3-connectparticipant-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.403068 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.403068 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-03 19:50:36.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 19:50:36.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:36.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:36.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:36.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 19:50:36.000000 mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:36.403068 mypy-boto3-connectparticipant-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-03 19:35:07.000000 mypy-boto3-connectparticipant-1.27.0/setup.py
```

### Comparing `mypy-boto3-connectparticipant-1.26.61/LICENSE` & `mypy-boto3-connectparticipant-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-connectparticipant-1.26.61/PKG-INFO` & `mypy-boto3-connectparticipant-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectparticipant
-Version: 1.26.61
-Summary: Type annotations for boto3.ConnectParticipant 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ConnectParticipant 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-connectparticipant"></a>
 
 # mypy-boto3-connectparticipant
 
 [![PyPI - mypy-boto3-connectparticipant](https://img.shields.io/pypi/v/mypy-boto3-connectparticipant.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectparticipant)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectparticipant.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectparticipant)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectparticipant?color=blue)](https://pypistats.org/packages/mypy-boto3-connectparticipant)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectParticipant 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
+[boto3.ConnectParticipant 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
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
 [mypy-boto3-connectparticipant docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,27 +307,27 @@
 
 ```python
 from mypy_boto3_connectparticipant.type_defs import (
     AttachmentItemTypeDef,
     CompleteAttachmentUploadRequestRequestTypeDef,
     ConnectionCredentialsTypeDef,
     CreateParticipantConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     WebsocketTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
     GetAttachmentRequestRequestTypeDef,
+    GetAttachmentResponseTypeDef,
     StartPositionTypeDef,
     ReceiptTypeDef,
+    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
+    SendEventResponseTypeDef,
     SendMessageRequestRequestTypeDef,
+    SendMessageResponseTypeDef,
     StartAttachmentUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
-    GetAttachmentResponseTypeDef,
-    SendEventResponseTypeDef,
-    SendMessageResponseTypeDef,
     CreateParticipantConnectionResponseTypeDef,
     GetTranscriptRequestRequestTypeDef,
     MessageMetadataTypeDef,
     StartAttachmentUploadResponseTypeDef,
     ItemTypeDef,
     GetTranscriptResponseTypeDef,
 )
@@ -340,42 +340,42 @@
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

### Comparing `mypy-boto3-connectparticipant-1.26.61/README.md` & `mypy-boto3-connectparticipant-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-connectparticipant"></a>
 
 # mypy-boto3-connectparticipant
 
 [![PyPI - mypy-boto3-connectparticipant](https://img.shields.io/pypi/v/mypy-boto3-connectparticipant.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectparticipant)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectparticipant.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectparticipant)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectparticipant?color=blue)](https://pypistats.org/packages/mypy-boto3-connectparticipant)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectParticipant 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
+[boto3.ConnectParticipant 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
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
 [mypy-boto3-connectparticipant docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/).
 
 See how it helps to find and fix potential bugs:
 
@@ -275,27 +275,27 @@
 
 ```python
 from mypy_boto3_connectparticipant.type_defs import (
     AttachmentItemTypeDef,
     CompleteAttachmentUploadRequestRequestTypeDef,
     ConnectionCredentialsTypeDef,
     CreateParticipantConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     WebsocketTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
     GetAttachmentRequestRequestTypeDef,
+    GetAttachmentResponseTypeDef,
     StartPositionTypeDef,
     ReceiptTypeDef,
+    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
+    SendEventResponseTypeDef,
     SendMessageRequestRequestTypeDef,
+    SendMessageResponseTypeDef,
     StartAttachmentUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
-    GetAttachmentResponseTypeDef,
-    SendEventResponseTypeDef,
-    SendMessageResponseTypeDef,
     CreateParticipantConnectionResponseTypeDef,
     GetTranscriptRequestRequestTypeDef,
     MessageMetadataTypeDef,
     StartAttachmentUploadResponseTypeDef,
     ItemTypeDef,
     GetTranscriptResponseTypeDef,
 )
@@ -308,42 +308,42 @@
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

### Comparing `mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/__main__.py` & `mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectParticipant 1.26.61\nVersion:         1.26.61\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.ConnectParticipant 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.61")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/client.py` & `mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/client.pyi` & `mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/literals.py` & `mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
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
@@ -111,14 +112,15 @@
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
@@ -197,14 +199,15 @@
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
@@ -215,14 +218,15 @@
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
@@ -258,14 +262,15 @@
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
@@ -284,16 +289,19 @@
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
@@ -373,18 +381,21 @@
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

### Comparing `mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/literals.pyi` & `mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
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
@@ -109,14 +110,15 @@
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
@@ -195,14 +197,15 @@
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
@@ -213,14 +216,15 @@
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
@@ -256,14 +260,15 @@
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
@@ -282,16 +287,19 @@
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
@@ -371,18 +379,21 @@
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

### Comparing `mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/type_defs.py` & `mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,27 @@
 
 
 __all__ = (
     "AttachmentItemTypeDef",
     "CompleteAttachmentUploadRequestRequestTypeDef",
     "ConnectionCredentialsTypeDef",
     "CreateParticipantConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "WebsocketTypeDef",
     "DisconnectParticipantRequestRequestTypeDef",
     "GetAttachmentRequestRequestTypeDef",
+    "GetAttachmentResponseTypeDef",
     "StartPositionTypeDef",
     "ReceiptTypeDef",
+    "ResponseMetadataTypeDef",
     "SendEventRequestRequestTypeDef",
+    "SendEventResponseTypeDef",
     "SendMessageRequestRequestTypeDef",
+    "SendMessageResponseTypeDef",
     "StartAttachmentUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
-    "GetAttachmentResponseTypeDef",
-    "SendEventResponseTypeDef",
-    "SendMessageResponseTypeDef",
     "CreateParticipantConnectionResponseTypeDef",
     "GetTranscriptRequestRequestTypeDef",
     "MessageMetadataTypeDef",
     "StartAttachmentUploadResponseTypeDef",
     "ItemTypeDef",
     "GetTranscriptResponseTypeDef",
 )
@@ -103,25 +103,14 @@
 class CreateParticipantConnectionRequestRequestTypeDef(
     _RequiredCreateParticipantConnectionRequestRequestTypeDef,
     _OptionalCreateParticipantConnectionRequestRequestTypeDef,
 ):
     pass
 
 
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
 WebsocketTypeDef = TypedDict(
     "WebsocketTypeDef",
     {
         "Url": str,
         "ConnectionExpiry": str,
     },
     total=False,
@@ -153,14 +142,23 @@
     "GetAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
         "ConnectionToken": str,
     },
 )
 
+GetAttachmentResponseTypeDef = TypedDict(
+    "GetAttachmentResponseTypeDef",
+    {
+        "Url": str,
+        "UrlExpiry": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartPositionTypeDef = TypedDict(
     "StartPositionTypeDef",
     {
         "Id": str,
         "AbsoluteTime": str,
         "MostRecent": int,
     },
@@ -173,14 +171,25 @@
         "DeliveredTimestamp": str,
         "ReadTimestamp": str,
         "RecipientParticipantId": str,
     },
     total=False,
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
 _RequiredSendEventRequestRequestTypeDef = TypedDict(
     "_RequiredSendEventRequestRequestTypeDef",
     {
         "ContentType": str,
         "ConnectionToken": str,
     },
 )
@@ -196,14 +205,23 @@
 
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
 
+SendEventResponseTypeDef = TypedDict(
+    "SendEventResponseTypeDef",
+    {
+        "Id": str,
+        "AbsoluteTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSendMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendMessageRequestRequestTypeDef",
     {
         "ContentType": str,
         "Content": str,
         "ConnectionToken": str,
     },
@@ -219,14 +237,23 @@
 
 class SendMessageRequestRequestTypeDef(
     _RequiredSendMessageRequestRequestTypeDef, _OptionalSendMessageRequestRequestTypeDef
 ):
     pass
 
 
+SendMessageResponseTypeDef = TypedDict(
+    "SendMessageResponseTypeDef",
+    {
+        "Id": str,
+        "AbsoluteTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartAttachmentUploadRequestRequestTypeDef = TypedDict(
     "StartAttachmentUploadRequestRequestTypeDef",
     {
         "ContentType": str,
         "AttachmentSizeInBytes": int,
         "AttachmentName": str,
         "ClientToken": str,
@@ -240,47 +267,20 @@
         "Url": str,
         "UrlExpiry": str,
         "HeadersToInclude": Dict[str, str],
     },
     total=False,
 )
 
-GetAttachmentResponseTypeDef = TypedDict(
-    "GetAttachmentResponseTypeDef",
-    {
-        "Url": str,
-        "UrlExpiry": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendEventResponseTypeDef = TypedDict(
-    "SendEventResponseTypeDef",
-    {
-        "Id": str,
-        "AbsoluteTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendMessageResponseTypeDef = TypedDict(
-    "SendMessageResponseTypeDef",
-    {
-        "Id": str,
-        "AbsoluteTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateParticipantConnectionResponseTypeDef = TypedDict(
     "CreateParticipantConnectionResponseTypeDef",
     {
         "Websocket": WebsocketTypeDef,
         "ConnectionCredentials": ConnectionCredentialsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetTranscriptRequestRequestTypeDef = TypedDict(
     "_RequiredGetTranscriptRequestRequestTypeDef",
     {
         "ConnectionToken": str,
@@ -316,15 +316,15 @@
 )
 
 StartAttachmentUploadResponseTypeDef = TypedDict(
     "StartAttachmentUploadResponseTypeDef",
     {
         "AttachmentId": str,
         "UploadMetadata": UploadMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ItemTypeDef = TypedDict(
     "ItemTypeDef",
     {
         "AbsoluteTime": str,
@@ -345,10 +345,10 @@
 
 GetTranscriptResponseTypeDef = TypedDict(
     "GetTranscriptResponseTypeDef",
     {
         "InitialContactId": str,
         "Transcript": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant/type_defs.pyi` & `mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -29,27 +29,27 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttachmentItemTypeDef",
     "CompleteAttachmentUploadRequestRequestTypeDef",
     "ConnectionCredentialsTypeDef",
     "CreateParticipantConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "WebsocketTypeDef",
     "DisconnectParticipantRequestRequestTypeDef",
     "GetAttachmentRequestRequestTypeDef",
+    "GetAttachmentResponseTypeDef",
     "StartPositionTypeDef",
     "ReceiptTypeDef",
+    "ResponseMetadataTypeDef",
     "SendEventRequestRequestTypeDef",
+    "SendEventResponseTypeDef",
     "SendMessageRequestRequestTypeDef",
+    "SendMessageResponseTypeDef",
     "StartAttachmentUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
-    "GetAttachmentResponseTypeDef",
-    "SendEventResponseTypeDef",
-    "SendMessageResponseTypeDef",
     "CreateParticipantConnectionResponseTypeDef",
     "GetTranscriptRequestRequestTypeDef",
     "MessageMetadataTypeDef",
     "StartAttachmentUploadResponseTypeDef",
     "ItemTypeDef",
     "GetTranscriptResponseTypeDef",
 )
@@ -100,25 +100,14 @@
 
 class CreateParticipantConnectionRequestRequestTypeDef(
     _RequiredCreateParticipantConnectionRequestRequestTypeDef,
     _OptionalCreateParticipantConnectionRequestRequestTypeDef,
 ):
     pass
 
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
 WebsocketTypeDef = TypedDict(
     "WebsocketTypeDef",
     {
         "Url": str,
         "ConnectionExpiry": str,
     },
     total=False,
@@ -148,14 +137,23 @@
     "GetAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
         "ConnectionToken": str,
     },
 )
 
+GetAttachmentResponseTypeDef = TypedDict(
+    "GetAttachmentResponseTypeDef",
+    {
+        "Url": str,
+        "UrlExpiry": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartPositionTypeDef = TypedDict(
     "StartPositionTypeDef",
     {
         "Id": str,
         "AbsoluteTime": str,
         "MostRecent": int,
     },
@@ -168,14 +166,25 @@
         "DeliveredTimestamp": str,
         "ReadTimestamp": str,
         "RecipientParticipantId": str,
     },
     total=False,
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
 _RequiredSendEventRequestRequestTypeDef = TypedDict(
     "_RequiredSendEventRequestRequestTypeDef",
     {
         "ContentType": str,
         "ConnectionToken": str,
     },
 )
@@ -189,14 +198,23 @@
 )
 
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
+SendEventResponseTypeDef = TypedDict(
+    "SendEventResponseTypeDef",
+    {
+        "Id": str,
+        "AbsoluteTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSendMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendMessageRequestRequestTypeDef",
     {
         "ContentType": str,
         "Content": str,
         "ConnectionToken": str,
     },
@@ -210,14 +228,23 @@
 )
 
 class SendMessageRequestRequestTypeDef(
     _RequiredSendMessageRequestRequestTypeDef, _OptionalSendMessageRequestRequestTypeDef
 ):
     pass
 
+SendMessageResponseTypeDef = TypedDict(
+    "SendMessageResponseTypeDef",
+    {
+        "Id": str,
+        "AbsoluteTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartAttachmentUploadRequestRequestTypeDef = TypedDict(
     "StartAttachmentUploadRequestRequestTypeDef",
     {
         "ContentType": str,
         "AttachmentSizeInBytes": int,
         "AttachmentName": str,
         "ClientToken": str,
@@ -231,47 +258,20 @@
         "Url": str,
         "UrlExpiry": str,
         "HeadersToInclude": Dict[str, str],
     },
     total=False,
 )
 
-GetAttachmentResponseTypeDef = TypedDict(
-    "GetAttachmentResponseTypeDef",
-    {
-        "Url": str,
-        "UrlExpiry": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendEventResponseTypeDef = TypedDict(
-    "SendEventResponseTypeDef",
-    {
-        "Id": str,
-        "AbsoluteTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendMessageResponseTypeDef = TypedDict(
-    "SendMessageResponseTypeDef",
-    {
-        "Id": str,
-        "AbsoluteTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateParticipantConnectionResponseTypeDef = TypedDict(
     "CreateParticipantConnectionResponseTypeDef",
     {
         "Websocket": WebsocketTypeDef,
         "ConnectionCredentials": ConnectionCredentialsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetTranscriptRequestRequestTypeDef = TypedDict(
     "_RequiredGetTranscriptRequestRequestTypeDef",
     {
         "ConnectionToken": str,
@@ -305,15 +305,15 @@
 )
 
 StartAttachmentUploadResponseTypeDef = TypedDict(
     "StartAttachmentUploadResponseTypeDef",
     {
         "AttachmentId": str,
         "UploadMetadata": UploadMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ItemTypeDef = TypedDict(
     "ItemTypeDef",
     {
         "AbsoluteTime": str,
@@ -334,10 +334,10 @@
 
 GetTranscriptResponseTypeDef = TypedDict(
     "GetTranscriptResponseTypeDef",
     {
         "InitialContactId": str,
         "Transcript": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant.egg-info/PKG-INFO` & `mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectparticipant
-Version: 1.26.61
-Summary: Type annotations for boto3.ConnectParticipant 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ConnectParticipant 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-connectparticipant"></a>
 
 # mypy-boto3-connectparticipant
 
 [![PyPI - mypy-boto3-connectparticipant](https://img.shields.io/pypi/v/mypy-boto3-connectparticipant.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectparticipant)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectparticipant.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectparticipant)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectparticipant?color=blue)](https://pypistats.org/packages/mypy-boto3-connectparticipant)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectParticipant 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
+[boto3.ConnectParticipant 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
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
 [mypy-boto3-connectparticipant docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,27 +307,27 @@
 
 ```python
 from mypy_boto3_connectparticipant.type_defs import (
     AttachmentItemTypeDef,
     CompleteAttachmentUploadRequestRequestTypeDef,
     ConnectionCredentialsTypeDef,
     CreateParticipantConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     WebsocketTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
     GetAttachmentRequestRequestTypeDef,
+    GetAttachmentResponseTypeDef,
     StartPositionTypeDef,
     ReceiptTypeDef,
+    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
+    SendEventResponseTypeDef,
     SendMessageRequestRequestTypeDef,
+    SendMessageResponseTypeDef,
     StartAttachmentUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
-    GetAttachmentResponseTypeDef,
-    SendEventResponseTypeDef,
-    SendMessageResponseTypeDef,
     CreateParticipantConnectionResponseTypeDef,
     GetTranscriptRequestRequestTypeDef,
     MessageMetadataTypeDef,
     StartAttachmentUploadResponseTypeDef,
     ItemTypeDef,
     GetTranscriptResponseTypeDef,
 )
@@ -340,42 +340,42 @@
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

### Comparing `mypy-boto3-connectparticipant-1.26.61/mypy_boto3_connectparticipant.egg-info/SOURCES.txt` & `mypy-boto3-connectparticipant-1.27.0/mypy_boto3_connectparticipant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectparticipant-1.26.61/setup.py` & `mypy-boto3-connectparticipant-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-connectparticipant.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectparticipant",
-    version="1.26.61",
+    version="1.27.0",
     packages=["mypy_boto3_connectparticipant"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectParticipant 1.26.61 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.ConnectParticipant 1.27.0 service generated with"
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
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/"
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


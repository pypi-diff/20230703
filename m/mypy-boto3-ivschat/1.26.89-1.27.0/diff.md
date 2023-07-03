# Comparing `tmp/mypy-boto3-ivschat-1.26.89.tar.gz` & `tmp/mypy-boto3-ivschat-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivschat-1.26.89.tar", last modified: Fri Mar 10 20:32:12 2023, max compression
+gzip compressed data, was "mypy-boto3-ivschat-1.27.0.tar", last modified: Mon Jul  3 19:50:57 2023, max compression
```

## Comparing `mypy-boto3-ivschat-1.26.89.tar` & `mypy-boto3-ivschat-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:32:12.076089 mypy-boto3-ivschat-1.26.89/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-10 20:32:01.000000 mypy-boto3-ivschat-1.26.89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-03-10 20:32:12.076089 mypy-boto3-ivschat-1.26.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-03-10 20:32:01.000000 mypy-boto3-ivschat-1.26.89/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:32:12.076089 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-10 20:32:02.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-10 20:32:02.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-10 20:32:02.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-03-10 20:32:02.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-03-10 20:32:02.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-03-10 20:32:02.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-03-10 20:32:02.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 20:32:02.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-03-10 20:32:02.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-03-10 20:32:02.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-10 20:32:01.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:32:12.076089 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-03-10 20:32:11.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-10 20:32:12.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 20:32:11.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 20:32:11.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-10 20:32:11.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-10 20:32:11.000000 mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 20:32:12.076089 mypy-boto3-ivschat-1.26.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-10 20:32:01.000000 mypy-boto3-ivschat-1.26.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.027477 mypy-boto3-ivschat-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:04.000000 mypy-boto3-ivschat-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-07-03 19:50:57.027477 mypy-boto3-ivschat-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-07-03 19:40:04.000000 mypy-boto3-ivschat-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.027477 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-03 19:40:04.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-03 19:40:04.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:40:04.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-07-03 19:40:04.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-03 19:40:04.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-07-03 19:40:05.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-07-03 19:40:04.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:04.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-07-03 19:40:05.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-07-03 19:40:05.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:04.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.027477 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-07-03 19:50:56.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-03 19:50:56.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:56.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:56.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:56.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:50:56.000000 mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:57.027477 mypy-boto3-ivschat-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:40:04.000000 mypy-boto3-ivschat-1.27.0/setup.py
```

### Comparing `mypy-boto3-ivschat-1.26.89/LICENSE` & `mypy-boto3-ivschat-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-ivschat-1.26.89/PKG-INFO` & `mypy-boto3-ivschat-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivschat
-Version: 1.26.89
-Summary: Type annotations for boto3.ivschat 1.26.89 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.ivschat 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ivschat"></a>
 
 # mypy-boto3-ivschat
 
 [![PyPI - mypy-boto3-ivschat](https://img.shields.io/pypi/v/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivschat?color=blue)](https://pypistats.org/packages/mypy-boto3-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivschat 1.26.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[boto3.ivschat 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivschat docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,35 +302,35 @@
 `mypy_boto3_ivschat.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivschat.type_defs import (
     CloudWatchLogsDestinationConfigurationTypeDef,
     CreateChatTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateChatTokenResponseTypeDef,
     MessageReviewHandlerTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeleteMessageRequestRequestTypeDef,
+    DeleteMessageResponseTypeDef,
     DeleteRoomRequestRequestTypeDef,
     FirehoseDestinationConfigurationTypeDef,
     S3DestinationConfigurationTypeDef,
     DisconnectUserRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
+    SendEventResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateChatTokenResponseTypeDef,
-    DeleteMessageResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SendEventResponseTypeDef,
     CreateRoomRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     RoomSummaryTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateRoomResponseTypeDef,
     DestinationConfigurationTypeDef,
@@ -352,42 +352,42 @@
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

### Comparing `mypy-boto3-ivschat-1.26.89/README.md` & `mypy-boto3-ivschat-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ivschat"></a>
 
 # mypy-boto3-ivschat
 
 [![PyPI - mypy-boto3-ivschat](https://img.shields.io/pypi/v/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivschat?color=blue)](https://pypistats.org/packages/mypy-boto3-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivschat 1.26.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[boto3.ivschat 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivschat docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,35 +270,35 @@
 `mypy_boto3_ivschat.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivschat.type_defs import (
     CloudWatchLogsDestinationConfigurationTypeDef,
     CreateChatTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateChatTokenResponseTypeDef,
     MessageReviewHandlerTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeleteMessageRequestRequestTypeDef,
+    DeleteMessageResponseTypeDef,
     DeleteRoomRequestRequestTypeDef,
     FirehoseDestinationConfigurationTypeDef,
     S3DestinationConfigurationTypeDef,
     DisconnectUserRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
+    SendEventResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateChatTokenResponseTypeDef,
-    DeleteMessageResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SendEventResponseTypeDef,
     CreateRoomRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     RoomSummaryTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateRoomResponseTypeDef,
     DestinationConfigurationTypeDef,
@@ -320,42 +320,42 @@
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

### Comparing `mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/__main__.py` & `mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ivschat 1.26.89\nVersion:         1.26.89\nBuilder version:"
-        " 7.12.5\nDocs:           "
+        "Type annotations for boto3.ivschat 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.89")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/client.py` & `mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/client.pyi` & `mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/literals.py` & `mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
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
@@ -98,14 +99,15 @@
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
@@ -203,14 +205,15 @@
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
@@ -246,14 +249,15 @@
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
@@ -272,16 +276,19 @@
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
@@ -365,15 +372,17 @@
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
```

### Comparing `mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/literals.pyi` & `mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
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
@@ -96,14 +97,15 @@
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
@@ -201,14 +203,15 @@
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
@@ -244,14 +247,15 @@
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
@@ -270,16 +274,19 @@
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
@@ -363,15 +370,17 @@
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
```

### Comparing `mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/type_defs.py` & `mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,35 +26,35 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CloudWatchLogsDestinationConfigurationTypeDef",
     "CreateChatTokenRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateChatTokenResponseTypeDef",
     "MessageReviewHandlerTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeleteMessageRequestRequestTypeDef",
+    "DeleteMessageResponseTypeDef",
     "DeleteRoomRequestRequestTypeDef",
     "FirehoseDestinationConfigurationTypeDef",
     "S3DestinationConfigurationTypeDef",
     "DisconnectUserRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
     "ListRoomsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SendEventRequestRequestTypeDef",
+    "SendEventResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CreateChatTokenResponseTypeDef",
-    "DeleteMessageResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "SendEventResponseTypeDef",
     "CreateRoomRequestRequestTypeDef",
     "CreateRoomResponseTypeDef",
     "GetRoomResponseTypeDef",
     "RoomSummaryTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateRoomResponseTypeDef",
     "DestinationConfigurationTypeDef",
@@ -95,22 +95,21 @@
 
 class CreateChatTokenRequestRequestTypeDef(
     _RequiredCreateChatTokenRequestRequestTypeDef, _OptionalCreateChatTokenRequestRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateChatTokenResponseTypeDef = TypedDict(
+    "CreateChatTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "sessionExpirationTime": datetime,
+        "token": str,
+        "tokenExpirationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MessageReviewHandlerTypeDef = TypedDict(
     "MessageReviewHandlerTypeDef",
     {
         "fallbackResult": FallbackResultType,
@@ -144,14 +143,22 @@
 
 class DeleteMessageRequestRequestTypeDef(
     _RequiredDeleteMessageRequestRequestTypeDef, _OptionalDeleteMessageRequestRequestTypeDef
 ):
     pass
 
 
+DeleteMessageResponseTypeDef = TypedDict(
+    "DeleteMessageResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRoomRequestRequestTypeDef = TypedDict(
     "DeleteRoomRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
@@ -187,14 +194,21 @@
 
 class DisconnectUserRequestRequestTypeDef(
     _RequiredDisconnectUserRequestRequestTypeDef, _OptionalDisconnectUserRequestRequestTypeDef
 ):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetLoggingConfigurationRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
@@ -229,14 +243,33 @@
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
         "eventName": str,
         "roomIdentifier": str,
     },
 )
@@ -251,14 +284,22 @@
 
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
 
+SendEventResponseTypeDef = TypedDict(
+    "SendEventResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -267,55 +308,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-CreateChatTokenResponseTypeDef = TypedDict(
-    "CreateChatTokenResponseTypeDef",
-    {
-        "sessionExpirationTime": datetime,
-        "token": str,
-        "tokenExpirationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteMessageResponseTypeDef = TypedDict(
-    "DeleteMessageResponseTypeDef",
-    {
-        "id": str,
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
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendEventResponseTypeDef = TypedDict(
-    "SendEventResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateRoomRequestRequestTypeDef = TypedDict(
     "CreateRoomRequestRequestTypeDef",
     {
         "loggingConfigurationIdentifiers": Sequence[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
         "messageReviewHandler": MessageReviewHandlerTypeDef,
@@ -334,15 +334,15 @@
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
         "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRoomResponseTypeDef = TypedDict(
     "GetRoomResponseTypeDef",
     {
         "arn": str,
@@ -351,15 +351,15 @@
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
         "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RoomSummaryTypeDef = TypedDict(
     "RoomSummaryTypeDef",
     {
         "arn": str,
@@ -408,15 +408,15 @@
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
         "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsDestinationConfigurationTypeDef,
@@ -427,15 +427,15 @@
 )
 
 ListRoomsResponseTypeDef = TypedDict(
     "ListRoomsResponseTypeDef",
     {
         "nextToken": str,
         "rooms": List[RoomSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
     {
         "destinationConfiguration": DestinationConfigurationTypeDef,
@@ -465,30 +465,30 @@
         "createTime": datetime,
         "destinationConfiguration": DestinationConfigurationTypeDef,
         "id": str,
         "name": str,
         "state": Literal["ACTIVE"],
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "destinationConfiguration": DestinationConfigurationTypeDef,
         "id": str,
         "name": str,
         "state": LoggingConfigurationStateType,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoggingConfigurationSummaryTypeDef = TypedDict(
     "LoggingConfigurationSummaryTypeDef",
     {
         "arn": str,
@@ -533,19 +533,19 @@
         "createTime": datetime,
         "destinationConfiguration": DestinationConfigurationTypeDef,
         "id": str,
         "name": str,
         "state": Literal["ACTIVE"],
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
         "loggingConfigurations": List[LoggingConfigurationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat/type_defs.pyi` & `mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -25,35 +25,35 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CloudWatchLogsDestinationConfigurationTypeDef",
     "CreateChatTokenRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateChatTokenResponseTypeDef",
     "MessageReviewHandlerTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeleteMessageRequestRequestTypeDef",
+    "DeleteMessageResponseTypeDef",
     "DeleteRoomRequestRequestTypeDef",
     "FirehoseDestinationConfigurationTypeDef",
     "S3DestinationConfigurationTypeDef",
     "DisconnectUserRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
     "ListRoomsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SendEventRequestRequestTypeDef",
+    "SendEventResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CreateChatTokenResponseTypeDef",
-    "DeleteMessageResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "SendEventResponseTypeDef",
     "CreateRoomRequestRequestTypeDef",
     "CreateRoomResponseTypeDef",
     "GetRoomResponseTypeDef",
     "RoomSummaryTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateRoomResponseTypeDef",
     "DestinationConfigurationTypeDef",
@@ -92,22 +92,21 @@
 )
 
 class CreateChatTokenRequestRequestTypeDef(
     _RequiredCreateChatTokenRequestRequestTypeDef, _OptionalCreateChatTokenRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateChatTokenResponseTypeDef = TypedDict(
+    "CreateChatTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "sessionExpirationTime": datetime,
+        "token": str,
+        "tokenExpirationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MessageReviewHandlerTypeDef = TypedDict(
     "MessageReviewHandlerTypeDef",
     {
         "fallbackResult": FallbackResultType,
@@ -139,14 +138,22 @@
 )
 
 class DeleteMessageRequestRequestTypeDef(
     _RequiredDeleteMessageRequestRequestTypeDef, _OptionalDeleteMessageRequestRequestTypeDef
 ):
     pass
 
+DeleteMessageResponseTypeDef = TypedDict(
+    "DeleteMessageResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRoomRequestRequestTypeDef = TypedDict(
     "DeleteRoomRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
@@ -180,14 +187,21 @@
 )
 
 class DisconnectUserRequestRequestTypeDef(
     _RequiredDisconnectUserRequestRequestTypeDef, _OptionalDisconnectUserRequestRequestTypeDef
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetLoggingConfigurationRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
@@ -222,14 +236,33 @@
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
         "eventName": str,
         "roomIdentifier": str,
     },
 )
@@ -242,14 +275,22 @@
 )
 
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
+SendEventResponseTypeDef = TypedDict(
+    "SendEventResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -258,55 +299,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-CreateChatTokenResponseTypeDef = TypedDict(
-    "CreateChatTokenResponseTypeDef",
-    {
-        "sessionExpirationTime": datetime,
-        "token": str,
-        "tokenExpirationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteMessageResponseTypeDef = TypedDict(
-    "DeleteMessageResponseTypeDef",
-    {
-        "id": str,
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
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendEventResponseTypeDef = TypedDict(
-    "SendEventResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateRoomRequestRequestTypeDef = TypedDict(
     "CreateRoomRequestRequestTypeDef",
     {
         "loggingConfigurationIdentifiers": Sequence[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
         "messageReviewHandler": MessageReviewHandlerTypeDef,
@@ -325,15 +325,15 @@
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
         "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRoomResponseTypeDef = TypedDict(
     "GetRoomResponseTypeDef",
     {
         "arn": str,
@@ -342,15 +342,15 @@
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
         "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RoomSummaryTypeDef = TypedDict(
     "RoomSummaryTypeDef",
     {
         "arn": str,
@@ -397,15 +397,15 @@
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
         "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsDestinationConfigurationTypeDef,
@@ -416,15 +416,15 @@
 )
 
 ListRoomsResponseTypeDef = TypedDict(
     "ListRoomsResponseTypeDef",
     {
         "nextToken": str,
         "rooms": List[RoomSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
     {
         "destinationConfiguration": DestinationConfigurationTypeDef,
@@ -452,30 +452,30 @@
         "createTime": datetime,
         "destinationConfiguration": DestinationConfigurationTypeDef,
         "id": str,
         "name": str,
         "state": Literal["ACTIVE"],
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "destinationConfiguration": DestinationConfigurationTypeDef,
         "id": str,
         "name": str,
         "state": LoggingConfigurationStateType,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoggingConfigurationSummaryTypeDef = TypedDict(
     "LoggingConfigurationSummaryTypeDef",
     {
         "arn": str,
@@ -518,19 +518,19 @@
         "createTime": datetime,
         "destinationConfiguration": DestinationConfigurationTypeDef,
         "id": str,
         "name": str,
         "state": Literal["ACTIVE"],
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
         "loggingConfigurations": List[LoggingConfigurationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat.egg-info/PKG-INFO` & `mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivschat
-Version: 1.26.89
-Summary: Type annotations for boto3.ivschat 1.26.89 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.ivschat 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ivschat"></a>
 
 # mypy-boto3-ivschat
 
 [![PyPI - mypy-boto3-ivschat](https://img.shields.io/pypi/v/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivschat?color=blue)](https://pypistats.org/packages/mypy-boto3-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivschat 1.26.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[boto3.ivschat 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivschat docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,35 +302,35 @@
 `mypy_boto3_ivschat.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivschat.type_defs import (
     CloudWatchLogsDestinationConfigurationTypeDef,
     CreateChatTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateChatTokenResponseTypeDef,
     MessageReviewHandlerTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeleteMessageRequestRequestTypeDef,
+    DeleteMessageResponseTypeDef,
     DeleteRoomRequestRequestTypeDef,
     FirehoseDestinationConfigurationTypeDef,
     S3DestinationConfigurationTypeDef,
     DisconnectUserRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
+    SendEventResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateChatTokenResponseTypeDef,
-    DeleteMessageResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SendEventResponseTypeDef,
     CreateRoomRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     RoomSummaryTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateRoomResponseTypeDef,
     DestinationConfigurationTypeDef,
@@ -352,42 +352,42 @@
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

### Comparing `mypy-boto3-ivschat-1.26.89/mypy_boto3_ivschat.egg-info/SOURCES.txt` & `mypy-boto3-ivschat-1.27.0/mypy_boto3_ivschat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.26.89/setup.py` & `mypy-boto3-ivschat-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Setup script for mypy-boto3-ivschat.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivschat",
-    version="1.26.89",
+    version="1.27.0",
     packages=["mypy_boto3_ivschat"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ivschat 1.26.89 service generated with mypy-boto3-builder"
-        " 7.12.5"
+        "Type annotations for boto3.ivschat 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/",
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


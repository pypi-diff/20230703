# Comparing `tmp/mypy-boto3-kinesis-video-webrtc-storage-1.26.36.tar.gz` & `tmp/mypy-boto3-kinesis-video-webrtc-storage-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesis-video-webrtc-storage-1.26.36.tar", last modified: Thu Dec 22 20:32:39 2022, max compression
+gzip compressed data, was "mypy-boto3-kinesis-video-webrtc-storage-1.27.0.tar", last modified: Mon Jul  3 19:50:59 2023, max compression
```

## Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36.tar` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:32:39.068699 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12966 2022-12-22 20:32:39.068699 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:32:39.064699 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      996 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:32:39.068699 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12966 2022-12-22 20:32:38.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2022-12-22 20:32:38.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 20:32:38.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 20:32:38.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-22 20:32:38.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-22 20:32:38.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-22 20:32:39.068699 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2022-12-22 20:32:20.000000 mypy-boto3-kinesis-video-webrtc-storage-1.26.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:59.287517 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-07-03 19:50:59.283517 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:59.283517 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:59.283517 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-07-03 19:50:59.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-03 19:50:59.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:59.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:59.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:59.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 19:50:59.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:59.287517 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-03 19:40:22.000000 mypy-boto3-kinesis-video-webrtc-storage-1.27.0/setup.py
```

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/LICENSE` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/PKG-INFO` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-webrtc-storage
-Version: 1.26.36
-Summary: Type annotations for boto3.KinesisVideoWebRTCStorage 1.26.36 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.KinesisVideoWebRTCStorage 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_webrtc_storage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-kinesis-video-webrtc-storage"></a>
 
 # mypy-boto3-kinesis-video-webrtc-storage
 
 [![PyPI - mypy-boto3-kinesis-video-webrtc-storage](https://img.shields.io/pypi/v/mypy-boto3-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-webrtc-storage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-webrtc-storage)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_webrtc_storage/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesis-video-webrtc-storage?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesis-video-webrtc-storage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoWebRTCStorage 1.26.36](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
+[boto3.KinesisVideoWebRTCStorage 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kinesis-video-webrtc-storage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_webrtc_storage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,59 +297,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_kinesis_video_webrtc_storage.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesis_video_webrtc_storage.type_defs import (
-    ResponseMetadataTypeDef,
-    JoinStorageSessionInputRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    JoinStorageSessionInputRequestTypeDef,
+    ResponseMetadataTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> EmptyResponseMetadataTypeDef:
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

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/README.md` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-kinesis-video-webrtc-storage"></a>
 
 # mypy-boto3-kinesis-video-webrtc-storage
 
 [![PyPI - mypy-boto3-kinesis-video-webrtc-storage](https://img.shields.io/pypi/v/mypy-boto3-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-webrtc-storage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-webrtc-storage)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_webrtc_storage/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesis-video-webrtc-storage?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesis-video-webrtc-storage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoWebRTCStorage 1.26.36](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
+[boto3.KinesisVideoWebRTCStorage 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kinesis-video-webrtc-storage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_webrtc_storage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,59 +265,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_kinesis_video_webrtc_storage.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesis_video_webrtc_storage.type_defs import (
-    ResponseMetadataTypeDef,
-    JoinStorageSessionInputRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    JoinStorageSessionInputRequestTypeDef,
+    ResponseMetadataTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> EmptyResponseMetadataTypeDef:
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

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/__init__.py` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/__init__.pyi` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/__main__.py` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideoWebRTCStorage 1.26.36\nVersion:        "
-        " 1.26.36\nBuilder version: 7.12.2\nDocs:           "
+        "Type annotations for boto3.KinesisVideoWebRTCStorage 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_webrtc_storage//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.36")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/client.py` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/client.pyi` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/literals.py` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,21 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "KinesisVideoWebRTCStorageServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 KinesisVideoWebRTCStorageServiceName = Literal["kinesis-video-webrtc-storage"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -39,14 +37,15 @@
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
@@ -67,31 +66,34 @@
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
@@ -170,14 +172,15 @@
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
@@ -188,18 +191,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -230,14 +235,15 @@
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
@@ -256,16 +262,19 @@
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
@@ -345,18 +354,21 @@
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

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/literals.pyi` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "KinesisVideoWebRTCStorageServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 KinesisVideoWebRTCStorageServiceName = Literal["kinesis-video-webrtc-storage"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -37,14 +39,15 @@
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
@@ -65,31 +68,34 @@
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
@@ -168,14 +174,15 @@
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
@@ -186,18 +193,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -228,14 +237,15 @@
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
@@ -254,16 +264,19 @@
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
@@ -343,18 +356,21 @@
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

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/type_defs.py` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,51 +2,51 @@
 Type annotations for kinesis-video-webrtc-storage service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_webrtc_storage/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_kinesis_video_webrtc_storage.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_kinesis_video_webrtc_storage.type_defs import EmptyResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: EmptyResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ResponseMetadataTypeDef",
-    "JoinStorageSessionInputRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "JoinStorageSessionInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
 )
 
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
 
 JoinStorageSessionInputRequestTypeDef = TypedDict(
     "JoinStorageSessionInputRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
```

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage/type_defs.pyi` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,50 +2,50 @@
 Type annotations for kinesis-video-webrtc-storage service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_webrtc_storage/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_kinesis_video_webrtc_storage.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_kinesis_video_webrtc_storage.type_defs import EmptyResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: EmptyResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ResponseMetadataTypeDef",
-    "JoinStorageSessionInputRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "JoinStorageSessionInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
 )
 
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
 
 JoinStorageSessionInputRequestTypeDef = TypedDict(
     "JoinStorageSessionInputRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
```

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage.egg-info/PKG-INFO` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-webrtc-storage
-Version: 1.26.36
-Summary: Type annotations for boto3.KinesisVideoWebRTCStorage 1.26.36 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.KinesisVideoWebRTCStorage 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_webrtc_storage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-kinesis-video-webrtc-storage"></a>
 
 # mypy-boto3-kinesis-video-webrtc-storage
 
 [![PyPI - mypy-boto3-kinesis-video-webrtc-storage](https://img.shields.io/pypi/v/mypy-boto3-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-webrtc-storage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-webrtc-storage)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_webrtc_storage/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesis-video-webrtc-storage?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesis-video-webrtc-storage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoWebRTCStorage 1.26.36](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
+[boto3.KinesisVideoWebRTCStorage 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kinesis-video-webrtc-storage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_webrtc_storage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,59 +297,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_kinesis_video_webrtc_storage.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesis_video_webrtc_storage.type_defs import (
-    ResponseMetadataTypeDef,
-    JoinStorageSessionInputRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    JoinStorageSessionInputRequestTypeDef,
+    ResponseMetadataTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> EmptyResponseMetadataTypeDef:
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

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/mypy_boto3_kinesis_video_webrtc_storage.egg-info/SOURCES.txt` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/mypy_boto3_kinesis_video_webrtc_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-webrtc-storage-1.26.36/setup.py` & `mypy-boto3-kinesis-video-webrtc-storage-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-kinesis-video-webrtc-storage.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesis-video-webrtc-storage",
-    version="1.26.36",
+    version="1.27.0",
     packages=["mypy_boto3_kinesis_video_webrtc_storage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideoWebRTCStorage 1.26.36 service generated with"
-        " mypy-boto3-builder 7.12.2"
+        "Type annotations for boto3.KinesisVideoWebRTCStorage 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -49,11 +49,11 @@
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_webrtc_storage/"
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


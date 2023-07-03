# Comparing `tmp/mypy-boto3-ivs-1.26.85.tar.gz` & `tmp/mypy-boto3-ivs-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivs-1.26.85.tar", last modified: Mon Mar  6 20:27:45 2023, max compression
+gzip compressed data, was "mypy-boto3-ivs-1.27.0.tar", last modified: Mon Jul  3 19:50:57 2023, max compression
```

## Comparing `mypy-boto3-ivs-1.26.85.tar` & `mypy-boto3-ivs-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:45.512846 mypy-boto3-ivs-1.26.85/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-03-06 20:27:45.512846 mypy-boto3-ivs-1.26.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:45.508846 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21260 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21220 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23265 2023-03-06 20:27:35.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23244 2023-03-06 20:27:35.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:45.508846 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-03-06 20:27:45.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-06 20:27:45.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 20:27:45.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 20:27:45.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-06 20:27:45.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-06 20:27:45.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 20:27:45.512846 mypy-boto3-ivs-1.26.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:56.991476 mypy-boto3-ivs-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-03 19:50:56.991476 mypy-boto3-ivs-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:56.991476 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26328 2023-07-03 19:40:02.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26301 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:56.991476 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-03 19:50:56.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:50:56.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:56.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:56.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:56.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:56.000000 mypy-boto3-ivs-1.27.0/mypy_boto3_ivs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:56.991476 mypy-boto3-ivs-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:40:01.000000 mypy-boto3-ivs-1.27.0/setup.py
```

### Comparing `mypy-boto3-ivs-1.26.85/LICENSE` & `mypy-boto3-ivs-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-ivs-1.26.85/PKG-INFO` & `mypy-boto3-ivs-1.27.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.26.85
-Summary: Type annotations for boto3.IVS 1.26.85 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.IVS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ivs"></a>
 
 # mypy-boto3-ivs
 
 [![PyPI - mypy-boto3-ivs](https://img.shields.io/pypi/v/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.26.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,14 +320,15 @@
     ListRecordingConfigurationsPaginatorName,
     ListStreamKeysPaginatorName,
     ListStreamsPaginatorName,
     RecordingConfigurationStateType,
     RecordingModeType,
     StreamHealthType,
     StreamStateType,
+    TranscodePresetType,
     IVSServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -345,73 +346,78 @@
 
 ```python
 from mypy_boto3_ivs.type_defs import (
     AudioConfigurationTypeDef,
     BatchErrorTypeDef,
     BatchGetChannelRequestRequestTypeDef,
     ChannelTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetStreamKeyRequestRequestTypeDef,
     StreamKeyTypeDef,
+    BatchStartViewerSessionRevocationErrorTypeDef,
+    BatchStartViewerSessionRevocationViewerSessionTypeDef,
     ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
     ThumbnailConfigurationTypeDef,
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
     S3DestinationConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
     StreamTypeDef,
     GetStreamSessionRequestRequestTypeDef,
     ImportPlaybackKeyPairRequestRequestTypeDef,
     VideoConfigurationTypeDef,
-    PaginatorConfigTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
     ListPlaybackKeyPairsRequestRequestTypeDef,
     PlaybackKeyPairSummaryTypeDef,
+    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
     ListRecordingConfigurationsRequestRequestTypeDef,
+    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListStreamKeysRequestRequestTypeDef,
     StreamKeySummaryTypeDef,
     ListStreamSessionsRequestRequestTypeDef,
     StreamSessionSummaryTypeDef,
     StreamFiltersTypeDef,
     StreamSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutMetadataRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    StartViewerSessionRevocationRequestRequestTypeDef,
     StopStreamRequestRequestTypeDef,
     StreamEventTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     BatchGetChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdateChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
+    BatchStartViewerSessionRevocationResponseTypeDef,
+    BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
-    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
-    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
     CreateRecordingConfigurationRequestRequestTypeDef,
@@ -432,42 +438,42 @@
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

### Comparing `mypy-boto3-ivs-1.26.85/README.md` & `mypy-boto3-ivs-1.27.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ivs"></a>
 
 # mypy-boto3-ivs
 
 [![PyPI - mypy-boto3-ivs](https://img.shields.io/pypi/v/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.26.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,14 +288,15 @@
     ListRecordingConfigurationsPaginatorName,
     ListStreamKeysPaginatorName,
     ListStreamsPaginatorName,
     RecordingConfigurationStateType,
     RecordingModeType,
     StreamHealthType,
     StreamStateType,
+    TranscodePresetType,
     IVSServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -313,73 +314,78 @@
 
 ```python
 from mypy_boto3_ivs.type_defs import (
     AudioConfigurationTypeDef,
     BatchErrorTypeDef,
     BatchGetChannelRequestRequestTypeDef,
     ChannelTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetStreamKeyRequestRequestTypeDef,
     StreamKeyTypeDef,
+    BatchStartViewerSessionRevocationErrorTypeDef,
+    BatchStartViewerSessionRevocationViewerSessionTypeDef,
     ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
     ThumbnailConfigurationTypeDef,
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
     S3DestinationConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
     StreamTypeDef,
     GetStreamSessionRequestRequestTypeDef,
     ImportPlaybackKeyPairRequestRequestTypeDef,
     VideoConfigurationTypeDef,
-    PaginatorConfigTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
     ListPlaybackKeyPairsRequestRequestTypeDef,
     PlaybackKeyPairSummaryTypeDef,
+    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
     ListRecordingConfigurationsRequestRequestTypeDef,
+    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListStreamKeysRequestRequestTypeDef,
     StreamKeySummaryTypeDef,
     ListStreamSessionsRequestRequestTypeDef,
     StreamSessionSummaryTypeDef,
     StreamFiltersTypeDef,
     StreamSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutMetadataRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    StartViewerSessionRevocationRequestRequestTypeDef,
     StopStreamRequestRequestTypeDef,
     StreamEventTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     BatchGetChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdateChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
+    BatchStartViewerSessionRevocationResponseTypeDef,
+    BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
-    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
-    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
     CreateRecordingConfigurationRequestRequestTypeDef,
@@ -400,42 +406,42 @@
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

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/__init__.py` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/__init__.pyi` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/__main__.py` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IVS 1.26.85\nVersion:         1.26.85\nBuilder version:"
-        " 7.12.5\nDocs:           "
+        "Type annotations for boto3.IVS 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.85")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/client.py` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,27 @@
     ```
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ChannelLatencyModeType, ChannelTypeType
+from .literals import ChannelLatencyModeType, ChannelTypeType, TranscodePresetType
 from .paginator import (
     ListChannelsPaginator,
     ListPlaybackKeyPairsPaginator,
     ListRecordingConfigurationsPaginator,
     ListStreamKeysPaginator,
     ListStreamsPaginator,
 )
 from .type_defs import (
     BatchGetChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
+    BatchStartViewerSessionRevocationResponseTypeDef,
+    BatchStartViewerSessionRevocationViewerSessionTypeDef,
     CreateChannelResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     DestinationConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
@@ -113,14 +115,25 @@
         """
         Performs  GetStreamKey on multiple ARNs simultaneously.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.batch_get_stream_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#batch_get_stream_key)
         """
 
+    def batch_start_viewer_session_revocation(
+        self, *, viewerSessions: Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef]
+    ) -> BatchStartViewerSessionRevocationResponseTypeDef:
+        """
+        Performs  StartViewerSessionRevocation on multiple channel ARN and viewer ID
+        pairs simultaneously.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.batch_start_viewer_session_revocation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#batch_start_viewer_session_revocation)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#can_paginate)
         """
@@ -133,16 +146,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#close)
         """
 
     def create_channel(
         self,
         *,
         authorized: bool = ...,
+        insecureIngest: bool = ...,
         latencyMode: ChannelLatencyModeType = ...,
         name: str = ...,
+        preset: TranscodePresetType = ...,
         recordingConfigurationArn: str = ...,
         tags: Mapping[str, str] = ...,
         type: ChannelTypeType = ...
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a new channel and an associated stream key to start streaming.
 
@@ -366,14 +381,25 @@
         """
         Inserts metadata into the active stream of the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.put_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#put_metadata)
         """
 
+    def start_viewer_session_revocation(
+        self, *, channelArn: str, viewerId: str, viewerSessionVersionsLessThanOrEqualTo: int = ...
+    ) -> Dict[str, Any]:
+        """
+        Starts the process of revoking the viewer session associated with a specified
+        channel ARN and viewer ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.start_viewer_session_revocation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#start_viewer_session_revocation)
+        """
+
     def stop_stream(self, *, channelArn: str) -> Dict[str, Any]:
         """
         Disconnects the incoming RTMPS stream for the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.stop_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#stop_stream)
         """
@@ -396,16 +422,18 @@
         """
 
     def update_channel(
         self,
         *,
         arn: str,
         authorized: bool = ...,
+        insecureIngest: bool = ...,
         latencyMode: ChannelLatencyModeType = ...,
         name: str = ...,
+        preset: TranscodePresetType = ...,
         recordingConfigurationArn: str = ...,
         type: ChannelTypeType = ...
     ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.update_channel)
```

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/client.pyi` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,27 @@
     ```
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ChannelLatencyModeType, ChannelTypeType
+from .literals import ChannelLatencyModeType, ChannelTypeType, TranscodePresetType
 from .paginator import (
     ListChannelsPaginator,
     ListPlaybackKeyPairsPaginator,
     ListRecordingConfigurationsPaginator,
     ListStreamKeysPaginator,
     ListStreamsPaginator,
 )
 from .type_defs import (
     BatchGetChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
+    BatchStartViewerSessionRevocationResponseTypeDef,
+    BatchStartViewerSessionRevocationViewerSessionTypeDef,
     CreateChannelResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     DestinationConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
@@ -106,14 +108,24 @@
     def batch_get_stream_key(self, *, arns: Sequence[str]) -> BatchGetStreamKeyResponseTypeDef:
         """
         Performs  GetStreamKey on multiple ARNs simultaneously.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.batch_get_stream_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#batch_get_stream_key)
         """
+    def batch_start_viewer_session_revocation(
+        self, *, viewerSessions: Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef]
+    ) -> BatchStartViewerSessionRevocationResponseTypeDef:
+        """
+        Performs  StartViewerSessionRevocation on multiple channel ARN and viewer ID
+        pairs simultaneously.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.batch_start_viewer_session_revocation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#batch_start_viewer_session_revocation)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#can_paginate)
         """
@@ -124,16 +136,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#close)
         """
     def create_channel(
         self,
         *,
         authorized: bool = ...,
+        insecureIngest: bool = ...,
         latencyMode: ChannelLatencyModeType = ...,
         name: str = ...,
+        preset: TranscodePresetType = ...,
         recordingConfigurationArn: str = ...,
         tags: Mapping[str, str] = ...,
         type: ChannelTypeType = ...
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a new channel and an associated stream key to start streaming.
 
@@ -334,14 +348,24 @@
     def put_metadata(self, *, channelArn: str, metadata: str) -> EmptyResponseMetadataTypeDef:
         """
         Inserts metadata into the active stream of the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.put_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#put_metadata)
         """
+    def start_viewer_session_revocation(
+        self, *, channelArn: str, viewerId: str, viewerSessionVersionsLessThanOrEqualTo: int = ...
+    ) -> Dict[str, Any]:
+        """
+        Starts the process of revoking the viewer session associated with a specified
+        channel ARN and viewer ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.start_viewer_session_revocation)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#start_viewer_session_revocation)
+        """
     def stop_stream(self, *, channelArn: str) -> Dict[str, Any]:
         """
         Disconnects the incoming RTMPS stream for the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.stop_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#stop_stream)
         """
@@ -361,16 +385,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#untag_resource)
         """
     def update_channel(
         self,
         *,
         arn: str,
         authorized: bool = ...,
+        insecureIngest: bool = ...,
         latencyMode: ChannelLatencyModeType = ...,
         name: str = ...,
+        preset: TranscodePresetType = ...,
         recordingConfigurationArn: str = ...,
         type: ChannelTypeType = ...
     ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.update_channel)
```

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/literals.py` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,33 +27,35 @@
     "ListRecordingConfigurationsPaginatorName",
     "ListStreamKeysPaginatorName",
     "ListStreamsPaginatorName",
     "RecordingConfigurationStateType",
     "RecordingModeType",
     "StreamHealthType",
     "StreamStateType",
+    "TranscodePresetType",
     "IVSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
 ChannelLatencyModeType = Literal["LOW", "NORMAL"]
-ChannelTypeType = Literal["BASIC", "STANDARD"]
+ChannelTypeType = Literal["ADVANCED_HD", "ADVANCED_SD", "BASIC", "STANDARD"]
 ListChannelsPaginatorName = Literal["list_channels"]
 ListPlaybackKeyPairsPaginatorName = Literal["list_playback_key_pairs"]
 ListRecordingConfigurationsPaginatorName = Literal["list_recording_configurations"]
 ListStreamKeysPaginatorName = Literal["list_stream_keys"]
 ListStreamsPaginatorName = Literal["list_streams"]
 RecordingConfigurationStateType = Literal["ACTIVE", "CREATE_FAILED", "CREATING"]
 RecordingModeType = Literal["DISABLED", "INTERVAL"]
 StreamHealthType = Literal["HEALTHY", "STARVING", "UNKNOWN"]
 StreamStateType = Literal["LIVE", "OFFLINE"]
+TranscodePresetType = Literal["CONSTRAINED_BANDWIDTH_DELIVERY", "HIGHER_BANDWIDTH_DELIVERY"]
 IVSServiceName = Literal["ivs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -62,14 +64,15 @@
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
@@ -109,14 +112,15 @@
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
@@ -214,14 +218,15 @@
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
@@ -257,14 +262,15 @@
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
@@ -283,16 +289,19 @@
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
@@ -376,15 +385,17 @@
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

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/literals.pyi` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -26,32 +26,34 @@
     "ListRecordingConfigurationsPaginatorName",
     "ListStreamKeysPaginatorName",
     "ListStreamsPaginatorName",
     "RecordingConfigurationStateType",
     "RecordingModeType",
     "StreamHealthType",
     "StreamStateType",
+    "TranscodePresetType",
     "IVSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 ChannelLatencyModeType = Literal["LOW", "NORMAL"]
-ChannelTypeType = Literal["BASIC", "STANDARD"]
+ChannelTypeType = Literal["ADVANCED_HD", "ADVANCED_SD", "BASIC", "STANDARD"]
 ListChannelsPaginatorName = Literal["list_channels"]
 ListPlaybackKeyPairsPaginatorName = Literal["list_playback_key_pairs"]
 ListRecordingConfigurationsPaginatorName = Literal["list_recording_configurations"]
 ListStreamKeysPaginatorName = Literal["list_stream_keys"]
 ListStreamsPaginatorName = Literal["list_streams"]
 RecordingConfigurationStateType = Literal["ACTIVE", "CREATE_FAILED", "CREATING"]
 RecordingModeType = Literal["DISABLED", "INTERVAL"]
 StreamHealthType = Literal["HEALTHY", "STARVING", "UNKNOWN"]
 StreamStateType = Literal["LIVE", "OFFLINE"]
+TranscodePresetType = Literal["CONSTRAINED_BANDWIDTH_DELIVERY", "HIGHER_BANDWIDTH_DELIVERY"]
 IVSServiceName = Literal["ivs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -60,14 +62,15 @@
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
@@ -107,14 +110,15 @@
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
@@ -212,14 +216,15 @@
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
@@ -255,14 +260,15 @@
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
@@ -281,16 +287,19 @@
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
@@ -374,15 +383,17 @@
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

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/paginator.py` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,98 +45,91 @@
     "ListChannelsPaginator",
     "ListPlaybackKeyPairsPaginator",
     "ListRecordingConfigurationsPaginator",
     "ListStreamKeysPaginator",
     "ListStreamsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         filterByName: str = ...,
         filterByRecordingConfigurationArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listchannelspaginator)
         """
 
-
 class ListPlaybackKeyPairsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listplaybackkeypairspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPlaybackKeyPairsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listplaybackkeypairspaginator)
         """
 
-
 class ListRecordingConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listrecordingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecordingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listrecordingconfigurationspaginator)
         """
 
-
 class ListStreamKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamkeyspaginator)
     """
 
     def paginate(
-        self, *, channelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, channelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamkeyspaginator)
         """
 
-
 class ListStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         filterBy: StreamFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/paginator.pyi` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,91 +45,98 @@
     "ListChannelsPaginator",
     "ListPlaybackKeyPairsPaginator",
     "ListRecordingConfigurationsPaginator",
     "ListStreamKeysPaginator",
     "ListStreamsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         filterByName: str = ...,
         filterByRecordingConfigurationArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listchannelspaginator)
         """
 
+
 class ListPlaybackKeyPairsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listplaybackkeypairspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPlaybackKeyPairsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listplaybackkeypairspaginator)
         """
 
+
 class ListRecordingConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listrecordingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecordingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listrecordingconfigurationspaginator)
         """
 
+
 class ListStreamKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamkeyspaginator)
     """
 
     def paginate(
-        self, *, channelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, channelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamkeyspaginator)
         """
 
+
 class ListStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         filterBy: StreamFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/type_defs.py` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,86 +18,92 @@
 from .literals import (
     ChannelLatencyModeType,
     ChannelTypeType,
     RecordingConfigurationStateType,
     RecordingModeType,
     StreamHealthType,
     StreamStateType,
+    TranscodePresetType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AudioConfigurationTypeDef",
     "BatchErrorTypeDef",
     "BatchGetChannelRequestRequestTypeDef",
     "ChannelTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetStreamKeyRequestRequestTypeDef",
     "StreamKeyTypeDef",
+    "BatchStartViewerSessionRevocationErrorTypeDef",
+    "BatchStartViewerSessionRevocationViewerSessionTypeDef",
     "ChannelSummaryTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "ThumbnailConfigurationTypeDef",
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeletePlaybackKeyPairRequestRequestTypeDef",
     "DeleteRecordingConfigurationRequestRequestTypeDef",
     "DeleteStreamKeyRequestRequestTypeDef",
     "S3DestinationConfigurationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetPlaybackKeyPairRequestRequestTypeDef",
     "PlaybackKeyPairTypeDef",
     "GetRecordingConfigurationRequestRequestTypeDef",
     "GetStreamKeyRequestRequestTypeDef",
     "GetStreamRequestRequestTypeDef",
     "StreamTypeDef",
     "GetStreamSessionRequestRequestTypeDef",
     "ImportPlaybackKeyPairRequestRequestTypeDef",
     "VideoConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
     "ListPlaybackKeyPairsRequestRequestTypeDef",
     "PlaybackKeyPairSummaryTypeDef",
+    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
     "ListRecordingConfigurationsRequestRequestTypeDef",
+    "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListStreamKeysRequestRequestTypeDef",
     "StreamKeySummaryTypeDef",
     "ListStreamSessionsRequestRequestTypeDef",
     "StreamSessionSummaryTypeDef",
     "StreamFiltersTypeDef",
     "StreamSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutMetadataRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartViewerSessionRevocationRequestRequestTypeDef",
     "StopStreamRequestRequestTypeDef",
     "StreamEventTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "BatchGetChannelResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetChannelResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "BatchGetStreamKeyResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
+    "BatchStartViewerSessionRevocationResponseTypeDef",
+    "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
     "IngestConfigurationTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
-    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
-    "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
     "CreateRecordingConfigurationRequestRequestTypeDef",
@@ -140,35 +146,26 @@
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "arn": str,
         "authorized": bool,
         "ingestEndpoint": str,
+        "insecureIngest": bool,
         "latencyMode": ChannelLatencyModeType,
         "name": str,
         "playbackUrl": str,
+        "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
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
 BatchGetStreamKeyRequestRequestTypeDef = TypedDict(
     "BatchGetStreamKeyRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
 )
 
@@ -179,33 +176,85 @@
         "channelArn": str,
         "tags": Dict[str, str],
         "value": str,
     },
     total=False,
 )
 
+_RequiredBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "_RequiredBatchStartViewerSessionRevocationErrorTypeDef",
+    {
+        "channelArn": str,
+        "viewerId": str,
+    },
+)
+_OptionalBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "_OptionalBatchStartViewerSessionRevocationErrorTypeDef",
+    {
+        "code": str,
+        "message": str,
+    },
+    total=False,
+)
+
+
+class BatchStartViewerSessionRevocationErrorTypeDef(
+    _RequiredBatchStartViewerSessionRevocationErrorTypeDef,
+    _OptionalBatchStartViewerSessionRevocationErrorTypeDef,
+):
+    pass
+
+
+_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
+    "_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef",
+    {
+        "channelArn": str,
+        "viewerId": str,
+    },
+)
+_OptionalBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
+    "_OptionalBatchStartViewerSessionRevocationViewerSessionTypeDef",
+    {
+        "viewerSessionVersionsLessThanOrEqualTo": int,
+    },
+    total=False,
+)
+
+
+class BatchStartViewerSessionRevocationViewerSessionTypeDef(
+    _RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef,
+    _OptionalBatchStartViewerSessionRevocationViewerSessionTypeDef,
+):
+    pass
+
+
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "arn": str,
         "authorized": bool,
+        "insecureIngest": bool,
         "latencyMode": ChannelLatencyModeType,
         "name": str,
+        "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
+        "type": ChannelTypeType,
     },
     total=False,
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "authorized": bool,
+        "insecureIngest": bool,
         "latencyMode": ChannelLatencyModeType,
         "name": str,
+        "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Mapping[str, str],
         "type": ChannelTypeType,
     },
     total=False,
 )
 
@@ -270,14 +319,21 @@
 S3DestinationConfigurationTypeDef = TypedDict(
     "S3DestinationConfigurationTypeDef",
     {
         "bucketName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetChannelRequestRequestTypeDef = TypedDict(
     "GetChannelRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -389,20 +445,20 @@
         "targetFramerate": int,
         "videoHeight": int,
         "videoWidth": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "filterByName": str,
+        "filterByRecordingConfigurationArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
@@ -410,14 +466,22 @@
         "filterByRecordingConfigurationArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = TypedDict(
+    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPlaybackKeyPairsRequestRequestTypeDef = TypedDict(
     "ListPlaybackKeyPairsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -429,23 +493,53 @@
         "arn": str,
         "name": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = TypedDict(
+    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRecordingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListRecordingConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
+    "_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef",
+    {
+        "channelArn": str,
+    },
+)
+_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
+    "_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStreamKeysRequestListStreamKeysPaginateTypeDef(
+    _RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef,
+    _OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListStreamKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamKeysRequestRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 _OptionalListStreamKeysRequestRequestTypeDef = TypedDict(
@@ -532,22 +626,74 @@
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
 PutMetadataRequestRequestTypeDef = TypedDict(
     "PutMetadataRequestRequestTypeDef",
     {
         "channelArn": str,
         "metadata": str,
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
+_RequiredStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartViewerSessionRevocationRequestRequestTypeDef",
+    {
+        "channelArn": str,
+        "viewerId": str,
+    },
+)
+_OptionalStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartViewerSessionRevocationRequestRequestTypeDef",
+    {
+        "viewerSessionVersionsLessThanOrEqualTo": int,
+    },
+    total=False,
+)
+
+
+class StartViewerSessionRevocationRequestRequestTypeDef(
+    _RequiredStartViewerSessionRevocationRequestRequestTypeDef,
+    _OptionalStartViewerSessionRevocationRequestRequestTypeDef,
+):
+    pass
+
+
 StopStreamRequestRequestTypeDef = TypedDict(
     "StopStreamRequestRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 
@@ -583,16 +729,18 @@
         "arn": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "authorized": bool,
+        "insecureIngest": bool,
         "latencyMode": ChannelLatencyModeType,
         "name": str,
+        "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "type": ChannelTypeType,
     },
     total=False,
 )
 
 
@@ -603,89 +751,89 @@
 
 
 BatchGetChannelResponseTypeDef = TypedDict(
     "BatchGetChannelResponseTypeDef",
     {
         "channels": List[ChannelTypeDef],
         "errors": List[BatchErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetStreamKeyResponseTypeDef = TypedDict(
     "BatchGetStreamKeyResponseTypeDef",
     {
         "errors": List[BatchErrorTypeDef],
         "streamKeys": List[StreamKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStreamKeyResponseTypeDef = TypedDict(
     "CreateStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStreamKeyResponseTypeDef = TypedDict(
     "GetStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchStartViewerSessionRevocationResponseTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationResponseTypeDef",
+    {
+        "errors": List[BatchStartViewerSessionRevocationErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationRequestRequestTypeDef",
+    {
+        "viewerSessions": Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef],
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "s3": S3DestinationConfigurationTypeDef,
@@ -693,123 +841,75 @@
     total=False,
 )
 
 GetPlaybackKeyPairResponseTypeDef = TypedDict(
     "GetPlaybackKeyPairResponseTypeDef",
     {
         "keyPair": PlaybackKeyPairTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportPlaybackKeyPairResponseTypeDef = TypedDict(
     "ImportPlaybackKeyPairResponseTypeDef",
     {
         "keyPair": PlaybackKeyPairTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStreamResponseTypeDef = TypedDict(
     "GetStreamResponseTypeDef",
     {
         "stream": StreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IngestConfigurationTypeDef = TypedDict(
     "IngestConfigurationTypeDef",
     {
         "audio": AudioConfigurationTypeDef,
         "video": VideoConfigurationTypeDef,
     },
     total=False,
 )
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "filterByName": str,
-        "filterByRecordingConfigurationArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = TypedDict(
-    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = TypedDict(
-    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
-    "_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef",
-    {
-        "channelArn": str,
-    },
-)
-_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
-    "_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStreamKeysRequestListStreamKeysPaginateTypeDef(
-    _RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef,
-    _OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef,
-):
-    pass
-
-
 ListPlaybackKeyPairsResponseTypeDef = TypedDict(
     "ListPlaybackKeyPairsResponseTypeDef",
     {
         "keyPairs": List[PlaybackKeyPairSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamKeysResponseTypeDef = TypedDict(
     "ListStreamKeysResponseTypeDef",
     {
         "nextToken": str,
         "streamKeys": List[StreamKeySummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamSessionsResponseTypeDef = TypedDict(
     "ListStreamSessionsResponseTypeDef",
     {
         "nextToken": str,
         "streamSessions": List[StreamSessionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsRequestListStreamsPaginateTypeDef",
     {
         "filterBy": StreamFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListStreamsRequestRequestTypeDef = TypedDict(
     "ListStreamsRequestRequestTypeDef",
     {
@@ -821,15 +921,15 @@
 )
 
 ListStreamsResponseTypeDef = TypedDict(
     "ListStreamsResponseTypeDef",
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
     {
         "destinationConfiguration": DestinationConfigurationTypeDef,
@@ -905,31 +1005,31 @@
 
 
 ListRecordingConfigurationsResponseTypeDef = TypedDict(
     "ListRecordingConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "recordingConfigurations": List[RecordingConfigurationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRecordingConfigurationResponseTypeDef = TypedDict(
     "CreateRecordingConfigurationResponseTypeDef",
     {
         "recordingConfiguration": RecordingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecordingConfigurationResponseTypeDef = TypedDict(
     "GetRecordingConfigurationResponseTypeDef",
     {
         "recordingConfiguration": RecordingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StreamSessionTypeDef = TypedDict(
     "StreamSessionTypeDef",
     {
         "channel": ChannelTypeDef,
@@ -943,10 +1043,10 @@
     total=False,
 )
 
 GetStreamSessionResponseTypeDef = TypedDict(
     "GetStreamSessionResponseTypeDef",
     {
         "streamSession": StreamSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/type_defs.pyi` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -18,85 +18,91 @@
 from .literals import (
     ChannelLatencyModeType,
     ChannelTypeType,
     RecordingConfigurationStateType,
     RecordingModeType,
     StreamHealthType,
     StreamStateType,
+    TranscodePresetType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AudioConfigurationTypeDef",
     "BatchErrorTypeDef",
     "BatchGetChannelRequestRequestTypeDef",
     "ChannelTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetStreamKeyRequestRequestTypeDef",
     "StreamKeyTypeDef",
+    "BatchStartViewerSessionRevocationErrorTypeDef",
+    "BatchStartViewerSessionRevocationViewerSessionTypeDef",
     "ChannelSummaryTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "ThumbnailConfigurationTypeDef",
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeletePlaybackKeyPairRequestRequestTypeDef",
     "DeleteRecordingConfigurationRequestRequestTypeDef",
     "DeleteStreamKeyRequestRequestTypeDef",
     "S3DestinationConfigurationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetPlaybackKeyPairRequestRequestTypeDef",
     "PlaybackKeyPairTypeDef",
     "GetRecordingConfigurationRequestRequestTypeDef",
     "GetStreamKeyRequestRequestTypeDef",
     "GetStreamRequestRequestTypeDef",
     "StreamTypeDef",
     "GetStreamSessionRequestRequestTypeDef",
     "ImportPlaybackKeyPairRequestRequestTypeDef",
     "VideoConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
     "ListPlaybackKeyPairsRequestRequestTypeDef",
     "PlaybackKeyPairSummaryTypeDef",
+    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
     "ListRecordingConfigurationsRequestRequestTypeDef",
+    "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListStreamKeysRequestRequestTypeDef",
     "StreamKeySummaryTypeDef",
     "ListStreamSessionsRequestRequestTypeDef",
     "StreamSessionSummaryTypeDef",
     "StreamFiltersTypeDef",
     "StreamSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutMetadataRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartViewerSessionRevocationRequestRequestTypeDef",
     "StopStreamRequestRequestTypeDef",
     "StreamEventTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "BatchGetChannelResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetChannelResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "BatchGetStreamKeyResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
+    "BatchStartViewerSessionRevocationResponseTypeDef",
+    "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
     "IngestConfigurationTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
-    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
-    "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
     "CreateRecordingConfigurationRequestRequestTypeDef",
@@ -139,35 +145,26 @@
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "arn": str,
         "authorized": bool,
         "ingestEndpoint": str,
+        "insecureIngest": bool,
         "latencyMode": ChannelLatencyModeType,
         "name": str,
         "playbackUrl": str,
+        "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
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
 BatchGetStreamKeyRequestRequestTypeDef = TypedDict(
     "BatchGetStreamKeyRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
 )
 
@@ -178,33 +175,81 @@
         "channelArn": str,
         "tags": Dict[str, str],
         "value": str,
     },
     total=False,
 )
 
+_RequiredBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "_RequiredBatchStartViewerSessionRevocationErrorTypeDef",
+    {
+        "channelArn": str,
+        "viewerId": str,
+    },
+)
+_OptionalBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "_OptionalBatchStartViewerSessionRevocationErrorTypeDef",
+    {
+        "code": str,
+        "message": str,
+    },
+    total=False,
+)
+
+class BatchStartViewerSessionRevocationErrorTypeDef(
+    _RequiredBatchStartViewerSessionRevocationErrorTypeDef,
+    _OptionalBatchStartViewerSessionRevocationErrorTypeDef,
+):
+    pass
+
+_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
+    "_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef",
+    {
+        "channelArn": str,
+        "viewerId": str,
+    },
+)
+_OptionalBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
+    "_OptionalBatchStartViewerSessionRevocationViewerSessionTypeDef",
+    {
+        "viewerSessionVersionsLessThanOrEqualTo": int,
+    },
+    total=False,
+)
+
+class BatchStartViewerSessionRevocationViewerSessionTypeDef(
+    _RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef,
+    _OptionalBatchStartViewerSessionRevocationViewerSessionTypeDef,
+):
+    pass
+
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "arn": str,
         "authorized": bool,
+        "insecureIngest": bool,
         "latencyMode": ChannelLatencyModeType,
         "name": str,
+        "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
+        "type": ChannelTypeType,
     },
     total=False,
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "authorized": bool,
+        "insecureIngest": bool,
         "latencyMode": ChannelLatencyModeType,
         "name": str,
+        "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Mapping[str, str],
         "type": ChannelTypeType,
     },
     total=False,
 )
 
@@ -267,14 +312,21 @@
 S3DestinationConfigurationTypeDef = TypedDict(
     "S3DestinationConfigurationTypeDef",
     {
         "bucketName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetChannelRequestRequestTypeDef = TypedDict(
     "GetChannelRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -382,20 +434,20 @@
         "targetFramerate": int,
         "videoHeight": int,
         "videoWidth": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "filterByName": str,
+        "filterByRecordingConfigurationArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
@@ -403,14 +455,22 @@
         "filterByRecordingConfigurationArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = TypedDict(
+    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPlaybackKeyPairsRequestRequestTypeDef = TypedDict(
     "ListPlaybackKeyPairsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -422,23 +482,51 @@
         "arn": str,
         "name": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = TypedDict(
+    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRecordingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListRecordingConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
+    "_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef",
+    {
+        "channelArn": str,
+    },
+)
+_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
+    "_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStreamKeysRequestListStreamKeysPaginateTypeDef(
+    _RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef,
+    _OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef,
+):
+    pass
+
 _RequiredListStreamKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamKeysRequestRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 _OptionalListStreamKeysRequestRequestTypeDef = TypedDict(
@@ -521,22 +609,72 @@
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
 PutMetadataRequestRequestTypeDef = TypedDict(
     "PutMetadataRequestRequestTypeDef",
     {
         "channelArn": str,
         "metadata": str,
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
+_RequiredStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartViewerSessionRevocationRequestRequestTypeDef",
+    {
+        "channelArn": str,
+        "viewerId": str,
+    },
+)
+_OptionalStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartViewerSessionRevocationRequestRequestTypeDef",
+    {
+        "viewerSessionVersionsLessThanOrEqualTo": int,
+    },
+    total=False,
+)
+
+class StartViewerSessionRevocationRequestRequestTypeDef(
+    _RequiredStartViewerSessionRevocationRequestRequestTypeDef,
+    _OptionalStartViewerSessionRevocationRequestRequestTypeDef,
+):
+    pass
+
 StopStreamRequestRequestTypeDef = TypedDict(
     "StopStreamRequestRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 
@@ -572,16 +710,18 @@
         "arn": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "authorized": bool,
+        "insecureIngest": bool,
         "latencyMode": ChannelLatencyModeType,
         "name": str,
+        "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "type": ChannelTypeType,
     },
     total=False,
 )
 
 class UpdateChannelRequestRequestTypeDef(
@@ -590,89 +730,89 @@
     pass
 
 BatchGetChannelResponseTypeDef = TypedDict(
     "BatchGetChannelResponseTypeDef",
     {
         "channels": List[ChannelTypeDef],
         "errors": List[BatchErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetStreamKeyResponseTypeDef = TypedDict(
     "BatchGetStreamKeyResponseTypeDef",
     {
         "errors": List[BatchErrorTypeDef],
         "streamKeys": List[StreamKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStreamKeyResponseTypeDef = TypedDict(
     "CreateStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStreamKeyResponseTypeDef = TypedDict(
     "GetStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchStartViewerSessionRevocationResponseTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationResponseTypeDef",
+    {
+        "errors": List[BatchStartViewerSessionRevocationErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationRequestRequestTypeDef",
+    {
+        "viewerSessions": Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef],
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "s3": S3DestinationConfigurationTypeDef,
@@ -680,121 +820,75 @@
     total=False,
 )
 
 GetPlaybackKeyPairResponseTypeDef = TypedDict(
     "GetPlaybackKeyPairResponseTypeDef",
     {
         "keyPair": PlaybackKeyPairTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportPlaybackKeyPairResponseTypeDef = TypedDict(
     "ImportPlaybackKeyPairResponseTypeDef",
     {
         "keyPair": PlaybackKeyPairTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStreamResponseTypeDef = TypedDict(
     "GetStreamResponseTypeDef",
     {
         "stream": StreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IngestConfigurationTypeDef = TypedDict(
     "IngestConfigurationTypeDef",
     {
         "audio": AudioConfigurationTypeDef,
         "video": VideoConfigurationTypeDef,
     },
     total=False,
 )
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "filterByName": str,
-        "filterByRecordingConfigurationArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = TypedDict(
-    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = TypedDict(
-    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
-    "_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef",
-    {
-        "channelArn": str,
-    },
-)
-_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
-    "_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListStreamKeysRequestListStreamKeysPaginateTypeDef(
-    _RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef,
-    _OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef,
-):
-    pass
-
 ListPlaybackKeyPairsResponseTypeDef = TypedDict(
     "ListPlaybackKeyPairsResponseTypeDef",
     {
         "keyPairs": List[PlaybackKeyPairSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamKeysResponseTypeDef = TypedDict(
     "ListStreamKeysResponseTypeDef",
     {
         "nextToken": str,
         "streamKeys": List[StreamKeySummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamSessionsResponseTypeDef = TypedDict(
     "ListStreamSessionsResponseTypeDef",
     {
         "nextToken": str,
         "streamSessions": List[StreamSessionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsRequestListStreamsPaginateTypeDef",
     {
         "filterBy": StreamFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListStreamsRequestRequestTypeDef = TypedDict(
     "ListStreamsRequestRequestTypeDef",
     {
@@ -806,15 +900,15 @@
 )
 
 ListStreamsResponseTypeDef = TypedDict(
     "ListStreamsResponseTypeDef",
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
     {
         "destinationConfiguration": DestinationConfigurationTypeDef,
@@ -884,31 +978,31 @@
     pass
 
 ListRecordingConfigurationsResponseTypeDef = TypedDict(
     "ListRecordingConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "recordingConfigurations": List[RecordingConfigurationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRecordingConfigurationResponseTypeDef = TypedDict(
     "CreateRecordingConfigurationResponseTypeDef",
     {
         "recordingConfiguration": RecordingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecordingConfigurationResponseTypeDef = TypedDict(
     "GetRecordingConfigurationResponseTypeDef",
     {
         "recordingConfiguration": RecordingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StreamSessionTypeDef = TypedDict(
     "StreamSessionTypeDef",
     {
         "channel": ChannelTypeDef,
@@ -922,10 +1016,10 @@
     total=False,
 )
 
 GetStreamSessionResponseTypeDef = TypedDict(
     "GetStreamSessionResponseTypeDef",
     {
         "streamSession": StreamSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/PKG-INFO` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.26.85
-Summary: Type annotations for boto3.IVS 1.26.85 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.IVS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ivs"></a>
 
 # mypy-boto3-ivs
 
 [![PyPI - mypy-boto3-ivs](https://img.shields.io/pypi/v/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.26.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,14 +320,15 @@
     ListRecordingConfigurationsPaginatorName,
     ListStreamKeysPaginatorName,
     ListStreamsPaginatorName,
     RecordingConfigurationStateType,
     RecordingModeType,
     StreamHealthType,
     StreamStateType,
+    TranscodePresetType,
     IVSServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -345,73 +346,78 @@
 
 ```python
 from mypy_boto3_ivs.type_defs import (
     AudioConfigurationTypeDef,
     BatchErrorTypeDef,
     BatchGetChannelRequestRequestTypeDef,
     ChannelTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetStreamKeyRequestRequestTypeDef,
     StreamKeyTypeDef,
+    BatchStartViewerSessionRevocationErrorTypeDef,
+    BatchStartViewerSessionRevocationViewerSessionTypeDef,
     ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
     ThumbnailConfigurationTypeDef,
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
     S3DestinationConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
     StreamTypeDef,
     GetStreamSessionRequestRequestTypeDef,
     ImportPlaybackKeyPairRequestRequestTypeDef,
     VideoConfigurationTypeDef,
-    PaginatorConfigTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
     ListPlaybackKeyPairsRequestRequestTypeDef,
     PlaybackKeyPairSummaryTypeDef,
+    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
     ListRecordingConfigurationsRequestRequestTypeDef,
+    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListStreamKeysRequestRequestTypeDef,
     StreamKeySummaryTypeDef,
     ListStreamSessionsRequestRequestTypeDef,
     StreamSessionSummaryTypeDef,
     StreamFiltersTypeDef,
     StreamSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutMetadataRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    StartViewerSessionRevocationRequestRequestTypeDef,
     StopStreamRequestRequestTypeDef,
     StreamEventTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     BatchGetChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdateChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
+    BatchStartViewerSessionRevocationResponseTypeDef,
+    BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
-    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
-    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
     CreateRecordingConfigurationRequestRequestTypeDef,
@@ -432,42 +438,42 @@
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

### Comparing `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/SOURCES.txt` & `mypy-boto3-ivs-1.27.0/mypy_boto3_ivs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.85/setup.py` & `mypy-boto3-ivs-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-ivs.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivs",
-    version="1.26.85",
+    version="1.27.0",
     packages=["mypy_boto3_ivs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IVS 1.26.85 service generated with mypy-boto3-builder 7.12.5"
+        "Type annotations for boto3.IVS 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/",
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


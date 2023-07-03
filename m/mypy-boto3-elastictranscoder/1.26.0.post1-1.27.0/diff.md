# Comparing `tmp/mypy-boto3-elastictranscoder-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-elastictranscoder-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elastictranscoder-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:24 2022, max compression
+gzip compressed data, was "mypy-boto3-elastictranscoder-1.27.0.tar", last modified: Mon Jul  3 19:50:43 2023, max compression
```

## Comparing `mypy-boto3-elastictranscoder-1.26.0.post1.tar` & `mypy-boto3-elastictranscoder-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:24.352827 mypy-boto3-elastictranscoder-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16450 2022-11-01 21:43:24.352827 mypy-boto3-elastictranscoder-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14969 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:24.352827 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17037 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    17008 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7718 2022-11-01 21:34:21.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7716 2022-11-01 21:34:21.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5364 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5358 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    22835 2022-11-01 21:34:21.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    22816 2022-11-01 21:34:21.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:24.352827 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16450 2022-11-01 21:43:24.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-11-01 21:43:24.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:24.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:24.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:24.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-01 21:43:24.000000 mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:24.352827 mypy-boto3-elastictranscoder-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-11-01 21:34:20.000000 mypy-boto3-elastictranscoder-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.507197 mypy-boto3-elastictranscoder-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16482 2023-07-03 19:50:43.507197 mypy-boto3-elastictranscoder-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.507197 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22871 2023-07-03 19:37:21.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22852 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.507197 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16482 2023-07-03 19:50:43.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-03 19:50:43.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:43.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:43.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:43.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:50:43.000000 mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:43.507197 mypy-boto3-elastictranscoder-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-03 19:37:20.000000 mypy-boto3-elastictranscoder-1.27.0/setup.py
```

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/LICENSE` & `mypy-boto3-elastictranscoder-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/PKG-INFO` & `mypy-boto3-elastictranscoder-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastictranscoder
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ElasticTranscoder 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ElasticTranscoder 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/
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
 
 <a id="mypy-boto3-elastictranscoder"></a>
 
 # mypy-boto3-elastictranscoder
 
 [![PyPI - mypy-boto3-elastictranscoder](https://img.shields.io/pypi/v/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elastictranscoder?color=blue)](https://pypistats.org/packages/mypy-boto3-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticTranscoder 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[boto3.ElasticTranscoder 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [mypy-boto3-elastictranscoder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,49 +364,49 @@
 from mypy_boto3_elastictranscoder.type_defs import (
     EncryptionTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
     TimeSpanTypeDef,
     HlsContentProtectionTypeDef,
     PlayReadyDrmTypeDef,
-    ResponseMetadataTypeDef,
     NotificationsTypeDef,
     WarningTypeDef,
     ThumbnailsTypeDef,
     DeletePipelineRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DetectedPropertiesTypeDef,
     TimingTypeDef,
-    PaginatorConfigTypeDef,
+    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
     ListJobsByPipelineRequestRequestTypeDef,
+    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
     ListJobsByStatusRequestRequestTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PermissionTypeDef,
     PresetWatermarkTypeDef,
     WaiterConfigTypeDef,
     ReadJobRequestRequestTypeDef,
     ReadPipelineRequestRequestTypeDef,
     ReadPresetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TestRoleRequestRequestTypeDef,
+    TestRoleResponseTypeDef,
     UpdatePipelineStatusRequestRequestTypeDef,
     ArtworkTypeDef,
     CaptionFormatTypeDef,
     CaptionSourceTypeDef,
     JobWatermarkTypeDef,
     AudioParametersTypeDef,
     ClipTypeDef,
     CreateJobPlaylistTypeDef,
     PlaylistTypeDef,
-    TestRoleResponseTypeDef,
     UpdatePipelineNotificationsRequestRequestTypeDef,
-    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     PipelineOutputConfigTypeDef,
     VideoParametersTypeDef,
     ReadJobRequestJobCompleteWaitTypeDef,
     JobAlbumArtTypeDef,
     CaptionsTypeDef,
     InputCaptionsTypeDef,
     CreatePipelineRequestRequestTypeDef,
@@ -441,42 +442,42 @@
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

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/README.md` & `mypy-boto3-elastictranscoder-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-elastictranscoder"></a>
 
 # mypy-boto3-elastictranscoder
 
 [![PyPI - mypy-boto3-elastictranscoder](https://img.shields.io/pypi/v/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elastictranscoder?color=blue)](https://pypistats.org/packages/mypy-boto3-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticTranscoder 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[boto3.ElasticTranscoder 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [mypy-boto3-elastictranscoder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,49 +332,49 @@
 from mypy_boto3_elastictranscoder.type_defs import (
     EncryptionTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
     TimeSpanTypeDef,
     HlsContentProtectionTypeDef,
     PlayReadyDrmTypeDef,
-    ResponseMetadataTypeDef,
     NotificationsTypeDef,
     WarningTypeDef,
     ThumbnailsTypeDef,
     DeletePipelineRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DetectedPropertiesTypeDef,
     TimingTypeDef,
-    PaginatorConfigTypeDef,
+    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
     ListJobsByPipelineRequestRequestTypeDef,
+    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
     ListJobsByStatusRequestRequestTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PermissionTypeDef,
     PresetWatermarkTypeDef,
     WaiterConfigTypeDef,
     ReadJobRequestRequestTypeDef,
     ReadPipelineRequestRequestTypeDef,
     ReadPresetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TestRoleRequestRequestTypeDef,
+    TestRoleResponseTypeDef,
     UpdatePipelineStatusRequestRequestTypeDef,
     ArtworkTypeDef,
     CaptionFormatTypeDef,
     CaptionSourceTypeDef,
     JobWatermarkTypeDef,
     AudioParametersTypeDef,
     ClipTypeDef,
     CreateJobPlaylistTypeDef,
     PlaylistTypeDef,
-    TestRoleResponseTypeDef,
     UpdatePipelineNotificationsRequestRequestTypeDef,
-    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     PipelineOutputConfigTypeDef,
     VideoParametersTypeDef,
     ReadJobRequestJobCompleteWaitTypeDef,
     JobAlbumArtTypeDef,
     CaptionsTypeDef,
     InputCaptionsTypeDef,
     CreatePipelineRequestRequestTypeDef,
@@ -410,42 +410,42 @@
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

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/__init__.py` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/__init__.pyi` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/__main__.py` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticTranscoder 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.ElasticTranscoder 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder\nOther"
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

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/client.py` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/client.pyi` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/literals.py` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,23 +51,25 @@
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
@@ -77,30 +79,35 @@
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
@@ -126,14 +133,15 @@
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
@@ -178,51 +186,57 @@
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
@@ -235,14 +249,15 @@
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
@@ -254,28 +269,35 @@
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
@@ -284,14 +306,15 @@
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
@@ -302,55 +325,64 @@
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

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/literals.pyi` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -49,23 +49,25 @@
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
@@ -75,30 +77,35 @@
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
@@ -124,14 +131,15 @@
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
@@ -176,51 +184,57 @@
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
@@ -233,14 +247,15 @@
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
@@ -252,28 +267,35 @@
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
@@ -282,14 +304,15 @@
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
@@ -300,55 +323,64 @@
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

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/paginator.py` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -40,80 +40,74 @@
 __all__ = (
     "ListJobsByPipelinePaginator",
     "ListJobsByStatusPaginator",
     "ListPipelinesPaginator",
     "ListPresetsPaginator",
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
 class ListJobsByPipelinePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbypipelinepaginator)
     """
 
     def paginate(
         self,
         *,
         PipelineId: str,
         Ascending: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsByPipelineResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbypipelinepaginator)
         """
 
-
 class ListJobsByStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbystatuspaginator)
     """
 
     def paginate(
-        self, *, Status: str, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Status: str, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsByStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbystatuspaginator)
         """
 
-
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpipelinespaginator)
         """
 
-
 class ListPresetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpresetspaginator)
     """
 
     def paginate(
-        self, *, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpresetspaginator)
         """
```

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/paginator.pyi` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,74 +40,80 @@
 __all__ = (
     "ListJobsByPipelinePaginator",
     "ListJobsByStatusPaginator",
     "ListPipelinesPaginator",
     "ListPresetsPaginator",
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
 class ListJobsByPipelinePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbypipelinepaginator)
     """
 
     def paginate(
         self,
         *,
         PipelineId: str,
         Ascending: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsByPipelineResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbypipelinepaginator)
         """
 
+
 class ListJobsByStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbystatuspaginator)
     """
 
     def paginate(
-        self, *, Status: str, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Status: str, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsByStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listjobsbystatuspaginator)
         """
 
+
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpipelinespaginator)
         """
 
+
 class ListPresetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpresetspaginator)
     """
 
     def paginate(
-        self, *, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/paginators/#listpresetspaginator)
         """
```

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/type_defs.py` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,49 +23,49 @@
 __all__ = (
     "EncryptionTypeDef",
     "AudioCodecOptionsTypeDef",
     "CancelJobRequestRequestTypeDef",
     "TimeSpanTypeDef",
     "HlsContentProtectionTypeDef",
     "PlayReadyDrmTypeDef",
-    "ResponseMetadataTypeDef",
     "NotificationsTypeDef",
     "WarningTypeDef",
     "ThumbnailsTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DetectedPropertiesTypeDef",
     "TimingTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
     "ListJobsByPipelineRequestRequestTypeDef",
+    "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
     "ListJobsByStatusRequestRequestTypeDef",
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PermissionTypeDef",
     "PresetWatermarkTypeDef",
     "WaiterConfigTypeDef",
     "ReadJobRequestRequestTypeDef",
     "ReadPipelineRequestRequestTypeDef",
     "ReadPresetRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TestRoleRequestRequestTypeDef",
+    "TestRoleResponseTypeDef",
     "UpdatePipelineStatusRequestRequestTypeDef",
     "ArtworkTypeDef",
     "CaptionFormatTypeDef",
     "CaptionSourceTypeDef",
     "JobWatermarkTypeDef",
     "AudioParametersTypeDef",
     "ClipTypeDef",
     "CreateJobPlaylistTypeDef",
     "PlaylistTypeDef",
-    "TestRoleResponseTypeDef",
     "UpdatePipelineNotificationsRequestRequestTypeDef",
-    "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
-    "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
     "PipelineOutputConfigTypeDef",
     "VideoParametersTypeDef",
     "ReadJobRequestJobCompleteWaitTypeDef",
     "JobAlbumArtTypeDef",
     "CaptionsTypeDef",
     "InputCaptionsTypeDef",
     "CreatePipelineRequestRequestTypeDef",
@@ -153,25 +153,14 @@
         "KeyId": str,
         "InitializationVector": str,
         "LicenseAcquisitionUrl": str,
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
 NotificationsTypeDef = TypedDict(
     "NotificationsTypeDef",
     {
         "Progressing": str,
         "Completed": str,
         "Warning": str,
         "Error": str,
@@ -235,24 +224,37 @@
         "SubmitTimeMillis": int,
         "StartTimeMillis": int,
         "FinishTimeMillis": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
+    "_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PipelineId": str,
+    },
+)
+_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
+    "_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(
+    _RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    _OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListJobsByPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsByPipelineRequestRequestTypeDef",
     {
         "PipelineId": str,
     },
 )
 _OptionalListJobsByPipelineRequestRequestTypeDef = TypedDict(
@@ -268,14 +270,37 @@
 class ListJobsByPipelineRequestRequestTypeDef(
     _RequiredListJobsByPipelineRequestRequestTypeDef,
     _OptionalListJobsByPipelineRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
+    "_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    {
+        "Status": str,
+    },
+)
+_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
+    "_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(
+    _RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+    _OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListJobsByStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsByStatusRequestRequestTypeDef",
     {
         "Status": str,
     },
 )
 _OptionalListJobsByStatusRequestRequestTypeDef = TypedDict(
@@ -290,32 +315,60 @@
 
 class ListJobsByStatusRequestRequestTypeDef(
     _RequiredListJobsByStatusRequestRequestTypeDef, _OptionalListJobsByStatusRequestRequestTypeDef
 ):
     pass
 
 
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPipelinesRequestRequestTypeDef = TypedDict(
     "ListPipelinesRequestRequestTypeDef",
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Ascending": str,
         "PageToken": str,
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
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "GranteeType": str,
         "Grantee": str,
         "Access": Sequence[str],
     },
@@ -365,24 +418,44 @@
 ReadPresetRequestRequestTypeDef = TypedDict(
     "ReadPresetRequestRequestTypeDef",
     {
         "Id": str,
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
 TestRoleRequestRequestTypeDef = TypedDict(
     "TestRoleRequestRequestTypeDef",
     {
         "Role": str,
         "InputBucket": str,
         "OutputBucket": str,
         "Topics": Sequence[str],
     },
 )
 
+TestRoleResponseTypeDef = TypedDict(
+    "TestRoleResponseTypeDef",
+    {
+        "Success": str,
+        "Messages": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdatePipelineStatusRequestRequestTypeDef = TypedDict(
     "UpdatePipelineStatusRequestRequestTypeDef",
     {
         "Id": str,
         "Status": str,
     },
 )
@@ -476,95 +549,22 @@
         "PlayReadyDrm": PlayReadyDrmTypeDef,
         "Status": str,
         "StatusDetail": str,
     },
     total=False,
 )
 
-TestRoleResponseTypeDef = TypedDict(
-    "TestRoleResponseTypeDef",
-    {
-        "Success": str,
-        "Messages": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdatePipelineNotificationsRequestRequestTypeDef = TypedDict(
     "UpdatePipelineNotificationsRequestRequestTypeDef",
     {
         "Id": str,
         "Notifications": NotificationsTypeDef,
     },
 )
 
-_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
-    "_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
-    {
-        "PipelineId": str,
-    },
-)
-_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
-    "_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(
-    _RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-    _OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-):
-    pass
-
-
-_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
-    "_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    {
-        "Status": str,
-    },
-)
-_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
-    "_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(
-    _RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-    _OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-):
-    pass
-
-
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 PipelineOutputConfigTypeDef = TypedDict(
     "PipelineOutputConfigTypeDef",
     {
         "Bucket": str,
         "StorageClass": str,
         "Permissions": Sequence[PermissionTypeDef],
     },
@@ -819,84 +819,84 @@
 )
 
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "Pipelines": List[PipelineTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReadPipelineResponseTypeDef = TypedDict(
     "ReadPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePipelineNotificationsResponseTypeDef = TypedDict(
     "UpdatePipelineNotificationsResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePipelineResponseTypeDef = TypedDict(
     "UpdatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePipelineStatusResponseTypeDef = TypedDict(
     "UpdatePipelineStatusResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "Warning": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPresetsResponseTypeDef = TypedDict(
     "ListPresetsResponseTypeDef",
     {
         "Presets": List[PresetTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReadPresetResponseTypeDef = TypedDict(
     "ReadPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "PipelineId": str,
@@ -942,36 +942,36 @@
     total=False,
 )
 
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsByPipelineResponseTypeDef = TypedDict(
     "ListJobsByPipelineResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsByStatusResponseTypeDef = TypedDict(
     "ListJobsByStatusResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReadJobResponseTypeDef = TypedDict(
     "ReadJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/type_defs.pyi` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,49 +22,49 @@
 __all__ = (
     "EncryptionTypeDef",
     "AudioCodecOptionsTypeDef",
     "CancelJobRequestRequestTypeDef",
     "TimeSpanTypeDef",
     "HlsContentProtectionTypeDef",
     "PlayReadyDrmTypeDef",
-    "ResponseMetadataTypeDef",
     "NotificationsTypeDef",
     "WarningTypeDef",
     "ThumbnailsTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DetectedPropertiesTypeDef",
     "TimingTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
     "ListJobsByPipelineRequestRequestTypeDef",
+    "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
     "ListJobsByStatusRequestRequestTypeDef",
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PermissionTypeDef",
     "PresetWatermarkTypeDef",
     "WaiterConfigTypeDef",
     "ReadJobRequestRequestTypeDef",
     "ReadPipelineRequestRequestTypeDef",
     "ReadPresetRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TestRoleRequestRequestTypeDef",
+    "TestRoleResponseTypeDef",
     "UpdatePipelineStatusRequestRequestTypeDef",
     "ArtworkTypeDef",
     "CaptionFormatTypeDef",
     "CaptionSourceTypeDef",
     "JobWatermarkTypeDef",
     "AudioParametersTypeDef",
     "ClipTypeDef",
     "CreateJobPlaylistTypeDef",
     "PlaylistTypeDef",
-    "TestRoleResponseTypeDef",
     "UpdatePipelineNotificationsRequestRequestTypeDef",
-    "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
-    "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
     "PipelineOutputConfigTypeDef",
     "VideoParametersTypeDef",
     "ReadJobRequestJobCompleteWaitTypeDef",
     "JobAlbumArtTypeDef",
     "CaptionsTypeDef",
     "InputCaptionsTypeDef",
     "CreatePipelineRequestRequestTypeDef",
@@ -152,25 +152,14 @@
         "KeyId": str,
         "InitializationVector": str,
         "LicenseAcquisitionUrl": str,
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
 NotificationsTypeDef = TypedDict(
     "NotificationsTypeDef",
     {
         "Progressing": str,
         "Completed": str,
         "Warning": str,
         "Error": str,
@@ -234,24 +223,35 @@
         "SubmitTimeMillis": int,
         "StartTimeMillis": int,
         "FinishTimeMillis": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
+    "_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PipelineId": str,
+    },
+)
+_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
+    "_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(
+    _RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    _OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+):
+    pass
+
 _RequiredListJobsByPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsByPipelineRequestRequestTypeDef",
     {
         "PipelineId": str,
     },
 )
 _OptionalListJobsByPipelineRequestRequestTypeDef = TypedDict(
@@ -265,14 +265,35 @@
 
 class ListJobsByPipelineRequestRequestTypeDef(
     _RequiredListJobsByPipelineRequestRequestTypeDef,
     _OptionalListJobsByPipelineRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
+    "_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    {
+        "Status": str,
+    },
+)
+_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
+    "_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(
+    _RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+    _OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+):
+    pass
+
 _RequiredListJobsByStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsByStatusRequestRequestTypeDef",
     {
         "Status": str,
     },
 )
 _OptionalListJobsByStatusRequestRequestTypeDef = TypedDict(
@@ -285,32 +306,60 @@
 )
 
 class ListJobsByStatusRequestRequestTypeDef(
     _RequiredListJobsByStatusRequestRequestTypeDef, _OptionalListJobsByStatusRequestRequestTypeDef
 ):
     pass
 
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPipelinesRequestRequestTypeDef = TypedDict(
     "ListPipelinesRequestRequestTypeDef",
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Ascending": str,
         "PageToken": str,
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
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "GranteeType": str,
         "Grantee": str,
         "Access": Sequence[str],
     },
@@ -360,24 +409,44 @@
 ReadPresetRequestRequestTypeDef = TypedDict(
     "ReadPresetRequestRequestTypeDef",
     {
         "Id": str,
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
 TestRoleRequestRequestTypeDef = TypedDict(
     "TestRoleRequestRequestTypeDef",
     {
         "Role": str,
         "InputBucket": str,
         "OutputBucket": str,
         "Topics": Sequence[str],
     },
 )
 
+TestRoleResponseTypeDef = TypedDict(
+    "TestRoleResponseTypeDef",
+    {
+        "Success": str,
+        "Messages": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdatePipelineStatusRequestRequestTypeDef = TypedDict(
     "UpdatePipelineStatusRequestRequestTypeDef",
     {
         "Id": str,
         "Status": str,
     },
 )
@@ -471,91 +540,22 @@
         "PlayReadyDrm": PlayReadyDrmTypeDef,
         "Status": str,
         "StatusDetail": str,
     },
     total=False,
 )
 
-TestRoleResponseTypeDef = TypedDict(
-    "TestRoleResponseTypeDef",
-    {
-        "Success": str,
-        "Messages": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdatePipelineNotificationsRequestRequestTypeDef = TypedDict(
     "UpdatePipelineNotificationsRequestRequestTypeDef",
     {
         "Id": str,
         "Notifications": NotificationsTypeDef,
     },
 )
 
-_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
-    "_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
-    {
-        "PipelineId": str,
-    },
-)
-_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
-    "_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(
-    _RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-    _OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-):
-    pass
-
-_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
-    "_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    {
-        "Status": str,
-    },
-)
-_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
-    "_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(
-    _RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-    _OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-):
-    pass
-
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 PipelineOutputConfigTypeDef = TypedDict(
     "PipelineOutputConfigTypeDef",
     {
         "Bucket": str,
         "StorageClass": str,
         "Permissions": Sequence[PermissionTypeDef],
     },
@@ -802,84 +802,84 @@
 )
 
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "Pipelines": List[PipelineTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReadPipelineResponseTypeDef = TypedDict(
     "ReadPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePipelineNotificationsResponseTypeDef = TypedDict(
     "UpdatePipelineNotificationsResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePipelineResponseTypeDef = TypedDict(
     "UpdatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePipelineStatusResponseTypeDef = TypedDict(
     "UpdatePipelineStatusResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "Warning": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPresetsResponseTypeDef = TypedDict(
     "ListPresetsResponseTypeDef",
     {
         "Presets": List[PresetTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReadPresetResponseTypeDef = TypedDict(
     "ReadPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "PipelineId": str,
@@ -923,36 +923,36 @@
     total=False,
 )
 
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsByPipelineResponseTypeDef = TypedDict(
     "ListJobsByPipelineResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsByStatusResponseTypeDef = TypedDict(
     "ListJobsByStatusResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReadJobResponseTypeDef = TypedDict(
     "ReadJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/waiter.py` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder/waiter.pyi` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder.egg-info/PKG-INFO` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastictranscoder
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ElasticTranscoder 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ElasticTranscoder 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/
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
 
 <a id="mypy-boto3-elastictranscoder"></a>
 
 # mypy-boto3-elastictranscoder
 
 [![PyPI - mypy-boto3-elastictranscoder](https://img.shields.io/pypi/v/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elastictranscoder?color=blue)](https://pypistats.org/packages/mypy-boto3-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticTranscoder 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[boto3.ElasticTranscoder 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [mypy-boto3-elastictranscoder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,49 +364,49 @@
 from mypy_boto3_elastictranscoder.type_defs import (
     EncryptionTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
     TimeSpanTypeDef,
     HlsContentProtectionTypeDef,
     PlayReadyDrmTypeDef,
-    ResponseMetadataTypeDef,
     NotificationsTypeDef,
     WarningTypeDef,
     ThumbnailsTypeDef,
     DeletePipelineRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DetectedPropertiesTypeDef,
     TimingTypeDef,
-    PaginatorConfigTypeDef,
+    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
     ListJobsByPipelineRequestRequestTypeDef,
+    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
     ListJobsByStatusRequestRequestTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PermissionTypeDef,
     PresetWatermarkTypeDef,
     WaiterConfigTypeDef,
     ReadJobRequestRequestTypeDef,
     ReadPipelineRequestRequestTypeDef,
     ReadPresetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TestRoleRequestRequestTypeDef,
+    TestRoleResponseTypeDef,
     UpdatePipelineStatusRequestRequestTypeDef,
     ArtworkTypeDef,
     CaptionFormatTypeDef,
     CaptionSourceTypeDef,
     JobWatermarkTypeDef,
     AudioParametersTypeDef,
     ClipTypeDef,
     CreateJobPlaylistTypeDef,
     PlaylistTypeDef,
-    TestRoleResponseTypeDef,
     UpdatePipelineNotificationsRequestRequestTypeDef,
-    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     PipelineOutputConfigTypeDef,
     VideoParametersTypeDef,
     ReadJobRequestJobCompleteWaitTypeDef,
     JobAlbumArtTypeDef,
     CaptionsTypeDef,
     InputCaptionsTypeDef,
     CreatePipelineRequestRequestTypeDef,
@@ -441,42 +442,42 @@
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

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt` & `mypy-boto3-elastictranscoder-1.27.0/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.26.0.post1/setup.py` & `mypy-boto3-elastictranscoder-1.27.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-elastictranscoder.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elastictranscoder",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_elastictranscoder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticTranscoder 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.ElasticTranscoder 1.27.0 service generated with"
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
     keywords="boto3 elastictranscoder type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_elastictranscoder": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_elastictranscoder": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/",
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


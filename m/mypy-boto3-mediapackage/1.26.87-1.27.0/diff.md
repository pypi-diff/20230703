# Comparing `tmp/mypy-boto3-mediapackage-1.26.87.tar.gz` & `tmp/mypy-boto3-mediapackage-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackage-1.26.87.tar", last modified: Wed Mar  8 20:35:46 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackage-1.27.0.tar", last modified: Mon Jul  3 19:51:06 2023, max compression
```

## Comparing `mypy-boto3-mediapackage-1.26.87.tar` & `mypy-boto3-mediapackage-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.202592 mypy-boto3-mediapackage-1.26.87/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-03-08 20:35:46.202592 mypy-boto3-mediapackage-1.26.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.198592 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25727 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25704 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-08 20:35:11.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.202592 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-03-08 20:35:46.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-08 20:35:46.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 20:35:46.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 20:35:46.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-08 20:35:46.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-08 20:35:46.000000 mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 20:35:46.202592 mypy-boto3-mediapackage-1.26.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-08 20:35:10.000000 mypy-boto3-mediapackage-1.26.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.255644 mypy-boto3-mediapackage-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-07-03 19:51:06.255644 mypy-boto3-mediapackage-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.251644 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25765 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25742 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.255644 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:06.255644 mypy-boto3-mediapackage-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/setup.py
```

### Comparing `mypy-boto3-mediapackage-1.26.87/LICENSE` & `mypy-boto3-mediapackage-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-mediapackage-1.26.87/PKG-INFO` & `mypy-boto3-mediapackage-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage
-Version: 1.26.87
-Summary: Type annotations for boto3.MediaPackage 1.26.87 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.MediaPackage 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-mediapackage"></a>
 
 # mypy-boto3-mediapackage
 
 [![PyPI - mypy-boto3-mediapackage](https://img.shields.io/pypi/v/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -351,46 +351,46 @@
 from mypy_boto3_mediapackage.type_defs import (
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
     IngressAccessLogsTypeDef,
     HlsManifestCreateOrUpdateParametersTypeDef,
     StreamSelectionTypeDef,
     HlsManifestTypeDef,
-    ResponseMetadataTypeDef,
     CreateChannelRequestRequestTypeDef,
     S3DestinationTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeHarvestJobRequestRequestTypeDef,
     DescribeOriginEndpointRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionContractConfigurationTypeDef,
     IngestEndpointTypeDef,
-    PaginatorConfigTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
     ListHarvestJobsRequestRequestTypeDef,
+    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RotateChannelCredentialsRequestRequestTypeDef,
     RotateIngestEndpointCredentialsRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateHarvestJobRequestRequestTypeDef,
     CreateHarvestJobResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     HarvestJobTypeDef,
     SpekeKeyProviderTypeDef,
     HlsIngestTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListHarvestJobsResponseTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
     HlsEncryptionTypeDef,
     MssEncryptionTypeDef,
     ChannelTypeDef,
     ConfigureLogsResponseTypeDef,
@@ -422,42 +422,42 @@
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

### Comparing `mypy-boto3-mediapackage-1.26.87/README.md` & `mypy-boto3-mediapackage-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mediapackage"></a>
 
 # mypy-boto3-mediapackage
 
 [![PyPI - mypy-boto3-mediapackage](https://img.shields.io/pypi/v/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,46 +319,46 @@
 from mypy_boto3_mediapackage.type_defs import (
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
     IngressAccessLogsTypeDef,
     HlsManifestCreateOrUpdateParametersTypeDef,
     StreamSelectionTypeDef,
     HlsManifestTypeDef,
-    ResponseMetadataTypeDef,
     CreateChannelRequestRequestTypeDef,
     S3DestinationTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeHarvestJobRequestRequestTypeDef,
     DescribeOriginEndpointRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionContractConfigurationTypeDef,
     IngestEndpointTypeDef,
-    PaginatorConfigTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
     ListHarvestJobsRequestRequestTypeDef,
+    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RotateChannelCredentialsRequestRequestTypeDef,
     RotateIngestEndpointCredentialsRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateHarvestJobRequestRequestTypeDef,
     CreateHarvestJobResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     HarvestJobTypeDef,
     SpekeKeyProviderTypeDef,
     HlsIngestTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListHarvestJobsResponseTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
     HlsEncryptionTypeDef,
     MssEncryptionTypeDef,
     ChannelTypeDef,
     ConfigureLogsResponseTypeDef,
@@ -390,42 +390,42 @@
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

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/__init__.py` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/__init__.pyi` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/__main__.py` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaPackage 1.26.87\nVersion:         1.26.87\nBuilder"
-        " version: 7.12.5\nDocs:           "
+        "Type annotations for boto3.MediaPackage 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.87")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/client.py` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/client.pyi` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/literals.py` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AdMarkersType",
     "AdTriggersElementType",
     "AdsOnDeliveryRestrictionsType",
     "CmafEncryptionMethodType",
     "EncryptionMethodType",
     "ListChannelsPaginatorName",
@@ -42,15 +41,14 @@
     "MediaPackageServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdMarkersType = Literal["DATERANGE", "NONE", "PASSTHROUGH", "SCTE35_ENHANCED"]
 AdTriggersElementType = Literal[
     "BREAK",
     "DISTRIBUTOR_ADVERTISEMENT",
     "DISTRIBUTOR_OVERLAY_PLACEMENT_OPPORTUNITY",
     "DISTRIBUTOR_PLACEMENT_OPPORTUNITY",
     "PROVIDER_ADVERTISEMENT",
@@ -102,14 +100,15 @@
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
@@ -149,14 +148,15 @@
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
@@ -254,14 +254,15 @@
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
@@ -297,14 +298,15 @@
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
@@ -323,16 +325,19 @@
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
@@ -416,15 +421,17 @@
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

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/literals.pyi` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AdMarkersType",
     "AdTriggersElementType",
     "AdsOnDeliveryRestrictionsType",
     "CmafEncryptionMethodType",
     "EncryptionMethodType",
     "ListChannelsPaginatorName",
@@ -41,14 +42,15 @@
     "MediaPackageServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AdMarkersType = Literal["DATERANGE", "NONE", "PASSTHROUGH", "SCTE35_ENHANCED"]
 AdTriggersElementType = Literal[
     "BREAK",
     "DISTRIBUTOR_ADVERTISEMENT",
     "DISTRIBUTOR_OVERLAY_PLACEMENT_OPPORTUNITY",
     "DISTRIBUTOR_PLACEMENT_OPPORTUNITY",
     "PROVIDER_ADVERTISEMENT",
@@ -100,14 +102,15 @@
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
@@ -147,14 +150,15 @@
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
@@ -252,14 +256,15 @@
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
@@ -295,14 +300,15 @@
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
@@ -321,16 +327,19 @@
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
@@ -414,15 +423,17 @@
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

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/paginator.py` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listchannelspaginator)
         """
 
 
@@ -69,28 +69,28 @@
     """
 
     def paginate(
         self,
         *,
         IncludeChannelId: str = ...,
         IncludeStatus: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHarvestJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListHarvestJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listharvestjobspaginator)
         """
 
 
 class ListOriginEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListOriginEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listoriginendpointspaginator)
     """
 
     def paginate(
-        self, *, ChannelId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ChannelId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOriginEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListOriginEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listoriginendpointspaginator)
         """
```

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/paginator.pyi` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listchannelspaginator)
         """
 
 class ListHarvestJobsPaginator(Paginator):
@@ -65,27 +65,27 @@
     """
 
     def paginate(
         self,
         *,
         IncludeChannelId: str = ...,
         IncludeStatus: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHarvestJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListHarvestJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listharvestjobspaginator)
         """
 
 class ListOriginEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListOriginEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listoriginendpointspaginator)
     """
 
     def paginate(
-        self, *, ChannelId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ChannelId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOriginEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListOriginEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/paginators/#listoriginendpointspaginator)
         """
```

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/type_defs.py` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,46 +45,46 @@
 __all__ = (
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
     "IngressAccessLogsTypeDef",
     "HlsManifestCreateOrUpdateParametersTypeDef",
     "StreamSelectionTypeDef",
     "HlsManifestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "S3DestinationTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeHarvestJobRequestRequestTypeDef",
     "DescribeOriginEndpointRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionContractConfigurationTypeDef",
     "IngestEndpointTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
     "ListHarvestJobsRequestRequestTypeDef",
+    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RotateChannelCredentialsRequestRequestTypeDef",
     "RotateIngestEndpointCredentialsRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "ConfigureLogsRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateHarvestJobRequestRequestTypeDef",
     "CreateHarvestJobResponseTypeDef",
     "DescribeHarvestJobResponseTypeDef",
     "HarvestJobTypeDef",
     "SpekeKeyProviderTypeDef",
     "HlsIngestTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
-    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListHarvestJobsResponseTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
     "HlsEncryptionTypeDef",
     "MssEncryptionTypeDef",
     "ChannelTypeDef",
     "ConfigureLogsResponseTypeDef",
@@ -194,25 +194,14 @@
 )
 
 
 class HlsManifestTypeDef(_RequiredHlsManifestTypeDef, _OptionalHlsManifestTypeDef):
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
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalCreateChannelRequestRequestTypeDef = TypedDict(
@@ -271,14 +260,21 @@
 DescribeOriginEndpointRequestRequestTypeDef = TypedDict(
     "DescribeOriginEndpointRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncryptionContractConfigurationTypeDef = TypedDict(
     "EncryptionContractConfigurationTypeDef",
     {
         "PresetSpeke20Audio": PresetSpeke20AudioType,
         "PresetSpeke20Video": PresetSpeke20VideoType,
     },
 )
@@ -290,44 +286,61 @@
         "Password": str,
         "Url": str,
         "Username": str,
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
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListHarvestJobsRequestListHarvestJobsPaginateTypeDef = TypedDict(
+    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
+    {
+        "IncludeChannelId": str,
+        "IncludeStatus": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListHarvestJobsRequestRequestTypeDef = TypedDict(
     "ListHarvestJobsRequestRequestTypeDef",
     {
         "IncludeChannelId": str,
         "IncludeStatus": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
+    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
+    {
+        "ChannelId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOriginEndpointsRequestRequestTypeDef = TypedDict(
     "ListOriginEndpointsRequestRequestTypeDef",
     {
         "ChannelId": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -337,14 +350,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
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
 RotateChannelCredentialsRequestRequestTypeDef = TypedDict(
     "RotateChannelCredentialsRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -411,29 +453,14 @@
 
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
 
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
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateHarvestJobRequestRequestTypeDef = TypedDict(
     "CreateHarvestJobRequestRequestTypeDef",
     {
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
         "S3Destination": S3DestinationTypeDef,
@@ -449,15 +476,15 @@
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
         "S3Destination": S3DestinationTypeDef,
         "StartTime": str,
         "Status": StatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeHarvestJobResponseTypeDef = TypedDict(
     "DescribeHarvestJobResponseTypeDef",
     {
         "Arn": str,
@@ -465,15 +492,15 @@
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
         "S3Destination": S3DestinationTypeDef,
         "StartTime": str,
         "Status": StatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HarvestJobTypeDef = TypedDict(
     "HarvestJobTypeDef",
     {
         "Arn": str,
@@ -516,47 +543,20 @@
     "HlsIngestTypeDef",
     {
         "IngestEndpoints": List[IngestEndpointTypeDef],
     },
     total=False,
 )
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListHarvestJobsRequestListHarvestJobsPaginateTypeDef = TypedDict(
-    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
-    {
-        "IncludeChannelId": str,
-        "IncludeStatus": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
-    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
-    {
-        "ChannelId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListHarvestJobsResponseTypeDef = TypedDict(
     "ListHarvestJobsResponseTypeDef",
     {
         "HarvestJobs": List[HarvestJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCmafEncryptionTypeDef = TypedDict(
     "_RequiredCmafEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
@@ -647,90 +647,90 @@
         "CreatedAt": str,
         "Description": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RotateChannelCredentialsResponseTypeDef = TypedDict(
     "RotateChannelCredentialsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RotateIngestEndpointCredentialsResponseTypeDef = TypedDict(
     "RotateIngestEndpointCredentialsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CmafPackageCreateOrUpdateParametersTypeDef = TypedDict(
     "CmafPackageCreateOrUpdateParametersTypeDef",
     {
         "Encryption": CmafEncryptionTypeDef,
@@ -808,15 +808,15 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelId": str,
@@ -866,15 +866,15 @@
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOriginEndpointResponseTypeDef = TypedDict(
     "DescribeOriginEndpointResponseTypeDef",
     {
         "Arn": str,
@@ -890,15 +890,15 @@
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OriginEndpointTypeDef = TypedDict(
     "OriginEndpointTypeDef",
     {
         "Arn": str,
@@ -970,19 +970,19 @@
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "NextToken": str,
         "OriginEndpoints": List[OriginEndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage/type_defs.pyi` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -44,46 +44,46 @@
 __all__ = (
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
     "IngressAccessLogsTypeDef",
     "HlsManifestCreateOrUpdateParametersTypeDef",
     "StreamSelectionTypeDef",
     "HlsManifestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "S3DestinationTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeHarvestJobRequestRequestTypeDef",
     "DescribeOriginEndpointRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionContractConfigurationTypeDef",
     "IngestEndpointTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
     "ListHarvestJobsRequestRequestTypeDef",
+    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RotateChannelCredentialsRequestRequestTypeDef",
     "RotateIngestEndpointCredentialsRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "ConfigureLogsRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateHarvestJobRequestRequestTypeDef",
     "CreateHarvestJobResponseTypeDef",
     "DescribeHarvestJobResponseTypeDef",
     "HarvestJobTypeDef",
     "SpekeKeyProviderTypeDef",
     "HlsIngestTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
-    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListHarvestJobsResponseTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
     "HlsEncryptionTypeDef",
     "MssEncryptionTypeDef",
     "ChannelTypeDef",
     "ConfigureLogsResponseTypeDef",
@@ -189,25 +189,14 @@
     },
     total=False,
 )
 
 class HlsManifestTypeDef(_RequiredHlsManifestTypeDef, _OptionalHlsManifestTypeDef):
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
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalCreateChannelRequestRequestTypeDef = TypedDict(
@@ -264,14 +253,21 @@
 DescribeOriginEndpointRequestRequestTypeDef = TypedDict(
     "DescribeOriginEndpointRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncryptionContractConfigurationTypeDef = TypedDict(
     "EncryptionContractConfigurationTypeDef",
     {
         "PresetSpeke20Audio": PresetSpeke20AudioType,
         "PresetSpeke20Video": PresetSpeke20VideoType,
     },
 )
@@ -283,44 +279,61 @@
         "Password": str,
         "Url": str,
         "Username": str,
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
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListHarvestJobsRequestListHarvestJobsPaginateTypeDef = TypedDict(
+    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
+    {
+        "IncludeChannelId": str,
+        "IncludeStatus": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListHarvestJobsRequestRequestTypeDef = TypedDict(
     "ListHarvestJobsRequestRequestTypeDef",
     {
         "IncludeChannelId": str,
         "IncludeStatus": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
+    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
+    {
+        "ChannelId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOriginEndpointsRequestRequestTypeDef = TypedDict(
     "ListOriginEndpointsRequestRequestTypeDef",
     {
         "ChannelId": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -330,14 +343,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
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
 RotateChannelCredentialsRequestRequestTypeDef = TypedDict(
     "RotateChannelCredentialsRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -400,29 +442,14 @@
 )
 
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
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
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateHarvestJobRequestRequestTypeDef = TypedDict(
     "CreateHarvestJobRequestRequestTypeDef",
     {
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
         "S3Destination": S3DestinationTypeDef,
@@ -438,15 +465,15 @@
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
         "S3Destination": S3DestinationTypeDef,
         "StartTime": str,
         "Status": StatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeHarvestJobResponseTypeDef = TypedDict(
     "DescribeHarvestJobResponseTypeDef",
     {
         "Arn": str,
@@ -454,15 +481,15 @@
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
         "S3Destination": S3DestinationTypeDef,
         "StartTime": str,
         "Status": StatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HarvestJobTypeDef = TypedDict(
     "HarvestJobTypeDef",
     {
         "Arn": str,
@@ -503,47 +530,20 @@
     "HlsIngestTypeDef",
     {
         "IngestEndpoints": List[IngestEndpointTypeDef],
     },
     total=False,
 )
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListHarvestJobsRequestListHarvestJobsPaginateTypeDef = TypedDict(
-    "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
-    {
-        "IncludeChannelId": str,
-        "IncludeStatus": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
-    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
-    {
-        "ChannelId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListHarvestJobsResponseTypeDef = TypedDict(
     "ListHarvestJobsResponseTypeDef",
     {
         "HarvestJobs": List[HarvestJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCmafEncryptionTypeDef = TypedDict(
     "_RequiredCmafEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
@@ -628,90 +628,90 @@
         "CreatedAt": str,
         "Description": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RotateChannelCredentialsResponseTypeDef = TypedDict(
     "RotateChannelCredentialsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RotateIngestEndpointCredentialsResponseTypeDef = TypedDict(
     "RotateIngestEndpointCredentialsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CmafPackageCreateOrUpdateParametersTypeDef = TypedDict(
     "CmafPackageCreateOrUpdateParametersTypeDef",
     {
         "Encryption": CmafEncryptionTypeDef,
@@ -789,15 +789,15 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelId": str,
@@ -845,15 +845,15 @@
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOriginEndpointResponseTypeDef = TypedDict(
     "DescribeOriginEndpointResponseTypeDef",
     {
         "Arn": str,
@@ -869,15 +869,15 @@
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OriginEndpointTypeDef = TypedDict(
     "OriginEndpointTypeDef",
     {
         "Arn": str,
@@ -947,19 +947,19 @@
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "NextToken": str,
         "OriginEndpoints": List[OriginEndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage.egg-info/PKG-INFO` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage
-Version: 1.26.87
-Summary: Type annotations for boto3.MediaPackage 1.26.87 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.MediaPackage 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-mediapackage"></a>
 
 # mypy-boto3-mediapackage
 
 [![PyPI - mypy-boto3-mediapackage](https://img.shields.io/pypi/v/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -351,46 +351,46 @@
 from mypy_boto3_mediapackage.type_defs import (
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
     IngressAccessLogsTypeDef,
     HlsManifestCreateOrUpdateParametersTypeDef,
     StreamSelectionTypeDef,
     HlsManifestTypeDef,
-    ResponseMetadataTypeDef,
     CreateChannelRequestRequestTypeDef,
     S3DestinationTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeHarvestJobRequestRequestTypeDef,
     DescribeOriginEndpointRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionContractConfigurationTypeDef,
     IngestEndpointTypeDef,
-    PaginatorConfigTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
     ListHarvestJobsRequestRequestTypeDef,
+    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RotateChannelCredentialsRequestRequestTypeDef,
     RotateIngestEndpointCredentialsRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateHarvestJobRequestRequestTypeDef,
     CreateHarvestJobResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     HarvestJobTypeDef,
     SpekeKeyProviderTypeDef,
     HlsIngestTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListHarvestJobsResponseTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
     HlsEncryptionTypeDef,
     MssEncryptionTypeDef,
     ChannelTypeDef,
     ConfigureLogsResponseTypeDef,
@@ -422,42 +422,42 @@
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

### Comparing `mypy-boto3-mediapackage-1.26.87/mypy_boto3_mediapackage.egg-info/SOURCES.txt` & `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.26.87/setup.py` & `mypy-boto3-mediapackage-1.27.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-mediapackage.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackage",
-    version="1.26.87",
+    version="1.27.0",
     packages=["mypy_boto3_mediapackage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaPackage 1.26.87 service generated with mypy-boto3-builder"
-        " 7.12.5"
+        "Type annotations for boto3.MediaPackage 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/",
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


# Comparing `tmp/mypy-boto3-mediapackage-vod-1.26.87.tar.gz` & `tmp/mypy-boto3-mediapackage-vod-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackage-vod-1.26.87.tar", last modified: Wed Mar  8 20:35:46 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackage-vod-1.27.0.tar", last modified: Mon Jul  3 19:51:06 2023, max compression
```

## Comparing `mypy-boto3-mediapackage-vod-1.26.87.tar` & `mypy-boto3-mediapackage-vod-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.202592 mypy-boto3-mediapackage-vod-1.26.87/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-03-08 20:35:46.198592 mypy-boto3-mediapackage-vod-1.26.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.198592 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20090 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.198592 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-03-08 20:35:46.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-08 20:35:46.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 20:35:46.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 20:35:46.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-08 20:35:46.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-08 20:35:46.000000 mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 20:35:46.202592 mypy-boto3-mediapackage-vod-1.26.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-08 20:35:09.000000 mypy-boto3-mediapackage-vod-1.26.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.419647 mypy-boto3-mediapackage-vod-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15702 2023-07-03 19:51:06.419647 mypy-boto3-mediapackage-vod-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.415647 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-07-03 19:42:06.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-07-03 19:42:06.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20122 2023-07-03 19:42:06.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.419647 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15702 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:06.419647 mypy-boto3-mediapackage-vod-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-vod-1.27.0/setup.py
```

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/LICENSE` & `mypy-boto3-mediapackage-vod-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/PKG-INFO` & `mypy-boto3-mediapackage-vod-1.27.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage-vod
-Version: 1.26.87
-Summary: Type annotations for boto3.MediaPackageVod 1.26.87 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.MediaPackageVod 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-mediapackage-vod"></a>
 
 # mypy-boto3-mediapackage-vod
 
 [![PyPI - mypy-boto3-mediapackage-vod](https://img.shields.io/pypi/v/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage-vod?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackageVod 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[boto3.MediaPackageVod 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,52 +345,52 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage_vod.type_defs import (
     AssetShallowTypeDef,
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
-    ResponseMetadataTypeDef,
     CreateAssetRequestRequestTypeDef,
     EgressEndpointTypeDef,
     StreamSelectionTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeletePackagingConfigurationRequestRequestTypeDef,
     DeletePackagingGroupRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribePackagingConfigurationRequestRequestTypeDef,
     DescribePackagingGroupRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionContractConfigurationTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssetsRequestListAssetsPaginateTypeDef,
     ListAssetsRequestRequestTypeDef,
+    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
     ListPackagingConfigurationsRequestRequestTypeDef,
+    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ListAssetsResponseTypeDef,
     UpdatePackagingGroupRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
-    CreatePackagingGroupRequestRequestTypeDef,
-    PackagingGroupTypeDef,
     ConfigureLogsResponseTypeDef,
+    CreatePackagingGroupRequestRequestTypeDef,
     CreatePackagingGroupResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAssetsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    PackagingGroupTypeDef,
     UpdatePackagingGroupResponseTypeDef,
     CreateAssetResponseTypeDef,
     DescribeAssetResponseTypeDef,
     DashManifestTypeDef,
     HlsManifestTypeDef,
     MssManifestTypeDef,
     SpekeKeyProviderTypeDef,
-    ListAssetsRequestListAssetsPaginateTypeDef,
-    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
-    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsResponseTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
     HlsEncryptionTypeDef,
     MssEncryptionTypeDef,
     CmafPackageTypeDef,
     DashPackageTypeDef,
@@ -411,42 +411,42 @@
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

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/README.md` & `mypy-boto3-mediapackage-vod-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mediapackage-vod"></a>
 
 # mypy-boto3-mediapackage-vod
 
 [![PyPI - mypy-boto3-mediapackage-vod](https://img.shields.io/pypi/v/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage-vod?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackageVod 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[boto3.MediaPackageVod 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,52 +313,52 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage_vod.type_defs import (
     AssetShallowTypeDef,
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
-    ResponseMetadataTypeDef,
     CreateAssetRequestRequestTypeDef,
     EgressEndpointTypeDef,
     StreamSelectionTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeletePackagingConfigurationRequestRequestTypeDef,
     DeletePackagingGroupRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribePackagingConfigurationRequestRequestTypeDef,
     DescribePackagingGroupRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionContractConfigurationTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssetsRequestListAssetsPaginateTypeDef,
     ListAssetsRequestRequestTypeDef,
+    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
     ListPackagingConfigurationsRequestRequestTypeDef,
+    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ListAssetsResponseTypeDef,
     UpdatePackagingGroupRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
-    CreatePackagingGroupRequestRequestTypeDef,
-    PackagingGroupTypeDef,
     ConfigureLogsResponseTypeDef,
+    CreatePackagingGroupRequestRequestTypeDef,
     CreatePackagingGroupResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAssetsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    PackagingGroupTypeDef,
     UpdatePackagingGroupResponseTypeDef,
     CreateAssetResponseTypeDef,
     DescribeAssetResponseTypeDef,
     DashManifestTypeDef,
     HlsManifestTypeDef,
     MssManifestTypeDef,
     SpekeKeyProviderTypeDef,
-    ListAssetsRequestListAssetsPaginateTypeDef,
-    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
-    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsResponseTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
     HlsEncryptionTypeDef,
     MssEncryptionTypeDef,
     CmafPackageTypeDef,
     DashPackageTypeDef,
@@ -379,42 +379,42 @@
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

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/__init__.py` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/__init__.pyi` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/__main__.py` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaPackageVod 1.26.87\nVersion:         1.26.87\nBuilder"
-        " version: 7.12.5\nDocs:           "
+        "Type annotations for boto3.MediaPackageVod 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod\nOther"
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

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/client.py` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/client.pyi` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/literals.py` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
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
@@ -128,14 +129,15 @@
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
@@ -233,14 +235,15 @@
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
@@ -276,14 +279,15 @@
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
@@ -302,16 +306,19 @@
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
@@ -395,15 +402,17 @@
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

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/literals.pyi` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
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
@@ -126,14 +127,15 @@
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
@@ -231,14 +233,15 @@
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
@@ -274,14 +277,15 @@
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
@@ -300,16 +304,19 @@
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
@@ -393,15 +400,17 @@
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

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/paginator.py` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,43 +54,43 @@
 class ListAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listassetspaginator)
     """
 
     def paginate(
-        self, *, PackagingGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PackagingGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listassetspaginator)
         """
 
 
 class ListPackagingConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackagingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PackagingGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PackagingGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPackagingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackagingconfigurationspaginator)
         """
 
 
 class ListPackagingGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackaginggroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPackagingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackaginggroupspaginator)
         """
```

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/paginator.pyi` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -51,41 +51,41 @@
 class ListAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listassetspaginator)
     """
 
     def paginate(
-        self, *, PackagingGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PackagingGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listassetspaginator)
         """
 
 class ListPackagingConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackagingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PackagingGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PackagingGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPackagingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackagingconfigurationspaginator)
         """
 
 class ListPackagingGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackaginggroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPackagingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/paginators/#listpackaginggroupspaginator)
         """
```

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/type_defs.py` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,52 +36,52 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssetShallowTypeDef",
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "EgressEndpointTypeDef",
     "StreamSelectionTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeletePackagingConfigurationRequestRequestTypeDef",
     "DeletePackagingGroupRequestRequestTypeDef",
     "DescribeAssetRequestRequestTypeDef",
     "DescribePackagingConfigurationRequestRequestTypeDef",
     "DescribePackagingGroupRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionContractConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAssetsRequestListAssetsPaginateTypeDef",
     "ListAssetsRequestRequestTypeDef",
+    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
     "ListPackagingConfigurationsRequestRequestTypeDef",
+    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
     "ListPackagingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ListAssetsResponseTypeDef",
     "UpdatePackagingGroupRequestRequestTypeDef",
     "ConfigureLogsRequestRequestTypeDef",
-    "CreatePackagingGroupRequestRequestTypeDef",
-    "PackagingGroupTypeDef",
     "ConfigureLogsResponseTypeDef",
+    "CreatePackagingGroupRequestRequestTypeDef",
     "CreatePackagingGroupResponseTypeDef",
     "DescribePackagingGroupResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListAssetsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "PackagingGroupTypeDef",
     "UpdatePackagingGroupResponseTypeDef",
     "CreateAssetResponseTypeDef",
     "DescribeAssetResponseTypeDef",
     "DashManifestTypeDef",
     "HlsManifestTypeDef",
     "MssManifestTypeDef",
     "SpekeKeyProviderTypeDef",
-    "ListAssetsRequestListAssetsPaginateTypeDef",
-    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
-    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
     "ListPackagingGroupsResponseTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
     "HlsEncryptionTypeDef",
     "MssEncryptionTypeDef",
     "CmafPackageTypeDef",
     "DashPackageTypeDef",
@@ -121,25 +121,14 @@
     "EgressAccessLogsTypeDef",
     {
         "LogGroupName": str,
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
 _RequiredCreateAssetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetRequestRequestTypeDef",
     {
         "Id": str,
         "PackagingGroupId": str,
         "SourceArn": str,
         "SourceRoleArn": str,
@@ -219,52 +208,75 @@
 DescribePackagingGroupRequestRequestTypeDef = TypedDict(
     "DescribePackagingGroupRequestRequestTypeDef",
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
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
+    "ListAssetsRequestListAssetsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PackagingGroupId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAssetsRequestRequestTypeDef = TypedDict(
     "ListAssetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "PackagingGroupId": str,
     },
     total=False,
 )
 
+ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef = TypedDict(
+    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
+    {
+        "PackagingGroupId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPackagingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListPackagingConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "PackagingGroupId": str,
     },
     total=False,
 )
 
+ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef = TypedDict(
+    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPackagingGroupsRequestRequestTypeDef = TypedDict(
     "ListPackagingGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -273,14 +285,43 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -289,14 +330,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+ListAssetsResponseTypeDef = TypedDict(
+    "ListAssetsResponseTypeDef",
+    {
+        "Assets": List[AssetShallowTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePackagingGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePackagingGroupRequestRequestTypeDef = TypedDict(
@@ -332,14 +382,28 @@
 
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
 
+ConfigureLogsResponseTypeDef = TypedDict(
+    "ConfigureLogsResponseTypeDef",
+    {
+        "Arn": str,
+        "Authorization": AuthorizationTypeDef,
+        "CreatedAt": str,
+        "DomainName": str,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "Id": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackagingGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalCreatePackagingGroupRequestRequestTypeDef = TypedDict(
@@ -356,108 +420,70 @@
 class CreatePackagingGroupRequestRequestTypeDef(
     _RequiredCreatePackagingGroupRequestRequestTypeDef,
     _OptionalCreatePackagingGroupRequestRequestTypeDef,
 ):
     pass
 
 
-PackagingGroupTypeDef = TypedDict(
-    "PackagingGroupTypeDef",
-    {
-        "ApproximateAssetCount": int,
-        "Arn": str,
-        "Authorization": AuthorizationTypeDef,
-        "CreatedAt": str,
-        "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
-        "Id": str,
-        "Tags": Dict[str, str],
-    },
-    total=False,
-)
-
-ConfigureLogsResponseTypeDef = TypedDict(
-    "ConfigureLogsResponseTypeDef",
+CreatePackagingGroupResponseTypeDef = TypedDict(
+    "CreatePackagingGroupResponseTypeDef",
     {
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreatePackagingGroupResponseTypeDef = TypedDict(
-    "CreatePackagingGroupResponseTypeDef",
+DescribePackagingGroupResponseTypeDef = TypedDict(
+    "DescribePackagingGroupResponseTypeDef",
     {
+        "ApproximateAssetCount": int,
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribePackagingGroupResponseTypeDef = TypedDict(
-    "DescribePackagingGroupResponseTypeDef",
+PackagingGroupTypeDef = TypedDict(
+    "PackagingGroupTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
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
-ListAssetsResponseTypeDef = TypedDict(
-    "ListAssetsResponseTypeDef",
-    {
-        "Assets": List[AssetShallowTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
 UpdatePackagingGroupResponseTypeDef = TypedDict(
     "UpdatePackagingGroupResponseTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAssetResponseTypeDef = TypedDict(
     "CreateAssetResponseTypeDef",
     {
         "Arn": str,
@@ -465,15 +491,15 @@
         "EgressEndpoints": List[EgressEndpointTypeDef],
         "Id": str,
         "PackagingGroupId": str,
         "ResourceId": str,
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAssetResponseTypeDef = TypedDict(
     "DescribeAssetResponseTypeDef",
     {
         "Arn": str,
@@ -481,15 +507,15 @@
         "EgressEndpoints": List[EgressEndpointTypeDef],
         "Id": str,
         "PackagingGroupId": str,
         "ResourceId": str,
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DashManifestTypeDef = TypedDict(
     "DashManifestTypeDef",
     {
         "ManifestLayout": ManifestLayoutType,
@@ -541,46 +567,20 @@
 )
 
 
 class SpekeKeyProviderTypeDef(_RequiredSpekeKeyProviderTypeDef, _OptionalSpekeKeyProviderTypeDef):
     pass
 
 
-ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
-    "ListAssetsRequestListAssetsPaginateTypeDef",
-    {
-        "PackagingGroupId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef = TypedDict(
-    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
-    {
-        "PackagingGroupId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef = TypedDict(
-    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListPackagingGroupsResponseTypeDef = TypedDict(
     "ListPackagingGroupsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingGroups": List[PackagingGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCmafEncryptionTypeDef = TypedDict(
     "_RequiredCmafEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
@@ -755,15 +755,15 @@
         "CreatedAt": str,
         "DashPackage": DashPackageTypeDef,
         "HlsPackage": HlsPackageTypeDef,
         "Id": str,
         "MssPackage": MssPackageTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackagingConfigurationResponseTypeDef = TypedDict(
     "DescribePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
@@ -771,15 +771,15 @@
         "CreatedAt": str,
         "DashPackage": DashPackageTypeDef,
         "HlsPackage": HlsPackageTypeDef,
         "Id": str,
         "MssPackage": MssPackageTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PackagingConfigurationTypeDef = TypedDict(
     "PackagingConfigurationTypeDef",
     {
         "Arn": str,
@@ -796,10 +796,10 @@
 )
 
 ListPackagingConfigurationsResponseTypeDef = TypedDict(
     "ListPackagingConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingConfigurations": List[PackagingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod/type_defs.pyi` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod/type_defs.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -35,52 +35,52 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssetShallowTypeDef",
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "EgressEndpointTypeDef",
     "StreamSelectionTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeletePackagingConfigurationRequestRequestTypeDef",
     "DeletePackagingGroupRequestRequestTypeDef",
     "DescribeAssetRequestRequestTypeDef",
     "DescribePackagingConfigurationRequestRequestTypeDef",
     "DescribePackagingGroupRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionContractConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAssetsRequestListAssetsPaginateTypeDef",
     "ListAssetsRequestRequestTypeDef",
+    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
     "ListPackagingConfigurationsRequestRequestTypeDef",
+    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
     "ListPackagingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ListAssetsResponseTypeDef",
     "UpdatePackagingGroupRequestRequestTypeDef",
     "ConfigureLogsRequestRequestTypeDef",
-    "CreatePackagingGroupRequestRequestTypeDef",
-    "PackagingGroupTypeDef",
     "ConfigureLogsResponseTypeDef",
+    "CreatePackagingGroupRequestRequestTypeDef",
     "CreatePackagingGroupResponseTypeDef",
     "DescribePackagingGroupResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListAssetsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "PackagingGroupTypeDef",
     "UpdatePackagingGroupResponseTypeDef",
     "CreateAssetResponseTypeDef",
     "DescribeAssetResponseTypeDef",
     "DashManifestTypeDef",
     "HlsManifestTypeDef",
     "MssManifestTypeDef",
     "SpekeKeyProviderTypeDef",
-    "ListAssetsRequestListAssetsPaginateTypeDef",
-    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
-    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
     "ListPackagingGroupsResponseTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
     "HlsEncryptionTypeDef",
     "MssEncryptionTypeDef",
     "CmafPackageTypeDef",
     "DashPackageTypeDef",
@@ -120,25 +120,14 @@
     "EgressAccessLogsTypeDef",
     {
         "LogGroupName": str,
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
 _RequiredCreateAssetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetRequestRequestTypeDef",
     {
         "Id": str,
         "PackagingGroupId": str,
         "SourceArn": str,
         "SourceRoleArn": str,
@@ -216,52 +205,75 @@
 DescribePackagingGroupRequestRequestTypeDef = TypedDict(
     "DescribePackagingGroupRequestRequestTypeDef",
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
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
+    "ListAssetsRequestListAssetsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PackagingGroupId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAssetsRequestRequestTypeDef = TypedDict(
     "ListAssetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "PackagingGroupId": str,
     },
     total=False,
 )
 
+ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef = TypedDict(
+    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
+    {
+        "PackagingGroupId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPackagingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListPackagingConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "PackagingGroupId": str,
     },
     total=False,
 )
 
+ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef = TypedDict(
+    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPackagingGroupsRequestRequestTypeDef = TypedDict(
     "ListPackagingGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -270,14 +282,43 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -286,14 +327,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+ListAssetsResponseTypeDef = TypedDict(
+    "ListAssetsResponseTypeDef",
+    {
+        "Assets": List[AssetShallowTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePackagingGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePackagingGroupRequestRequestTypeDef = TypedDict(
@@ -325,14 +375,28 @@
 )
 
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
+ConfigureLogsResponseTypeDef = TypedDict(
+    "ConfigureLogsResponseTypeDef",
+    {
+        "Arn": str,
+        "Authorization": AuthorizationTypeDef,
+        "CreatedAt": str,
+        "DomainName": str,
+        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "Id": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackagingGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalCreatePackagingGroupRequestRequestTypeDef = TypedDict(
@@ -347,108 +411,70 @@
 
 class CreatePackagingGroupRequestRequestTypeDef(
     _RequiredCreatePackagingGroupRequestRequestTypeDef,
     _OptionalCreatePackagingGroupRequestRequestTypeDef,
 ):
     pass
 
-PackagingGroupTypeDef = TypedDict(
-    "PackagingGroupTypeDef",
-    {
-        "ApproximateAssetCount": int,
-        "Arn": str,
-        "Authorization": AuthorizationTypeDef,
-        "CreatedAt": str,
-        "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
-        "Id": str,
-        "Tags": Dict[str, str],
-    },
-    total=False,
-)
-
-ConfigureLogsResponseTypeDef = TypedDict(
-    "ConfigureLogsResponseTypeDef",
+CreatePackagingGroupResponseTypeDef = TypedDict(
+    "CreatePackagingGroupResponseTypeDef",
     {
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreatePackagingGroupResponseTypeDef = TypedDict(
-    "CreatePackagingGroupResponseTypeDef",
+DescribePackagingGroupResponseTypeDef = TypedDict(
+    "DescribePackagingGroupResponseTypeDef",
     {
+        "ApproximateAssetCount": int,
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribePackagingGroupResponseTypeDef = TypedDict(
-    "DescribePackagingGroupResponseTypeDef",
+PackagingGroupTypeDef = TypedDict(
+    "PackagingGroupTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
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
-ListAssetsResponseTypeDef = TypedDict(
-    "ListAssetsResponseTypeDef",
-    {
-        "Assets": List[AssetShallowTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
 UpdatePackagingGroupResponseTypeDef = TypedDict(
     "UpdatePackagingGroupResponseTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
         "DomainName": str,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAssetResponseTypeDef = TypedDict(
     "CreateAssetResponseTypeDef",
     {
         "Arn": str,
@@ -456,15 +482,15 @@
         "EgressEndpoints": List[EgressEndpointTypeDef],
         "Id": str,
         "PackagingGroupId": str,
         "ResourceId": str,
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAssetResponseTypeDef = TypedDict(
     "DescribeAssetResponseTypeDef",
     {
         "Arn": str,
@@ -472,15 +498,15 @@
         "EgressEndpoints": List[EgressEndpointTypeDef],
         "Id": str,
         "PackagingGroupId": str,
         "ResourceId": str,
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DashManifestTypeDef = TypedDict(
     "DashManifestTypeDef",
     {
         "ManifestLayout": ManifestLayoutType,
@@ -530,46 +556,20 @@
     },
     total=False,
 )
 
 class SpekeKeyProviderTypeDef(_RequiredSpekeKeyProviderTypeDef, _OptionalSpekeKeyProviderTypeDef):
     pass
 
-ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
-    "ListAssetsRequestListAssetsPaginateTypeDef",
-    {
-        "PackagingGroupId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef = TypedDict(
-    "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
-    {
-        "PackagingGroupId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef = TypedDict(
-    "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListPackagingGroupsResponseTypeDef = TypedDict(
     "ListPackagingGroupsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingGroups": List[PackagingGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCmafEncryptionTypeDef = TypedDict(
     "_RequiredCmafEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
@@ -730,15 +730,15 @@
         "CreatedAt": str,
         "DashPackage": DashPackageTypeDef,
         "HlsPackage": HlsPackageTypeDef,
         "Id": str,
         "MssPackage": MssPackageTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackagingConfigurationResponseTypeDef = TypedDict(
     "DescribePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
@@ -746,15 +746,15 @@
         "CreatedAt": str,
         "DashPackage": DashPackageTypeDef,
         "HlsPackage": HlsPackageTypeDef,
         "Id": str,
         "MssPackage": MssPackageTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PackagingConfigurationTypeDef = TypedDict(
     "PackagingConfigurationTypeDef",
     {
         "Arn": str,
@@ -771,10 +771,10 @@
 )
 
 ListPackagingConfigurationsResponseTypeDef = TypedDict(
     "ListPackagingConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingConfigurations": List[PackagingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage-vod
-Version: 1.26.87
-Summary: Type annotations for boto3.MediaPackageVod 1.26.87 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.MediaPackageVod 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-mediapackage-vod"></a>
 
 # mypy-boto3-mediapackage-vod
 
 [![PyPI - mypy-boto3-mediapackage-vod](https://img.shields.io/pypi/v/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage-vod?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackageVod 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[boto3.MediaPackageVod 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,52 +345,52 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage_vod.type_defs import (
     AssetShallowTypeDef,
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
-    ResponseMetadataTypeDef,
     CreateAssetRequestRequestTypeDef,
     EgressEndpointTypeDef,
     StreamSelectionTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeletePackagingConfigurationRequestRequestTypeDef,
     DeletePackagingGroupRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribePackagingConfigurationRequestRequestTypeDef,
     DescribePackagingGroupRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionContractConfigurationTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssetsRequestListAssetsPaginateTypeDef,
     ListAssetsRequestRequestTypeDef,
+    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
     ListPackagingConfigurationsRequestRequestTypeDef,
+    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ListAssetsResponseTypeDef,
     UpdatePackagingGroupRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
-    CreatePackagingGroupRequestRequestTypeDef,
-    PackagingGroupTypeDef,
     ConfigureLogsResponseTypeDef,
+    CreatePackagingGroupRequestRequestTypeDef,
     CreatePackagingGroupResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAssetsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    PackagingGroupTypeDef,
     UpdatePackagingGroupResponseTypeDef,
     CreateAssetResponseTypeDef,
     DescribeAssetResponseTypeDef,
     DashManifestTypeDef,
     HlsManifestTypeDef,
     MssManifestTypeDef,
     SpekeKeyProviderTypeDef,
-    ListAssetsRequestListAssetsPaginateTypeDef,
-    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
-    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsResponseTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
     HlsEncryptionTypeDef,
     MssEncryptionTypeDef,
     CmafPackageTypeDef,
     DashPackageTypeDef,
@@ -411,42 +411,42 @@
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

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt` & `mypy-boto3-mediapackage-vod-1.27.0/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.26.87/setup.py` & `mypy-boto3-mediapackage-vod-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-mediapackage-vod.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackage-vod",
-    version="1.26.87",
+    version="1.27.0",
     packages=["mypy_boto3_mediapackage_vod"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaPackageVod 1.26.87 service generated with"
-        " mypy-boto3-builder 7.12.5"
+        "Type annotations for boto3.MediaPackageVod 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/",
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

